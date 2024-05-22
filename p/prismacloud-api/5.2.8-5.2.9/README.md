# Comparing `tmp/prismacloud-api-5.2.8.tar.gz` & `tmp/prismacloud-api-5.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prismacloud-api-5.2.8.tar", last modified: Tue Oct  3 13:06:39 2023, max compression
+gzip compressed data, was "prismacloud-api-5.2.9.tar", last modified: Thu Dec 21 12:24:15 2023, max compression
```

## Comparing `prismacloud-api-5.2.8.tar` & `prismacloud-api-5.2.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 13:06:39.374402 prismacloud-api-5.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2023-10-03 13:06:39.370402 prismacloud-api-5.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 13:06:39.366402 prismacloud-api-5.2.8/prismacloud/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 13:06:39.366402 prismacloud-api-5.2.8/prismacloud/api/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 13:06:39.366402 prismacloud-api-5.2.8/prismacloud/api/cspm/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cspm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18880 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cspm/_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cspm/_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     8900 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cspm/cspm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 13:06:39.370402 prismacloud-api-5.2.8/prismacloud/api/cwpp/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/_audits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/_defenders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/_feeds.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/_scans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/_vms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/cwpp/cwpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/pc_lib_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17122 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/pc_lib_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 13:06:39.370402 prismacloud-api-5.2.8/prismacloud/api/pccs/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/pccs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/pccs/_checkov_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/pccs/_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/pccs/_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/pccs/_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/pccs/_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/pccs/_scans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/pccs/_suppressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/pccs/pccs.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/prismacloud/api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 13:06:39.370402 prismacloud-api-5.2.8/prismacloud_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2023-10-03 13:06:39.000000 prismacloud-api-5.2.8/prismacloud_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2023-10-03 13:06:39.000000 prismacloud-api-5.2.8/prismacloud_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-03 13:06:39.000000 prismacloud-api-5.2.8/prismacloud_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-03 13:06:39.000000 prismacloud-api-5.2.8/prismacloud_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-10-03 13:06:39.000000 prismacloud-api-5.2.8/prismacloud_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 13:06:39.366402 prismacloud-api-5.2.8/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 13:06:39.370402 prismacloud-api-5.2.8/scripts/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/scripts/examples/pcs_vuln_container_with_cve_2022_22965.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-03 13:06:39.374402 prismacloud-api-5.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 13:06:39.370402 prismacloud-api-5.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2023-10-03 13:06:20.000000 prismacloud-api-5.2.8/tests/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 12:24:15.271259 prismacloud-api-5.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2023-12-21 12:24:15.271259 prismacloud-api-5.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 12:24:15.263259 prismacloud-api-5.2.9/prismacloud/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 12:24:15.263259 prismacloud-api-5.2.9/prismacloud/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 12:24:15.263259 prismacloud-api-5.2.9/prismacloud/api/cspm/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cspm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19276 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cspm/_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cspm/_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8900 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cspm/cspm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 12:24:15.267259 prismacloud-api-5.2.9/prismacloud/api/cwpp/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/_audits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/_defenders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/_scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/_vms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/cwpp/cwpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/pc_lib_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17332 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/pc_lib_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 12:24:15.271259 prismacloud-api-5.2.9/prismacloud/api/pccs/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/pccs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/pccs/_checkov_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/pccs/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/pccs/_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/pccs/_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/pccs/_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/pccs/_scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/pccs/_suppressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/pccs/pccs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/prismacloud/api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 12:24:15.271259 prismacloud-api-5.2.9/prismacloud_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2023-12-21 12:24:15.000000 prismacloud-api-5.2.9/prismacloud_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2023-12-21 12:24:15.000000 prismacloud-api-5.2.9/prismacloud_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 12:24:15.000000 prismacloud-api-5.2.9/prismacloud_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-21 12:24:15.000000 prismacloud-api-5.2.9/prismacloud_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-21 12:24:15.000000 prismacloud-api-5.2.9/prismacloud_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 12:24:15.263259 prismacloud-api-5.2.9/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 12:24:15.271259 prismacloud-api-5.2.9/scripts/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/scripts/examples/pcs_vuln_container_with_cve_2022_22965.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-21 12:24:15.271259 prismacloud-api-5.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 12:24:15.271259 prismacloud-api-5.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2023-12-21 12:23:59.000000 prismacloud-api-5.2.9/tests/unit.py
```

### Comparing `prismacloud-api-5.2.8/LICENSE` & `prismacloud-api-5.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/PKG-INFO` & `prismacloud-api-5.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prismacloud-api
-Version: 5.2.8
+Version: 5.2.9
 Summary: Prisma Cloud API SDK for Python
 Home-page: https://github.com/PaloAltoNetworks/prismacloud-api-python
 Author: Tom Kishel
 Author-email: tkishel@paloaltonetworks.com
 Keywords: prisma cloud api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prismacloud-api-5.2.8/README.md` & `prismacloud-api-5.2.9/README.md`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cspm/_endpoints.py` & `prismacloud-api-5.2.9/prismacloud/api/cspm/_endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -534,14 +534,22 @@
             api_response = self.execute(
                 'POST', 'api/v1/permission/page', body_params={'limit': 1000, 'pageToken': next_page_token, 'withResourceJson': 'true'})
             if 'items' in api_response:
                 result.extend(api_response['items'])
             next_page_token = api_response.pop('nextPageToken', None)
         return result
 
+    def search_iam_source_to_granter(self, search_params):
+        search_url = 'api/v1/permission/graph/source_to_granter'
+        return self.execute('POST', search_url, body_params=search_params)
+
+    def search_iam_granter_to_dest(self, search_params):
+        search_url = 'api/v1/permission/graph/granter_to_dest'
+        return self.execute('POST', search_url, body_params=search_params)
+
     def search_suggest_list_read(self, query_to_suggest):
         return self.execute('POST', 'search/suggest', body_params=query_to_suggest)
 
     """
     Configuration
 
     [ ] LIST
```

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cspm/_extended.py` & `prismacloud-api-5.2.9/prismacloud/api/cspm/_extended.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cspm/cspm.py` & `prismacloud-api-5.2.9/prismacloud/api/cspm/cspm.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cwpp/__init__.py` & `prismacloud-api-5.2.9/prismacloud/api/cwpp/__init__.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cwpp/_audits.py` & `prismacloud-api-5.2.9/prismacloud/api/cwpp/_audits.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cwpp/_cloud.py` & `prismacloud-api-5.2.9/prismacloud/api/cwpp/_cloud.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cwpp/_collections.py` & `prismacloud-api-5.2.9/prismacloud/api/cwpp/_collections.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cwpp/_containers.py` & `prismacloud-api-5.2.9/prismacloud/api/cwpp/_containers.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cwpp/_credentials.py` & `prismacloud-api-5.2.9/prismacloud/api/cwpp/_credentials.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cwpp/_defenders.py` & `prismacloud-api-5.2.9/prismacloud/api/cwpp/_defenders.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cwpp/_feeds.py` & `prismacloud-api-5.2.9/prismacloud/api/cwpp/_feeds.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cwpp/_hosts.py` & `prismacloud-api-5.2.9/prismacloud/api/cwpp/_hosts.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cwpp/_images.py` & `prismacloud-api-5.2.9/prismacloud/api/cwpp/_images.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cwpp/_logs.py` & `prismacloud-api-5.2.9/prismacloud/api/cwpp/_logs.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cwpp/_policies.py` & `prismacloud-api-5.2.9/prismacloud/api/cwpp/_policies.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cwpp/_registry.py` & `prismacloud-api-5.2.9/prismacloud/api/cwpp/_registry.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cwpp/_scans.py` & `prismacloud-api-5.2.9/prismacloud/api/cwpp/_scans.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cwpp/_settings.py` & `prismacloud-api-5.2.9/prismacloud/api/cwpp/_settings.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cwpp/_stats.py` & `prismacloud-api-5.2.9/prismacloud/api/cwpp/_stats.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cwpp/_tags.py` & `prismacloud-api-5.2.9/prismacloud/api/cwpp/_tags.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/cwpp/cwpp.py` & `prismacloud-api-5.2.9/prismacloud/api/cwpp/cwpp.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/pc_lib_api.py` & `prismacloud-api-5.2.9/prismacloud/api/pc_lib_api.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/pc_lib_utility.py` & `prismacloud-api-5.2.9/prismacloud/api/pc_lib_utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,24 +13,33 @@
 
 try:
     # pylint: disable=redefined-builtin
     input = raw_input
 except NameError:
     pass
 
+try:
+    from pathlib import Path
+    homefolder = str(Path.home())
+except:
+    if "USERPROFILE" in os.environ:
+        homefolder = os.environ["USERPROFILE"]
+    else:
+        homefolder = os.environ["HOME"]
+        
 # --Description-- #
 
 # Prisma Cloud Helper library.
 
 # --Helper Methods-- #
 
 class PrismaCloudUtility():
     """ Prisma Cloud Utility Class """
 
-    CONFIG_DIRECTORY = os.path.join(os.environ['HOME'], '.prismacloud')
+    CONFIG_DIRECTORY = os.path.join(homefolder, '.prismacloud')
     DEFAULT_CONFIG_FILE = os.path.join(CONFIG_DIRECTORY, 'credentials.json')
 
     @classmethod
     def package_version_check(cls, package_name='prismacloud-api'):
         package_version_message = 'version: %s' % api_version
         checker = UpdateChecker()
         result = checker.check(package_name, api_version)
```

### Comparing `prismacloud-api-5.2.8/prismacloud/api/pccs/__init__.py` & `prismacloud-api-5.2.9/prismacloud/api/pccs/__init__.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/pccs/_errors.py` & `prismacloud-api-5.2.9/prismacloud/api/pccs/_errors.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/pccs/_repositories.py` & `prismacloud-api-5.2.9/prismacloud/api/pccs/_repositories.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/pccs/_suppressions.py` & `prismacloud-api-5.2.9/prismacloud/api/pccs/_suppressions.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud/api/pccs/pccs.py` & `prismacloud-api-5.2.9/prismacloud/api/pccs/pccs.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/prismacloud_api.egg-info/PKG-INFO` & `prismacloud-api-5.2.9/prismacloud_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prismacloud-api
-Version: 5.2.8
+Version: 5.2.9
 Summary: Prisma Cloud API SDK for Python
 Home-page: https://github.com/PaloAltoNetworks/prismacloud-api-python
 Author: Tom Kishel
 Author-email: tkishel@paloaltonetworks.com
 Keywords: prisma cloud api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prismacloud-api-5.2.8/prismacloud_api.egg-info/SOURCES.txt` & `prismacloud-api-5.2.9/prismacloud_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/scripts/examples/pcs_vuln_container_with_cve_2022_22965.py` & `prismacloud-api-5.2.9/scripts/examples/pcs_vuln_container_with_cve_2022_22965.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/setup.py` & `prismacloud-api-5.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.8/tests/unit.py` & `prismacloud-api-5.2.9/tests/unit.py`

 * *Files identical despite different names*

