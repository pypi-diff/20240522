# Comparing `tmp/faraday_agent_dispatcher-3.2.1.tar.gz` & `tmp/faraday_agent_dispatcher-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faraday_agent_dispatcher-3.2.1.tar", last modified: Thu Feb  8 16:46:03 2024, max compression
+gzip compressed data, was "faraday_agent_dispatcher-3.3.0.tar", last modified: Tue Mar 12 18:13:15 2024, max compression
```

## Comparing `faraday_agent_dispatcher-3.2.1.tar` & `faraday_agent_dispatcher-3.3.0.tar`

### file list

```diff
@@ -1,365 +1,375 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.793536 faraday_agent_dispatcher-3.2.1/
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/.flake8
--rw-rw-rw-   0 root         (0) root         (0)     2366 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.723535 faraday_agent_dispatcher-3.2.1/.gitlab/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.736535 faraday_agent_dispatcher-3.2.1/.gitlab/ci/
--rw-rw-rw-   0 root         (0) root         (0)     1387 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/.gitlab/ci/.pre-gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      508 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/.gitlab/ci/.rules-conditions.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.736535 faraday_agent_dispatcher-3.2.1/.gitlab/ci/build_ci/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/.gitlab/ci/build_ci/.build-gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      717 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/.gitlab/ci/fetch-secrets.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.737536 faraday_agent_dispatcher-3.2.1/.gitlab/ci/plugins-integration/
--rw-rw-rw-   0 root         (0) root         (0)     1017 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/.gitlab/ci/plugins-integration/.build-gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      877 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/.gitlab/ci/plugins-integration/.testing-gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.737536 faraday_agent_dispatcher-3.2.1/.gitlab/ci/publish/
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/.gitlab/ci/publish/.publish-dockerhub-gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      283 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/.gitlab/ci/publish/.pypi-gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.738536 faraday_agent_dispatcher-3.2.1/.gitlab/ci/testing/
--rw-rw-rw-   0 root         (0) root         (0)      447 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/.gitlab/ci/testing/.post-gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     2765 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/.gitlab/ci/testing/.testing-gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1470 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      743 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/.pre-push-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/AUTHORS.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.738536 faraday_agent_dispatcher-3.2.1/CHANGELOG/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.738536 faraday_agent_dispatcher-3.2.1/CHANGELOG/0.1/
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/0.1/01.first version.md
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/0.1/02.minimal structure.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/0.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/0.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.740536 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.0/
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.0/01.env_var.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.0/02.executor.md
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.0/03.params.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.0/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.741536 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.1/
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.1/01.run.md
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.1/02.wizard.md
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.1/03.01.manage_execution_id.md
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.1/03.02.change_ws_route.md
--rw-rw-rw-   0 root         (0) root         (0)       79 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.1/04.error_management.md
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.1/05.invalid token.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.1/06.ssl.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.743536 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2/
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2/01.package_executor.md
--rw-rw-rw-   0 root         (0) root         (0)       31 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2/02.signal.md
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2/03.close_connection.md
--rw-rw-rw-   0 root         (0) root         (0)       46 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2/04.sslcert.md
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2/05.config_folder.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2/E00.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2/date.md
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.745535 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2.1/01.check_command_before_run.md
--rw-rw-rw-   0 root         (0) root         (0)       91 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2.1/02.connect_checks_timeout.md
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2.1/03.connect_checks_not_responding.md
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2.1/04.connect_checks_ssl_verify_fails.md
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2.1/05.executor_with_comma.md
--rw-rw-rw-   0 root         (0) root         (0)       59 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2.1/06.ssl_wizard.md
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2.1/07.doc.md
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2.1/E00.md
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2.1/E01.nmap_multi_target.md
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2.1/E02.w3af_use_python2.md
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2.1/E03.escape.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.2.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.747536 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.3.0/
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.3.0/1.multi_workspace.md
--rw-rw-rw-   0 root         (0) root         (0)      116 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.3.0/2.migrate_in_run.md
--rw-rw-rw-   0 root         (0) root         (0)       82 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.3.0/3.fix_close_agent.md
--rw-rw-rw-   0 root         (0) root         (0)       89 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.3.0/4.page-size.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.3.0/E00.md
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.3.0/E01.fix_arachni.md
--rw-rw-rw-   0 root         (0) root         (0)       74 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.3.0/E02.fix_nmap.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.3.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.3.0/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.748535 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.3.1/
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.3.1/1.proxy_setup.md
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.3.1/E01.fix_nessus.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.3.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.3.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.749535 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.0/
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.0/1.base_route.md
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.0/2.duration.md
--rw-rw-rw-   0 root         (0) root         (0)      147 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.0/E00.md
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.0/E01_flags_nmap.md
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.0/E02_env_python.md
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.0/E03_scheme_http_s_nmap.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.0/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.750536 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.1/
--rw-rw-rw-   0 root         (0) root         (0)      461 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.1/1.general_changes.md
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.1/E1.wpscan_not_use_docker.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.1/E2.fix_nuclei.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.751536 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.2/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.2/1.plugins.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.2/date.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.4.2/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.752535 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.5.0/
--rw-rw-rw-   0 root         (0) root         (0)      152 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.5.0/1.change_wizard.md
--rw-rw-rw-   0 root         (0) root         (0)       64 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.5.0/2.v3.md
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.5.0/3.connectivity_endpoint.md
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.5.0/4.token.md
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.5.0/5.update_host_input.md
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.5.0/E1.update_openvas.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.5.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.5.0/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.753536 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.5.1/
--rw-rw-rw-   0 root         (0) root         (0)       31 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.5.1/1.fix_burp_executor.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.5.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/1.5.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.754536 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.0.0/1.typing.md
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.0.0/2.add_manifests_versioning.md
--rw-rw-rw-   0 root         (0) root         (0)       19 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.0.0/3.FIX_typo_in_wizard.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.0.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.0.0/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.755535 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       57 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.0/1.add_reminder_for_token.md
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.0/2.fix_dates.md
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.0/3.manage_402.md
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.0/E1.add_insightvm_executor.md
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.0/E2.update_burp.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.0/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.756536 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.1/
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.1/1.add_option_ignore_ssl.md
--rw-rw-rw-   0 root         (0) root         (0)       97 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.1/2.redo_defaults_ports_after_ssl.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.756536 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.2/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.2/add_script_to_nmap.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.2/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.757536 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.3/
--rw-rw-rw-   0 root         (0) root         (0)       46 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.3/add_commands_to_wpscan.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.3/date.md
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.1.3/move_shodan_to_official.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.758535 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.2.0/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.2.0/Add_timeout_parameter_to_arachni.md
--rw-rw-rw-   0 root         (0) root         (0)       57 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.2.0/add w3af.md
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.2.0/add_ignore_info_and_hostname_resolution.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.2.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.2.0/fix_exectuors.md
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.2.0/fix_logs.md
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.2.0/remove_ws.md
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.2.0/send_parameters_at_connection_time.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.760536 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.3.0/
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.3.0/add_scan_functionality_to_insightvm.md
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.3.0/add_tags_for_plugins.md
--rw-rw-rw-   0 root         (0) root         (0)       57 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.3.0/add_vulners.md
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.3.0/change_api_key.md
--rw-rw-rw-   0 root         (0) root         (0)       80 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.3.0/change_venvs.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.3.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.3.0/update_docs.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.760536 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.4.0/
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.4.0/Add_qualys.md
--rw-rw-rw-   0 root         (0) root         (0)       46 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.4.0/change_pgrep_for_psutil.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.4.0/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.761536 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.5.0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.5.0/add_sonar_executor.md
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.5.0/add_tenableio_executor.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.5.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       66 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.5.0/fix_gvm_executor.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.5.0/transform_to_str.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.762536 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.5.1/
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.5.1/allow_ip_target_for_nuclei.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.5.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.5.1/fixes_for_bandit.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.762536 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.6.0/
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.6.0/186.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.6.0/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.763536 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.6.1/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.6.1/187.md
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.6.1/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.763536 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.6.2/
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.6.2/192.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.6.2/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.764536 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.6.3/
--rw-rw-rw-   0 root         (0) root         (0)       53 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.6.3/194.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/2.6.3/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.764536 faraday_agent_dispatcher-3.2.1/CHANGELOG/3.0.0/
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/3.0.0/195.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/3.0.0/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.764536 faraday_agent_dispatcher-3.2.1/CHANGELOG/3.0.1/
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/3.0.1/199.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/3.0.1/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.765535 faraday_agent_dispatcher-3.2.1/CHANGELOG/3.2.0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/3.2.0/206.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/3.2.0/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.765535 faraday_agent_dispatcher-3.2.1/CHANGELOG/current/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/current/.keep
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CHANGELOG/footer.md
--rw-rw-rw-   0 root         (0) root         (0)     3711 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    35149 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/COPYING
--rw-rw-rw-   0 root         (0) root         (0)       93 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     2313 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/Makefile
--rw-r--r--   0 root         (0) root         (0)    16641 2024-02-08 16:46:03.793536 faraday_agent_dispatcher-3.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6247 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     8648 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/RELEASE.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.728536 faraday_agent_dispatcher-3.2.1/docker/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.765535 faraday_agent_dispatcher-3.2.1/docker/plugins-docker/
--rw-rw-rw-   0 root         (0) root         (0)     3095 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docker/plugins-docker/Dockerfile
--rwxrwxrwx   0 root         (0) root         (0)      802 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docker/plugins-docker/docker.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.766536 faraday_agent_dispatcher-3.2.1/docker/publish/
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docker/publish/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)      588 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docker/publish/Dockerfile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.767536 faraday_agent_dispatcher-3.2.1/docker/publish/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2059 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docker/publish/templates/template_dispatcher.ini
--rw-rw-rw-   0 root         (0) root         (0)     4473 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docker/publish/templates/template_dispatcher.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2227 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docker/publish/templates/template_dispatcher_with_report.ini
--rw-rw-rw-   0 root         (0) root         (0)     4830 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docker/publish/templates/template_dispatcher_with_report.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.767536 faraday_agent_dispatcher-3.2.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      927 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.768535 faraday_agent_dispatcher-3.2.1/docs/docs/
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/418.md
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/CNAME
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.768535 faraday_agent_dispatcher-3.2.1/docs/docs/css/
--rw-rw-rw-   0 root         (0) root         (0)      114 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/css/faraday_doc.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.768535 faraday_agent_dispatcher-3.2.1/docs/docs/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/examples/new-custom-executor.md
--rw-rw-rw-   0 root         (0) root         (0)     9813 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/getting-started.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.770536 faraday_agent_dispatcher-3.2.1/docs/docs/images/
--rw-rw-rw-   0 root         (0) root         (0)    31633 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/images/agent_example.png
--rw-rw-rw-   0 root         (0) root         (0)    44658 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/images/arch.png
--rw-rw-rw-   0 root         (0) root         (0)    20584 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/images/arch_dispatcher.png
--rw-rw-rw-   0 root         (0) root         (0)    26625 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/images/arch_executors.png
--rw-rw-rw-   0 root         (0) root         (0)    21253 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/images/executor_example.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.730536 faraday_agent_dispatcher-3.2.1/docs/docs/images/executors/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.771535 faraday_agent_dispatcher-3.2.1/docs/docs/images/executors/qualys/
--rw-rw-rw-   0 root         (0) root         (0)    54521 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/images/executors/qualys/check_profile.png
--rw-rw-rw-   0 root         (0) root         (0)   280745 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/images/executors/qualys/new_profile.png
--rw-rw-rw-   0 root         (0) root         (0)   194186 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/images/executors/qualys/profileid.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.772536 faraday_agent_dispatcher-3.2.1/docs/docs/images/executors/sonarqube/
--rw-rw-rw-   0 root         (0) root         (0)    34458 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/images/executors/sonarqube/generate_token.png
--rw-rw-rw-   0 root         (0) root         (0)    10160 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/images/executors/sonarqube/profile_icon.png
--rw-rw-rw-   0 root         (0) root         (0)     3175 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/images/favicon.png
--rw-rw-rw-   0 root         (0) root         (0)      581 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/images/logo.svg
--rw-rw-rw-   0 root         (0) root         (0)    20392 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/images/token.png
--rw-rw-rw-   0 root         (0) root         (0)     1428 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.772536 faraday_agent_dispatcher-3.2.1/docs/docs/js/
--rw-rw-rw-   0 root         (0) root         (0)     2051 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/js/details.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.774536 faraday_agent_dispatcher-3.2.1/docs/docs/misc/
--rw-rw-rw-   0 root         (0) root         (0)      846 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/misc/appscan.md
--rw-rw-rw-   0 root         (0) root         (0)     2533 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/misc/docker.md
--rw-rw-rw-   0 root         (0) root         (0)     1545 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/misc/qualys.md
--rw-rw-rw-   0 root         (0) root         (0)     1045 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/misc/sonarqube.md
--rw-rw-rw-   0 root         (0) root         (0)     2059 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/misc/template_dispatcher.ini
--rw-rw-rw-   0 root         (0) root         (0)     4473 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/misc/template_dispatcher.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2227 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/misc/template_dispatcher_with_report.ini
--rw-rw-rw-   0 root         (0) root         (0)     4830 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/misc/template_dispatcher_with_report.yaml
--rw-rw-rw-   0 root         (0) root         (0)      767 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/misc/tenableio.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.774536 faraday_agent_dispatcher-3.2.1/docs/docs/technical/
--rw-rw-rw-   0 root         (0) root         (0)     6633 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/technical/agents.md
--rw-rw-rw-   0 root         (0) root         (0)     1770 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/docs/technical/arch.md
--rw-rw-rw-   0 root         (0) root         (0)     2025 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/docs/mkdocs.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.776536 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/
--rw-rw-rw-   0 root         (0) root         (0)      883 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.778536 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5418 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/cli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.779536 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/cli/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/cli/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/cli/utils/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2991 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/cli/utils/general_inputs.py
--rw-rw-rw-   0 root         (0) root         (0)      558 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/cli/utils/general_prompts.py
--rw-rw-rw-   0 root         (0) root         (0)    12031 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/cli/utils/model_load.py
--rw-rw-rw-   0 root         (0) root         (0)     9859 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/cli/wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    14016 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/config.py
--rw-rw-rw-   0 root         (0) root         (0)    27418 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)    34398 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/dispatcher_io.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/example_config.ini
--rw-rw-rw-   0 root         (0) root         (0)      165 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/example_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2537 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/executor.py
--rw-rw-rw-   0 root         (0) root         (0)     6288 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/executor_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     3858 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.731536 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.731536 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.784536 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/
--rw-rw-rw-   0 root         (0) root         (0)     9484 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/appscan.py
--rw-rw-rw-   0 root         (0) root         (0)     3269 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/arachni.py
--rw-rw-rw-   0 root         (0) root         (0)     9215 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/burp.py
--rw-rw-rw-   0 root         (0) root         (0)     3808 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/crackmapexec.py
--rw-rw-rw-   0 root         (0) root         (0)     4862 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/dependabot.py
--rw-rw-rw-   0 root         (0) root         (0)     6135 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/gvm_openvas.py
--rw-rw-rw-   0 root         (0) root         (0)     6447 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/insightvm.py
--rwxrwxrwx   0 root         (0) root         (0)     9563 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/nessus.py
--rw-rw-rw-   0 root         (0) root         (0)     2104 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/nikto2.py
--rwxrwxrwx   0 root         (0) root         (0)     3551 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/nmap.py
--rwxrwxrwx   0 root         (0) root         (0)     3152 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/nuclei.py
--rw-rw-rw-   0 root         (0) root         (0)     4424 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/openvas_legacy.py
--rw-rw-rw-   0 root         (0) root         (0)     6205 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/qualys.py
--rw-rw-rw-   0 root         (0) root         (0)     1908 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/report_processor.py
--rw-rw-rw-   0 root         (0) root         (0)     2010 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/shodan2.py
--rw-rw-rw-   0 root         (0) root         (0)     2780 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/sonarqube.py
--rwxrwxrwx   0 root         (0) root         (0)      887 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/sublist3r.sh
--rw-rw-rw-   0 root         (0) root         (0)     4134 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/tenableio.py
--rw-rw-rw-   0 root         (0) root         (0)     3960 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/w3af.py
--rw-rw-rw-   0 root         (0) root         (0)     2521 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/wpscan.py
--rw-rw-rw-   0 root         (0) root         (0)     2416 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/wpscan_legacy.py
--rw-rw-rw-   0 root         (0) root         (0)     2160 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/zap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.785536 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3861 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/utils/control_values_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2217 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/utils/metadata_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      281 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/utils/text_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1103 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/utils/url_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.792536 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16641 2024-02-08 16:46:03.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10521 2024-02-08 16:46:03.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-08 16:46:03.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2024-02-08 16:46:03.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-08 16:46:03.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      345 2024-02-08 16:46:03.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-02-08 16:46:03.000000 faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      466 2024-02-08 16:46:03.794536 faraday_agent_dispatcher-3.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3103 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.785536 faraday_agent_dispatcher-3.2.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.786536 faraday_agent_dispatcher-3.2.1/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/data/basic_executor.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/data/mock.pub
--rw-rw-rw-   0 root         (0) root         (0)     1302 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/data/ok.crt
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/data/ok.key
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.788536 faraday_agent_dispatcher-3.2.1/tests/data/old_version_inis/
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/data/old_version_inis/0.1.ini
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/data/old_version_inis/0.1_with_agent_token.ini
--rw-rw-rw-   0 root         (0) root         (0)      507 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/data/old_version_inis/1.0.ini
--rw-rw-rw-   0 root         (0) root         (0)      359 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/data/old_version_inis/1.0_error0.ini
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/data/old_version_inis/1.0_error1.ini
--rw-rw-rw-   0 root         (0) root         (0)      578 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/data/old_version_inis/1.0_with_agent_token.ini
--rw-rw-rw-   0 root         (0) root         (0)      611 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/data/old_version_inis/1.2.ini
--rw-rw-rw-   0 root         (0) root         (0)      681 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/data/old_version_inis/1.2_with_agent_token.ini
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/data/old_version_inis/1.5.ini
--rw-rw-rw-   0 root         (0) root         (0)      822 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/data/test_config.ini
--rw-rw-rw-   0 root         (0) root         (0)     1302 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/data/wrong.crt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.788536 faraday_agent_dispatcher-3.2.1/tests/integration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.789536 faraday_agent_dispatcher-3.2.1/tests/integration/faraday/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/integration/faraday/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7330 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/integration/faraday/test_execution.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.789536 faraday_agent_dispatcher-3.2.1/tests/plugins-docker/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/plugins-docker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3674 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/plugins-docker/test_executors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.790536 faraday_agent_dispatcher-3.2.1/tests/unittests/
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/unittests/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/unittests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.791536 faraday_agent_dispatcher-3.2.1/tests/unittests/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/unittests/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    46373 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/unittests/config/agent_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)    37399 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/unittests/config/wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    12779 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/unittests/test_agent_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     5088 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/unittests/test_config_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/unittests/test_import_official_executors.py
--rw-rw-rw-   0 root         (0) root         (0)     7983 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/unittests/wizard_input.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:46:03.792536 faraday_agent_dispatcher-3.2.1/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9651 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/utils/testing_faraday_server.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tests/utils/text_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      571 2024-02-08 16:45:32.000000 faraday_agent_dispatcher-3.2.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.785042 faraday_agent_dispatcher-3.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)     2366 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.712042 faraday_agent_dispatcher-3.3.0/.gitlab/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.725042 faraday_agent_dispatcher-3.3.0/.gitlab/ci/
+-rw-rw-rw-   0 root         (0) root         (0)     1387 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/.pre-gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      508 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/.rules-conditions.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.725042 faraday_agent_dispatcher-3.3.0/.gitlab/ci/build_ci/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/build_ci/.build-gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      717 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/fetch-secrets.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.726042 faraday_agent_dispatcher-3.3.0/.gitlab/ci/plugins-integration/
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/plugins-integration/.build-gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      877 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/plugins-integration/.testing-gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.726042 faraday_agent_dispatcher-3.3.0/.gitlab/ci/publish/
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/publish/.publish-dockerhub-gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      283 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/publish/.pypi-gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.727042 faraday_agent_dispatcher-3.3.0/.gitlab/ci/testing/
+-rw-rw-rw-   0 root         (0) root         (0)      447 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/testing/.post-gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2765 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/testing/.testing-gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1470 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      743 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.pre-push-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/AUTHORS.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.727042 faraday_agent_dispatcher-3.3.0/CHANGELOG/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.728042 faraday_agent_dispatcher-3.3.0/CHANGELOG/0.1/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/0.1/01.first version.md
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/0.1/02.minimal structure.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/0.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/0.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.729042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.0/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.0/01.env_var.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.0/02.executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.0/03.params.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.0/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.730042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/01.run.md
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/02.wizard.md
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/03.01.manage_execution_id.md
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/03.02.change_ws_route.md
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/04.error_management.md
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/05.invalid token.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/06.ssl.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.732042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2/01.package_executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       31 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2/02.signal.md
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2/03.close_connection.md
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2/04.sslcert.md
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2/05.config_folder.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2/E00.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.735042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/01.check_command_before_run.md
+-rw-rw-rw-   0 root         (0) root         (0)       91 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/02.connect_checks_timeout.md
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/03.connect_checks_not_responding.md
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/04.connect_checks_ssl_verify_fails.md
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/05.executor_with_comma.md
+-rw-rw-rw-   0 root         (0) root         (0)       59 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/06.ssl_wizard.md
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/07.doc.md
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/E00.md
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/E01.nmap_multi_target.md
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/E02.w3af_use_python2.md
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/E03.escape.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.736042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/1.multi_workspace.md
+-rw-rw-rw-   0 root         (0) root         (0)      116 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/2.migrate_in_run.md
+-rw-rw-rw-   0 root         (0) root         (0)       82 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/3.fix_close_agent.md
+-rw-rw-rw-   0 root         (0) root         (0)       89 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/4.page-size.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/E00.md
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/E01.fix_arachni.md
+-rw-rw-rw-   0 root         (0) root         (0)       74 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/E02.fix_nmap.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.737042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.1/1.proxy_setup.md
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.1/E01.fix_nessus.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.739042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.0/1.base_route.md
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.0/2.duration.md
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.0/E00.md
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.0/E01_flags_nmap.md
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.0/E02_env_python.md
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.0/E03_scheme_http_s_nmap.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.0/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.740042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)      461 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.1/1.general_changes.md
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.1/E1.wpscan_not_use_docker.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.1/E2.fix_nuclei.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.740042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.2/1.plugins.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.2/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.2/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.742042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)      152 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.0/1.change_wizard.md
+-rw-rw-rw-   0 root         (0) root         (0)       64 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.0/2.v3.md
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.0/3.connectivity_endpoint.md
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.0/4.token.md
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.0/5.update_host_input.md
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.0/E1.update_openvas.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.0/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.742042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.1/1.fix_burp_executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.743042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.0.0/1.typing.md
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.0.0/2.add_manifests_versioning.md
+-rw-rw-rw-   0 root         (0) root         (0)       19 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.0.0/3.FIX_typo_in_wizard.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.0.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.0.0/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.745042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.0/1.add_reminder_for_token.md
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.0/2.fix_dates.md
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.0/3.manage_402.md
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.0/E1.add_insightvm_executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.0/E2.update_burp.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.0/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.746042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.1/1.add_option_ignore_ssl.md
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.1/2.redo_defaults_ports_after_ssl.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.746042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.2/add_script_to_nmap.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.2/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.747042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.3/add_commands_to_wpscan.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.3/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.3/move_shodan_to_official.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.748042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.2.0/Add_timeout_parameter_to_arachni.md
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.2.0/add w3af.md
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.2.0/add_ignore_info_and_hostname_resolution.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.2.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.2.0/fix_exectuors.md
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.2.0/fix_logs.md
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.2.0/remove_ws.md
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.2.0/send_parameters_at_connection_time.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.750042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.3.0/add_scan_functionality_to_insightvm.md
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.3.0/add_tags_for_plugins.md
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.3.0/add_vulners.md
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.3.0/change_api_key.md
+-rw-rw-rw-   0 root         (0) root         (0)       80 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.3.0/change_venvs.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.3.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.3.0/update_docs.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.750042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.4.0/Add_qualys.md
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.4.0/change_pgrep_for_psutil.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.4.0/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.751042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.0/add_sonar_executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.0/add_tenableio_executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       66 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.0/fix_gvm_executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.0/transform_to_str.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.752042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.1/allow_ip_target_for_nuclei.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.1/fixes_for_bandit.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.752042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.0/186.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.0/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.753042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.1/187.md
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.1/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.753042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.2/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.2/192.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.2/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.753042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.3/
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.3/194.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.3/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.754042 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.0.0/195.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.0.0/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.754042 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.0.1/199.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.0.1/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.755042 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.2.0/206.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.2.0/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.756042 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)       45 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.3.0/197.md
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.3.0/203.md
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.3.0/208.md
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.3.0/209.md
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.3.0/210.md
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.3.0/212.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.3.0/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.756042 faraday_agent_dispatcher-3.3.0/CHANGELOG/current/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/current/.keep
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/footer.md
+-rw-rw-rw-   0 root         (0) root         (0)     3711 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)       93 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)    17119 2024-03-12 18:13:15.785042 faraday_agent_dispatcher-3.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6247 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     9126 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/RELEASE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.717042 faraday_agent_dispatcher-3.3.0/docker/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.757042 faraday_agent_dispatcher-3.3.0/docker/plugins-docker/
+-rw-rw-rw-   0 root         (0) root         (0)     3095 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docker/plugins-docker/Dockerfile
+-rwxrwxrwx   0 root         (0) root         (0)      802 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docker/plugins-docker/docker.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.757042 faraday_agent_dispatcher-3.3.0/docker/publish/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docker/publish/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      588 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docker/publish/Dockerfile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.758042 faraday_agent_dispatcher-3.3.0/docker/publish/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2059 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docker/publish/templates/template_dispatcher.ini
+-rw-rw-rw-   0 root         (0) root         (0)     4473 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docker/publish/templates/template_dispatcher.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2227 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docker/publish/templates/template_dispatcher_with_report.ini
+-rw-rw-rw-   0 root         (0) root         (0)     4830 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docker/publish/templates/template_dispatcher_with_report.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.758042 faraday_agent_dispatcher-3.3.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.759042 faraday_agent_dispatcher-3.3.0/docs/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/418.md
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/CNAME
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.759042 faraday_agent_dispatcher-3.3.0/docs/docs/css/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/css/faraday_doc.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.759042 faraday_agent_dispatcher-3.3.0/docs/docs/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/examples/new-custom-executor.md
+-rw-rw-rw-   0 root         (0) root         (0)     9813 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/getting-started.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.761042 faraday_agent_dispatcher-3.3.0/docs/docs/images/
+-rw-rw-rw-   0 root         (0) root         (0)    31633 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/agent_example.png
+-rw-rw-rw-   0 root         (0) root         (0)    44658 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/arch.png
+-rw-rw-rw-   0 root         (0) root         (0)    20584 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/arch_dispatcher.png
+-rw-rw-rw-   0 root         (0) root         (0)    26625 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/arch_executors.png
+-rw-rw-rw-   0 root         (0) root         (0)    21253 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/executor_example.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.718042 faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.762042 faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/qualys/
+-rw-rw-rw-   0 root         (0) root         (0)    54521 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/qualys/check_profile.png
+-rw-rw-rw-   0 root         (0) root         (0)   280745 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/qualys/new_profile.png
+-rw-rw-rw-   0 root         (0) root         (0)   194186 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/qualys/profileid.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.763042 faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/sonarqube/
+-rw-rw-rw-   0 root         (0) root         (0)    34458 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/sonarqube/generate_token.png
+-rw-rw-rw-   0 root         (0) root         (0)    10160 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/sonarqube/profile_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     3175 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/favicon.png
+-rw-rw-rw-   0 root         (0) root         (0)      581 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)    20392 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/token.png
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.763042 faraday_agent_dispatcher-3.3.0/docs/docs/js/
+-rw-rw-rw-   0 root         (0) root         (0)     2051 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/js/details.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.765042 faraday_agent_dispatcher-3.3.0/docs/docs/misc/
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/misc/appscan.md
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/misc/docker.md
+-rw-rw-rw-   0 root         (0) root         (0)     1545 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/misc/qualys.md
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/misc/sonarqube.md
+-rw-rw-rw-   0 root         (0) root         (0)     2059 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/misc/template_dispatcher.ini
+-rw-rw-rw-   0 root         (0) root         (0)     4473 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/misc/template_dispatcher.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2227 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/misc/template_dispatcher_with_report.ini
+-rw-rw-rw-   0 root         (0) root         (0)     4830 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/misc/template_dispatcher_with_report.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      767 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/misc/tenableio.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.765042 faraday_agent_dispatcher-3.3.0/docs/docs/technical/
+-rw-rw-rw-   0 root         (0) root         (0)     6633 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/technical/agents.md
+-rw-rw-rw-   0 root         (0) root         (0)     1770 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/technical/arch.md
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/mkdocs.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.767042 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/
+-rw-rw-rw-   0 root         (0) root         (0)      883 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.769042 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5447 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.770042 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/utils/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2991 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/utils/general_inputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      558 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/utils/general_prompts.py
+-rw-rw-rw-   0 root         (0) root         (0)    12031 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/utils/model_load.py
+-rw-rw-rw-   0 root         (0) root         (0)     9859 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    14016 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    27418 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)    35094 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/dispatcher_io.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/example_config.ini
+-rw-rw-rw-   0 root         (0) root         (0)      165 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/example_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6288 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/executor_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     3858 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.720042 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.720042 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.775042 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/
+-rw-rw-rw-   0 root         (0) root         (0)     9484 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/appscan.py
+-rw-rw-rw-   0 root         (0) root         (0)     3269 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/arachni.py
+-rw-rw-rw-   0 root         (0) root         (0)     9215 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/burp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7449 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/codeql.py
+-rw-rw-rw-   0 root         (0) root         (0)     3808 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/crackmapexec.py
+-rw-rw-rw-   0 root         (0) root         (0)     4786 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/dependabot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2546 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/github_secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     6135 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/gvm_openvas.py
+-rw-rw-rw-   0 root         (0) root         (0)     6447 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/insightvm.py
+-rwxrwxrwx   0 root         (0) root         (0)    11430 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/nessus.py
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/nikto2.py
+-rwxrwxrwx   0 root         (0) root         (0)     3551 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/nmap.py
+-rwxrwxrwx   0 root         (0) root         (0)     3152 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/nuclei.py
+-rw-rw-rw-   0 root         (0) root         (0)     4424 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/openvas_legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6205 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/qualys.py
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/report_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2010 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/shodan2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4734 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/sonarqube.py
+-rwxrwxrwx   0 root         (0) root         (0)      887 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/sublist3r.sh
+-rw-rw-rw-   0 root         (0) root         (0)     4134 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/tenableio.py
+-rw-rw-rw-   0 root         (0) root         (0)     3960 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/w3af.py
+-rw-rw-rw-   0 root         (0) root         (0)     2521 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/wpscan.py
+-rw-rw-rw-   0 root         (0) root         (0)     2416 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/wpscan_legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/zap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.776042 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3861 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/utils/control_values_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2217 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/utils/metadata_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      281 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/utils/text_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/utils/url_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.783042 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17119 2024-03-12 18:13:15.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10813 2024-03-12 18:13:15.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-12 18:13:15.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2024-03-12 18:13:15.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-12 18:13:15.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      345 2024-03-12 18:13:15.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-03-12 18:13:15.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      466 2024-03-12 18:13:15.785042 faraday_agent_dispatcher-3.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3103 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.776042 faraday_agent_dispatcher-3.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.778042 faraday_agent_dispatcher-3.3.0/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/basic_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/mock.pub
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/ok.crt
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/ok.key
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.780042 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/0.1.ini
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/0.1_with_agent_token.ini
+-rw-rw-rw-   0 root         (0) root         (0)      507 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.0.ini
+-rw-rw-rw-   0 root         (0) root         (0)      359 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.0_error0.ini
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.0_error1.ini
+-rw-rw-rw-   0 root         (0) root         (0)      578 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.0_with_agent_token.ini
+-rw-rw-rw-   0 root         (0) root         (0)      611 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.2.ini
+-rw-rw-rw-   0 root         (0) root         (0)      681 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.2_with_agent_token.ini
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.5.ini
+-rw-rw-rw-   0 root         (0) root         (0)      822 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/test_config.ini
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/wrong.crt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.780042 faraday_agent_dispatcher-3.3.0/tests/integration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.780042 faraday_agent_dispatcher-3.3.0/tests/integration/faraday/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/integration/faraday/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7330 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/integration/faraday/test_execution.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.781042 faraday_agent_dispatcher-3.3.0/tests/plugins-docker/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/plugins-docker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3674 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/plugins-docker/test_executors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.782042 faraday_agent_dispatcher-3.3.0/tests/unittests/
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/unittests/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/unittests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.782042 faraday_agent_dispatcher-3.3.0/tests/unittests/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/unittests/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    46373 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/unittests/config/agent_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)    37399 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/unittests/config/wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    12779 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/unittests/test_agent_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     5088 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/unittests/test_config_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/unittests/test_import_official_executors.py
+-rw-rw-rw-   0 root         (0) root         (0)     7983 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/unittests/wizard_input.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.783042 faraday_agent_dispatcher-3.3.0/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9651 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/utils/testing_faraday_server.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/utils/text_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      571 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tox.ini
```

### Comparing `faraday_agent_dispatcher-3.2.1/.gitignore` & `faraday_agent_dispatcher-3.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/.gitlab/ci/.pre-gitlab-ci.yml` & `faraday_agent_dispatcher-3.3.0/.gitlab/ci/.pre-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/.gitlab/ci/build_ci/.build-gitlab-ci.yml` & `faraday_agent_dispatcher-3.3.0/.gitlab/ci/build_ci/.build-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/.gitlab/ci/fetch-secrets.yml` & `faraday_agent_dispatcher-3.3.0/.gitlab/ci/fetch-secrets.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/.gitlab/ci/plugins-integration/.build-gitlab-ci.yml` & `faraday_agent_dispatcher-3.3.0/.gitlab/ci/plugins-integration/.build-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/.gitlab/ci/plugins-integration/.testing-gitlab-ci.yml` & `faraday_agent_dispatcher-3.3.0/.gitlab/ci/plugins-integration/.testing-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/.gitlab/ci/publish/.publish-dockerhub-gitlab-ci.yml` & `faraday_agent_dispatcher-3.3.0/.gitlab/ci/publish/.publish-dockerhub-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/.gitlab/ci/testing/.testing-gitlab-ci.yml` & `faraday_agent_dispatcher-3.3.0/.gitlab/ci/testing/.testing-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/.gitlab-ci.yml` & `faraday_agent_dispatcher-3.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/.pre-commit-config.yaml` & `faraday_agent_dispatcher-3.3.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     -   id: check-json
     -   id: check-yaml
         args: [ --unsafe ]
     -   id: debug-statements
     #-   id: name-tests-test
     #-   id: requirements-txt-fixer
     #-   id: double-quote-string-fixer
--   repo: https://gitlab.com/pycqa/flake8
+-   repo: https://github.com/pycqa/flake8
     rev: 3.9.1
     hooks:
     -   id: flake8
         additional_dependencies: [flake8-typing-imports==1.9.0]
 -   repo: https://github.com/psf/black
     rev: 22.3.0
     hooks:
```

### Comparing `faraday_agent_dispatcher-3.2.1/CONTRIBUTING.rst` & `faraday_agent_dispatcher-3.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/COPYING` & `faraday_agent_dispatcher-3.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/Makefile` & `faraday_agent_dispatcher-3.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/PKG-INFO` & `faraday_agent_dispatcher-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faraday_agent_dispatcher
-Version: 3.2.1
+Version: 3.3.0
 Summary: Faraday agent dispatcher to communicate an agent to faraday
 Home-page: https://github.com/infobyte/faraday_agent_dispatcher
 Author: Faraday Development Team
 Author-email: devel@infobytesec.com
 License: GNU General Public License v3
 Keywords: faraday integration
 Classifier: Development Status :: 5 - Production/Stable
@@ -207,14 +207,23 @@
 
 For more info you can check our [documentation][doc]
 
 [doc]: https://docs.agents.faradaysec.com
 [API]: https://api.faradaysec.com/
 
 
+3.3.0 [Mar 12th, 2024]:
+---
+ * [ADD] Add hotspots option to SonarQube. #197
+ * [ADD] New GitHub CodeQL agent. #208
+ * [ADD] Added new agent for GitHub Secrets Scanning. #209
+ * [MOD] Now Nessus executor tries to login again after a 401 response from the Nessus's server. #203
+ * [MOD] Change Dependabot agent to work with the new manifest of parameter types. #210
+ * [FIX] We were not verifying the configuration value `ignore_ssl` at the moment of `socketio` connection. #212
+
 3.2.0 [Feb 8th, 2024]:
 ---
  * [ADD] Add dependabot agent. #206
 
 3.0.1 [Dec 22th, 2023]:
 ---
  * [FIX] Fix on_diconnect method and limit python-socketio to 5.8.0 #199
```

### Comparing `faraday_agent_dispatcher-3.2.1/README.md` & `faraday_agent_dispatcher-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/RELEASE.md` & `faraday_agent_dispatcher-3.3.0/RELEASE.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+3.3.0 [Mar 12th, 2024]:
+---
+ * [ADD] Add hotspots option to SonarQube. #197
+ * [ADD] New GitHub CodeQL agent. #208
+ * [ADD] Added new agent for GitHub Secrets Scanning. #209
+ * [MOD] Now Nessus executor tries to login again after a 401 response from the Nessus's server. #203
+ * [MOD] Change Dependabot agent to work with the new manifest of parameter types. #210
+ * [FIX] We were not verifying the configuration value `ignore_ssl` at the moment of `socketio` connection. #212
+
 3.2.0 [Feb 8th, 2024]:
 ---
  * [ADD] Add dependabot agent. #206
 
 3.0.1 [Dec 22th, 2023]:
 ---
  * [FIX] Fix on_diconnect method and limit python-socketio to 5.8.0 #199
```

### Comparing `faraday_agent_dispatcher-3.2.1/docker/plugins-docker/Dockerfile` & `faraday_agent_dispatcher-3.3.0/docker/plugins-docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docker/plugins-docker/docker.sh` & `faraday_agent_dispatcher-3.3.0/docker/plugins-docker/docker.sh`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docker/publish/Dockerfile` & `faraday_agent_dispatcher-3.3.0/docker/publish/Dockerfile`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docker/publish/templates/template_dispatcher.ini` & `faraday_agent_dispatcher-3.3.0/docker/publish/templates/template_dispatcher.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docker/publish/templates/template_dispatcher.yaml` & `faraday_agent_dispatcher-3.3.0/docker/publish/templates/template_dispatcher.yaml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docker/publish/templates/template_dispatcher_with_report.ini` & `faraday_agent_dispatcher-3.3.0/docker/publish/templates/template_dispatcher_with_report.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docker/publish/templates/template_dispatcher_with_report.yaml` & `faraday_agent_dispatcher-3.3.0/docker/publish/templates/template_dispatcher_with_report.yaml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/.gitlab-ci.yml` & `faraday_agent_dispatcher-3.3.0/docs/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/getting-started.md` & `faraday_agent_dispatcher-3.3.0/docs/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/images/agent_example.png` & `faraday_agent_dispatcher-3.3.0/docs/docs/images/agent_example.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/images/arch.png` & `faraday_agent_dispatcher-3.3.0/docs/docs/images/arch.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/images/arch_dispatcher.png` & `faraday_agent_dispatcher-3.3.0/docs/docs/images/arch_dispatcher.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/images/arch_executors.png` & `faraday_agent_dispatcher-3.3.0/docs/docs/images/arch_executors.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/images/executor_example.png` & `faraday_agent_dispatcher-3.3.0/docs/docs/images/executor_example.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/images/executors/qualys/check_profile.png` & `faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/qualys/check_profile.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/images/executors/qualys/new_profile.png` & `faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/qualys/new_profile.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/images/executors/qualys/profileid.png` & `faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/qualys/profileid.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/images/executors/sonarqube/generate_token.png` & `faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/sonarqube/generate_token.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/images/executors/sonarqube/profile_icon.png` & `faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/sonarqube/profile_icon.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/images/favicon.png` & `faraday_agent_dispatcher-3.3.0/docs/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/images/logo.svg` & `faraday_agent_dispatcher-3.3.0/docs/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/images/token.png` & `faraday_agent_dispatcher-3.3.0/docs/docs/images/token.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/index.md` & `faraday_agent_dispatcher-3.3.0/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/js/details.js` & `faraday_agent_dispatcher-3.3.0/docs/docs/js/details.js`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/misc/appscan.md` & `faraday_agent_dispatcher-3.3.0/docs/docs/misc/appscan.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/misc/docker.md` & `faraday_agent_dispatcher-3.3.0/docs/docs/misc/docker.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/misc/qualys.md` & `faraday_agent_dispatcher-3.3.0/docs/docs/misc/qualys.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/misc/sonarqube.md` & `faraday_agent_dispatcher-3.3.0/docs/docs/misc/sonarqube.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/misc/template_dispatcher.ini` & `faraday_agent_dispatcher-3.3.0/docs/docs/misc/template_dispatcher.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/misc/template_dispatcher.yaml` & `faraday_agent_dispatcher-3.3.0/docs/docs/misc/template_dispatcher.yaml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/misc/template_dispatcher_with_report.ini` & `faraday_agent_dispatcher-3.3.0/docs/docs/misc/template_dispatcher_with_report.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/misc/template_dispatcher_with_report.yaml` & `faraday_agent_dispatcher-3.3.0/docs/docs/misc/template_dispatcher_with_report.yaml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/misc/tenableio.md` & `faraday_agent_dispatcher-3.3.0/docs/docs/misc/tenableio.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/technical/agents.md` & `faraday_agent_dispatcher-3.3.0/docs/docs/technical/agents.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/docs/technical/arch.md` & `faraday_agent_dispatcher-3.3.0/docs/docs/technical/arch.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/docs/mkdocs.yml` & `faraday_agent_dispatcher-3.3.0/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/__init__.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 """Top-level package for faraday_agent_dispatcher."""
 
 __author__ = """Faraday Development Team"""
 __email__ = "devel@infobytesec.com"
-__version__ = "3.2.1"
+__version__ = "3.3.0"
```

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/cli/main.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 import click
 import asyncio
 
 from aiohttp import ClientSession
 
 from faraday_agent_dispatcher.cli.wizard import Wizard, DEFAULT_PAGE_SIZE
-from faraday_agent_dispatcher.dispatcher_io import Dispatcher, sio, DispatcherNamespace
+from faraday_agent_dispatcher.dispatcher_io import Dispatcher, DispatcherNamespace
 from faraday_agent_dispatcher import config, __version__
 from faraday_agent_dispatcher.utils.text_utils import Bcolors
 import faraday_agent_dispatcher.logger as logging
 from pathlib import Path
 
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
@@ -69,22 +69,23 @@
                 getattr(signal, signame),
                 lambda: asyncio.ensure_future(dispatcher.close(signame)),
             )
 
         await dispatcher.register(token)
         namespace = DispatcherNamespace(namespace="/dispatcher")
         namespace.dispatcher = dispatcher
-        sio.register_namespace(namespace)
+        dispatcher.sio.register_namespace(namespace)
         schema = "http"
         if dispatcher.api_ssl_enabled:
             schema = "https"
         uri = f"{schema}://{namespace.dispatcher.host}:{namespace.dispatcher.websocket_port}"
         logger.info(f"Trying to connect to: {uri}")
-        await sio.connect(uri)
-        await sio.wait()
+
+        await dispatcher.sio.connect(uri)
+        await dispatcher.sio.wait()
 
     return 0 if dispatcher.sigterm_received else 1
 
 
 @click.command(help="faraday-dispatcher run")
 @click.option("-c", "--config-file", default=None, help="Path to config ini file")
 @click.option("--logdir", default="~", help="Path to logger directory")
```

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/cli/utils/general_inputs.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/utils/general_inputs.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/cli/utils/general_prompts.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/utils/general_prompts.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/cli/utils/model_load.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/utils/model_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 def append_keys(agent_dict, section):
     agent_dict[section]["api_port"] = {
         "default_value": lambda _ssl: "443" if _ssl else "5985",
         "type": click.IntRange(min=1, max=65535),
     }
     agent_dict[section]["websocket_port"] = {
-        "default_value": lambda _ssl: "443" if _ssl else "9000",
+        "default_value": lambda _ssl: "443" if _ssl else "5985",
         "type": click.IntRange(min=1, max=65535),
     }
     return agent_dict
 
 
 def url_setting(url):
     url_info = {
@@ -51,15 +51,15 @@
     if url_info["check_ssl"] is not None:
         if url_host.scheme == "http":
             if url_host.port:
                 url_info["api_port"] = url_host.port
                 url_info["websocket_port"] = url_host.port
             else:
                 url_info["api_port"] = 5985
-                url_info["websocket_port"] = 9000
+                url_info["websocket_port"] = 5985
             url_info["check_ssl"] = False
         elif url_host.scheme == "https":
             if url_host.port:
                 url_info["api_port"] = url_host.port
                 url_info["websocket_port"] = url_host.port
             else:
                 url_info["api_port"] = 443
```

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/cli/wizard.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/wizard.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/config.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/config.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/dispatcher.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/dispatcher.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/dispatcher_io.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/dispatcher_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import os
 import ssl
 import json
 
+import aiohttp
 import socketio
 import asyncio
 from datetime import datetime
 from pathlib import Path
 from asyncio import Task
 from typing import List, Dict
 import sys
@@ -59,15 +60,14 @@
 )
 from faraday_agent_dispatcher.cli.utils.model_load import set_repo_params
 from faraday_agent_dispatcher.executor import Executor
 from faraday_agent_parameters_types.utils import type_validate
 
 logger = logging.get_logger()
 logging.setup_logging()
-sio = socketio.AsyncClient(engineio_logger=False, logger=False)
 
 
 class Dispatcher:
     class TaskLabels:
         CONNECTION_CHECK = "Connection check"
         EXECUTOR = "EXECUTOR"
 
@@ -91,30 +91,41 @@
         self.websocket = None
         self.websocket_token = None
         self.executors = {
             executor_name: Executor(executor_name, executor_data)
             for executor_name, executor_data in config.instance[Sections.AGENT].get("executors", {}).items()
         }
         self.ws_ssl_enabled = self.api_ssl_enabled = config.instance[Sections.SERVER].get("ssl", False)
+        self.sio = socketio.AsyncClient()
         ssl_cert_path = config.instance[Sections.SERVER].get("ssl_cert", None)
         ssl_ignore = config.instance[Sections.SERVER].get("ssl_ignore", False)
         if not Path(ssl_cert_path).exists():
             raise ValueError(f"SSL cert does not exist in path {ssl_cert_path}")
         if self.api_ssl_enabled:
+            logger.info("api_ssl is enabled")
             if ssl_cert_path:
                 ssl_cert_context = ssl.create_default_context(cafile=ssl_cert_path)
                 self.api_kwargs = {"ssl": ssl_cert_context}
                 self.ws_kwargs = {"ssl": ssl_cert_context}
+                connector = aiohttp.TCPConnector(ssl=ssl_cert_context)
+                http_session = aiohttp.ClientSession(connector=connector)
+                self.sio = socketio.AsyncClient(http_session=http_session)
             else:
                 if ssl_ignore or "HTTPS_PROXY" in os.environ:
+                    logger.info(f"ssl_ignore config is {ssl_ignore}")
+                    if "HTTPS_PROXY" in os.environ:
+                        logger.info("HTTPS_PROXY variable found in environment")
                     ignore_ssl_context = ssl.create_default_context()
                     ignore_ssl_context.check_hostname = False
                     ignore_ssl_context.verify_mode = ssl.CERT_NONE
                     self.api_kwargs = {"ssl": ignore_ssl_context}
                     self.ws_kwargs = {"ssl": ignore_ssl_context}
+                    connector = aiohttp.TCPConnector(ssl=ignore_ssl_context)
+                    http_session = aiohttp.ClientSession(connector=connector)
+                    self.sio = socketio.AsyncClient(http_session=http_session)
                 else:
                     self.api_kwargs: Dict[str, object] = {}
                     self.ws_kwargs: Dict[str, object] = {}
         else:
             self.api_kwargs: Dict[str, object] = {}
             self.ws_kwargs: Dict[str, object] = {}
         self.execution_ids = None
```

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/example_config.ini` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/example_config.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [server]
 host = localhost
 api_port = 5985
-websocket_port = 9000
+websocket_port = 5985
 ssl = False
 ssl_cert =
 
 [agent]
 agent_name = unnamed_agent
 ; Complete the executor option with a comma separated list of executor names
 executors = ex1,ex2
```

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/executor.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/executor.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/executor_helper.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/executor_helper.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/logger.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/logger.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/appscan.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/appscan.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/arachni.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/arachni.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/burp.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/burp.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/crackmapexec.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/crackmapexec.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/dependabot.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/dependabot.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 import os
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 def main():
-    DEPENDABOT_OWNER = os.getenv("EXECUTOR_CONFIG_DEPENDABOT_OWNER")
-    DEPENDABOT_REPOSITORY = os.getenv("EXECUTOR_CONFIG_DEPENDABOT_REPOSITORY")
-    DEPENDABOT_TOKEN = os.getenv("DEPENDABOT_TOKEN")
+    GITHUB_REPOSITORY = os.getenv("EXECUTOR_CONFIG_GITHUB_REPOSITORY")
+    GITHUB_OWNER = os.getenv("GITHUB_OWNER")
+    GITHUB_TOKEN = os.getenv("GITHUB_TOKEN")
 
     vuln_tag = os.getenv("AGENT_CONFIG_VULN_TAG", [])
     if vuln_tag:
         vuln_tag = vuln_tag.split(",")
     host_tag = os.getenv("AGENT_CONFIG_HOSTNAME_TAG", [])
     if host_tag:
         host_tag = host_tag.split(",")
 
     # TODO: should validate config?
-    dependabot_url = f"https://api.github.com/repos/{DEPENDABOT_OWNER}/{DEPENDABOT_REPOSITORY}/dependabot/alerts"
-    dependabot_auth = {"Authorization": f"Bearer {DEPENDABOT_TOKEN}"}
-    repo_url = f"https://github.com/{DEPENDABOT_OWNER}/{DEPENDABOT_REPOSITORY}"
+    dependabot_url = f"https://api.github.com/repos/{GITHUB_OWNER}/{GITHUB_REPOSITORY}/dependabot/alerts"
+    github_auth = {"Authorization": f"Bearer {GITHUB_TOKEN}"}
+    repo_url = f"https://github.com/{GITHUB_OWNER}/{GITHUB_REPOSITORY}"
 
     CVSS_3_PREFIX = "CVSS:3"
 
-    response = requests.get(dependabot_url, headers=dependabot_auth)
+    response = requests.get(dependabot_url, headers=github_auth)
 
     if response.status_code == http.HTTPStatus.OK:
         security_events = response.json()
         hosts_ips = list({security_event["dependency"]["manifest_path"] for security_event in security_events})
         hosts = []
 
         for ip in hosts_ips:
@@ -89,15 +89,15 @@
                         else:
                             vulnerability.update({"cvss2": {"vector_string": cvss_vector_string.strip("CVSS:")[-1]}})
 
                     host_vulns.append(vulnerability)
 
             hosts.append(
                 {
-                    "ip": f"{DEPENDABOT_OWNER}/{DEPENDABOT_REPOSITORY}/{ip}",
+                    "ip": f"{GITHUB_OWNER}/{GITHUB_REPOSITORY}/{ip}",
                     "description": f"Dependabot recommendations on file {ip}\n\nRepository: {repo_url}",
                     "hostnames": [],
                     "vulnerabilities": host_vulns,
                     "tags": host_tag,
                 }
             )
```

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/gvm_openvas.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/gvm_openvas.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/insightvm.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/insightvm.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/nessus.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/nessus.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,32 +6,69 @@
 import time
 import requests
 import datetime
 from posixpath import join as urljoin
 
 from faraday_plugins.plugins.repo.nessus.plugin import NessusPlugin
 
-MAX_TRIES = 3
+import urllib3
+
+urllib3.disable_warnings()
+
+MAX_TRIES = 1000
 TIME_BETWEEN_TRIES = 5
 
 
 def get_report_name():
     return f"{datetime.datetime.now().timestamp()}-faraday-agent"
 
 
+def log(msg):
+    print(msg, file=sys.stderr)
+
+
+def get_token_and_x_token(url, username, password):
+    token = nessus_login(url, username, password)
+    if not token:
+        sys.exit(1)
+
+    x_token = get_x_api_token(url, token)
+    if not x_token:
+        sys.exit(1)
+    return token, x_token
+
+
+def get_scans(url, scan_name, token, x_token):
+    headers = {"X-Cookie": f"token={token}", "X-API-Token": x_token}
+    response = requests.get(urljoin(url, "scans/"), headers=headers, verify=False, timeout=600)
+    if response.status_code != 200:
+        log("Could not get scan list. Response from server was" f" {response.status_code}")
+        return None
+    for scan in response.json().get("scans", []):
+        if scan["name"] == scan_name:
+            if scan["status"].lower() == "running":
+                log(
+                    "A scan with the NESSUS_SCAN_NAME provided was found but is running,"
+                    "choose a different NESSUS_SCAN_NAME, cancel the scan manually or wait to finish"
+                )
+                exit(1)
+            log(f'Scan {scan_name} was found with id {scan["id"]}')
+            return scan["id"]
+
+
 def nessus_login(url, user, password):
     payload = {"username": user, "password": password}
     response = requests.post(urljoin(url, "session"), payload, verify=False, timeout=60)
 
     if response.status_code == 200:
         if response.headers["content-type"].lower() == "application/json" and "token" in response.json():
             return response.json()["token"]
-        print("Nessus did not response with a valid token", file=sys.stderr)
+        log("Nessus did not response with a valid token")
     else:
-        print(f"Login failed with status {response.status_code}", file=sys.stderr)
+        log(f"Login failed with status {response.status_code}")
 
     return None
 
 
 def nessus_templates(url, token, x_token):
     headers = {"X-Cookie": "token={}".format(token), "X-API-Token": x_token}
     payload = {}
@@ -52,25 +89,19 @@
     return None
 
 
 def nessus_add_target(url, token, x_token, target="", template="basic", name="nessus_scan"):
     headers = {"X-Cookie": f"token={token}", "X-API-Token": x_token}
     templates = nessus_templates(url, token, x_token)
     if not templates:
-        print("Templates not available", file=sys.stderr)
+        log("Templates not available")
         return None
     if template not in templates:
-        print(
-            f"Template {template} not valid. Setting basic as default",
-            file=sys.stderr,
-        )
-        print(
-            f"The templates available are {list(templates.keys())}",
-            file=sys.stderr,
-        )
+        log(f"Template {template} not valid. Setting basic as default")
+        log(f"The templates available are {list(templates.keys())}")
         template = "basic"
 
     payload = {
         "uuid": "{}".format(templates[template]),
         "settings": {
             "name": "{}".format(name),
             "enabled": True,
@@ -84,113 +115,116 @@
         response.status_code == 200
         and response.headers["content-type"].lower() == "application" "/json"
         and "scan" in response.json()
         and "id" in response.json()["scan"]
     ):
         return response.json()["scan"]["id"]
     else:
-        print(
-            f"Could not create scan. Response from server was " f"{response.status_code}, {response.text}",
-            file=sys.stderr,
-        )
+        log(f"Could not create scan. Response from server was " f"{response.status_code}, {response.text}")
     return None
 
 
-def nessus_scan_run(url, scan_id, token, x_token):
+def nessus_scan_run(url, scan_id, token, x_token, username, password):
     headers = {"X-Cookie": f"token={token}", "X-API-Token": x_token}
 
-    response = requests.post(urljoin(url, f"scans/{scan_id}/launch"), headers=headers, verify=False, timeout=60)
+    response = requests.post(urljoin(url, f"scans/{scan_id}/launch"), headers=headers, verify=False, timeout=600)
     if response.status_code != 200:
-        print(
-            "Could not launch scan. Response from server was" f" {response.status_code}",
-            file=sys.stderr,
-        )
+        log("Could not launch scan. Response from server was" f" {response.status_code}")
         return None
 
     status = "running"
     tries = 0
     while status == "running":
-        response = requests.get(urljoin(url, f"scans/{scan_id}"), headers=headers, verify=False, timeout=60)
+        response = requests.get(urljoin(url, f"scans/{scan_id}"), headers=headers, verify=False, timeout=600)
         if response.status_code == 200:
             if (
                 response.headers["content-type"].lower() == "application/json"
                 and "info" in response.json()
                 and "status" in response.json()["info"]
             ):
                 status = response.json()["info"]["status"]
             else:
-                print(
-                    "The nessus server give a 200 with unexpected response",
-                    file=sys.stderr,
-                )
+                log("The nessus server give a 200 with unexpected response")
                 status = "error"
         else:
             if tries == MAX_TRIES:
                 status = "error"
-                print(
+                log(
                     "Could not get scan status. Response from server was "
                     f"{response.status_code}. This error ocurred {tries} "
-                    f"time[s]",
-                    file=sys.stderr,
+                    f"time[s]"
                 )
+            if response.status_code == 401:
+                log("The nessus respond with a 401 status code, I'm login and try again")
+                # Some scans take too long and the token expires
+                token = nessus_login(url, username, password)
+                if not token:
+                    sys.exit(1)
+
+                x_token = get_x_api_token(url, token)
+                if not x_token:
+                    sys.exit(1)
+                headers = {"X-Cookie": "token={}".format(token), "X-API-Token": x_token}
+            else:
+                log(f"Try number {tries}")
             tries += 1
         time.sleep(TIME_BETWEEN_TRIES)
     return status
 
 
-def nessus_scan_export(url, scan_id, token, x_token):
+def nessus_scan_export(url, scan_id, token, x_token, username, password):
     headers = {"X-Cookie": "token={}".format(token), "X-API-Token": x_token}
 
     response = requests.post(
-        urljoin(url, f"scans/{scan_id}/export?limit=2500"),
+        urljoin(url, f"scans/{scan_id}/export?limit=500000"),
         data={"format": "nessus"},
         headers=headers,
         verify=False,
-        timeout=60,
+        timeout=600,
     )
     if (
         response.status_code == 200
         and response.headers["content-type"].lower() == "application" "/json"
         and "token" in response.json()
     ):
         export_token = response.json()["token"]
     else:
-        print(
-            f"Export failed with status {response.status_code}",
-            file=sys.stderr,
-        )
+        log(f"Export failed with status {response.status_code}")
         return None
 
     status = "processing"
     tries = 0
     while status != "ready":
-        response = requests.get(urljoin(url, f"tokens/{export_token}/status"), verify=False, timeout=60)
+        response = requests.get(urljoin(url, f"tokens/{export_token}/status"), verify=False, timeout=600)
         if response.status_code == 200:
             if response.headers["content-type"].lower() == "application/json" and "status" in response.json():
                 status = response.json()["status"]
             else:
-                print(
-                    "The nessus server give a 200 with unexpected response",
-                    file=sys.stderr,
-                )
+                log("The nessus server give a 200 with unexpected response")
                 status = "error"
         else:
             if tries == MAX_TRIES:
                 status = "error"
-                print(
+                log(
                     "Could not get export status. Response from server was "
                     f"{response.status_code}. This error ocurred {tries}"
-                    f"time[s]",
-                    file=sys.stderr,
+                    f"time[s]"
                 )
+            if response.status_code == 401:
+                log("The nessus respond with a 401 status code, I'm login and try again")
+                # Some scans take too long and the token expires
+                nessus_login(url, username, password)
+            else:
+                log(f"Try number {tries}")
+
             tries += 1
 
         time.sleep(TIME_BETWEEN_TRIES)
 
-    print(f"Report export status {status}", file=sys.stderr)
+    log(f"Report export status {status}")
     response = requests.get(
         urljoin(url, f"tokens/{export_token}/download"), allow_redirects=True, verify=False, timeout=60
     )
     if response.status_code == 200:
         return response.content
 
     return None
@@ -209,20 +243,17 @@
     response = requests.get(urljoin(url, "nessus6.js"), headers=headers, verify=False, timeout=60)
 
     if response.status_code == 200:
         matched = re.search(pattern, str(response.content))
         if matched:
             x_token = matched.group(1)
         else:
-            print("X-api-token not found :(", file=sys.stderr)
+            log("X-api-token not found :(")
     else:
-        print(
-            "Could not get x-api-token. Response from server was " f"{response.status_code}",
-            file=sys.stderr,
-        )
+        log("Could not get x-api-token. Response from server was " f"{response.status_code}")
 
     return x_token
 
 
 def main():
     ignore_info = os.getenv("AGENT_CONFIG_IGNORE_INFO", "False").lower() == "true"
     hostname_resolution = os.getenv("AGENT_CONFIG_RESOLVE_HOSTNAME", "True").lower() == "true"
@@ -248,51 +279,50 @@
         "EXECUTOR_CONFIG_NESSUS_SCAN_TEMPLATE",
         "basic",
     )
 
     if not NESSUS_URL:
         NESSUS_URL = os.getenv("NESSUS_URL")
         if not NESSUS_URL:
-            print("URL not provided", file=sys.stderr)
+            log("URL not provided")
             sys.exit(1)
 
     scan_file = None
 
-    token = nessus_login(NESSUS_URL, NESSUS_USERNAME, NESSUS_PASSWORD)
-    if not token:
-        sys.exit(1)
-
-    x_token = get_x_api_token(NESSUS_URL, token)
-    if not x_token:
-        sys.exit(1)
-
-    scan_id = nessus_add_target(
-        NESSUS_URL,
-        token,
-        x_token,
-        NESSUS_SCAN_TARGET,
-        NESSUS_SCAN_TEMPLATE,
-        NESSUS_SCAN_NAME,
-    )
+    token, x_token = get_token_and_x_token(NESSUS_URL, NESSUS_USERNAME, NESSUS_PASSWORD)
+    scan_id = get_scans(NESSUS_URL, NESSUS_SCAN_NAME, token, x_token)
+    # If NESSUS_SCAN_NAME is not found launch a new scan else relaunch the scan
     if not scan_id:
-        sys.exit(1)
-
-    status = nessus_scan_run(NESSUS_URL, scan_id, token, x_token)
+        if not NESSUS_SCAN_TARGET:
+            log("Scan name wasn't found and scan target wasn't provided. Exiting executor")
+            exit(1)
+        scan_id = nessus_add_target(
+            NESSUS_URL,
+            token,
+            x_token,
+            NESSUS_SCAN_TARGET,
+            NESSUS_SCAN_TEMPLATE,
+            NESSUS_SCAN_NAME,
+        )
+        if not scan_id:
+            sys.exit(1)
+    status = nessus_scan_run(NESSUS_URL, scan_id, token, x_token, NESSUS_USERNAME, NESSUS_PASSWORD)
     if status != "error":
-        scan_file = nessus_scan_export(NESSUS_URL, scan_id, token, x_token)
+        token, x_token = get_token_and_x_token(NESSUS_URL, NESSUS_USERNAME, NESSUS_PASSWORD)
+        scan_file = nessus_scan_export(NESSUS_URL, scan_id, token, x_token, NESSUS_USERNAME, NESSUS_PASSWORD)
 
     if scan_file:
         plugin = NessusPlugin(
             ignore_info=ignore_info,
             hostname_resolution=hostname_resolution,
             host_tag=host_tag,
             service_tag=service_tag,
             vuln_tag=vuln_tag,
         )
         plugin.parseOutputString(scan_file)
         print(plugin.get_json())
     else:
-        print("Scan file was empty", file=sys.stderr)
+        log("Scan file was empty")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/nikto2.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/nikto2.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/nmap.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/nmap.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/nuclei.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/nuclei.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/openvas_legacy.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/openvas_legacy.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/qualys.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/qualys.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/report_processor.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/report_processor.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/shodan2.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/shodan2.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/sonarqube.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/zap.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,86 +1,68 @@
-import json
+#!/usr/bin/env python
 import os
 import sys
-import requests
-from faraday_plugins.plugins.repo.sonarqubeapi.plugin import SonarQubeAPIPlugin
-
-# ATTENTION: We only want to find vulnerabilities. Code smell and bugs doesn't matters for us.
-TYPE_VULNS = "VULNERABILITY"
-PAGE_SIZE = 500
+import time
+import psutil
+from zapv2 import ZAPv2
+from faraday_plugins.plugins.repo.zap.plugin import ZapPlugin
 
 
 def main():
     # If the script is run outside the dispatcher the environment variables
     # are checked.
-    # ['EXECUTOR_CONFIG_TOKEN', 'EXECUTOR_CONFIG_URL', 'EXECUTOR_CONFIG_PROJECT']
+    # ['ZAP_API_KEY', 'EXECUTOR_CONFIG_TARGET_URL']
     ignore_info = os.getenv("AGENT_CONFIG_IGNORE_INFO", "False").lower() == "true"
     hostname_resolution = os.getenv("AGENT_CONFIG_RESOLVE_HOSTNAME", "True").lower() == "true"
     vuln_tag = os.getenv("AGENT_CONFIG_VULN_TAG", None)
     if vuln_tag:
         vuln_tag = vuln_tag.split(",")
     service_tag = os.getenv("AGENT_CONFIG_SERVICE_TAG", None)
     if service_tag:
         service_tag = service_tag.split(",")
     host_tag = os.getenv("AGENT_CONFIG_HOSTNAME_TAG", None)
     if host_tag:
         host_tag = host_tag.split(",")
-
     try:
-        sonar_qube_url = os.environ["SONAR_URL"]
-        token = os.environ["EXECUTOR_CONFIG_TOKEN"]
-        component_key = os.environ.get("EXECUTOR_CONFIG_COMPONENT_KEY", None)
+        target = os.environ["EXECUTOR_CONFIG_TARGET_URL"]
+        api_key = os.environ["ZAP_API_KEY"]
     except KeyError:
-        print("Environment variable not found", file=sys.stderr)
+        print("environment variable not found", file=sys.stderr)
         sys.exit()
 
-    session = requests.Session()
+    # zap is required to be started
+    if zap_is_running():
+        # the apikey from ZAP->Tools->Options-API
+        zap = ZAPv2(apikey=api_key)
+        # it passes the url to scan and starts
+        scanID = zap.spider.scan(target)
+        # Wait for the scan to finish
+        while int(zap.spider.status(scanID)) < 100:
+            time.sleep(1)
+        # If finish the scan and the xml is generated
+        zap_result = zap.core.xmlreport()
+        plugin = ZapPlugin(
+            ignore_info=ignore_info,
+            hostname_resolution=hostname_resolution,
+            host_tag=host_tag,
+            service_tag=service_tag,
+            vuln_tag=vuln_tag,
+        )
+        plugin.parseOutputString(zap_result)
+        print(plugin.get_json())
 
-    # ATTENTION: SonarQube API requires an empty password when auth method is via token
-    session.auth = (token, "")
+    else:
+        print("ZAP not running", file=sys.stderr)
+        sys.exit()
 
-    # Issues api config
-    page = 0
-    has_more_vulns = True
-
-    vulnerabilities = []
-
-    while has_more_vulns:
-        page += 1
-
-        params = {"types": TYPE_VULNS, "p": page, "ps": PAGE_SIZE}
-        if component_key:
-            params["componentKeys"] = component_key
-        try:
-            response = session.get(
-                url=f"{sonar_qube_url}/api/issues/search",
-                params=params,
-            )
-            response_json = response.json()
-        except Exception:
-            print(
-                f"There was an error finding issues. Component Key {component_key}; "
-                f"Status Code {response.status_code} - {response.content}",
-                file=sys.stderr,
-            )
-            sys.exit(1)
-
-        issues = response_json.get("issues")
-        vulnerabilities.extend(issues)
-        total_items = response_json.get("paging").get("total")
-
-        has_more_vulns = page * PAGE_SIZE < total_items
-
-    response_json["issues"] = vulnerabilities
-    sonar = SonarQubeAPIPlugin(
-        ignore_info=ignore_info,
-        hostname_resolution=hostname_resolution,
-        host_tag=host_tag,
-        service_tag=service_tag,
-        vuln_tag=vuln_tag,
-    )
-    sonar.parseOutputString(json.dumps(response_json))
-    print(sonar.get_json())
+
+def zap_is_running():
+    try:
+        for proc in psutil.process_iter():
+            if ("zap" in proc.cmdline()[-1]) if len(proc.cmdline()) > 0 else False:
+                return True
+    finally:
+        return False
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/sublist3r.sh` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/sublist3r.sh`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/tenableio.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/tenableio.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/w3af.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/w3af.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/wpscan.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/wpscan.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/static/executors/official/wpscan_legacy.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/wpscan_legacy.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/utils/control_values_utils.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/utils/control_values_utils.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/utils/metadata_utils.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/utils/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher/utils/url_utils.py` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/utils/url_utils.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher.egg-info/PKG-INFO` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faraday_agent_dispatcher
-Version: 3.2.1
+Version: 3.3.0
 Summary: Faraday agent dispatcher to communicate an agent to faraday
 Home-page: https://github.com/infobyte/faraday_agent_dispatcher
 Author: Faraday Development Team
 Author-email: devel@infobytesec.com
 License: GNU General Public License v3
 Keywords: faraday integration
 Classifier: Development Status :: 5 - Production/Stable
@@ -207,14 +207,23 @@
 
 For more info you can check our [documentation][doc]
 
 [doc]: https://docs.agents.faradaysec.com
 [API]: https://api.faradaysec.com/
 
 
+3.3.0 [Mar 12th, 2024]:
+---
+ * [ADD] Add hotspots option to SonarQube. #197
+ * [ADD] New GitHub CodeQL agent. #208
+ * [ADD] Added new agent for GitHub Secrets Scanning. #209
+ * [MOD] Now Nessus executor tries to login again after a 401 response from the Nessus's server. #203
+ * [MOD] Change Dependabot agent to work with the new manifest of parameter types. #210
+ * [FIX] We were not verifying the configuration value `ignore_ssl` at the moment of `socketio` connection. #212
+
 3.2.0 [Feb 8th, 2024]:
 ---
  * [ADD] Add dependabot agent. #206
 
 3.0.1 [Dec 22th, 2023]:
 ---
  * [FIX] Fix on_diconnect method and limit python-socketio to 5.8.0 #199
```

### Comparing `faraday_agent_dispatcher-3.2.1/faraday_agent_dispatcher.egg-info/SOURCES.txt` & `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,21 @@
 CHANGELOG/2.6.3/date.md
 CHANGELOG/3.0.0/195.md
 CHANGELOG/3.0.0/date.md
 CHANGELOG/3.0.1/199.md
 CHANGELOG/3.0.1/date.md
 CHANGELOG/3.2.0/206.md
 CHANGELOG/3.2.0/date.md
+CHANGELOG/3.3.0/197.md
+CHANGELOG/3.3.0/203.md
+CHANGELOG/3.3.0/208.md
+CHANGELOG/3.3.0/209.md
+CHANGELOG/3.3.0/210.md
+CHANGELOG/3.3.0/212.md
+CHANGELOG/3.3.0/date.md
 CHANGELOG/current/.keep
 docker/plugins-docker/Dockerfile
 docker/plugins-docker/docker.sh
 docker/publish/.dockerignore
 docker/publish/Dockerfile
 docker/publish/templates/template_dispatcher.ini
 docker/publish/templates/template_dispatcher.yaml
@@ -230,16 +237,18 @@
 faraday_agent_dispatcher/cli/utils/exceptions.py
 faraday_agent_dispatcher/cli/utils/general_inputs.py
 faraday_agent_dispatcher/cli/utils/general_prompts.py
 faraday_agent_dispatcher/cli/utils/model_load.py
 faraday_agent_dispatcher/static/executors/official/appscan.py
 faraday_agent_dispatcher/static/executors/official/arachni.py
 faraday_agent_dispatcher/static/executors/official/burp.py
+faraday_agent_dispatcher/static/executors/official/codeql.py
 faraday_agent_dispatcher/static/executors/official/crackmapexec.py
 faraday_agent_dispatcher/static/executors/official/dependabot.py
+faraday_agent_dispatcher/static/executors/official/github_secrets.py
 faraday_agent_dispatcher/static/executors/official/gvm_openvas.py
 faraday_agent_dispatcher/static/executors/official/insightvm.py
 faraday_agent_dispatcher/static/executors/official/nessus.py
 faraday_agent_dispatcher/static/executors/official/nikto2.py
 faraday_agent_dispatcher/static/executors/official/nmap.py
 faraday_agent_dispatcher/static/executors/official/nuclei.py
 faraday_agent_dispatcher/static/executors/official/openvas_legacy.py
```

### Comparing `faraday_agent_dispatcher-3.2.1/setup.py` & `faraday_agent_dispatcher-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tests/data/basic_executor.py` & `faraday_agent_dispatcher-3.3.0/tests/data/basic_executor.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tests/data/ok.crt` & `faraday_agent_dispatcher-3.3.0/tests/data/ok.crt`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tests/data/ok.key` & `faraday_agent_dispatcher-3.3.0/tests/data/ok.key`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tests/data/old_version_inis/1.0_with_agent_token.ini` & `faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.0_with_agent_token.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tests/data/old_version_inis/1.2.ini` & `faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.2.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tests/data/old_version_inis/1.2_with_agent_token.ini` & `faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.2_with_agent_token.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tests/data/old_version_inis/1.5.ini` & `faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.5.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tests/data/test_config.ini` & `faraday_agent_dispatcher-3.3.0/tests/data/test_config.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tests/data/wrong.crt` & `faraday_agent_dispatcher-3.3.0/tests/data/wrong.crt`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tests/integration/faraday/test_execution.py` & `faraday_agent_dispatcher-3.3.0/tests/integration/faraday/test_execution.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tests/plugins-docker/test_executors.py` & `faraday_agent_dispatcher-3.3.0/tests/plugins-docker/test_executors.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tests/unittests/config/agent_dispatcher.py` & `faraday_agent_dispatcher-3.3.0/tests/unittests/config/agent_dispatcher.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tests/unittests/config/wizard.py` & `faraday_agent_dispatcher-3.3.0/tests/unittests/config/wizard.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tests/unittests/test_agent_dispatcher.py` & `faraday_agent_dispatcher-3.3.0/tests/unittests/test_agent_dispatcher.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tests/unittests/test_config_wizard.py` & `faraday_agent_dispatcher-3.3.0/tests/unittests/test_config_wizard.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tests/unittests/test_import_official_executors.py` & `faraday_agent_dispatcher-3.3.0/tests/unittests/test_import_official_executors.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tests/unittests/wizard_input.py` & `faraday_agent_dispatcher-3.3.0/tests/unittests/wizard_input.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tests/utils/testing_faraday_server.py` & `faraday_agent_dispatcher-3.3.0/tests/utils/testing_faraday_server.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.2.1/tox.ini` & `faraday_agent_dispatcher-3.3.0/tox.ini`

 * *Files identical despite different names*

