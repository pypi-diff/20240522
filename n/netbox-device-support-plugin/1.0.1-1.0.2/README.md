# Comparing `tmp/netbox_device_support_plugin-1.0.1.tar.gz` & `tmp/netbox_device_support_plugin-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_device_support_plugin-1.0.1.tar", last modified: Fri May 17 18:07:56 2024, max compression
+gzip compressed data, was "netbox_device_support_plugin-1.0.2.tar", last modified: Fri May 17 19:44:05 2024, max compression
```

## Comparing `netbox_device_support_plugin-1.0.1.tar` & `netbox_device_support_plugin-1.0.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.941671 netbox_device_support_plugin-1.0.1/
--rw-r--r--   0 vsts      (1001) docker     (127)     1068 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)       58 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    13514 2024-05-17 18:07:56.941671 netbox_device_support_plugin-1.0.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    12867 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.937671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2917 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/admin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.937671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/api/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4667 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/api/serializers.py
--rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/api/urls.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1657 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/api/views.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6089 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/filtersets.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13398 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/forms.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.937671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/management/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/management/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.937671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/management/commands/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/management/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40834 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8273 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/management/commands/sync_fortinet_support_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8319 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/management/commands/sync_purestorage_support_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.937671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/migrations/
--rw-r--r--   0 vsts      (1001) docker     (127)     7956 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/migrations/0001_initial.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/migrations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    32812 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/models.py
--rw-r--r--   0 vsts      (1001) docker     (127)      739 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/navigation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5749 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/tables.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6535 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/template_content.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.933671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.937671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/
--rw-r--r--   0 vsts      (1001) docker     (127)     6284 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/cisco_device_support.html
--rw-r--r--   0 vsts      (1001) docker     (127)     4237 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.941671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/
--rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      896 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1078 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1030 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      966 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1046 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.941671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/fortinet/
--rw-r--r--   0 vsts      (1001) docker     (127)     4308 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.941671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/fortinet/inc/
--rw-r--r--   0 vsts      (1001) docker     (127)      896 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/fortinet/inc/device_eor_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      896 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/fortinet/inc/device_eos_bar.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.941671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/purestorage/
--rw-r--r--   0 vsts      (1001) docker     (127)     1845 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/purestorage/purestorage_device_support.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.941671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templatetags/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templatetags/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2960 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templatetags/filters.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2107 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/urls.py
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3402 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/views.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.941671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    13514 2024-05-17 18:07:56.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2649 2024-05-17 18:07:56.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-17 18:07:56.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-17 18:07:56.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-05-17 18:07:56.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-17 18:07:56.941671 netbox_device_support_plugin-1.0.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1570 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.606308 netbox_device_support_plugin-1.0.2/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1068 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)       58 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    13514 2024-05-17 19:44:05.606308 netbox_device_support_plugin-1.0.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    12867 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.602308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2917 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/admin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.602308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/api/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4667 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/api/serializers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/api/urls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1657 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/api/views.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6089 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/filtersets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13398 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/forms.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.602308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.602308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/commands/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40821 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8273 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/commands/sync_fortinet_support_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8319 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/commands/sync_purestorage_support_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.602308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/migrations/
+-rw-r--r--   0 vsts      (1001) docker     (127)     7956 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/migrations/0001_initial.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/migrations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    32812 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/models.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      739 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/navigation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5749 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/tables.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6535 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/template_content.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.598308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.602308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6284 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/cisco_device_support.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     4237 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.602308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/
+-rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      896 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1078 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1030 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      966 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1046 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.602308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/fortinet/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4308 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.606308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/fortinet/inc/
+-rw-r--r--   0 vsts      (1001) docker     (127)      896 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/fortinet/inc/device_eor_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      896 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/fortinet/inc/device_eos_bar.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.606308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/purestorage/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1845 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/purestorage/purestorage_device_support.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.606308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templatetags/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templatetags/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2960 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templatetags/filters.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2107 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/urls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3402 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/views.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 19:44:05.606308 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    13514 2024-05-17 19:44:05.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2649 2024-05-17 19:44:05.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-17 19:44:05.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-17 19:44:05.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-05-17 19:44:05.000000 netbox_device_support_plugin-1.0.2/netbox_device_support_plugin.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-17 19:44:05.606308 netbox_device_support_plugin-1.0.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1570 2024-05-17 19:43:50.000000 netbox_device_support_plugin-1.0.2/setup.py
```

### Comparing `netbox_device_support_plugin-1.0.1/LICENSE` & `netbox_device_support_plugin-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/PKG-INFO` & `netbox_device_support_plugin-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-device-support-plugin
-Version: 1.0.1
+Version: 1.0.2
 Summary: Cisco device support, device type support, and software release information with the Cisco support APIs
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox_device_support_plugin-1.0.1/README.md` & `netbox_device_support_plugin-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/__init__.py` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/admin.py` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/admin.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/api/serializers.py` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/api/views.py` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/filtersets.py` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/forms.py` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -825,17 +825,17 @@
                 text = f"Get data for serial number {serial_number}"
                 print(self.task_error(text=text, changed=False))
                 print(f"{serial_number} - No PID found for this serial number")
                 continue
 
             # Normalize the PID list to match the base_pid of the API specs
             # Find PIDs which don't have a Cisco software
-            rm_prefixes = ["UCSC", "AIR-CAP"]
-            rm_suffixes = ["AXI", "AXI-E", "AXE", "AXE-E"]
-            if pid.startswith(tuple(rm_prefixes)) or pid.endswith(tuple(rm_suffixes)):
+            prefixes = ["UCSC", "AIR-AP"]
+            suffixes = ["AXI", "AXI-E", "AXE", "AXE-E"]
+            if pid.startswith(tuple(prefixes)) or pid.endswith(tuple(suffixes)):
                 data = "PID without Cisco software"
                 # Call our Device Type Update method for that particular PID
                 self.update_device_ss_data(serial_number, pid, data)
                 continue
 
             # Call the release suggestions
             url = f"{base_url}/software/suggestion/v2/suggestions/releases/productIds/{pid}"
```

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/management/commands/sync_fortinet_support_data.py` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/commands/sync_fortinet_support_data.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/management/commands/sync_purestorage_support_data.py` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/management/commands/sync_purestorage_support_data.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/migrations/0001_initial.py` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/models.py` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/models.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/navigation.py` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/tables.py` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/template_content.py` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/cisco_device_support.html` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/cisco_device_support.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/fortinet/inc/device_eor_bar.html` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/fortinet/inc/device_eor_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/fortinet/inc/device_eos_bar.html` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/fortinet/inc/device_eos_bar.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/purestorage/purestorage_device_support.html` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templates/purestorage/purestorage_device_support.html`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templatetags/filters.py` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/templatetags/filters.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/urls.py` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/views.py` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin/views.py`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin.egg-info/PKG-INFO` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-device-support-plugin
-Version: 1.0.1
+Version: 1.0.2
 Summary: Cisco device support, device type support, and software release information with the Cisco support APIs
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin.egg-info/SOURCES.txt` & `netbox_device_support_plugin-1.0.2/netbox_device_support_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox_device_support_plugin-1.0.1/setup.py` & `netbox_device_support_plugin-1.0.2/setup.py`

 * *Files identical despite different names*

