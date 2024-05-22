# Comparing `tmp/osc_tiny-0.9.0.tar.gz` & `tmp/osc_tiny-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osc_tiny-0.9.0.tar", last modified: Mon Apr 22 15:26:59 2024, max compression
+gzip compressed data, was "osc_tiny-0.9.1.tar", last modified: Wed May 22 08:58:11 2024, max compression
```

## Comparing `osc_tiny-0.9.0.tar` & `osc_tiny-0.9.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:26:59.603191 osc_tiny-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-22 15:26:59.603191 osc_tiny-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:26:59.603191 osc_tiny-0.9.0/osc_tiny.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-22 15:26:59.000000 osc_tiny-0.9.0/osc_tiny.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-22 15:26:59.000000 osc_tiny-0.9.0/osc_tiny.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 15:26:59.000000 osc_tiny-0.9.0/osc_tiny.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-22 15:26:59.000000 osc_tiny-0.9.0/osc_tiny.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 15:26:59.000000 osc_tiny-0.9.0/osc_tiny.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:26:59.595191 osc_tiny-0.9.0/osctiny/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:26:59.599191 osc_tiny-0.9.0/osctiny/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/extensions/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/extensions/bs_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/extensions/buildresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/extensions/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/extensions/distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/extensions/issues.py
--rw-r--r--   0 runner    (1001) docker     (127)    20126 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/extensions/origin.py
--rw-r--r--   0 runner    (1001) docker     (127)    20807 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/extensions/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/extensions/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/extensions/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    15223 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/extensions/staging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/extensions/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:26:59.599191 osc_tiny-0.9.0/osctiny/models/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/models/staging.py
--rw-r--r--   0 runner    (1001) docker     (127)    18578 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/osc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:26:59.599191 osc_tiny-0.9.0/osctiny/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:26:59.603191 osc_tiny-0.9.0/osctiny/tests/osc/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/tests/osc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/tests/osc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/tests/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/tests/test_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/tests/test_datadir.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/tests/test_distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/tests/test_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/tests/test_origin.py
--rw-r--r--   0 runner    (1001) docker     (127)    21742 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/tests/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)    20523 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)    14531 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    14170 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/tests/test_staging.py
--rw-r--r--   0 runner    (1001) docker     (127)    21382 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:26:59.603191 osc_tiny-0.9.0/osctiny/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/utils/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/utils/backports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/utils/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9092 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/utils/changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/utils/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/utils/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/osctiny/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/requirements_devel.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/requirements_pre38.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 15:26:59.603191 osc_tiny-0.9.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1722 2024-04-22 15:26:55.000000 osc_tiny-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:58:11.398337 osc_tiny-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-22 08:58:11.398337 osc_tiny-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:58:11.398337 osc_tiny-0.9.1/osc_tiny.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-22 08:58:11.000000 osc_tiny-0.9.1/osc_tiny.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-22 08:58:11.000000 osc_tiny-0.9.1/osc_tiny.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 08:58:11.000000 osc_tiny-0.9.1/osc_tiny.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-22 08:58:11.000000 osc_tiny-0.9.1/osc_tiny.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 08:58:11.000000 osc_tiny-0.9.1/osc_tiny.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:58:11.390337 osc_tiny-0.9.1/osctiny/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:58:11.394337 osc_tiny-0.9.1/osctiny/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/extensions/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/extensions/bs_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/extensions/buildresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/extensions/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/extensions/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/extensions/issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20126 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/extensions/origin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20807 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/extensions/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/extensions/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/extensions/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15136 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/extensions/staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/extensions/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:58:11.394337 osc_tiny-0.9.1/osctiny/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/models/staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18578 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/osc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:58:11.394337 osc_tiny-0.9.1/osctiny/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:58:11.398337 osc_tiny-0.9.1/osctiny/tests/osc/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/tests/osc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/tests/osc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/tests/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/tests/test_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/tests/test_datadir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/tests/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/tests/test_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/tests/test_origin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21742 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/tests/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20523 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14531 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14170 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10184 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/tests/test_staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21382 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:58:11.398337 osc_tiny-0.9.1/osctiny/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/utils/backports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/utils/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9092 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/utils/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/utils/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/utils/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/osctiny/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/requirements_devel.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/requirements_pre38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 08:58:11.398337 osc_tiny-0.9.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1722 2024-05-22 08:58:07.000000 osc_tiny-0.9.1/setup.py
```

### Comparing `osc_tiny-0.9.0/LICENSE` & `osc_tiny-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/PKG-INFO` & `osc_tiny-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osc-tiny
-Version: 0.9.0
+Version: 0.9.1
 Summary: Client API for openSUSE BuildService
 Home-page: https://github.com/SUSE/osc-tiny
 Author: Andreas Hasenkopf
 Author-email: ahasenkopf@suse.com
 Maintainer: SUSE Maintenance Automation Engineering team
 Maintainer-email: maintenance-automation-team@suse.de
 License: MIT
```

### Comparing `osc_tiny-0.9.0/README.md` & `osc_tiny-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osc_tiny.egg-info/PKG-INFO` & `osc_tiny-0.9.1/osc_tiny.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osc-tiny
-Version: 0.9.0
+Version: 0.9.1
 Summary: Client API for openSUSE BuildService
 Home-page: https://github.com/SUSE/osc-tiny
 Author: Andreas Hasenkopf
 Author-email: ahasenkopf@suse.com
 Maintainer: SUSE Maintenance Automation Engineering team
 Maintainer-email: maintenance-automation-team@suse.de
 License: MIT
```

### Comparing `osc_tiny-0.9.0/osc_tiny.egg-info/SOURCES.txt` & `osc_tiny-0.9.1/osc_tiny.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/extensions/attributes.py` & `osc_tiny-0.9.1/osctiny/extensions/attributes.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/extensions/bs_requests.py` & `osc_tiny-0.9.1/osctiny/extensions/bs_requests.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/extensions/buildresults.py` & `osc_tiny-0.9.1/osctiny/extensions/buildresults.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/extensions/comments.py` & `osc_tiny-0.9.1/osctiny/extensions/comments.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/extensions/distributions.py` & `osc_tiny-0.9.1/osctiny/extensions/distributions.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/extensions/issues.py` & `osc_tiny-0.9.1/osctiny/extensions/issues.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/extensions/origin.py` & `osc_tiny-0.9.1/osctiny/extensions/origin.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/extensions/packages.py` & `osc_tiny-0.9.1/osctiny/extensions/packages.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/extensions/projects.py` & `osc_tiny-0.9.1/osctiny/extensions/projects.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/extensions/search.py` & `osc_tiny-0.9.1/osctiny/extensions/search.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/extensions/staging.py` & `osc_tiny-0.9.1/osctiny/extensions/staging.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,12 +373,11 @@
 
         response = self.osc.request(
             method="POST",
             url=urljoin(self.osc.url, url_path),
             data=report.asxml()
         )
 
-        parsed = self.osc.get_objectified_xml(response)
-        if response.status_code == 200 and parsed.get("code") == "ok":
+        if response.status_code == 200:
             return True
 
         return False
```

### Comparing `osc_tiny-0.9.0/osctiny/extensions/users.py` & `osc_tiny-0.9.1/osctiny/extensions/users.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/models/staging.py` & `osc_tiny-0.9.1/osctiny/models/staging.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/osc.py` & `osc_tiny-0.9.1/osctiny/osc.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/tests/base.py` & `osc_tiny-0.9.1/osctiny/tests/base.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/tests/test_attributes.py` & `osc_tiny-0.9.1/osctiny/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/tests/test_basic.py` & `osc_tiny-0.9.1/osctiny/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/tests/test_build.py` & `osc_tiny-0.9.1/osctiny/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/tests/test_comments.py` & `osc_tiny-0.9.1/osctiny/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/tests/test_datadir.py` & `osc_tiny-0.9.1/osctiny/tests/test_datadir.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/tests/test_distributions.py` & `osc_tiny-0.9.1/osctiny/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/tests/test_issues.py` & `osc_tiny-0.9.1/osctiny/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/tests/test_origin.py` & `osc_tiny-0.9.1/osctiny/tests/test_origin.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/tests/test_packages.py` & `osc_tiny-0.9.1/osctiny/tests/test_packages.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/tests/test_projects.py` & `osc_tiny-0.9.1/osctiny/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/tests/test_requests.py` & `osc_tiny-0.9.1/osctiny/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/tests/test_search.py` & `osc_tiny-0.9.1/osctiny/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/tests/test_staging.py` & `osc_tiny-0.9.1/osctiny/tests/test_staging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 
+from lxml import etree
 import responses
 
 from osctiny.models.staging import ExcludedRequest, CheckState, CheckReport
 
 from .base import OscTest
 
 
@@ -230,15 +231,15 @@
             elem = self.osc.get_objectified_xml(request.body)
             self.assertEqual(report.name, elem.get("name"))
             self.assertEqual("false", elem.get("required"))
             self.assertEqual(elem.state.text, report.state.value)
             self.assertEqual(elem.short_description.text, report.short_description)
             self.assertEqual(elem.url.text, report.url)
 
-            return 200, {}, "<status code=\"ok\"/>"
+            return 200, {}, etree.tostring(report.asxml()).decode()
 
         responses.add_callback(
             method="POST",
             url=re.compile("http://api.example.com/status_reports/(published|built)"),
             callback=callback
         )
```

### Comparing `osc_tiny-0.9.0/osctiny/tests/test_utils.py` & `osc_tiny-0.9.1/osctiny/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/utils/auth.py` & `osc_tiny-0.9.1/osctiny/utils/auth.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/utils/base.py` & `osc_tiny-0.9.1/osctiny/utils/base.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/utils/changelog.py` & `osc_tiny-0.9.1/osctiny/utils/changelog.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/utils/conf.py` & `osc_tiny-0.9.1/osctiny/utils/conf.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/utils/errors.py` & `osc_tiny-0.9.1/osctiny/utils/errors.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/utils/mapping.py` & `osc_tiny-0.9.1/osctiny/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/osctiny/utils/xml.py` & `osc_tiny-0.9.1/osctiny/utils/xml.py`

 * *Files identical despite different names*

### Comparing `osc_tiny-0.9.0/setup.py` & `osc_tiny-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 
 setup(
     name='osc-tiny',
-    version='0.9.0',
+    version='0.9.1',
     description='Client API for openSUSE BuildService',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Andreas Hasenkopf',
     author_email='ahasenkopf@suse.com',
     maintainer='SUSE Maintenance Automation Engineering team',
     maintainer_email='maintenance-automation-team@suse.de',
```

