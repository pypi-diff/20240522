# Comparing `tmp/pulp_certguard-client-3.52.0.tar.gz` & `tmp/pulp_certguard-client-3.53.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp_certguard-client-3.52.0.tar", last modified: Tue Apr 23 16:18:00 2024, max compression
+gzip compressed data, was "pulp_certguard-client-3.53.0.tar", last modified: Tue Apr 30 18:17:35 2024, max compression
```

## Comparing `pulp_certguard-client-3.52.0.tar` & `pulp_certguard-client-3.53.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:18:00.030754 pulp_certguard-client-3.52.0/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-23 16:18:00.030754 pulp_certguard-client-3.52.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:18:00.026754 pulp_certguard-client-3.52.0/pulp_certguard_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulp_certguard_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulp_certguard_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulp_certguard_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulp_certguard_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulp_certguard_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:18:00.026754 pulp_certguard-client-3.52.0/pulpcore/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:18:00.026754 pulp_certguard-client-3.52.0/pulpcore/client/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:18:00.026754 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:18:00.026754 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/api/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43046 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/api/contentguards_rhsm_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    42854 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/api/contentguards_x509_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26305 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13977 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:18:00.030754 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/paginatedcertguard_rhsm_cert_guard_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/paginatedcertguard_x509_cert_guard_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/patchedcertguard_rhsm_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/patchedcertguard_x509_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 16:18:00.030754 pulp_certguard-client-3.52.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:18:00.030754 pulp_certguard-client-3.52.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/test/test_certguard_rhsm_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/test/test_certguard_rhsm_cert_guard_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/test/test_certguard_x509_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/test/test_certguard_x509_cert_guard_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/test/test_contentguards_rhsm_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/test/test_contentguards_x509_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/test/test_paginatedcertguard_rhsm_cert_guard_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/test/test_paginatedcertguard_x509_cert_guard_response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/test/test_patchedcertguard_rhsm_cert_guard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-23 16:17:59.000000 pulp_certguard-client-3.52.0/test/test_patchedcertguard_x509_cert_guard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:17:35.168875 pulp_certguard-client-3.53.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-30 18:17:35.168875 pulp_certguard-client-3.53.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:17:35.164875 pulp_certguard-client-3.53.0/pulp_certguard_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-30 18:17:35.000000 pulp_certguard-client-3.53.0/pulp_certguard_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-30 18:17:35.000000 pulp_certguard-client-3.53.0/pulp_certguard_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:17:35.000000 pulp_certguard-client-3.53.0/pulp_certguard_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 18:17:35.000000 pulp_certguard-client-3.53.0/pulp_certguard_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 18:17:35.000000 pulp_certguard-client-3.53.0/pulp_certguard_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:17:35.164875 pulp_certguard-client-3.53.0/pulpcore/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:17:35.164875 pulp_certguard-client-3.53.0/pulpcore/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:17:35.168875 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:17:35.168875 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43046 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/api/contentguards_rhsm_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42854 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/api/contentguards_x509_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26305 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13977 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:17:35.168875 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/paginatedcertguard_rhsm_cert_guard_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/paginatedcertguard_x509_cert_guard_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/patchedcertguard_rhsm_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/patchedcertguard_x509_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 18:17:35.168875 pulp_certguard-client-3.53.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:17:35.168875 pulp_certguard-client-3.53.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/test/test_certguard_rhsm_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/test/test_certguard_rhsm_cert_guard_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/test/test_certguard_x509_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/test/test_certguard_x509_cert_guard_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/test/test_contentguards_rhsm_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/test/test_contentguards_x509_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/test/test_paginatedcertguard_rhsm_cert_guard_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/test/test_paginatedcertguard_x509_cert_guard_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/test/test_patchedcertguard_rhsm_cert_guard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-30 18:17:34.000000 pulp_certguard-client-3.53.0/test/test_patchedcertguard_x509_cert_guard.py
```

### Comparing `pulp_certguard-client-3.52.0/README.md` & `pulp_certguard-client-3.53.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pulp_certguard-client
 Fetch, Upload, Organize, and Distribute Software Packages
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v3
-- Package version: 3.52.0
+- Package version: 3.53.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pulpproject.org](https://pulpproject.org)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `pulp_certguard-client-3.52.0/pulp_certguard_client.egg-info/SOURCES.txt` & `pulp_certguard-client-3.53.0/pulp_certguard_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/__init__.py` & `pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: pulp-list@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "3.52.0"
+__version__ = "3.53.0"
 
 # import apis into sdk package
 from pulpcore.client.pulp_certguard.api.contentguards_rhsm_api import ContentguardsRhsmApi
 from pulpcore.client.pulp_certguard.api.contentguards_x509_api import ContentguardsX509Api
 
 # import ApiClient
 from pulpcore.client.pulp_certguard.api_client import ApiClient
```

### Comparing `pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/api/contentguards_rhsm_api.py` & `pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/api/contentguards_rhsm_api.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/api/contentguards_x509_api.py` & `pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/api/contentguards_x509_api.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/api_client.py` & `pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/3.52.0/python'
+        self.user_agent = 'OpenAPI-Generator/3.53.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/configuration.py` & `pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v3\n"\
-               "SDK Package Version: 3.52.0".\
+               "SDK Package Version: 3.53.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/exceptions.py` & `pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/exceptions.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/__init__.py` & `pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard.py` & `pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard_response.py` & `pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/certguard_rhsm_cert_guard_response.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard.py` & `pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard_response.py` & `pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/certguard_x509_cert_guard_response.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/paginatedcertguard_rhsm_cert_guard_response_list.py` & `pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/paginatedcertguard_rhsm_cert_guard_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/paginatedcertguard_x509_cert_guard_response_list.py` & `pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/paginatedcertguard_x509_cert_guard_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/patchedcertguard_rhsm_cert_guard.py` & `pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/patchedcertguard_rhsm_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/models/patchedcertguard_x509_cert_guard.py` & `pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/models/patchedcertguard_x509_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/pulpcore/client/pulp_certguard/rest.py` & `pulp_certguard-client-3.53.0/pulpcore/client/pulp_certguard/rest.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/setup.py` & `pulp_certguard-client-3.53.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "pulp_certguard-client"
-VERSION = "3.52.0"
+VERSION = "3.53.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `pulp_certguard-client-3.52.0/test/test_certguard_rhsm_cert_guard.py` & `pulp_certguard-client-3.53.0/test/test_certguard_rhsm_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/test/test_certguard_rhsm_cert_guard_response.py` & `pulp_certguard-client-3.53.0/test/test_certguard_rhsm_cert_guard_response.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/test/test_certguard_x509_cert_guard.py` & `pulp_certguard-client-3.53.0/test/test_certguard_x509_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/test/test_certguard_x509_cert_guard_response.py` & `pulp_certguard-client-3.53.0/test/test_certguard_x509_cert_guard_response.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/test/test_contentguards_rhsm_api.py` & `pulp_certguard-client-3.53.0/test/test_contentguards_rhsm_api.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/test/test_contentguards_x509_api.py` & `pulp_certguard-client-3.53.0/test/test_contentguards_x509_api.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/test/test_paginatedcertguard_rhsm_cert_guard_response_list.py` & `pulp_certguard-client-3.53.0/test/test_paginatedcertguard_rhsm_cert_guard_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/test/test_paginatedcertguard_x509_cert_guard_response_list.py` & `pulp_certguard-client-3.53.0/test/test_paginatedcertguard_x509_cert_guard_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/test/test_patchedcertguard_rhsm_cert_guard.py` & `pulp_certguard-client-3.53.0/test/test_patchedcertguard_rhsm_cert_guard.py`

 * *Files identical despite different names*

### Comparing `pulp_certguard-client-3.52.0/test/test_patchedcertguard_x509_cert_guard.py` & `pulp_certguard-client-3.53.0/test/test_patchedcertguard_x509_cert_guard.py`

 * *Files identical despite different names*

