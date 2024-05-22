# Comparing `tmp/faraday_agent_parameters_types-1.5.0.tar.gz` & `tmp/faraday_agent_parameters_types-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faraday_agent_parameters_types-1.5.0.tar", last modified: Wed Mar  6 17:55:10 2024, max compression
+gzip compressed data, was "faraday_agent_parameters_types-1.5.1.tar", last modified: Thu Mar  7 19:49:44 2024, max compression
```

## Comparing `faraday_agent_parameters_types-1.5.0.tar` & `faraday_agent_parameters_types-1.5.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 17:55:10.025354 faraday_agent_parameters_types-1.5.0/
--rw-rw-rw-   0 root         (0) root         (0)      244 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)      383 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     3781 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    35149 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      317 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2721 2024-03-06 17:55:10.025354 faraday_agent_parameters_types-1.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      928 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 17:55:09.953354 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/
--rw-rw-rw-   0 root         (0) root         (0)      318 2024-03-06 17:47:44.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 17:55:09.969354 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/custom_types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/custom_types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/custom_types/faraday_boolean.py
--rw-rw-rw-   0 root         (0) root         (0)      387 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/custom_types/faraday_float.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/custom_types/faraday_int_range.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/custom_types/faraday_integer.py
--rw-rw-rw-   0 root         (0) root         (0)      486 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/custom_types/faraday_ip.py
--rw-rw-rw-   0 root         (0) root         (0)      684 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/custom_types/faraday_list.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/custom_types/faraday_string.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/custom_types/faraday_url.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/data_types.py
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-05-05 20:35:41.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/faraday_agent_parameters_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 17:55:09.945354 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 17:55:10.009354 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/
--rw-rw-rw-   0 root         (0) root         (0)      562 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/arachni-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      722 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/burp-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      650 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/burp-2.0.1.json
--rw-rw-rw-   0 root         (0) root         (0)      515 2024-02-29 18:53:56.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/codeql-1.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      885 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/crackmapexec-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      530 2024-02-29 18:53:56.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/dependabot-1.1.0.json
--rw-rw-rw-   0 root         (0) root         (0)      542 2024-03-06 17:43:01.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/github_secrets-1.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)     1427 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/gvm_openvas-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      814 2023-05-11 13:05:06.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/hclappscan-2.6.0.json
--rw-rw-rw-   0 root         (0) root         (0)      651 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/insightvm-2.0.1.json
--rw-rw-rw-   0 root         (0) root         (0)      843 2024-01-31 20:13:02.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/nessus-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      541 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/nikto2-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      458 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/nikto2-2.1.3.json
--rw-rw-rw-   0 root         (0) root         (0)     1060 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/nmap-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)     1146 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/nmap-2.1.2.json
--rw-rw-rw-   0 root         (0) root         (0)      631 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/nuclei-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      937 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/openvas_legacy-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      679 2022-10-26 15:05:28.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/qualys-2.4.0.json
--rw-rw-rw-   0 root         (0) root         (0)      597 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/report_processor-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      476 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/shodan2-2.1.2.json
--rw-rw-rw-   0 root         (0) root         (0)      571 2024-01-11 17:51:26.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/sonarqube-2.3.0.json
--rw-rw-rw-   0 root         (0) root         (0)      533 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/sublist3r-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-08-02 17:55:33.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/tenableio-2.3.0.json
--rw-rw-rw-   0 root         (0) root         (0)      501 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/w3af-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      519 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/wpscan-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      701 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/wpscan-2.1.2.json
--rw-rw-rw-   0 root         (0) root         (0)      581 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/wpscan_legacy-2.0.0.json
--rw-rw-rw-   0 root         (0) root         (0)      472 2022-10-19 20:21:37.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/zap-2.0.1.json
--rw-rw-rw-   0 root         (0) root         (0)     3278 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 17:55:10.021354 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2721 2024-03-06 17:55:09.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3307 2024-03-06 17:55:09.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-06 17:55:09.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-06 17:55:09.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      135 2024-03-06 17:55:09.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2024-03-06 17:55:09.000000 faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      472 2024-03-06 17:55:10.025354 faraday_agent_parameters_types-1.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2084 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 17:55:10.017354 faraday_agent_parameters_types-1.5.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      215 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/tests/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       60 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9588 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/tests/test_faraday_agent_parameters_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 17:55:10.021354 faraday_agent_parameters_types-1.5.0/tests/test_manifests/
--rw-rw-rw-   0 root         (0) root         (0)      458 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/tests/test_manifests/test-1.5.0.json
--rw-rw-rw-   0 root         (0) root         (0)      458 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/tests/test_manifests/test-1.7.0.json
--rw-rw-rw-   0 root         (0) root         (0)      458 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/tests/test_manifests/test-1.8.0.json
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-08-22 21:01:04.000000 faraday_agent_parameters_types-1.5.0/tests/test_manifests/test2-1.6.0.json
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-05-11 13:14:49.000000 faraday_agent_parameters_types-1.5.0/tests/test_manifests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 19:49:44.428908 faraday_agent_parameters_types-1.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     3781 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2721 2024-03-07 19:49:44.428908 faraday_agent_parameters_types-1.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 19:49:44.416908 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/
+-rw-rw-rw-   0 root         (0) root         (0)      318 2024-03-07 19:44:35.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 19:49:44.420908 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/custom_types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/custom_types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/custom_types/faraday_boolean.py
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/custom_types/faraday_float.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/custom_types/faraday_int_range.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/custom_types/faraday_integer.py
+-rw-rw-rw-   0 root         (0) root         (0)      486 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/custom_types/faraday_ip.py
+-rw-rw-rw-   0 root         (0) root         (0)      684 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/custom_types/faraday_list.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/custom_types/faraday_string.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/custom_types/faraday_url.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/data_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/faraday_agent_parameters_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 19:49:44.412908 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 19:49:44.424908 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/arachni-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/burp-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      650 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/burp-2.0.1.json
+-rw-rw-rw-   0 root         (0) root         (0)      515 2024-02-29 18:54:28.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/codeql-1.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      885 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/crackmapexec-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      530 2024-02-29 18:54:28.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/dependabot-1.1.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      542 2024-03-04 16:08:52.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/github_secrets-1.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/gvm_openvas-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      814 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/hclappscan-2.6.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      651 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/insightvm-2.0.1.json
+-rw-rw-rw-   0 root         (0) root         (0)      843 2024-01-31 20:12:26.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/nessus-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/nikto2-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/nikto2-2.1.3.json
+-rw-rw-rw-   0 root         (0) root         (0)     1060 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/nmap-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)     1146 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/nmap-2.1.2.json
+-rw-rw-rw-   0 root         (0) root         (0)      631 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/nuclei-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      937 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/openvas_legacy-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/qualys-2.4.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      597 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/report_processor-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      476 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/shodan2-2.1.2.json
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-03-06 19:41:21.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/sonarqube-2.3.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      533 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/sublist3r-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/tenableio-2.3.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/w3af-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      519 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/wpscan-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/wpscan-2.1.2.json
+-rw-rw-rw-   0 root         (0) root         (0)      581 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/wpscan_legacy-2.0.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      472 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/zap-2.0.1.json
+-rw-rw-rw-   0 root         (0) root         (0)     3278 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 19:49:44.428908 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2721 2024-03-07 19:49:44.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3307 2024-03-07 19:49:44.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-07 19:49:44.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-07 19:49:44.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      135 2024-03-07 19:49:44.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2024-03-07 19:49:44.000000 faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      472 2024-03-07 19:49:44.432908 faraday_agent_parameters_types-1.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 19:49:44.428908 faraday_agent_parameters_types-1.5.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/tests/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9588 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/tests/test_faraday_agent_parameters_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 19:49:44.428908 faraday_agent_parameters_types-1.5.1/tests/test_manifests/
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/tests/test_manifests/test-1.5.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/tests/test_manifests/test-1.7.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/tests/test_manifests/test-1.8.0.json
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/tests/test_manifests/test2-1.6.0.json
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-11-10 19:02:56.000000 faraday_agent_parameters_types-1.5.1/tests/test_manifests.py
```

### Comparing `faraday_agent_parameters_types-1.5.0/CONTRIBUTING.rst` & `faraday_agent_parameters_types-1.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/COPYING` & `faraday_agent_parameters_types-1.5.1/COPYING`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/PKG-INFO` & `faraday_agent_parameters_types-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faraday_agent_parameters_types
-Version: 1.5.0
+Version: 1.5.1
 Summary: The faraday agents run code remotely to ensure your domains. This info is triggered and published
 Home-page: https://github.com/infobyte/faraday_agent_parameters_types
 Author: Faraday Development Team
 Author-email: devel@infobytesec.com
 License: GNU General Public License v3
 Keywords: faraday
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `faraday_agent_parameters_types-1.5.0/README.md` & `faraday_agent_parameters_types-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/custom_types/faraday_int_range.py` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/custom_types/faraday_int_range.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/custom_types/faraday_list.py` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/custom_types/faraday_list.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/custom_types/faraday_string.py` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/custom_types/faraday_string.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/data_types.py` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/data_types.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/arachni-2.0.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/arachni-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/burp-2.0.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/burp-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/burp-2.0.1.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/burp-2.0.1.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/codeql-1.0.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/codeql-1.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/crackmapexec-2.0.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/crackmapexec-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/dependabot-1.1.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/dependabot-1.1.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/github_secrets-1.0.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/github_secrets-1.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/gvm_openvas-2.0.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/gvm_openvas-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/hclappscan-2.6.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/hclappscan-2.6.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/insightvm-2.0.1.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/insightvm-2.0.1.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/nessus-2.0.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/nessus-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/nikto2-2.0.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/nikto2-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/nmap-2.0.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/nmap-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/nmap-2.1.2.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/nmap-2.1.2.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/nuclei-2.0.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/nuclei-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/openvas_legacy-2.0.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/openvas_legacy-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/qualys-2.4.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/qualys-2.4.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/report_processor-2.0.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/report_processor-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/sonarqube-2.3.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/wpscan-2.1.2.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5833333333333334%*

 * *Differences: {"'arguments'": "{replace: OrderedDict([('WPSCAN_TARGET_URL', OrderedDict([('mandatory', True), "*

 * *                "('type', 'url'), ('base', 'string')])), ('WPSCAN_API_TOKEN', "*

 * *                "OrderedDict([('mandatory', False), ('type', 'string'), ('base', 'string')])), "*

 * *                "('WPSCAN_RANDOM_USER_AGENT', OrderedDict([('mandatory', False), ('type', "*

 * *                "'boolean'), ('base', 'boolean')]))])}",*

 * * "'category'": "'Web App Scanners'",*

 * * "'check_cmds'": "['wpscan --version']",*

 * * "'descrip […]*

```diff
@@ -1,27 +1,32 @@
 {
     "arguments": {
-        "COMPONENT_KEY": {
+        "WPSCAN_API_TOKEN": {
             "base": "string",
             "mandatory": false,
             "type": "string"
         },
-        "TOKEN": {
+        "WPSCAN_RANDOM_USER_AGENT": {
+            "base": "boolean",
+            "mandatory": false,
+            "type": "boolean"
+        },
+        "WPSCAN_TARGET_URL": {
             "base": "string",
             "mandatory": true,
-            "type": "string"
+            "type": "url"
         }
     },
-    "category": "Source Code Analisys",
-    "check_cmds": [],
-    "cmd": "{EXECUTOR_FILE_PATH}",
-    "description": "Source Code Analisys",
-    "environment_variables": [
-        "SONAR_URL"
+    "category": "Web App Scanners",
+    "check_cmds": [
+        "wpscan --version"
     ],
+    "cmd": "{EXECUTOR_FILE_PATH}",
+    "description": "WordPress Security Scanner",
+    "environment_variables": [],
     "image": null,
-    "manifest_version": "2.3.0",
-    "name": "sonarqube",
-    "repo_executor": "sonarqube.py",
-    "title": "SonarQube",
-    "website": "https://www.sonarqube.org/"
+    "manifest_version": "2.1.2",
+    "name": "wpscan",
+    "repo_executor": "wpscan.py",
+    "title": "Wpscan",
+    "website": "https://wpscan.com/wordpress-security-scanner"
 }
```

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/sublist3r-2.0.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/sublist3r-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/tenableio-2.3.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/tenableio-2.3.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/wpscan-2.0.0.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/wpscan-2.0.0.json`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/static/manifests/wpscan-2.1.2.json` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/static/manifests/wpscan_legacy-2.0.0.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7638888888888888%*

 * *Differences: {"'arguments'": "{delete: ['WPSCAN_API_TOKEN', 'WPSCAN_RANDOM_USER_AGENT']}",*

 * * "'check_cmds'": "['docker -v', 'docker images -q wpscanteam/wpscan']",*

 * * "'manifest_version'": "'2.0.0'",*

 * * "'name'": "'wpscan_legacy'",*

 * * "'repo_executor'": "'wpscan_legacy.py'",*

 * * "'title'": "'Wpscan (Legacy)'"}*

```diff
@@ -1,32 +1,23 @@
 {
     "arguments": {
-        "WPSCAN_API_TOKEN": {
-            "base": "string",
-            "mandatory": false,
-            "type": "string"
-        },
-        "WPSCAN_RANDOM_USER_AGENT": {
-            "base": "boolean",
-            "mandatory": false,
-            "type": "boolean"
-        },
         "WPSCAN_TARGET_URL": {
             "base": "string",
             "mandatory": true,
             "type": "url"
         }
     },
     "category": "Web App Scanners",
     "check_cmds": [
-        "wpscan --version"
+        "docker -v",
+        "docker images -q wpscanteam/wpscan"
     ],
     "cmd": "{EXECUTOR_FILE_PATH}",
     "description": "WordPress Security Scanner",
     "environment_variables": [],
     "image": null,
-    "manifest_version": "2.1.2",
-    "name": "wpscan",
-    "repo_executor": "wpscan.py",
-    "title": "Wpscan",
+    "manifest_version": "2.0.0",
+    "name": "wpscan_legacy",
+    "repo_executor": "wpscan_legacy.py",
+    "title": "Wpscan (Legacy)",
     "website": "https://wpscan.com/wordpress-security-scanner"
 }
```

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types/utils.py` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types/utils.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types.egg-info/PKG-INFO` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faraday_agent_parameters_types
-Version: 1.5.0
+Version: 1.5.1
 Summary: The faraday agents run code remotely to ensure your domains. This info is triggered and published
 Home-page: https://github.com/infobyte/faraday_agent_parameters_types
 Author: Faraday Development Team
 Author-email: devel@infobytesec.com
 License: GNU General Public License v3
 Keywords: faraday
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `faraday_agent_parameters_types-1.5.0/faraday_agent_parameters_types.egg-info/SOURCES.txt` & `faraday_agent_parameters_types-1.5.1/faraday_agent_parameters_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/setup.py` & `faraday_agent_parameters_types-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/tests/test_faraday_agent_parameters_types.py` & `faraday_agent_parameters_types-1.5.1/tests/test_faraday_agent_parameters_types.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_parameters_types-1.5.0/tests/test_manifests.py` & `faraday_agent_parameters_types-1.5.1/tests/test_manifests.py`

 * *Files identical despite different names*

