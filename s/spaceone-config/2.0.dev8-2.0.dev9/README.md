# Comparing `tmp/spaceone-config-2.0.dev8.tar.gz` & `tmp/spaceone-config-2.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaceone-config-2.0.dev8.tar", last modified: Fri Jan  5 11:20:19 2024, max compression
+gzip compressed data, was "spaceone-config-2.0.dev9.tar", last modified: Sat Jan  6 13:21:21 2024, max compression
```

## Comparing `spaceone-config-2.0.dev8.tar` & `spaceone-config-2.0.dev9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:19.634609 spaceone-config-2.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-05 11:20:19.634609 spaceone-config-2.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-05 11:20:19.634609 spaceone-config-2.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:19.630609 spaceone-config-2.0.dev8/spaceone/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:19.630609 spaceone-config-2.0.dev8/spaceone/config/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:19.630609 spaceone-config-2.0.dev8/spaceone/config/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/conf/global_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:19.630609 spaceone-config-2.0.dev8/spaceone/config/connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:19.630609 spaceone-config-2.0.dev8/spaceone/config/error/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/error/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:19.630609 spaceone-config-2.0.dev8/spaceone/config/info/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/info/common_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/info/domain_config_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/info/user_config_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:19.630609 spaceone-config-2.0.dev8/spaceone/config/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:19.630609 spaceone-config-2.0.dev8/spaceone/config/interface/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/interface/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/interface/grpc/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/interface/grpc/user_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:19.634609 spaceone-config-2.0.dev8/spaceone/config/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:19.634609 spaceone-config-2.0.dev8/spaceone/config/manager/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/manager/domain_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/manager/user_config_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:19.634609 spaceone-config-2.0.dev8/spaceone/config/model/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/model/domain_config_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/model/user_config_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:19.634609 spaceone-config-2.0.dev8/spaceone/config/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/service/domain_config_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-01-05 11:20:08.000000 spaceone-config-2.0.dev8/spaceone/config/service/user_config_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 11:20:19.634609 spaceone-config-2.0.dev8/spaceone_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-05 11:20:19.000000 spaceone-config-2.0.dev8/spaceone_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-01-05 11:20:19.000000 spaceone-config-2.0.dev8/spaceone_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 11:20:19.000000 spaceone-config-2.0.dev8/spaceone_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 11:20:19.000000 spaceone-config-2.0.dev8/spaceone_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-05 11:20:19.000000 spaceone-config-2.0.dev8/spaceone_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-05 11:20:19.000000 spaceone-config-2.0.dev8/spaceone_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:21.855971 spaceone-config-2.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-06 13:21:21.855971 spaceone-config-2.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-06 13:21:21.855971 spaceone-config-2.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:21.851971 spaceone-config-2.0.dev9/spaceone/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:21.851971 spaceone-config-2.0.dev9/spaceone/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:21.851971 spaceone-config-2.0.dev9/spaceone/config/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/conf/global_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:21.851971 spaceone-config-2.0.dev9/spaceone/config/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:21.851971 spaceone-config-2.0.dev9/spaceone/config/error/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:21.851971 spaceone-config-2.0.dev9/spaceone/config/info/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/info/common_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/info/domain_config_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/info/user_config_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:21.851971 spaceone-config-2.0.dev9/spaceone/config/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:21.851971 spaceone-config-2.0.dev9/spaceone/config/interface/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/interface/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/interface/grpc/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/interface/grpc/user_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:21.851971 spaceone-config-2.0.dev9/spaceone/config/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:21.855971 spaceone-config-2.0.dev9/spaceone/config/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/manager/domain_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/manager/user_config_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:21.855971 spaceone-config-2.0.dev9/spaceone/config/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/model/domain_config_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/model/user_config_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:21.855971 spaceone-config-2.0.dev9/spaceone/config/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/service/domain_config_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-01-06 13:21:14.000000 spaceone-config-2.0.dev9/spaceone/config/service/user_config_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 13:21:21.855971 spaceone-config-2.0.dev9/spaceone_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-06 13:21:21.000000 spaceone-config-2.0.dev9/spaceone_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-01-06 13:21:21.000000 spaceone-config-2.0.dev9/spaceone_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 13:21:21.000000 spaceone-config-2.0.dev9/spaceone_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 13:21:21.000000 spaceone-config-2.0.dev9/spaceone_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-06 13:21:21.000000 spaceone-config-2.0.dev9/spaceone_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-06 13:21:21.000000 spaceone-config-2.0.dev9/spaceone_config.egg-info/top_level.txt
```

### Comparing `spaceone-config-2.0.dev8/setup.py` & `spaceone-config-2.0.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `spaceone-config-2.0.dev8/spaceone/config/conf/global_conf.py` & `spaceone-config-2.0.dev9/spaceone/config/conf/global_conf.py`

 * *Files identical despite different names*

### Comparing `spaceone-config-2.0.dev8/spaceone/config/info/domain_config_info.py` & `spaceone-config-2.0.dev9/spaceone/config/info/domain_config_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-config-2.0.dev8/spaceone/config/info/user_config_info.py` & `spaceone-config-2.0.dev9/spaceone/config/info/user_config_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-config-2.0.dev8/spaceone/config/interface/grpc/domain_config.py` & `spaceone-config-2.0.dev9/spaceone/config/interface/grpc/domain_config.py`

 * *Files identical despite different names*

### Comparing `spaceone-config-2.0.dev8/spaceone/config/interface/grpc/user_config.py` & `spaceone-config-2.0.dev9/spaceone/config/interface/grpc/user_config.py`

 * *Files identical despite different names*

### Comparing `spaceone-config-2.0.dev8/spaceone/config/manager/domain_config_manager.py` & `spaceone-config-2.0.dev9/spaceone/config/manager/domain_config_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-config-2.0.dev8/spaceone/config/manager/user_config_manager.py` & `spaceone-config-2.0.dev9/spaceone/config/manager/user_config_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-config-2.0.dev8/spaceone/config/model/domain_config_model.py` & `spaceone-config-2.0.dev9/spaceone/config/model/domain_config_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-config-2.0.dev8/spaceone/config/model/user_config_model.py` & `spaceone-config-2.0.dev9/spaceone/config/model/user_config_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-config-2.0.dev8/spaceone/config/service/domain_config_service.py` & `spaceone-config-2.0.dev9/spaceone/config/service/domain_config_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-config-2.0.dev8/spaceone/config/service/user_config_service.py` & `spaceone-config-2.0.dev9/spaceone/config/service/user_config_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-config-2.0.dev8/spaceone_config.egg-info/SOURCES.txt` & `spaceone-config-2.0.dev9/spaceone_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

