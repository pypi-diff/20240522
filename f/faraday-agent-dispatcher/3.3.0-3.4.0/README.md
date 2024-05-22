# Comparing `tmp/faraday_agent_dispatcher-3.3.0.tar.gz` & `tmp/faraday_agent_dispatcher-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faraday_agent_dispatcher-3.3.0.tar", last modified: Tue Mar 12 18:13:15 2024, max compression
+gzip compressed data, was "faraday_agent_dispatcher-3.4.0.tar", last modified: Wed May 22 21:08:04 2024, max compression
```

## Comparing `faraday_agent_dispatcher-3.3.0.tar` & `faraday_agent_dispatcher-3.4.0.tar`

### file list

```diff
@@ -1,375 +1,384 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.785042 faraday_agent_dispatcher-3.3.0/
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.flake8
--rw-rw-rw-   0 root         (0) root         (0)     2366 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.712042 faraday_agent_dispatcher-3.3.0/.gitlab/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.725042 faraday_agent_dispatcher-3.3.0/.gitlab/ci/
--rw-rw-rw-   0 root         (0) root         (0)     1387 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/.pre-gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      508 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/.rules-conditions.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.725042 faraday_agent_dispatcher-3.3.0/.gitlab/ci/build_ci/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/build_ci/.build-gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      717 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/fetch-secrets.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.726042 faraday_agent_dispatcher-3.3.0/.gitlab/ci/plugins-integration/
--rw-rw-rw-   0 root         (0) root         (0)     1017 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/plugins-integration/.build-gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      877 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/plugins-integration/.testing-gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.726042 faraday_agent_dispatcher-3.3.0/.gitlab/ci/publish/
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/publish/.publish-dockerhub-gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      283 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/publish/.pypi-gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.727042 faraday_agent_dispatcher-3.3.0/.gitlab/ci/testing/
--rw-rw-rw-   0 root         (0) root         (0)      447 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/testing/.post-gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     2765 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab/ci/testing/.testing-gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1470 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      743 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/.pre-push-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/AUTHORS.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.727042 faraday_agent_dispatcher-3.3.0/CHANGELOG/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.728042 faraday_agent_dispatcher-3.3.0/CHANGELOG/0.1/
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/0.1/01.first version.md
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/0.1/02.minimal structure.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/0.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/0.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.729042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.0/
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.0/01.env_var.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.0/02.executor.md
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.0/03.params.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.0/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.730042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/01.run.md
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/02.wizard.md
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/03.01.manage_execution_id.md
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/03.02.change_ws_route.md
--rw-rw-rw-   0 root         (0) root         (0)       79 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/04.error_management.md
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/05.invalid token.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/06.ssl.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.732042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2/
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2/01.package_executor.md
--rw-rw-rw-   0 root         (0) root         (0)       31 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2/02.signal.md
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2/03.close_connection.md
--rw-rw-rw-   0 root         (0) root         (0)       46 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2/04.sslcert.md
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2/05.config_folder.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2/E00.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2/date.md
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.735042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/01.check_command_before_run.md
--rw-rw-rw-   0 root         (0) root         (0)       91 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/02.connect_checks_timeout.md
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/03.connect_checks_not_responding.md
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/04.connect_checks_ssl_verify_fails.md
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/05.executor_with_comma.md
--rw-rw-rw-   0 root         (0) root         (0)       59 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/06.ssl_wizard.md
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/07.doc.md
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/E00.md
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/E01.nmap_multi_target.md
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/E02.w3af_use_python2.md
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/E03.escape.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.2.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.736042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/1.multi_workspace.md
--rw-rw-rw-   0 root         (0) root         (0)      116 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/2.migrate_in_run.md
--rw-rw-rw-   0 root         (0) root         (0)       82 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/3.fix_close_agent.md
--rw-rw-rw-   0 root         (0) root         (0)       89 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/4.page-size.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/E00.md
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/E01.fix_arachni.md
--rw-rw-rw-   0 root         (0) root         (0)       74 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/E02.fix_nmap.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.0/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.737042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.1/
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.1/1.proxy_setup.md
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.1/E01.fix_nessus.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.3.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.739042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.0/
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.0/1.base_route.md
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.0/2.duration.md
--rw-rw-rw-   0 root         (0) root         (0)      147 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.0/E00.md
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.0/E01_flags_nmap.md
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.0/E02_env_python.md
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.0/E03_scheme_http_s_nmap.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.0/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.740042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.1/
--rw-rw-rw-   0 root         (0) root         (0)      461 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.1/1.general_changes.md
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.1/E1.wpscan_not_use_docker.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.1/E2.fix_nuclei.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.740042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.2/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.2/1.plugins.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.2/date.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.4.2/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.742042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.0/
--rw-rw-rw-   0 root         (0) root         (0)      152 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.0/1.change_wizard.md
--rw-rw-rw-   0 root         (0) root         (0)       64 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.0/2.v3.md
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.0/3.connectivity_endpoint.md
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.0/4.token.md
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.0/5.update_host_input.md
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.0/E1.update_openvas.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.0/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.742042 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.1/
--rw-rw-rw-   0 root         (0) root         (0)       31 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.1/1.fix_burp_executor.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/1.5.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.743042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.0.0/1.typing.md
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.0.0/2.add_manifests_versioning.md
--rw-rw-rw-   0 root         (0) root         (0)       19 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.0.0/3.FIX_typo_in_wizard.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.0.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.0.0/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.745042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       57 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.0/1.add_reminder_for_token.md
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.0/2.fix_dates.md
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.0/3.manage_402.md
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.0/E1.add_insightvm_executor.md
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.0/E2.update_burp.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.0/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.746042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.1/
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.1/1.add_option_ignore_ssl.md
--rw-rw-rw-   0 root         (0) root         (0)       97 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.1/2.redo_defaults_ports_after_ssl.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.746042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.2/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.2/add_script_to_nmap.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.2/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.747042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.3/
--rw-rw-rw-   0 root         (0) root         (0)       46 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.3/add_commands_to_wpscan.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.3/date.md
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.1.3/move_shodan_to_official.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.748042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.2.0/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.2.0/Add_timeout_parameter_to_arachni.md
--rw-rw-rw-   0 root         (0) root         (0)       57 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.2.0/add w3af.md
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.2.0/add_ignore_info_and_hostname_resolution.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.2.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.2.0/fix_exectuors.md
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.2.0/fix_logs.md
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.2.0/remove_ws.md
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.2.0/send_parameters_at_connection_time.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.750042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.3.0/
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.3.0/add_scan_functionality_to_insightvm.md
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.3.0/add_tags_for_plugins.md
--rw-rw-rw-   0 root         (0) root         (0)       57 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.3.0/add_vulners.md
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.3.0/change_api_key.md
--rw-rw-rw-   0 root         (0) root         (0)       80 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.3.0/change_venvs.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.3.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.3.0/update_docs.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.750042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.4.0/
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.4.0/Add_qualys.md
--rw-rw-rw-   0 root         (0) root         (0)       46 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.4.0/change_pgrep_for_psutil.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.4.0/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.751042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.0/add_sonar_executor.md
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.0/add_tenableio_executor.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       66 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.0/fix_gvm_executor.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.0/transform_to_str.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.752042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.1/
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.1/allow_ip_target_for_nuclei.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.5.1/fixes_for_bandit.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.752042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.0/
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.0/186.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.0/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.753042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.1/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.1/187.md
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.1/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.753042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.2/
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.2/192.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.2/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.753042 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.3/
--rw-rw-rw-   0 root         (0) root         (0)       53 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.3/194.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/2.6.3/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.754042 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.0.0/
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.0.0/195.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.0.0/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.754042 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.0.1/
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.0.1/199.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.0.1/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.755042 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.2.0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.2.0/206.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.2.0/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.756042 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.3.0/
--rw-rw-rw-   0 root         (0) root         (0)       45 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.3.0/197.md
--rw-rw-rw-   0 root         (0) root         (0)       99 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.3.0/203.md
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.3.0/208.md
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.3.0/209.md
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.3.0/210.md
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.3.0/212.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/3.3.0/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.756042 faraday_agent_dispatcher-3.3.0/CHANGELOG/current/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/current/.keep
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CHANGELOG/footer.md
--rw-rw-rw-   0 root         (0) root         (0)     3711 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    35149 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/COPYING
--rw-rw-rw-   0 root         (0) root         (0)       93 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     2313 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/Makefile
--rw-r--r--   0 root         (0) root         (0)    17119 2024-03-12 18:13:15.785042 faraday_agent_dispatcher-3.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6247 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     9126 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/RELEASE.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.717042 faraday_agent_dispatcher-3.3.0/docker/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.757042 faraday_agent_dispatcher-3.3.0/docker/plugins-docker/
--rw-rw-rw-   0 root         (0) root         (0)     3095 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docker/plugins-docker/Dockerfile
--rwxrwxrwx   0 root         (0) root         (0)      802 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docker/plugins-docker/docker.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.757042 faraday_agent_dispatcher-3.3.0/docker/publish/
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docker/publish/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)      588 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docker/publish/Dockerfile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.758042 faraday_agent_dispatcher-3.3.0/docker/publish/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2059 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docker/publish/templates/template_dispatcher.ini
--rw-rw-rw-   0 root         (0) root         (0)     4473 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docker/publish/templates/template_dispatcher.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2227 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docker/publish/templates/template_dispatcher_with_report.ini
--rw-rw-rw-   0 root         (0) root         (0)     4830 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docker/publish/templates/template_dispatcher_with_report.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.758042 faraday_agent_dispatcher-3.3.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      927 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.759042 faraday_agent_dispatcher-3.3.0/docs/docs/
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/418.md
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/CNAME
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.759042 faraday_agent_dispatcher-3.3.0/docs/docs/css/
--rw-rw-rw-   0 root         (0) root         (0)      114 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/css/faraday_doc.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.759042 faraday_agent_dispatcher-3.3.0/docs/docs/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/examples/new-custom-executor.md
--rw-rw-rw-   0 root         (0) root         (0)     9813 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/getting-started.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.761042 faraday_agent_dispatcher-3.3.0/docs/docs/images/
--rw-rw-rw-   0 root         (0) root         (0)    31633 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/agent_example.png
--rw-rw-rw-   0 root         (0) root         (0)    44658 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/arch.png
--rw-rw-rw-   0 root         (0) root         (0)    20584 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/arch_dispatcher.png
--rw-rw-rw-   0 root         (0) root         (0)    26625 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/arch_executors.png
--rw-rw-rw-   0 root         (0) root         (0)    21253 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/executor_example.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.718042 faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.762042 faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/qualys/
--rw-rw-rw-   0 root         (0) root         (0)    54521 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/qualys/check_profile.png
--rw-rw-rw-   0 root         (0) root         (0)   280745 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/qualys/new_profile.png
--rw-rw-rw-   0 root         (0) root         (0)   194186 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/qualys/profileid.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.763042 faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/sonarqube/
--rw-rw-rw-   0 root         (0) root         (0)    34458 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/sonarqube/generate_token.png
--rw-rw-rw-   0 root         (0) root         (0)    10160 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/sonarqube/profile_icon.png
--rw-rw-rw-   0 root         (0) root         (0)     3175 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/favicon.png
--rw-rw-rw-   0 root         (0) root         (0)      581 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/logo.svg
--rw-rw-rw-   0 root         (0) root         (0)    20392 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/images/token.png
--rw-rw-rw-   0 root         (0) root         (0)     1428 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.763042 faraday_agent_dispatcher-3.3.0/docs/docs/js/
--rw-rw-rw-   0 root         (0) root         (0)     2051 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/js/details.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.765042 faraday_agent_dispatcher-3.3.0/docs/docs/misc/
--rw-rw-rw-   0 root         (0) root         (0)      846 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/misc/appscan.md
--rw-rw-rw-   0 root         (0) root         (0)     2533 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/misc/docker.md
--rw-rw-rw-   0 root         (0) root         (0)     1545 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/misc/qualys.md
--rw-rw-rw-   0 root         (0) root         (0)     1045 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/misc/sonarqube.md
--rw-rw-rw-   0 root         (0) root         (0)     2059 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/misc/template_dispatcher.ini
--rw-rw-rw-   0 root         (0) root         (0)     4473 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/misc/template_dispatcher.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2227 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/misc/template_dispatcher_with_report.ini
--rw-rw-rw-   0 root         (0) root         (0)     4830 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/misc/template_dispatcher_with_report.yaml
--rw-rw-rw-   0 root         (0) root         (0)      767 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/misc/tenableio.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.765042 faraday_agent_dispatcher-3.3.0/docs/docs/technical/
--rw-rw-rw-   0 root         (0) root         (0)     6633 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/technical/agents.md
--rw-rw-rw-   0 root         (0) root         (0)     1770 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/docs/technical/arch.md
--rw-rw-rw-   0 root         (0) root         (0)     2025 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/docs/mkdocs.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.767042 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/
--rw-rw-rw-   0 root         (0) root         (0)      883 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.769042 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5447 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.770042 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/utils/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2991 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/utils/general_inputs.py
--rw-rw-rw-   0 root         (0) root         (0)      558 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/utils/general_prompts.py
--rw-rw-rw-   0 root         (0) root         (0)    12031 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/utils/model_load.py
--rw-rw-rw-   0 root         (0) root         (0)     9859 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    14016 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/config.py
--rw-rw-rw-   0 root         (0) root         (0)    27418 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)    35094 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/dispatcher_io.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/example_config.ini
--rw-rw-rw-   0 root         (0) root         (0)      165 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/example_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2537 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/executor.py
--rw-rw-rw-   0 root         (0) root         (0)     6288 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/executor_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     3858 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.720042 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.720042 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.775042 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/
--rw-rw-rw-   0 root         (0) root         (0)     9484 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/appscan.py
--rw-rw-rw-   0 root         (0) root         (0)     3269 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/arachni.py
--rw-rw-rw-   0 root         (0) root         (0)     9215 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/burp.py
--rw-rw-rw-   0 root         (0) root         (0)     7449 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/codeql.py
--rw-rw-rw-   0 root         (0) root         (0)     3808 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/crackmapexec.py
--rw-rw-rw-   0 root         (0) root         (0)     4786 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/dependabot.py
--rw-rw-rw-   0 root         (0) root         (0)     2546 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/github_secrets.py
--rw-rw-rw-   0 root         (0) root         (0)     6135 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/gvm_openvas.py
--rw-rw-rw-   0 root         (0) root         (0)     6447 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/insightvm.py
--rwxrwxrwx   0 root         (0) root         (0)    11430 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/nessus.py
--rw-rw-rw-   0 root         (0) root         (0)     2104 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/nikto2.py
--rwxrwxrwx   0 root         (0) root         (0)     3551 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/nmap.py
--rwxrwxrwx   0 root         (0) root         (0)     3152 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/nuclei.py
--rw-rw-rw-   0 root         (0) root         (0)     4424 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/openvas_legacy.py
--rw-rw-rw-   0 root         (0) root         (0)     6205 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/qualys.py
--rw-rw-rw-   0 root         (0) root         (0)     1908 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/report_processor.py
--rw-rw-rw-   0 root         (0) root         (0)     2010 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/shodan2.py
--rw-rw-rw-   0 root         (0) root         (0)     4734 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/sonarqube.py
--rwxrwxrwx   0 root         (0) root         (0)      887 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/sublist3r.sh
--rw-rw-rw-   0 root         (0) root         (0)     4134 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/tenableio.py
--rw-rw-rw-   0 root         (0) root         (0)     3960 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/w3af.py
--rw-rw-rw-   0 root         (0) root         (0)     2521 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/wpscan.py
--rw-rw-rw-   0 root         (0) root         (0)     2416 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/wpscan_legacy.py
--rw-rw-rw-   0 root         (0) root         (0)     2160 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/zap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.776042 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3861 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/utils/control_values_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2217 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/utils/metadata_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      281 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/utils/text_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1103 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/utils/url_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.783042 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17119 2024-03-12 18:13:15.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10813 2024-03-12 18:13:15.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-12 18:13:15.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2024-03-12 18:13:15.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-12 18:13:15.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      345 2024-03-12 18:13:15.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-12 18:13:15.000000 faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      466 2024-03-12 18:13:15.785042 faraday_agent_dispatcher-3.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3103 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.776042 faraday_agent_dispatcher-3.3.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.778042 faraday_agent_dispatcher-3.3.0/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/basic_executor.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/mock.pub
--rw-rw-rw-   0 root         (0) root         (0)     1302 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/ok.crt
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/ok.key
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.780042 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/0.1.ini
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/0.1_with_agent_token.ini
--rw-rw-rw-   0 root         (0) root         (0)      507 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.0.ini
--rw-rw-rw-   0 root         (0) root         (0)      359 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.0_error0.ini
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.0_error1.ini
--rw-rw-rw-   0 root         (0) root         (0)      578 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.0_with_agent_token.ini
--rw-rw-rw-   0 root         (0) root         (0)      611 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.2.ini
--rw-rw-rw-   0 root         (0) root         (0)      681 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.2_with_agent_token.ini
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.5.ini
--rw-rw-rw-   0 root         (0) root         (0)      822 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/test_config.ini
--rw-rw-rw-   0 root         (0) root         (0)     1302 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/data/wrong.crt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.780042 faraday_agent_dispatcher-3.3.0/tests/integration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.780042 faraday_agent_dispatcher-3.3.0/tests/integration/faraday/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/integration/faraday/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7330 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/integration/faraday/test_execution.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.781042 faraday_agent_dispatcher-3.3.0/tests/plugins-docker/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/plugins-docker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3674 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/plugins-docker/test_executors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.782042 faraday_agent_dispatcher-3.3.0/tests/unittests/
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/unittests/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/unittests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.782042 faraday_agent_dispatcher-3.3.0/tests/unittests/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/unittests/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    46373 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/unittests/config/agent_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)    37399 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/unittests/config/wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    12779 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/unittests/test_agent_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     5088 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/unittests/test_config_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/unittests/test_import_official_executors.py
--rw-rw-rw-   0 root         (0) root         (0)     7983 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/unittests/wizard_input.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 18:13:15.783042 faraday_agent_dispatcher-3.3.0/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9651 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/utils/testing_faraday_server.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tests/utils/text_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      571 2024-03-12 18:12:43.000000 faraday_agent_dispatcher-3.3.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.044505 faraday_agent_dispatcher-3.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.967506 faraday_agent_dispatcher-3.4.0/.gitlab/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.982505 faraday_agent_dispatcher-3.4.0/.gitlab/ci/
+-rw-rw-rw-   0 root         (0) root         (0)     1387 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/.gitlab/ci/.pre-gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      508 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/.gitlab/ci/.rules-conditions.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.982505 faraday_agent_dispatcher-3.4.0/.gitlab/ci/build_ci/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/.gitlab/ci/build_ci/.build-gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      717 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/.gitlab/ci/fetch-secrets.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.983505 faraday_agent_dispatcher-3.4.0/.gitlab/ci/plugins-integration/
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/.gitlab/ci/plugins-integration/.build-gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      877 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/.gitlab/ci/plugins-integration/.testing-gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.983505 faraday_agent_dispatcher-3.4.0/.gitlab/ci/publish/
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/.gitlab/ci/publish/.publish-dockerhub-gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      283 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/.gitlab/ci/publish/.pypi-gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.984506 faraday_agent_dispatcher-3.4.0/.gitlab/ci/testing/
+-rw-rw-rw-   0 root         (0) root         (0)      447 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/.gitlab/ci/testing/.post-gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2829 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/.gitlab/ci/testing/.testing-gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      743 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/.pre-push-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/AUTHORS.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.984506 faraday_agent_dispatcher-3.4.0/CHANGELOG/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.985505 faraday_agent_dispatcher-3.4.0/CHANGELOG/0.1/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/0.1/01.first version.md
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/0.1/02.minimal structure.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/0.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/0.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.986505 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.0/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.0/01.env_var.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.0/02.executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.0/03.params.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.0/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.988505 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.1/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.1/01.run.md
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.1/02.wizard.md
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.1/03.01.manage_execution_id.md
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.1/03.02.change_ws_route.md
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.1/04.error_management.md
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.1/05.invalid token.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.1/06.ssl.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.989505 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2/01.package_executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       31 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2/02.signal.md
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2/03.close_connection.md
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2/04.sslcert.md
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2/05.config_folder.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2/E00.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.992505 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2.1/01.check_command_before_run.md
+-rw-rw-rw-   0 root         (0) root         (0)       91 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2.1/02.connect_checks_timeout.md
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2.1/03.connect_checks_not_responding.md
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2.1/04.connect_checks_ssl_verify_fails.md
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2.1/05.executor_with_comma.md
+-rw-rw-rw-   0 root         (0) root         (0)       59 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2.1/06.ssl_wizard.md
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2.1/07.doc.md
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2.1/E00.md
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2.1/E01.nmap_multi_target.md
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2.1/E02.w3af_use_python2.md
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2.1/E03.escape.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.2.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.994506 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.3.0/1.multi_workspace.md
+-rw-rw-rw-   0 root         (0) root         (0)      116 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.3.0/2.migrate_in_run.md
+-rw-rw-rw-   0 root         (0) root         (0)       82 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.3.0/3.fix_close_agent.md
+-rw-rw-rw-   0 root         (0) root         (0)       89 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.3.0/4.page-size.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.3.0/E00.md
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.3.0/E01.fix_arachni.md
+-rw-rw-rw-   0 root         (0) root         (0)       74 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.3.0/E02.fix_nmap.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.3.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.3.0/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.994506 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.3.1/1.proxy_setup.md
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.3.1/E01.fix_nessus.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.3.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.3.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.996505 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.0/1.base_route.md
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.0/2.duration.md
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.0/E00.md
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.0/E01_flags_nmap.md
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.0/E02_env_python.md
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.0/E03_scheme_http_s_nmap.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.0/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.997506 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)      461 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.1/1.general_changes.md
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.1/E1.wpscan_not_use_docker.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.1/E2.fix_nuclei.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.998505 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.2/1.plugins.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.2/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.4.2/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.999505 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)      152 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.5.0/1.change_wizard.md
+-rw-rw-rw-   0 root         (0) root         (0)       64 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.5.0/2.v3.md
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.5.0/3.connectivity_endpoint.md
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.5.0/4.token.md
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.5.0/5.update_host_input.md
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.5.0/E1.update_openvas.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.5.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.5.0/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.000506 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.5.1/1.fix_burp_executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.5.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/1.5.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.001505 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.0.0/1.typing.md
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.0.0/2.add_manifests_versioning.md
+-rw-rw-rw-   0 root         (0) root         (0)       19 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.0.0/3.FIX_typo_in_wizard.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.0.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.0.0/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.002505 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.0/1.add_reminder_for_token.md
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.0/2.fix_dates.md
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.0/3.manage_402.md
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.0/E1.add_insightvm_executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.0/E2.update_burp.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.0/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.003505 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.1/1.add_option_ignore_ssl.md
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.1/2.redo_defaults_ports_after_ssl.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.003505 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.2/add_script_to_nmap.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.2/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.004505 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.3/add_commands_to_wpscan.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.3/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.1.3/move_shodan_to_official.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.006505 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.2.0/Add_timeout_parameter_to_arachni.md
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.2.0/add w3af.md
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.2.0/add_ignore_info_and_hostname_resolution.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.2.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.2.0/fix_exectuors.md
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.2.0/fix_logs.md
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.2.0/remove_ws.md
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.2.0/send_parameters_at_connection_time.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.007506 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.3.0/add_scan_functionality_to_insightvm.md
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.3.0/add_tags_for_plugins.md
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.3.0/add_vulners.md
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.3.0/change_api_key.md
+-rw-rw-rw-   0 root         (0) root         (0)       80 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.3.0/change_venvs.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.3.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.3.0/update_docs.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.008505 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.4.0/Add_qualys.md
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.4.0/change_pgrep_for_psutil.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.4.0/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.009505 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.5.0/add_sonar_executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.5.0/add_tenableio_executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.5.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       66 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.5.0/fix_gvm_executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.5.0/transform_to_str.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.009505 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.5.1/allow_ip_target_for_nuclei.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.5.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.5.1/fixes_for_bandit.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.010506 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.6.0/186.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.6.0/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.010506 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.6.1/187.md
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.6.1/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.010506 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.6.2/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.6.2/192.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.6.2/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.011505 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.6.3/
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.6.3/194.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/2.6.3/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.011505 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.0.0/195.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.0.0/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.012505 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.0.1/199.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.0.1/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.012505 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.2.0/206.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.2.0/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.013505 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)       45 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.3.0/197.md
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.3.0/203.md
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.3.0/208.md
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.3.0/209.md
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.3.0/210.md
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.3.0/212.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.3.0/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.014505 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.4.0/200.md
+-rw-rw-rw-   0 root         (0) root         (0)      237 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.4.0/214.md
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.4.0/216.md
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.4.0/217.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/3.4.0/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.014505 faraday_agent_dispatcher-3.4.0/CHANGELOG/current/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/current/.keep
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CHANGELOG/footer.md
+-rw-rw-rw-   0 root         (0) root         (0)     3711 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)       93 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)    17698 2024-05-22 21:08:04.044505 faraday_agent_dispatcher-3.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6247 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     9705 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/RELEASE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.973505 faraday_agent_dispatcher-3.4.0/docker/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.015505 faraday_agent_dispatcher-3.4.0/docker/plugins-docker/
+-rw-rw-rw-   0 root         (0) root         (0)     3095 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docker/plugins-docker/Dockerfile
+-rwxrwxrwx   0 root         (0) root         (0)      802 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docker/plugins-docker/docker.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.015505 faraday_agent_dispatcher-3.4.0/docker/publish/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docker/publish/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      588 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docker/publish/Dockerfile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.016505 faraday_agent_dispatcher-3.4.0/docker/publish/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2059 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docker/publish/templates/template_dispatcher.ini
+-rw-rw-rw-   0 root         (0) root         (0)     4473 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docker/publish/templates/template_dispatcher.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2227 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docker/publish/templates/template_dispatcher_with_report.ini
+-rw-rw-rw-   0 root         (0) root         (0)     4830 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docker/publish/templates/template_dispatcher_with_report.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.016505 faraday_agent_dispatcher-3.4.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.017506 faraday_agent_dispatcher-3.4.0/docs/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/418.md
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/CNAME
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.017506 faraday_agent_dispatcher-3.4.0/docs/docs/css/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/css/faraday_doc.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.018505 faraday_agent_dispatcher-3.4.0/docs/docs/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/examples/new-custom-executor.md
+-rw-rw-rw-   0 root         (0) root         (0)     9813 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/getting-started.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.020506 faraday_agent_dispatcher-3.4.0/docs/docs/images/
+-rw-rw-rw-   0 root         (0) root         (0)    31633 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/images/agent_example.png
+-rw-rw-rw-   0 root         (0) root         (0)    44658 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/images/arch.png
+-rw-rw-rw-   0 root         (0) root         (0)    20584 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/images/arch_dispatcher.png
+-rw-rw-rw-   0 root         (0) root         (0)    26625 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/images/arch_executors.png
+-rw-rw-rw-   0 root         (0) root         (0)    21253 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/images/executor_example.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.975505 faraday_agent_dispatcher-3.4.0/docs/docs/images/executors/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.021505 faraday_agent_dispatcher-3.4.0/docs/docs/images/executors/qualys/
+-rw-rw-rw-   0 root         (0) root         (0)    54521 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/images/executors/qualys/check_profile.png
+-rw-rw-rw-   0 root         (0) root         (0)   280745 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/images/executors/qualys/new_profile.png
+-rw-rw-rw-   0 root         (0) root         (0)   194186 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/images/executors/qualys/profileid.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.021505 faraday_agent_dispatcher-3.4.0/docs/docs/images/executors/sonarqube/
+-rw-rw-rw-   0 root         (0) root         (0)    34458 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/images/executors/sonarqube/generate_token.png
+-rw-rw-rw-   0 root         (0) root         (0)    10160 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/images/executors/sonarqube/profile_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     3175 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/images/favicon.png
+-rw-rw-rw-   0 root         (0) root         (0)      581 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/images/logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)    20392 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/images/token.png
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.022505 faraday_agent_dispatcher-3.4.0/docs/docs/js/
+-rw-rw-rw-   0 root         (0) root         (0)     2051 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/js/details.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.023505 faraday_agent_dispatcher-3.4.0/docs/docs/misc/
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/misc/appscan.md
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/misc/docker.md
+-rw-rw-rw-   0 root         (0) root         (0)     1545 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/misc/qualys.md
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/misc/sonarqube.md
+-rw-rw-rw-   0 root         (0) root         (0)     2059 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/misc/template_dispatcher.ini
+-rw-rw-rw-   0 root         (0) root         (0)     4473 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/misc/template_dispatcher.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2227 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/misc/template_dispatcher_with_report.ini
+-rw-rw-rw-   0 root         (0) root         (0)     4830 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/misc/template_dispatcher_with_report.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      767 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/misc/tenableio.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.024505 faraday_agent_dispatcher-3.4.0/docs/docs/technical/
+-rw-rw-rw-   0 root         (0) root         (0)     6633 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/technical/agents.md
+-rw-rw-rw-   0 root         (0) root         (0)     1770 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/docs/technical/arch.md
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/docs/mkdocs.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.026505 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/
+-rw-rw-rw-   0 root         (0) root         (0)      883 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.028505 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5447 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.029505 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/cli/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/cli/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/cli/utils/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2991 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/cli/utils/general_inputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      558 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/cli/utils/general_prompts.py
+-rw-rw-rw-   0 root         (0) root         (0)    12031 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/cli/utils/model_load.py
+-rw-rw-rw-   0 root         (0) root         (0)     9859 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/cli/wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    14016 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    27418 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)    35370 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/dispatcher_io.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/example_config.ini
+-rw-rw-rw-   0 root         (0) root         (0)      165 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/example_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6288 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/executor_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     3858 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.976505 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:03.977506 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.034505 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/
+-rw-rw-rw-   0 root         (0) root         (0)     9484 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/appscan.py
+-rw-rw-rw-   0 root         (0) root         (0)     3269 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/arachni.py
+-rw-rw-rw-   0 root         (0) root         (0)     9215 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/burp.py
+-rw-rw-rw-   0 root         (0) root         (0)     5463 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/cisco_cybervision.py
+-rw-rw-rw-   0 root         (0) root         (0)     7449 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/codeql.py
+-rw-rw-rw-   0 root         (0) root         (0)     3808 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/crackmapexec.py
+-rw-rw-rw-   0 root         (0) root         (0)     4786 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/dependabot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2546 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/github_secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     6135 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/gvm_openvas.py
+-rw-rw-rw-   0 root         (0) root         (0)     6447 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/insightvm.py
+-rwxrwxrwx   0 root         (0) root         (0)    11430 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/nessus.py
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/nikto2.py
+-rwxrwxrwx   0 root         (0) root         (0)     3551 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/nmap.py
+-rwxrwxrwx   0 root         (0) root         (0)     3152 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/nuclei.py
+-rw-rw-rw-   0 root         (0) root         (0)     4424 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/openvas_legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6205 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/qualys.py
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/report_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2010 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/shodan2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4734 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/sonarqube.py
+-rwxrwxrwx   0 root         (0) root         (0)      887 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/sublist3r.sh
+-rw-rw-rw-   0 root         (0) root         (0)     6537 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/tenableio.py
+-rw-rw-rw-   0 root         (0) root         (0)     3631 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/tenablesc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3960 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/w3af.py
+-rw-rw-rw-   0 root         (0) root         (0)     2521 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/wpscan.py
+-rw-rw-rw-   0 root         (0) root         (0)     2416 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/wpscan_legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/zap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.035505 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3861 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/utils/control_values_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2217 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/utils/metadata_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      687 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/utils/severity_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      281 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/utils/text_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/utils/url_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.043505 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17698 2024-05-22 21:08:03.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11114 2024-05-22 21:08:03.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 21:08:03.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2024-05-22 21:08:03.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 21:08:03.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      345 2024-05-22 21:08:03.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-22 21:08:03.000000 faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      466 2024-05-22 21:08:04.045505 faraday_agent_dispatcher-3.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3103 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.036505 faraday_agent_dispatcher-3.4.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.037505 faraday_agent_dispatcher-3.4.0/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/data/basic_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/data/mock.pub
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/data/ok.crt
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/data/ok.key
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.039505 faraday_agent_dispatcher-3.4.0/tests/data/old_version_inis/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/data/old_version_inis/0.1.ini
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/data/old_version_inis/0.1_with_agent_token.ini
+-rw-rw-rw-   0 root         (0) root         (0)      507 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/data/old_version_inis/1.0.ini
+-rw-rw-rw-   0 root         (0) root         (0)      359 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/data/old_version_inis/1.0_error0.ini
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/data/old_version_inis/1.0_error1.ini
+-rw-rw-rw-   0 root         (0) root         (0)      578 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/data/old_version_inis/1.0_with_agent_token.ini
+-rw-rw-rw-   0 root         (0) root         (0)      611 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/data/old_version_inis/1.2.ini
+-rw-rw-rw-   0 root         (0) root         (0)      681 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/data/old_version_inis/1.2_with_agent_token.ini
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/data/old_version_inis/1.5.ini
+-rw-rw-rw-   0 root         (0) root         (0)      822 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/data/test_config.ini
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/data/wrong.crt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.039505 faraday_agent_dispatcher-3.4.0/tests/integration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.039505 faraday_agent_dispatcher-3.4.0/tests/integration/faraday/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/integration/faraday/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7330 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/integration/faraday/test_execution.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.040506 faraday_agent_dispatcher-3.4.0/tests/plugins-docker/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/plugins-docker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3674 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/plugins-docker/test_executors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.041505 faraday_agent_dispatcher-3.4.0/tests/unittests/
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/unittests/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/unittests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.042505 faraday_agent_dispatcher-3.4.0/tests/unittests/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/unittests/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    46373 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/unittests/config/agent_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)    37399 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/unittests/config/wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    12779 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/unittests/test_agent_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     5088 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/unittests/test_config_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/unittests/test_import_official_executors.py
+-rw-rw-rw-   0 root         (0) root         (0)     7983 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/unittests/wizard_input.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:08:04.042505 faraday_agent_dispatcher-3.4.0/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9651 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/utils/testing_faraday_server.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tests/utils/text_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      571 2024-05-22 21:07:26.000000 faraday_agent_dispatcher-3.4.0/tox.ini
```

### Comparing `faraday_agent_dispatcher-3.3.0/.gitignore` & `faraday_agent_dispatcher-3.4.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -159,7 +159,10 @@
 .idea/httpRequests
 
 .idea/*
 
 logs/*
 */logs/*
 *.log.*
+
+# MacOS ds files
+.DS_Store
```

### Comparing `faraday_agent_dispatcher-3.3.0/.gitlab/ci/.pre-gitlab-ci.yml` & `faraday_agent_dispatcher-3.4.0/.gitlab/ci/.pre-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/.gitlab/ci/build_ci/.build-gitlab-ci.yml` & `faraday_agent_dispatcher-3.4.0/.gitlab/ci/build_ci/.build-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/.gitlab/ci/fetch-secrets.yml` & `faraday_agent_dispatcher-3.4.0/.gitlab/ci/fetch-secrets.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/.gitlab/ci/plugins-integration/.build-gitlab-ci.yml` & `faraday_agent_dispatcher-3.4.0/.gitlab/ci/plugins-integration/.build-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/.gitlab/ci/plugins-integration/.testing-gitlab-ci.yml` & `faraday_agent_dispatcher-3.4.0/.gitlab/ci/plugins-integration/.testing-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/.gitlab/ci/publish/.publish-dockerhub-gitlab-ci.yml` & `faraday_agent_dispatcher-3.4.0/.gitlab/ci/publish/.publish-dockerhub-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/.gitlab/ci/testing/.testing-gitlab-ci.yml` & `faraday_agent_dispatcher-3.4.0/.gitlab/ci/testing/.testing-gitlab-ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,16 @@
     - source faraday_venv/bin/activate
 
 .install_custom_typing_branch:
   before_script:
     - git clone https://gitlab-ci-token:${CI_JOB_TOKEN}@gitlab.com/faradaysec/cloud/faraday_agent_parameters_types.git typing
     - cd typing
     - if [ -z "$TYPING_BRANCH" ]; then export TYPING_BRANCH="master"; fi
-    - echo $TYPING_BRANCH
+    - echo "Using faraday_agent_parameters_type branch -> $TYPING_BRANCH"
+    - git fetch
     - git checkout $TYPING_BRANCH
     - pip install .
     - cd ..
 
 
 .unit_tests_base:
     stage: testing
```

### Comparing `faraday_agent_dispatcher-3.3.0/.gitlab-ci.yml` & `faraday_agent_dispatcher-3.4.0/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     FARADAY_PASSWORD: custom_pass
     FARADAY_EMAIL: test@test.com
     FARADAY_REF: white/dev
     EXECUTOR_DIR: ./basic_executor.py
     VAULT_ROLE: 'python-sast-readonly'
     VAULT_ADDR: 'https://tluav-lb.faradaysec.com'
     VAULT_SECRET_PATH: 'gitlab/SAST'
+    TYPING_BRANCH: 'dev'
 
 workflow:
   rules:
     - if: $CI_MERGE_REQUEST_ID
       when: never
     - when: always
```

### Comparing `faraday_agent_dispatcher-3.3.0/.pre-commit-config.yaml` & `faraday_agent_dispatcher-3.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/CONTRIBUTING.rst` & `faraday_agent_dispatcher-3.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/COPYING` & `faraday_agent_dispatcher-3.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/Makefile` & `faraday_agent_dispatcher-3.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/PKG-INFO` & `faraday_agent_dispatcher-3.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faraday_agent_dispatcher
-Version: 3.3.0
+Version: 3.4.0
 Summary: Faraday agent dispatcher to communicate an agent to faraday
 Home-page: https://github.com/infobyte/faraday_agent_dispatcher
 Author: Faraday Development Team
 Author-email: devel@infobytesec.com
 License: GNU General Public License v3
 Keywords: faraday integration
 Classifier: Development Status :: 5 - Production/Stable
@@ -207,14 +207,21 @@
 
 For more info you can check our [documentation][doc]
 
 [doc]: https://docs.agents.faradaysec.com
 [API]: https://api.faradaysec.com/
 
 
+3.4.0 [May 22th, 2024]:
+---
+ * [ADD] Introducing the new Tenable SC agent, now available for integration. This initial version focuses on supporting scan imports. #216
+ * [ADD] Added new agent for Cisco Cyber Vision. Also added severity calc utility. #217
+ * [FIX] Fix agent websocket token not changing on registration token update #200
+ * [FIX] Resolved the issue where users were unable to execute user-defined templates and pre-defined TenableIO templates. Additionally, fixed the functionality to retrieve completed scan results and relaunch previously created scans. #214
+
 3.3.0 [Mar 12th, 2024]:
 ---
  * [ADD] Add hotspots option to SonarQube. #197
  * [ADD] New GitHub CodeQL agent. #208
  * [ADD] Added new agent for GitHub Secrets Scanning. #209
  * [MOD] Now Nessus executor tries to login again after a 401 response from the Nessus's server. #203
  * [MOD] Change Dependabot agent to work with the new manifest of parameter types. #210
```

### Comparing `faraday_agent_dispatcher-3.3.0/README.md` & `faraday_agent_dispatcher-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/RELEASE.md` & `faraday_agent_dispatcher-3.4.0/RELEASE.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+3.4.0 [May 22th, 2024]:
+---
+ * [ADD] Introducing the new Tenable SC agent, now available for integration. This initial version focuses on supporting scan imports. #216
+ * [ADD] Added new agent for Cisco Cyber Vision. Also added severity calc utility. #217
+ * [FIX] Fix agent websocket token not changing on registration token update #200
+ * [FIX] Resolved the issue where users were unable to execute user-defined templates and pre-defined TenableIO templates. Additionally, fixed the functionality to retrieve completed scan results and relaunch previously created scans. #214
+
 3.3.0 [Mar 12th, 2024]:
 ---
  * [ADD] Add hotspots option to SonarQube. #197
  * [ADD] New GitHub CodeQL agent. #208
  * [ADD] Added new agent for GitHub Secrets Scanning. #209
  * [MOD] Now Nessus executor tries to login again after a 401 response from the Nessus's server. #203
  * [MOD] Change Dependabot agent to work with the new manifest of parameter types. #210
```

### Comparing `faraday_agent_dispatcher-3.3.0/docker/plugins-docker/Dockerfile` & `faraday_agent_dispatcher-3.4.0/docker/plugins-docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docker/plugins-docker/docker.sh` & `faraday_agent_dispatcher-3.4.0/docker/plugins-docker/docker.sh`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docker/publish/Dockerfile` & `faraday_agent_dispatcher-3.4.0/docker/publish/Dockerfile`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docker/publish/templates/template_dispatcher.ini` & `faraday_agent_dispatcher-3.4.0/docker/publish/templates/template_dispatcher.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docker/publish/templates/template_dispatcher.yaml` & `faraday_agent_dispatcher-3.4.0/docker/publish/templates/template_dispatcher.yaml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docker/publish/templates/template_dispatcher_with_report.ini` & `faraday_agent_dispatcher-3.4.0/docker/publish/templates/template_dispatcher_with_report.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docker/publish/templates/template_dispatcher_with_report.yaml` & `faraday_agent_dispatcher-3.4.0/docker/publish/templates/template_dispatcher_with_report.yaml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/.gitlab-ci.yml` & `faraday_agent_dispatcher-3.4.0/docs/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/getting-started.md` & `faraday_agent_dispatcher-3.4.0/docs/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/images/agent_example.png` & `faraday_agent_dispatcher-3.4.0/docs/docs/images/agent_example.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/images/arch.png` & `faraday_agent_dispatcher-3.4.0/docs/docs/images/arch.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/images/arch_dispatcher.png` & `faraday_agent_dispatcher-3.4.0/docs/docs/images/arch_dispatcher.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/images/arch_executors.png` & `faraday_agent_dispatcher-3.4.0/docs/docs/images/arch_executors.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/images/executor_example.png` & `faraday_agent_dispatcher-3.4.0/docs/docs/images/executor_example.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/qualys/check_profile.png` & `faraday_agent_dispatcher-3.4.0/docs/docs/images/executors/qualys/check_profile.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/qualys/new_profile.png` & `faraday_agent_dispatcher-3.4.0/docs/docs/images/executors/qualys/new_profile.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/qualys/profileid.png` & `faraday_agent_dispatcher-3.4.0/docs/docs/images/executors/qualys/profileid.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/sonarqube/generate_token.png` & `faraday_agent_dispatcher-3.4.0/docs/docs/images/executors/sonarqube/generate_token.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/images/executors/sonarqube/profile_icon.png` & `faraday_agent_dispatcher-3.4.0/docs/docs/images/executors/sonarqube/profile_icon.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/images/favicon.png` & `faraday_agent_dispatcher-3.4.0/docs/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/images/logo.svg` & `faraday_agent_dispatcher-3.4.0/docs/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/images/token.png` & `faraday_agent_dispatcher-3.4.0/docs/docs/images/token.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/index.md` & `faraday_agent_dispatcher-3.4.0/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/js/details.js` & `faraday_agent_dispatcher-3.4.0/docs/docs/js/details.js`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/misc/appscan.md` & `faraday_agent_dispatcher-3.4.0/docs/docs/misc/appscan.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/misc/docker.md` & `faraday_agent_dispatcher-3.4.0/docs/docs/misc/docker.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/misc/qualys.md` & `faraday_agent_dispatcher-3.4.0/docs/docs/misc/qualys.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/misc/sonarqube.md` & `faraday_agent_dispatcher-3.4.0/docs/docs/misc/sonarqube.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/misc/template_dispatcher.ini` & `faraday_agent_dispatcher-3.4.0/docs/docs/misc/template_dispatcher.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/misc/template_dispatcher.yaml` & `faraday_agent_dispatcher-3.4.0/docs/docs/misc/template_dispatcher.yaml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/misc/template_dispatcher_with_report.ini` & `faraday_agent_dispatcher-3.4.0/docs/docs/misc/template_dispatcher_with_report.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/misc/template_dispatcher_with_report.yaml` & `faraday_agent_dispatcher-3.4.0/docs/docs/misc/template_dispatcher_with_report.yaml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/misc/tenableio.md` & `faraday_agent_dispatcher-3.4.0/docs/docs/misc/tenableio.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/technical/agents.md` & `faraday_agent_dispatcher-3.4.0/docs/docs/technical/agents.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/docs/technical/arch.md` & `faraday_agent_dispatcher-3.4.0/docs/docs/technical/arch.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/docs/mkdocs.yml` & `faraday_agent_dispatcher-3.4.0/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/__init__.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 """Top-level package for faraday_agent_dispatcher."""
 
 __author__ = """Faraday Development Team"""
 __email__ = "devel@infobytesec.com"
-__version__ = "3.3.0"
+__version__ = "3.4.0"
```

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/main.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/cli/main.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/utils/general_inputs.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/cli/utils/general_inputs.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/utils/general_prompts.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/cli/utils/general_prompts.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/utils/model_load.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/cli/utils/model_load.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/cli/wizard.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/cli/wizard.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/config.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/config.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/dispatcher.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/dispatcher.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/dispatcher_io.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/dispatcher_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         websocket_token_json = await websocket_token_response.json()
         return websocket_token_json["token"]
 
     async def register(self, registration_token=None):
         if not await self.check_connection():
             exit(1)
 
-        if self.agent_token is None:
+        if self.agent_token is None or registration_token is not None:
             try:
                 control_registration_token("token", registration_token)
             except ValueError as ex:
                 print(f"{Bcolors.FAIL}{ex.args[0]}")
                 logger.error(ex.args[0])
                 exit(1)
 
@@ -511,15 +511,19 @@
 
     @staticmethod
     async def create_process(executor: Executor, args: dict, plugin_args: dict):
         env = os.environ.copy()
         # Executor Variables
         if isinstance(args, dict):
             for k in args:
-                env[f"EXECUTOR_CONFIG_{k.upper()}"] = str(args[k])
+                # This should allow to correctly get lists from environment with json.loads
+                if isinstance(args[k], list):
+                    env[f"EXECUTOR_CONFIG_{k.upper()}"] = json.dumps(args[k])
+                else:
+                    env[f"EXECUTOR_CONFIG_{k.upper()}"] = str(args[k])
         else:
             logger.error("Args from data received has a not supported type")
             raise ValueError("Args from data received has a not supported type")
         # Plugins Variables
         for pa in plugin_args:
             if isinstance(plugin_args.get(pa), list):
                 env[f"AGENT_CONFIG_{pa.upper()}"] = ",".join(plugin_args.get(pa))
```

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/example_config.ini` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/example_config.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/executor.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/executor.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/executor_helper.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/executor_helper.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/logger.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/logger.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/appscan.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/appscan.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/arachni.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/arachni.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/burp.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/burp.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/codeql.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/codeql.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/crackmapexec.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/crackmapexec.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/dependabot.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/dependabot.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/github_secrets.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/github_secrets.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/gvm_openvas.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/gvm_openvas.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/insightvm.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/insightvm.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/nessus.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/nessus.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/nikto2.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/nikto2.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/nmap.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/nmap.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/nuclei.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/nuclei.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/openvas_legacy.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/openvas_legacy.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/qualys.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/qualys.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/report_processor.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/report_processor.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/shodan2.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/shodan2.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/sonarqube.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/sonarqube.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/sublist3r.sh` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/sublist3r.sh`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/w3af.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/w3af.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/wpscan.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/wpscan.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/wpscan_legacy.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/wpscan_legacy.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/static/executors/official/zap.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/static/executors/official/zap.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/utils/control_values_utils.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/utils/control_values_utils.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/utils/metadata_utils.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/utils/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher/utils/url_utils.py` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher/utils/url_utils.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/PKG-INFO` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faraday_agent_dispatcher
-Version: 3.3.0
+Version: 3.4.0
 Summary: Faraday agent dispatcher to communicate an agent to faraday
 Home-page: https://github.com/infobyte/faraday_agent_dispatcher
 Author: Faraday Development Team
 Author-email: devel@infobytesec.com
 License: GNU General Public License v3
 Keywords: faraday integration
 Classifier: Development Status :: 5 - Production/Stable
@@ -207,14 +207,21 @@
 
 For more info you can check our [documentation][doc]
 
 [doc]: https://docs.agents.faradaysec.com
 [API]: https://api.faradaysec.com/
 
 
+3.4.0 [May 22th, 2024]:
+---
+ * [ADD] Introducing the new Tenable SC agent, now available for integration. This initial version focuses on supporting scan imports. #216
+ * [ADD] Added new agent for Cisco Cyber Vision. Also added severity calc utility. #217
+ * [FIX] Fix agent websocket token not changing on registration token update #200
+ * [FIX] Resolved the issue where users were unable to execute user-defined templates and pre-defined TenableIO templates. Additionally, fixed the functionality to retrieve completed scan results and relaunch previously created scans. #214
+
 3.3.0 [Mar 12th, 2024]:
 ---
  * [ADD] Add hotspots option to SonarQube. #197
  * [ADD] New GitHub CodeQL agent. #208
  * [ADD] Added new agent for GitHub Secrets Scanning. #209
  * [MOD] Now Nessus executor tries to login again after a 401 response from the Nessus's server. #203
  * [MOD] Change Dependabot agent to work with the new manifest of parameter types. #210
```

### Comparing `faraday_agent_dispatcher-3.3.0/faraday_agent_dispatcher.egg-info/SOURCES.txt` & `faraday_agent_dispatcher-3.4.0/faraday_agent_dispatcher.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,19 @@
 CHANGELOG/3.3.0/197.md
 CHANGELOG/3.3.0/203.md
 CHANGELOG/3.3.0/208.md
 CHANGELOG/3.3.0/209.md
 CHANGELOG/3.3.0/210.md
 CHANGELOG/3.3.0/212.md
 CHANGELOG/3.3.0/date.md
+CHANGELOG/3.4.0/200.md
+CHANGELOG/3.4.0/214.md
+CHANGELOG/3.4.0/216.md
+CHANGELOG/3.4.0/217.md
+CHANGELOG/3.4.0/date.md
 CHANGELOG/current/.keep
 docker/plugins-docker/Dockerfile
 docker/plugins-docker/docker.sh
 docker/publish/.dockerignore
 docker/publish/Dockerfile
 docker/publish/templates/template_dispatcher.ini
 docker/publish/templates/template_dispatcher.yaml
@@ -237,14 +242,15 @@
 faraday_agent_dispatcher/cli/utils/exceptions.py
 faraday_agent_dispatcher/cli/utils/general_inputs.py
 faraday_agent_dispatcher/cli/utils/general_prompts.py
 faraday_agent_dispatcher/cli/utils/model_load.py
 faraday_agent_dispatcher/static/executors/official/appscan.py
 faraday_agent_dispatcher/static/executors/official/arachni.py
 faraday_agent_dispatcher/static/executors/official/burp.py
+faraday_agent_dispatcher/static/executors/official/cisco_cybervision.py
 faraday_agent_dispatcher/static/executors/official/codeql.py
 faraday_agent_dispatcher/static/executors/official/crackmapexec.py
 faraday_agent_dispatcher/static/executors/official/dependabot.py
 faraday_agent_dispatcher/static/executors/official/github_secrets.py
 faraday_agent_dispatcher/static/executors/official/gvm_openvas.py
 faraday_agent_dispatcher/static/executors/official/insightvm.py
 faraday_agent_dispatcher/static/executors/official/nessus.py
@@ -254,21 +260,23 @@
 faraday_agent_dispatcher/static/executors/official/openvas_legacy.py
 faraday_agent_dispatcher/static/executors/official/qualys.py
 faraday_agent_dispatcher/static/executors/official/report_processor.py
 faraday_agent_dispatcher/static/executors/official/shodan2.py
 faraday_agent_dispatcher/static/executors/official/sonarqube.py
 faraday_agent_dispatcher/static/executors/official/sublist3r.sh
 faraday_agent_dispatcher/static/executors/official/tenableio.py
+faraday_agent_dispatcher/static/executors/official/tenablesc.py
 faraday_agent_dispatcher/static/executors/official/w3af.py
 faraday_agent_dispatcher/static/executors/official/wpscan.py
 faraday_agent_dispatcher/static/executors/official/wpscan_legacy.py
 faraday_agent_dispatcher/static/executors/official/zap.py
 faraday_agent_dispatcher/utils/__init__.py
 faraday_agent_dispatcher/utils/control_values_utils.py
 faraday_agent_dispatcher/utils/metadata_utils.py
+faraday_agent_dispatcher/utils/severity_utils.py
 faraday_agent_dispatcher/utils/text_utils.py
 faraday_agent_dispatcher/utils/url_utils.py
 tests/__init__.py
 tests/data/__init__.py
 tests/data/basic_executor.py
 tests/data/mock.pub
 tests/data/ok.crt
```

### Comparing `faraday_agent_dispatcher-3.3.0/setup.py` & `faraday_agent_dispatcher-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tests/data/basic_executor.py` & `faraday_agent_dispatcher-3.4.0/tests/data/basic_executor.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tests/data/ok.crt` & `faraday_agent_dispatcher-3.4.0/tests/data/ok.crt`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tests/data/ok.key` & `faraday_agent_dispatcher-3.4.0/tests/data/ok.key`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.0_with_agent_token.ini` & `faraday_agent_dispatcher-3.4.0/tests/data/old_version_inis/1.0_with_agent_token.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.2.ini` & `faraday_agent_dispatcher-3.4.0/tests/data/old_version_inis/1.2.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.2_with_agent_token.ini` & `faraday_agent_dispatcher-3.4.0/tests/data/old_version_inis/1.2_with_agent_token.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tests/data/old_version_inis/1.5.ini` & `faraday_agent_dispatcher-3.4.0/tests/data/old_version_inis/1.5.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tests/data/test_config.ini` & `faraday_agent_dispatcher-3.4.0/tests/data/test_config.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tests/data/wrong.crt` & `faraday_agent_dispatcher-3.4.0/tests/data/wrong.crt`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tests/integration/faraday/test_execution.py` & `faraday_agent_dispatcher-3.4.0/tests/integration/faraday/test_execution.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tests/plugins-docker/test_executors.py` & `faraday_agent_dispatcher-3.4.0/tests/plugins-docker/test_executors.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tests/unittests/config/agent_dispatcher.py` & `faraday_agent_dispatcher-3.4.0/tests/unittests/config/agent_dispatcher.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tests/unittests/config/wizard.py` & `faraday_agent_dispatcher-3.4.0/tests/unittests/config/wizard.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tests/unittests/test_agent_dispatcher.py` & `faraday_agent_dispatcher-3.4.0/tests/unittests/test_agent_dispatcher.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tests/unittests/test_config_wizard.py` & `faraday_agent_dispatcher-3.4.0/tests/unittests/test_config_wizard.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tests/unittests/test_import_official_executors.py` & `faraday_agent_dispatcher-3.4.0/tests/unittests/test_import_official_executors.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tests/unittests/wizard_input.py` & `faraday_agent_dispatcher-3.4.0/tests/unittests/wizard_input.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tests/utils/testing_faraday_server.py` & `faraday_agent_dispatcher-3.4.0/tests/utils/testing_faraday_server.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-3.3.0/tox.ini` & `faraday_agent_dispatcher-3.4.0/tox.ini`

 * *Files identical despite different names*

