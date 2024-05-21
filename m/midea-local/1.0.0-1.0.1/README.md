# Comparing `tmp/midea_local-1.0.0.tar.gz` & `tmp/midea_local-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midea_local-1.0.0.tar", last modified: Wed May 15 14:30:31 2024, max compression
+gzip compressed data, was "midea_local-1.0.1.tar", last modified: Tue May 21 22:19:41 2024, max compression
```

## Comparing `midea_local-1.0.0.tar` & `midea_local-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:30:31.551944 midea_local-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-15 14:30:26.000000 midea_local-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-15 14:30:31.551944 midea_local-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-15 14:30:26.000000 midea_local-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:30:31.551944 midea_local-1.0.0/midea_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-15 14:30:31.000000 midea_local-1.0.0/midea_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 14:30:31.000000 midea_local-1.0.0/midea_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:30:31.000000 midea_local-1.0.0/midea_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-15 14:30:31.000000 midea_local-1.0.0/midea_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 14:30:31.000000 midea_local-1.0.0/midea_local.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:30:31.551944 midea_local-1.0.0/midealocal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:30:26.000000 midea_local-1.0.0/midealocal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25014 2024-05-15 14:30:26.000000 midea_local-1.0.0/midealocal/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-15 14:30:26.000000 midea_local-1.0.0/midealocal/crc8.py
--rw-r--r--   0 runner    (1001) docker     (127)    15204 2024-05-15 14:30:26.000000 midea_local-1.0.0/midealocal/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:30:31.551944 midea_local-1.0.0/midealocal/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-15 14:30:26.000000 midea_local-1.0.0/midealocal/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-05-15 14:30:26.000000 midea_local-1.0.0/midealocal/discover.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-15 14:30:26.000000 midea_local-1.0.0/midealocal/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-15 14:30:26.000000 midea_local-1.0.0/midealocal/packet_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-05-15 14:30:26.000000 midea_local-1.0.0/midealocal/security.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:30:31.551944 midea_local-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-15 14:30:26.000000 midea_local-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.741025 midea_local-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 22:19:37.000000 midea_local-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-21 22:19:41.741025 midea_local-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-21 22:19:37.000000 midea_local-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.741025 midea_local-1.0.1/midea_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-21 22:19:41.000000 midea_local-1.0.1/midea_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-21 22:19:41.000000 midea_local-1.0.1/midea_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 22:19:41.000000 midea_local-1.0.1/midea_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 22:19:41.000000 midea_local-1.0.1/midea_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 22:19:41.000000 midea_local-1.0.1/midea_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.729025 midea_local-1.0.1/midealocal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.729025 midea_local-1.0.1/midealocal/backports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/backports/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25014 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/crc8.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15204 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.729025 midea_local-1.0.1/midealocal/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.729025 midea_local-1.0.1/midealocal/devices/a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/a1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/a1/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.729025 midea_local-1.0.1/midealocal/devices/ac/
+-rw-r--r--   0 runner    (1001) docker     (127)    16377 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/ac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25127 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/ac/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.729025 midea_local-1.0.1/midealocal/devices/b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/b0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/b0/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.729025 midea_local-1.0.1/midealocal/devices/b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/b1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/b1/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.729025 midea_local-1.0.1/midealocal/devices/b3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/b3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/b3/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.733025 midea_local-1.0.1/midealocal/devices/b4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/b4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/b4/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.733025 midea_local-1.0.1/midealocal/devices/b6/
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/b6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/b6/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.733025 midea_local-1.0.1/midealocal/devices/bf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/bf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/bf/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.733025 midea_local-1.0.1/midealocal/devices/c2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/c2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/c2/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.733025 midea_local-1.0.1/midealocal/devices/c3/
+-rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/c3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/c3/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.733025 midea_local-1.0.1/midealocal/devices/ca/
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/ca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/ca/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.733025 midea_local-1.0.1/midealocal/devices/cc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/cc/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.733025 midea_local-1.0.1/midealocal/devices/cd/
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/cd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/cd/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.733025 midea_local-1.0.1/midealocal/devices/ce/
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/ce/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.733025 midea_local-1.0.1/midealocal/devices/cf/
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/cf/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.733025 midea_local-1.0.1/midealocal/devices/da/
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/da/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/da/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.737025 midea_local-1.0.1/midealocal/devices/db/
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/db/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.737025 midea_local-1.0.1/midealocal/devices/dc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/dc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/dc/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.737025 midea_local-1.0.1/midealocal/devices/e1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/e1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/e1/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.737025 midea_local-1.0.1/midealocal/devices/e2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/e2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/e2/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.737025 midea_local-1.0.1/midealocal/devices/e3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/e3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/e3/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.737025 midea_local-1.0.1/midealocal/devices/e6/
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/e6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/e6/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.737025 midea_local-1.0.1/midealocal/devices/e8/
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/e8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/e8/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.737025 midea_local-1.0.1/midealocal/devices/ea/
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/ea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/ea/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.737025 midea_local-1.0.1/midealocal/devices/ec/
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/ec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/ec/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.737025 midea_local-1.0.1/midealocal/devices/ed/
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/ed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/ed/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.737025 midea_local-1.0.1/midealocal/devices/fa/
+-rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/fa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/fa/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.737025 midea_local-1.0.1/midealocal/devices/fb/
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/fb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/fb/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.741025 midea_local-1.0.1/midealocal/devices/fc/
+-rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/fc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/fc/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.741025 midea_local-1.0.1/midealocal/devices/fd/
+-rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/fd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/fd/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.741025 midea_local-1.0.1/midealocal/devices/x13/
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/x13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/x13/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.741025 midea_local-1.0.1/midealocal/devices/x26/
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/x26/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/x26/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.741025 midea_local-1.0.1/midealocal/devices/x34/
+-rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/x34/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/x34/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:41.741025 midea_local-1.0.1/midealocal/devices/x40/
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/x40/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/devices/x40/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/discover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/packet_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-05-21 22:19:37.000000 midea_local-1.0.1/midealocal/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 22:19:41.741025 midea_local-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-21 22:19:37.000000 midea_local-1.0.1/setup.py
```

### Comparing `midea_local-1.0.0/LICENSE` & `midea_local-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.0/midealocal/cloud.py` & `midea_local-1.0.1/midealocal/cloud.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.0/midealocal/crc8.py` & `midea_local-1.0.1/midealocal/crc8.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.0/midealocal/device.py` & `midea_local-1.0.1/midealocal/device.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.0/midealocal/devices/__init__.py` & `midea_local-1.0.1/midealocal/devices/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     protocol: int,
     model: str,
     subtype: int,
     customize: str,
 ):
     try:
         if device_type < 0xA0:
-            device_path = f".{'x%02x' % device_type}.device"
+            device_path = f".{'x%02x' % device_type}"
         else:
-            device_path = f".{'%02x' % device_type}.device"
+            device_path = f".{'%02x' % device_type}"
         module = import_module(device_path, __package__)
         device = module.MideaAppliance(
             name=name,
             device_id=device_id,
             ip_address=ip_address,
             port=port,
             token=token,
```

### Comparing `midea_local-1.0.0/midealocal/discover.py` & `midea_local-1.0.1/midealocal/discover.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.0/midealocal/message.py` & `midea_local-1.0.1/midealocal/message.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.0/midealocal/packet_builder.py` & `midea_local-1.0.1/midealocal/packet_builder.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.0/midealocal/security.py` & `midea_local-1.0.1/midealocal/security.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.0/setup.py` & `midea_local-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 requires = ["aiohttp", "ifaddr", "pycryptodome"]
 
 setuptools.setup(
     name="midea-local",
-    version="1.0.0",
+    version="1.0.1",
     author="rokam",
     author_email="lucas@mindello.com.br",
     description="Control your Midea M-Smart appliances via local area network",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rokam/midea-local",
```

