# Comparing `tmp/pulumi_ns1-3.3.0a1715925999.tar.gz` & `tmp/pulumi_ns1-3.3.0a1716395337.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_ns1-3.3.0a1715925999.tar", last modified: Fri May 17 06:15:14 2024, max compression
+gzip compressed data, was "pulumi_ns1-3.3.0a1716395337.tar", last modified: Wed May 22 16:31:46 2024, max compression
```

## Comparing `pulumi_ns1-3.3.0a1715925999.tar` & `pulumi_ns1-3.3.0a1716395337.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:15:14.360836 pulumi_ns1-3.3.0a1715925999/
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-17 06:15:14.360836 pulumi_ns1-3.3.0a1715925999/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:15:14.360836 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38901 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/account_whitelist.py
--rw-r--r--   0 runner    (1001) docker     (127)    87262 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    16619 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:15:14.360836 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    12682 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/data_feed.py
--rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/dnsview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/get_dns_sec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/get_monitoring_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/get_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/get_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/get_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)    45756 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/monitoring_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    11069 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/notify_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    46058 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10590 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17050 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/pulsar_job.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    44531 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/record.py
--rw-r--r--   0 runner    (1001) docker     (127)    19239 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    81714 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/tsigkey.py
--rw-r--r--   0 runner    (1001) docker     (127)    89234 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    42852 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1/zone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:15:14.360836 pulumi_ns1-3.3.0a1715925999/pulumi_ns1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-17 06:15:14.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-17 06:15:14.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:15:14.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 06:15:14.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 06:15:14.000000 pulumi_ns1-3.3.0a1715925999/pulumi_ns1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-17 06:15:05.000000 pulumi_ns1-3.3.0a1715925999/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 06:15:14.360836 pulumi_ns1-3.3.0a1715925999/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:31:46.977064 pulumi_ns1-3.3.0a1716395337/
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-22 16:31:46.977064 pulumi_ns1-3.3.0a1716395337/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:31:46.977064 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38901 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/account_whitelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87262 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16619 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:31:46.977064 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12682 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/data_feed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/dnsview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/get_dns_sec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/get_monitoring_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/get_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/get_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/get_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45756 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/monitoring_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11069 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/notify_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46058 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10590 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17050 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/pulsar_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    45469 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19239 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81714 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/tsigkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89234 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43790 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1/zone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:31:46.977064 pulumi_ns1-3.3.0a1716395337/pulumi_ns1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-22 16:31:46.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-22 16:31:46.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:31:46.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 16:31:46.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 16:31:46.000000 pulumi_ns1-3.3.0a1716395337/pulumi_ns1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-22 16:31:40.000000 pulumi_ns1-3.3.0a1716395337/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:31:46.977064 pulumi_ns1-3.3.0a1716395337/setup.cfg
```

### Comparing `pulumi_ns1-3.3.0a1715925999/PKG-INFO` & `pulumi_ns1-3.3.0a1716395337/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ns1
-Version: 3.3.0a1715925999
+Version: 3.3.0a1716395337
 Summary: A Pulumi package for creating and managing ns1 cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-ns1
 Keywords: pulumi,ns1
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_ns1-3.3.0a1715925999/README.md` & `pulumi_ns1-3.3.0a1716395337/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/__init__.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/_inputs.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/_utilities.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/account_whitelist.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/account_whitelist.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/api_key.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/application.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/application.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/config/__init__.pyi` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/config/vars.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/data_feed.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/data_feed.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/data_source.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/data_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/dataset.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/dataset.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/dnsview.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/dnsview.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/get_dns_sec.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/get_dns_sec.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/get_monitoring_regions.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/get_monitoring_regions.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/get_networks.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/get_networks.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/get_record.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/get_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/get_zone.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/get_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/monitoring_job.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/monitoring_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/notify_list.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/notify_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/outputs.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/provider.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/pulsar_job.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/pulsar_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/record.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
                Filters are documented below.
         :param pulumi.Input[str] link: The target record to link to. This means this record is a
                'linked' record, and it inherits all properties from its target.
         :param pulumi.Input[Sequence[pulumi.Input['RecordRegionArgs']]] regions: One or more "regions" for the record. These are really
                just groupings based on metadata, and are called "Answer Groups" in the NS1 UI,
                but remain `regions` here for legacy reasons. Regions are
                documented below. Please note the ordering requirement!
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: map of tags in the form of `"key" = "value"` where both key and value are strings
         :param pulumi.Input[int] ttl: The records' time to live (in seconds).
         :param pulumi.Input[bool] use_client_subnet: Whether to use EDNS client subnet data when
                available(in filter chain).
                * ` meta` - (Optional) meta is supported at the `record` level. Meta
                is documented below.
         """
         pulumi.set(__self__, "domain", domain)
@@ -212,14 +213,17 @@
     @short_answers.setter
     def short_answers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "short_answers", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        map of tags in the form of `"key" = "value"` where both key and value are strings
+        """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
@@ -277,14 +281,15 @@
                Filters are documented below.
         :param pulumi.Input[str] link: The target record to link to. This means this record is a
                'linked' record, and it inherits all properties from its target.
         :param pulumi.Input[Sequence[pulumi.Input['RecordRegionArgs']]] regions: One or more "regions" for the record. These are really
                just groupings based on metadata, and are called "Answer Groups" in the NS1 UI,
                but remain `regions` here for legacy reasons. Regions are
                documented below. Please note the ordering requirement!
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: map of tags in the form of `"key" = "value"` where both key and value are strings
         :param pulumi.Input[int] ttl: The records' time to live (in seconds).
         :param pulumi.Input[str] type: The records' RR type.
         :param pulumi.Input[bool] use_client_subnet: Whether to use EDNS client subnet data when
                available(in filter chain).
                * ` meta` - (Optional) meta is supported at the `record` level. Meta
                is documented below.
         :param pulumi.Input[str] zone: The zone the record belongs to. Cannot have leading or
@@ -427,14 +432,17 @@
     @short_answers.setter
     def short_answers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "short_answers", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        map of tags in the form of `"key" = "value"` where both key and value are strings
+        """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
@@ -649,14 +657,15 @@
                Filters are documented below.
         :param pulumi.Input[str] link: The target record to link to. This means this record is a
                'linked' record, and it inherits all properties from its target.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RecordRegionArgs']]]] regions: One or more "regions" for the record. These are really
                just groupings based on metadata, and are called "Answer Groups" in the NS1 UI,
                but remain `regions` here for legacy reasons. Regions are
                documented below. Please note the ordering requirement!
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: map of tags in the form of `"key" = "value"` where both key and value are strings
         :param pulumi.Input[int] ttl: The records' time to live (in seconds).
         :param pulumi.Input[str] type: The records' RR type.
         :param pulumi.Input[bool] use_client_subnet: Whether to use EDNS client subnet data when
                available(in filter chain).
                * ` meta` - (Optional) meta is supported at the `record` level. Meta
                is documented below.
         :param pulumi.Input[str] zone: The zone the record belongs to. Cannot have leading or
@@ -894,14 +903,15 @@
                Filters are documented below.
         :param pulumi.Input[str] link: The target record to link to. This means this record is a
                'linked' record, and it inherits all properties from its target.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RecordRegionArgs']]]] regions: One or more "regions" for the record. These are really
                just groupings based on metadata, and are called "Answer Groups" in the NS1 UI,
                but remain `regions` here for legacy reasons. Regions are
                documented below. Please note the ordering requirement!
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: map of tags in the form of `"key" = "value"` where both key and value are strings
         :param pulumi.Input[int] ttl: The records' time to live (in seconds).
         :param pulumi.Input[str] type: The records' RR type.
         :param pulumi.Input[bool] use_client_subnet: Whether to use EDNS client subnet data when
                available(in filter chain).
                * ` meta` - (Optional) meta is supported at the `record` level. Meta
                is documented below.
         :param pulumi.Input[str] zone: The zone the record belongs to. Cannot have leading or
@@ -996,14 +1006,17 @@
         pulumi.log.warn("""short_answers is deprecated: short_answers will be deprecated in a future release. It is suggested to migrate to a regular \"answers\" block.""")
 
         return pulumi.get(self, "short_answers")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
+        """
+        map of tags in the form of `"key" = "value"` where both key and value are strings
+        """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def ttl(self) -> pulumi.Output[int]:
         """
         The records' time to live (in seconds).
```

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/subnet.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/subnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/team.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/tsigkey.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/tsigkey.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/user.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1/zone.py` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1/zone.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         :param pulumi.Input[int] refresh: The SOA Refresh. Conflicts with `primary` and
                `additional_primaries` (default must be accepted).
         :param pulumi.Input[int] retry: The SOA Retry. Conflicts with `primary` and
                `additional_primaries` (default must be accepted).
         :param pulumi.Input[Sequence[pulumi.Input['ZoneSecondaryArgs']]] secondaries: List of secondary servers. This makes the zone a
                primary. Conflicts with `primary` and `additional_primaries`.
                Secondaries is documented below.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: map of tags in the form of `"key" = "value"` where both key and value are strings
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tsig: TSIG is documented below
         :param pulumi.Input[int] ttl: The SOA TTL.
         """
         pulumi.set(__self__, "zone", zone)
         if additional_ports is not None:
             pulumi.set(__self__, "additional_ports", additional_ports)
         if additional_primaries is not None:
@@ -281,14 +282,17 @@
     @secondaries.setter
     def secondaries(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ZoneSecondaryArgs']]]]):
         pulumi.set(self, "secondaries", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        map of tags in the form of `"key" = "value"` where both key and value are strings
+        """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
@@ -360,14 +364,15 @@
         :param pulumi.Input[int] refresh: The SOA Refresh. Conflicts with `primary` and
                `additional_primaries` (default must be accepted).
         :param pulumi.Input[int] retry: The SOA Retry. Conflicts with `primary` and
                `additional_primaries` (default must be accepted).
         :param pulumi.Input[Sequence[pulumi.Input['ZoneSecondaryArgs']]] secondaries: List of secondary servers. This makes the zone a
                primary. Conflicts with `primary` and `additional_primaries`.
                Secondaries is documented below.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: map of tags in the form of `"key" = "value"` where both key and value are strings
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tsig: TSIG is documented below
         :param pulumi.Input[int] ttl: The SOA TTL.
         :param pulumi.Input[str] zone: The domain name of the zone.
         """
         if additional_ports is not None:
             pulumi.set(__self__, "additional_ports", additional_ports)
         if additional_primaries is not None:
@@ -589,14 +594,17 @@
     @secondaries.setter
     def secondaries(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ZoneSecondaryArgs']]]]):
         pulumi.set(self, "secondaries", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        map of tags in the form of `"key" = "value"` where both key and value are strings
+        """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
@@ -694,14 +702,15 @@
         :param pulumi.Input[int] refresh: The SOA Refresh. Conflicts with `primary` and
                `additional_primaries` (default must be accepted).
         :param pulumi.Input[int] retry: The SOA Retry. Conflicts with `primary` and
                `additional_primaries` (default must be accepted).
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ZoneSecondaryArgs']]]] secondaries: List of secondary servers. This makes the zone a
                primary. Conflicts with `primary` and `additional_primaries`.
                Secondaries is documented below.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: map of tags in the form of `"key" = "value"` where both key and value are strings
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tsig: TSIG is documented below
         :param pulumi.Input[int] ttl: The SOA TTL.
         :param pulumi.Input[str] zone: The domain name of the zone.
         """
         ...
     @overload
     def __init__(__self__,
@@ -840,14 +849,15 @@
         :param pulumi.Input[int] refresh: The SOA Refresh. Conflicts with `primary` and
                `additional_primaries` (default must be accepted).
         :param pulumi.Input[int] retry: The SOA Retry. Conflicts with `primary` and
                `additional_primaries` (default must be accepted).
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ZoneSecondaryArgs']]]] secondaries: List of secondary servers. This makes the zone a
                primary. Conflicts with `primary` and `additional_primaries`.
                Secondaries is documented below.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: map of tags in the form of `"key" = "value"` where both key and value are strings
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tsig: TSIG is documented below
         :param pulumi.Input[int] ttl: The SOA TTL.
         :param pulumi.Input[str] zone: The domain name of the zone.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ZoneState.__new__(_ZoneState)
@@ -995,14 +1005,17 @@
         Secondaries is documented below.
         """
         return pulumi.get(self, "secondaries")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
+        """
+        map of tags in the form of `"key" = "value"` where both key and value are strings
+        """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def tsig(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         TSIG is documented below
```

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1.egg-info/PKG-INFO` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ns1
-Version: 3.3.0a1715925999
+Version: 3.3.0a1716395337
 Summary: A Pulumi package for creating and managing ns1 cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-ns1
 Keywords: pulumi,ns1
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_ns1-3.3.0a1715925999/pulumi_ns1.egg-info/SOURCES.txt` & `pulumi_ns1-3.3.0a1716395337/pulumi_ns1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1715925999/pyproject.toml` & `pulumi_ns1-3.3.0a1716395337/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_ns1"
   description = "A Pulumi package for creating and managing ns1 cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "ns1"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.3.0a1715925999"
+  version = "3.3.0a1716395337"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-ns1"
 
 [build-system]
```

