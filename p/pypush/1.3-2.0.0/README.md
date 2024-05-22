# Comparing `tmp/pypush-1.3.tar.gz` & `tmp/pypush-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypush-1.3.tar", last modified: Sat Jan 26 04:37:26 2013, max compression
+gzip compressed data, was "pypush-2.0.0.tar", last modified: Wed May 22 12:37:21 2024, max compression
```

## Comparing `pypush-1.3.tar` & `pypush-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,45 @@
-drwxr-xr-x   0 vivek      (501) staff       (20)        0 2013-01-26 04:37:26.000000 pypush-1.3/
--rw-r--r--   0 vivek      (501) staff       (20)      693 2013-01-26 04:37:26.000000 pypush-1.3/PKG-INFO
-drwxr-xr-x   0 vivek      (501) staff       (20)        0 2013-01-26 04:37:26.000000 pypush-1.3/pypush.egg-info/
--rw-r--r--   0 vivek      (501) staff       (20)        1 2013-01-26 04:37:26.000000 pypush-1.3/pypush.egg-info/dependency_links.txt
--rw-r--r--   0 vivek      (501) staff       (20)       40 2013-01-26 04:37:26.000000 pypush-1.3/pypush.egg-info/entry_points.txt
--rw-r--r--   0 vivek      (501) staff       (20)      693 2013-01-26 04:37:26.000000 pypush-1.3/pypush.egg-info/PKG-INFO
--rw-r--r--   0 vivek      (501) staff       (20)        8 2013-01-26 04:37:26.000000 pypush-1.3/pypush.egg-info/requires.txt
--rw-r--r--   0 vivek      (501) staff       (20)      200 2013-01-26 04:37:26.000000 pypush-1.3/pypush.egg-info/SOURCES.txt
--rw-r--r--   0 vivek      (501) staff       (20)        7 2013-01-26 04:37:26.000000 pypush-1.3/pypush.egg-info/top_level.txt
--rwxr-xr-x   0 vivek      (501) staff       (20)     9355 2013-01-26 04:36:10.000000 pypush-1.3/pypush.py
--rw-r--r--   0 vivek      (501) staff       (20)       59 2013-01-26 04:37:26.000000 pypush-1.3/setup.cfg
--rw-r--r--   0 vivek      (501) staff       (20)      764 2013-01-26 04:36:17.000000 pypush-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:37:21.008312 pypush-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:37:21.000312 pypush-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:37:21.004312 pypush-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-22 12:37:06.000000 pypush-2.0.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-22 12:37:06.000000 pypush-2.0.0/.github/workflows/upload.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-22 12:37:06.000000 pypush-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    29385 2024-05-22 12:37:06.000000 pypush-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-22 12:37:21.008312 pypush-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-22 12:37:06.000000 pypush-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-22 12:37:06.000000 pypush-2.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:37:21.004312 pypush-2.0.0/pypush/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 12:37:20.000000 pypush-2.0.0/pypush/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:37:21.008312 pypush-2.0.0/pypush/apns/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-22 12:37:06.000000 pypush-2.0.0/pypush/apns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-22 12:37:06.000000 pypush-2.0.0/pypush/apns/_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-22 12:37:06.000000 pypush-2.0.0/pypush/apns/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-05-22 12:37:06.000000 pypush-2.0.0/pypush/apns/albert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-22 12:37:06.000000 pypush-2.0.0/pypush/apns/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-05-22 12:37:06.000000 pypush-2.0.0/pypush/apns/lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18135 2024-05-22 12:37:06.000000 pypush-2.0.0/pypush/apns/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-22 12:37:06.000000 pypush-2.0.0/pypush/apns/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:37:21.008312 pypush-2.0.0/pypush/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-22 12:37:06.000000 pypush-2.0.0/pypush/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-22 12:37:06.000000 pypush-2.0.0/pypush/cli/_frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-22 12:37:06.000000 pypush-2.0.0/pypush/cli/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:37:21.008312 pypush-2.0.0/pypush/cloudkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:37:06.000000 pypush-2.0.0/pypush/cloudkit/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:37:21.008312 pypush-2.0.0/pypush/grandslam/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:37:06.000000 pypush-2.0.0/pypush/grandslam/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:37:21.008312 pypush-2.0.0/pypush/ids/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:37:06.000000 pypush-2.0.0/pypush/ids/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:37:21.008312 pypush-2.0.0/pypush/imessage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:37:06.000000 pypush-2.0.0/pypush/imessage/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:37:21.008312 pypush-2.0.0/pypush.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-22 12:37:20.000000 pypush-2.0.0/pypush.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-22 12:37:21.000000 pypush-2.0.0/pypush.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:37:20.000000 pypush-2.0.0/pypush.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 12:37:20.000000 pypush-2.0.0/pypush.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-22 12:37:20.000000 pypush-2.0.0/pypush.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 12:37:20.000000 pypush-2.0.0/pypush.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:37:21.008312 pypush-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:37:21.008312 pypush-2.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:37:21.008312 pypush-2.0.0/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-05-22 12:37:06.000000 pypush-2.0.0/tests/assets/dev.jjtech.pypush.tests.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-22 12:37:06.000000 pypush-2.0.0/tests/test_apns.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

