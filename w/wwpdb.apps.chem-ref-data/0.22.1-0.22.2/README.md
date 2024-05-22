# Comparing `tmp/wwpdb.apps.chem_ref_data-0.22.1.tar.gz` & `tmp/wwpdb_apps_chem_ref_data-0.22.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.chem_ref_data-0.22.1.tar", last modified: Fri Dec  1 13:04:59 2023, max compression
+gzip compressed data, was "wwpdb_apps_chem_ref_data-0.22.2.tar", last modified: Wed May 22 10:38:46 2024, max compression
```

## Comparing `wwpdb.apps.chem_ref_data-0.22.1.tar` & `wwpdb_apps_chem_ref_data-0.22.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-01 13:04:59.000463 wwpdb.apps.chem_ref_data-0.22.1/
--rw-r--r--   0 vsts      (1001) docker     (127)     1329 2023-12-01 13:04:59.000463 wwpdb.apps.chem_ref_data-0.22.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       92 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2023-12-01 13:04:59.000463 wwpdb.apps.chem_ref_data-0.22.1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2535 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-01 13:04:58.992462 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-01 13:04:58.996462 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-01 13:04:58.996462 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/
--rw-r--r--   0 vsts      (1001) docker     (127)       57 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      152 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-01 13:04:58.996462 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/depict/
--rw-r--r--   0 vsts      (1001) docker     (127)     8619 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4349 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepictBootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-01 13:04:58.996462 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/io/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-01 13:04:58.996462 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/report/
--rw-r--r--   0 vsts      (1001) docker     (127)     8147 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/report/BirdReport.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5517 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/report/ChemCompReport.py
--rw-r--r--   0 vsts      (1001) docker     (127)    32306 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/report/ChemRefReportDepictBootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3626 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/report/ReportUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/report/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-01 13:04:58.996462 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/search/
--rw-r--r--   0 vsts      (1001) docker     (127)    19576 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/search/ChemCompSearchIndexUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      672 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/search/ChemRefSearch.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26693 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/search/ChemRefSearchBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27353 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDef.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19563 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDepictBootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7854 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDuplicates.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2485 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/search/MiscUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/search/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-01 13:04:59.000463 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)    18235 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/utils/ChemRefDataCvsUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11314 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16203 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28056 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/utils/ChemRefDataMiscUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3671 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/utils/DownloadUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1115 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/utils/OSVersion.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-01 13:04:59.000463 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/webapp/
--rw-r--r--   0 vsts      (1001) docker     (127)    48963 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/webapp/ChemRefDataWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-12-01 13:03:34.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-01 13:04:59.000463 wwpdb.apps.chem_ref_data-0.22.1/wwpdb.apps.chem_ref_data.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1329 2023-12-01 13:04:58.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb.apps.chem_ref_data.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1749 2023-12-01 13:04:58.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb.apps.chem_ref_data.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-12-01 13:04:58.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb.apps.chem_ref_data.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-12-01 13:04:45.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb.apps.chem_ref_data.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      341 2023-12-01 13:04:58.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb.apps.chem_ref_data.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2023-12-01 13:04:58.000000 wwpdb.apps.chem_ref_data-0.22.1/wwpdb.apps.chem_ref_data.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 10:38:46.757409 wwpdb_apps_chem_ref_data-0.22.2/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1329 2024-05-22 10:38:46.757409 wwpdb_apps_chem_ref_data-0.22.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       92 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-22 10:38:46.757409 wwpdb_apps_chem_ref_data-0.22.2/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2535 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 10:38:46.753409 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 10:38:46.753409 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 10:38:46.753409 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/
+-rw-r--r--   0 vsts      (1001) docker     (127)       57 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 10:38:46.753409 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/depict/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8619 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4349 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepictBootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 10:38:46.753409 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/io/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 10:38:46.753409 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/report/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8191 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/report/BirdReport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5517 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/report/ChemCompReport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    32306 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/report/ChemRefReportDepictBootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3626 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/report/ReportUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/report/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 10:38:46.757409 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/search/
+-rw-r--r--   0 vsts      (1001) docker     (127)    19576 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/search/ChemCompSearchIndexUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      672 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/search/ChemRefSearch.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26875 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/search/ChemRefSearchBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27353 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/search/ChemRefSearchDef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19563 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/search/ChemRefSearchDepictBootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7854 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/search/ChemRefSearchDuplicates.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2485 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/search/MiscUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/search/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 10:38:46.757409 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)    18235 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/utils/ChemRefDataCvsUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11314 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16203 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28056 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/utils/ChemRefDataMiscUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3671 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/utils/DownloadUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1115 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/utils/OSVersion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 10:38:46.757409 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (127)    49124 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/webapp/ChemRefDataWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-22 10:36:56.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 10:38:46.757409 wwpdb_apps_chem_ref_data-0.22.2/wwpdb.apps.chem_ref_data.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1329 2024-05-22 10:38:46.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb.apps.chem_ref_data.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1749 2024-05-22 10:38:46.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb.apps.chem_ref_data.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-22 10:38:46.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb.apps.chem_ref_data.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-22 10:38:32.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb.apps.chem_ref_data.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      341 2024-05-22 10:38:46.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb.apps.chem_ref_data.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-22 10:38:46.000000 wwpdb_apps_chem_ref_data-0.22.2/wwpdb.apps.chem_ref_data.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/PKG-INFO` & `wwpdb_apps_chem_ref_data-0.22.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.chem_ref_data
-Version: 0.22.1
+Version: 0.22.2
 Summary: wwPDB chemical reference admin application
 Home-page: https://github.com/rcsb/py-wwpdb_apps_chem_ref_data
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/setup.py` & `wwpdb_apps_chem_ref_data-0.22.2/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepict.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepictBootstrap.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepictBootstrap.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/report/BirdReport.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/report/BirdReport.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,15 @@
             logger.exception("Report preparation failed for:  %s", fileName)
 
         #
         oD["hasExpt"] = False
         oD["hasIdeal"] = False
         if pathToImage is not None:
             try:
+                localPrdCcRelativePath = ""
                 prdCcFilePath = pathToImage
                 if prdCcFilePath is not None:
                     (_pth, prdCcFileName) = os.path.split(prdCcFilePath)
                     dp = os.path.join(self.__sessionPath, "report")
                     localPrdCcPath = os.path.join(dp, prdCcFileName)
                     localPrdCcRelativePath = os.path.join(self.__sessionRelativePath, "report", prdCcFileName)
                     if prdCcFilePath != localPrdCcPath:
```

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/report/ChemCompReport.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/report/ChemCompReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/report/ChemRefReportDepictBootstrap.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/report/ChemRefReportDepictBootstrap.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/report/ReportUtils.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/report/ReportUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/search/ChemCompSearchIndexUtils.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/search/ChemCompSearchIndexUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/search/ChemRefSearch.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/search/ChemRefSearch.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/search/ChemRefSearchBase.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/search/ChemRefSearchBase.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,14 +288,17 @@
         logger.debug("searchTarget %r qCols %r", searchTarget, qCols)
         for qCol in qCols:
             pc = "%"
             if compareType == "LIKE":
                 tId = pc + searchTarget + pc
             elif compareType in ["EXACT", "EQUAL"]:
                 tId = searchTarget + pc
+            else:
+                logger.error("compareType %s unknown", compareType)
+                continue
             queryConditionString = ' WHERE %s LIKE "%s"  ' % (qCol, tId)
 
             tL = qCol.split(".")
             tName = ".".join(tL[:-1])
 
             #
             queryString = "SELECT DISTINCT " + qCol + " FROM " + tName + " " + queryConditionString
@@ -559,14 +562,17 @@
         rId = 1
         #
         for sType, cType in zip(searchTypeList, compareTypeList):
             sD[rId] = {}
             # ----
             rList = []
             stdSearchTargetList = []
+            trList = []
+            cList = []
+            wdList = []
             for sTargInp in searchTargetList:
                 sTarg = self.__standardizedSearchTarget(sTargInp, sType)
                 stdSearchTargetList.append(sTarg)
                 if searchServiceType == "rdbms":
                     resourceId = self._getSearchDefResourceId(sType)
                     self.setResource(resourceName=resourceId)
                     ok = self.openConnection()
```

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDef.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/search/ChemRefSearchDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDepictBootstrap.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/search/ChemRefSearchDepictBootstrap.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDuplicates.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/search/ChemRefSearchDuplicates.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/search/MiscUtils.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/search/MiscUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/utils/ChemRefDataCvsUtils.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/utils/ChemRefDataCvsUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbExec.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbExec.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbUtils.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/utils/ChemRefDataMiscUtils.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/utils/ChemRefDataMiscUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/utils/DownloadUtils.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/utils/DownloadUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/utils/OSVersion.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/utils/OSVersion.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb/apps/chem_ref_data/webapp/ChemRefDataWebApp.py` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb/apps/chem_ref_data/webapp/ChemRefDataWebApp.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,14 +249,16 @@
         logger.info("+ChemRefDataWebAppWorker._chemRefInlineFileOps() starting with op %s", operation)
 
         isFile = False
         self.__getSession()
         self.__reqObj.setReturnFormat(return_format="json")
         rC = ResponseContent(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
 
+        filePath = None
+        rootName = None
         if self.__isFileUpload():
             # make a copy of the file in the session directory and set 'fileName'
             self.__uploadFile()
             fileName = self.__reqObj.getValue("fileName")
             filePath = os.path.join(self.__sessionPath, fileName)
             (rootName, _ext) = os.path.splitext(fileName)
             isFile = True
@@ -958,14 +960,17 @@
         rC = ResponseContent(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
 
         crdbu = ChemRefDataDbUtils(self.__reqObj, verbose=self.__debug, log=self.__lfh)
         if referenceDatabase in ["CC"]:
             ok = crdbu.loadChemCompMulti()
         elif referenceDatabase in ["BIRD", "PRD", "PRD_FAMILY"]:
             ok = crdbu.loadBird()
+        else:
+            logger.error("referenceDatabase %s unknown", referenceDatabase)
+            ok = False
 
         if ok:
             rC.setStatus(statusMsg="%s database load completed" % referenceDatabase)
         else:
             rC.setError(errMsg="Database load failed")
 
         return rC
```

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb.apps.chem_ref_data.egg-info/PKG-INFO` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb.apps.chem_ref_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wwpdb.apps.chem-ref-data
-Version: 0.22.1
+Name: wwpdb.apps.chem_ref_data
+Version: 0.22.2
 Summary: wwPDB chemical reference admin application
 Home-page: https://github.com/rcsb/py-wwpdb_apps_chem_ref_data
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.chem_ref_data-0.22.1/wwpdb.apps.chem_ref_data.egg-info/SOURCES.txt` & `wwpdb_apps_chem_ref_data-0.22.2/wwpdb.apps.chem_ref_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

