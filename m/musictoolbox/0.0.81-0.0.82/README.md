# Comparing `tmp/musictoolbox-0.0.81.tar.gz` & `tmp/musictoolbox-0.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musictoolbox-0.0.81.tar", last modified: Tue May 21 22:36:00 2024, max compression
+gzip compressed data, was "musictoolbox-0.0.82.tar", last modified: Tue May 21 22:38:23 2024, max compression
```

## Comparing `musictoolbox-0.0.81.tar` & `musictoolbox-0.0.82.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:36:00.103833 musictoolbox-0.0.81/
--rw-rw-r--   0 user      (1000) user      (1000)       90 2023-08-22 00:00:59.000000 musictoolbox-0.0.81/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     3332 2024-05-21 22:36:00.103833 musictoolbox-0.0.81/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2496 2022-12-04 13:26:51.000000 musictoolbox-0.0.81/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     1662 2022-01-26 01:46:12.000000 musictoolbox-0.0.81/TODO
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:36:00.093833 musictoolbox-0.0.81/lib/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:36:00.096833 musictoolbox-0.0.81/lib/musictoolbox/
--rw-rw-r--   0 user      (1000) user      (1000)       73 2024-05-21 22:22:52.000000 musictoolbox-0.0.81/lib/musictoolbox/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     6562 2023-08-21 15:18:18.000000 musictoolbox-0.0.81/lib/musictoolbox/cache.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:36:00.098832 musictoolbox-0.0.81/lib/musictoolbox/cmd/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-21 23:40:00.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/cpm3u.py
--rw-rw-r--   0 user      (1000) user      (1000)      979 2023-08-22 00:22:32.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/detect.py
--rw-rw-r--   0 user      (1000) user      (1000)     9272 2024-01-08 01:39:12.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/doreplaygain.py
--rw-rw-r--   0 user      (1000) user      (1000)     6395 2024-05-21 22:22:22.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/fixplaylist.py
--rw-rw-r--   0 user      (1000) user      (1000)     6151 2023-08-21 23:43:36.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/genplaylist.py
--rw-rw-r--   0 user      (1000) user      (1000)     2507 2023-08-22 00:44:26.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/makealbumplaylist.py
--rw-rw-r--   0 user      (1000) user      (1000)      421 2023-08-22 00:44:11.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/removemusicbrainz.py
--rw-rw-r--   0 user      (1000) user      (1000)     6737 2023-08-22 00:39:45.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/scanalbumartists.py
--rw-rw-r--   0 user      (1000) user      (1000)     2777 2023-08-22 00:39:42.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/view.py
--rw-rw-r--   0 user      (1000) user      (1000)     2124 2023-08-21 15:03:05.000000 musictoolbox-0.0.81/lib/musictoolbox/files.py
--rw-rw-r--   0 user      (1000) user      (1000)      881 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/logging.py
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-08-21 23:17:09.000000 musictoolbox-0.0.81/lib/musictoolbox/py.typed
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:36:00.099833 musictoolbox-0.0.81/lib/musictoolbox/sync/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/sync/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    10257 2024-01-06 03:13:55.000000 musictoolbox-0.0.81/lib/musictoolbox/sync/algo.py
--rw-rw-r--   0 user      (1000) user      (1000)    11079 2023-08-21 23:49:07.000000 musictoolbox-0.0.81/lib/musictoolbox/sync/cli.py
--rw-rw-r--   0 user      (1000) user      (1000)    12537 2022-12-04 13:18:42.000000 musictoolbox-0.0.81/lib/musictoolbox/sync/core.py
--rw-rw-r--   0 user      (1000) user      (1000)      299 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/sync/interfaces.py
--rw-rw-r--   0 user      (1000) user      (1000)    12909 2022-12-04 12:36:14.000000 musictoolbox-0.0.81/lib/musictoolbox/sync/test_algo.py
--rw-rw-r--   0 user      (1000) user      (1000)    13977 2022-12-04 13:19:54.000000 musictoolbox-0.0.81/lib/musictoolbox/sync/test_core.py
--rw-rw-r--   0 user      (1000) user      (1000)     4574 2023-08-21 22:23:46.000000 musictoolbox-0.0.81/lib/musictoolbox/tagging.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:36:00.101832 musictoolbox-0.0.81/lib/musictoolbox/transcoding/
--rw-rw-r--   0 user      (1000) user      (1000)       98 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     4266 2023-08-22 01:22:29.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/cli.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:36:00.102833 musictoolbox-0.0.81/lib/musictoolbox/transcoding/codecs/
--rw-rw-r--   0 user      (1000) user      (1000)       45 2023-08-21 23:04:16.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/codecs/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1704 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/codecs/base.py
--rw-rw-r--   0 user      (1000) user      (1000)      443 2023-08-21 23:34:54.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/codecs/basic.py
--rw-rw-r--   0 user      (1000) user      (1000)    10190 2023-08-22 00:10:35.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/codecs/gstreamerffmpeg.py
--rw-rw-r--   0 user      (1000) user      (1000)     2695 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/codecs/test_codecs.py
--rw-rw-r--   0 user      (1000) user      (1000)     6202 2023-08-21 13:05:57.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/config.py
--rw-rw-r--   0 user      (1000) user      (1000)     1166 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/interfaces.py
--rw-rw-r--   0 user      (1000) user      (1000)     5962 2023-08-22 01:40:30.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/policies.py
--rw-rw-r--   0 user      (1000) user      (1000)     6912 2023-08-22 00:23:32.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/registry.py
--rw-rw-r--   0 user      (1000) user      (1000)      810 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/settings.py
--rw-rw-r--   0 user      (1000) user      (1000)     3260 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/test_policies.py
--rw-rw-r--   0 user      (1000) user      (1000)     2079 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/test_registry.py
--rw-rw-r--   0 user      (1000) user      (1000)     4223 2023-08-22 00:23:10.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/transcoder.py
--rw-rw-r--   0 user      (1000) user      (1000)      370 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/util.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:36:00.102833 musictoolbox-0.0.81/lib/musictoolbox.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3332 2024-05-21 22:36:00.000000 musictoolbox-0.0.81/lib/musictoolbox.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1762 2024-05-21 22:36:00.000000 musictoolbox-0.0.81/lib/musictoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2024-05-21 22:36:00.000000 musictoolbox-0.0.81/lib/musictoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)     1315 2024-05-21 22:36:00.000000 musictoolbox-0.0.81/lib/musictoolbox.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       54 2024-05-21 22:36:00.000000 musictoolbox-0.0.81/lib/musictoolbox.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       13 2024-05-21 22:36:00.000000 musictoolbox-0.0.81/lib/musictoolbox.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)     1453 2024-05-21 22:22:36.000000 musictoolbox-0.0.81/musictoolbox.spec
--rw-rw-r--   0 user      (1000) user      (1000)      622 2023-08-22 00:40:13.000000 musictoolbox-0.0.81/mypy.ini
--rw-r--r--   0 user      (1000) user      (1000)       85 2023-08-21 23:23:51.000000 musictoolbox-0.0.81/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)     2290 2024-05-21 22:36:00.103833 musictoolbox-0.0.81/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      135 2023-08-22 01:51:14.000000 musictoolbox-0.0.81/tox.ini
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:38:23.148821 musictoolbox-0.0.82/
+-rw-rw-r--   0 user      (1000) user      (1000)       90 2023-08-22 00:00:59.000000 musictoolbox-0.0.82/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     3332 2024-05-21 22:38:23.148821 musictoolbox-0.0.82/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2496 2022-12-04 13:26:51.000000 musictoolbox-0.0.82/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     1662 2022-01-26 01:46:12.000000 musictoolbox-0.0.82/TODO
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:38:23.137821 musictoolbox-0.0.82/lib/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:38:23.141821 musictoolbox-0.0.82/lib/musictoolbox/
+-rw-rw-r--   0 user      (1000) user      (1000)       73 2024-05-21 22:37:39.000000 musictoolbox-0.0.82/lib/musictoolbox/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6562 2023-08-21 15:18:18.000000 musictoolbox-0.0.82/lib/musictoolbox/cache.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:38:23.144821 musictoolbox-0.0.82/lib/musictoolbox/cmd/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2022-01-26 01:40:28.000000 musictoolbox-0.0.82/lib/musictoolbox/cmd/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-21 23:40:00.000000 musictoolbox-0.0.82/lib/musictoolbox/cmd/cpm3u.py
+-rw-rw-r--   0 user      (1000) user      (1000)      979 2023-08-22 00:22:32.000000 musictoolbox-0.0.82/lib/musictoolbox/cmd/detect.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9272 2024-01-08 01:39:12.000000 musictoolbox-0.0.82/lib/musictoolbox/cmd/doreplaygain.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6468 2024-05-21 22:37:06.000000 musictoolbox-0.0.82/lib/musictoolbox/cmd/fixplaylist.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6151 2023-08-21 23:43:36.000000 musictoolbox-0.0.82/lib/musictoolbox/cmd/genplaylist.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2507 2023-08-22 00:44:26.000000 musictoolbox-0.0.82/lib/musictoolbox/cmd/makealbumplaylist.py
+-rw-rw-r--   0 user      (1000) user      (1000)      421 2023-08-22 00:44:11.000000 musictoolbox-0.0.82/lib/musictoolbox/cmd/removemusicbrainz.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6737 2023-08-22 00:39:45.000000 musictoolbox-0.0.82/lib/musictoolbox/cmd/scanalbumartists.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2777 2023-08-22 00:39:42.000000 musictoolbox-0.0.82/lib/musictoolbox/cmd/view.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2124 2023-08-21 15:03:05.000000 musictoolbox-0.0.82/lib/musictoolbox/files.py
+-rw-rw-r--   0 user      (1000) user      (1000)      881 2022-01-26 01:40:28.000000 musictoolbox-0.0.82/lib/musictoolbox/logging.py
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-08-21 23:17:09.000000 musictoolbox-0.0.82/lib/musictoolbox/py.typed
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:38:23.145821 musictoolbox-0.0.82/lib/musictoolbox/sync/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2022-01-26 01:40:28.000000 musictoolbox-0.0.82/lib/musictoolbox/sync/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10257 2024-01-06 03:13:55.000000 musictoolbox-0.0.82/lib/musictoolbox/sync/algo.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11079 2023-08-21 23:49:07.000000 musictoolbox-0.0.82/lib/musictoolbox/sync/cli.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12537 2022-12-04 13:18:42.000000 musictoolbox-0.0.82/lib/musictoolbox/sync/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)      299 2022-01-26 01:40:28.000000 musictoolbox-0.0.82/lib/musictoolbox/sync/interfaces.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12909 2022-12-04 12:36:14.000000 musictoolbox-0.0.82/lib/musictoolbox/sync/test_algo.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13977 2022-12-04 13:19:54.000000 musictoolbox-0.0.82/lib/musictoolbox/sync/test_core.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4574 2023-08-21 22:23:46.000000 musictoolbox-0.0.82/lib/musictoolbox/tagging.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:38:23.147821 musictoolbox-0.0.82/lib/musictoolbox/transcoding/
+-rw-rw-r--   0 user      (1000) user      (1000)       98 2022-01-26 01:40:28.000000 musictoolbox-0.0.82/lib/musictoolbox/transcoding/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4266 2023-08-22 01:22:29.000000 musictoolbox-0.0.82/lib/musictoolbox/transcoding/cli.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:38:23.148821 musictoolbox-0.0.82/lib/musictoolbox/transcoding/codecs/
+-rw-rw-r--   0 user      (1000) user      (1000)       45 2023-08-21 23:04:16.000000 musictoolbox-0.0.82/lib/musictoolbox/transcoding/codecs/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1704 2022-01-26 01:40:28.000000 musictoolbox-0.0.82/lib/musictoolbox/transcoding/codecs/base.py
+-rw-rw-r--   0 user      (1000) user      (1000)      443 2023-08-21 23:34:54.000000 musictoolbox-0.0.82/lib/musictoolbox/transcoding/codecs/basic.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10190 2023-08-22 00:10:35.000000 musictoolbox-0.0.82/lib/musictoolbox/transcoding/codecs/gstreamerffmpeg.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2695 2022-01-26 01:40:28.000000 musictoolbox-0.0.82/lib/musictoolbox/transcoding/codecs/test_codecs.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6202 2023-08-21 13:05:57.000000 musictoolbox-0.0.82/lib/musictoolbox/transcoding/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1166 2022-01-26 01:40:28.000000 musictoolbox-0.0.82/lib/musictoolbox/transcoding/interfaces.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5962 2023-08-22 01:40:30.000000 musictoolbox-0.0.82/lib/musictoolbox/transcoding/policies.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6912 2023-08-22 00:23:32.000000 musictoolbox-0.0.82/lib/musictoolbox/transcoding/registry.py
+-rw-rw-r--   0 user      (1000) user      (1000)      810 2022-01-26 01:40:28.000000 musictoolbox-0.0.82/lib/musictoolbox/transcoding/settings.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3260 2022-01-26 01:40:28.000000 musictoolbox-0.0.82/lib/musictoolbox/transcoding/test_policies.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2079 2022-01-26 01:40:28.000000 musictoolbox-0.0.82/lib/musictoolbox/transcoding/test_registry.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4223 2023-08-22 00:23:10.000000 musictoolbox-0.0.82/lib/musictoolbox/transcoding/transcoder.py
+-rw-rw-r--   0 user      (1000) user      (1000)      370 2022-01-26 01:40:28.000000 musictoolbox-0.0.82/lib/musictoolbox/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:38:23.148821 musictoolbox-0.0.82/lib/musictoolbox.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3332 2024-05-21 22:38:23.000000 musictoolbox-0.0.82/lib/musictoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1762 2024-05-21 22:38:23.000000 musictoolbox-0.0.82/lib/musictoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-05-21 22:38:23.000000 musictoolbox-0.0.82/lib/musictoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)     1315 2024-05-21 22:38:23.000000 musictoolbox-0.0.82/lib/musictoolbox.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)       54 2024-05-21 22:38:23.000000 musictoolbox-0.0.82/lib/musictoolbox.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       13 2024-05-21 22:38:23.000000 musictoolbox-0.0.82/lib/musictoolbox.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)     1453 2024-05-21 22:37:43.000000 musictoolbox-0.0.82/musictoolbox.spec
+-rw-rw-r--   0 user      (1000) user      (1000)      622 2023-08-22 00:40:13.000000 musictoolbox-0.0.82/mypy.ini
+-rw-r--r--   0 user      (1000) user      (1000)       85 2023-08-21 23:23:51.000000 musictoolbox-0.0.82/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)     2290 2024-05-21 22:38:23.149821 musictoolbox-0.0.82/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      135 2023-08-22 01:51:14.000000 musictoolbox-0.0.82/tox.ini
```

### Comparing `musictoolbox-0.0.81/PKG-INFO` & `musictoolbox-0.0.82/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musictoolbox
-Version: 0.0.81
+Version: 0.0.82
 Summary: Utilities to help you groom your music collection
 Home-page: https://github.com/Rudd-O/musictoolbox
 Author: Manuel Amador (Rudd-O)
 Author-email: rudd-o@rudd-o.com
 License: GPLv2
 Keywords: mp3 ogg mkv transcoding aac mp4 video flv flac
 Classifier: Development Status :: 4 - Beta
```

### Comparing `musictoolbox-0.0.81/README.md` & `musictoolbox-0.0.82/README.md`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/TODO` & `musictoolbox-0.0.82/TODO`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/cache.py` & `musictoolbox-0.0.82/lib/musictoolbox/cache.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/cmd/cpm3u.py` & `musictoolbox-0.0.82/lib/musictoolbox/cmd/cpm3u.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/cmd/detect.py` & `musictoolbox-0.0.82/lib/musictoolbox/cmd/detect.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/cmd/doreplaygain.py` & `musictoolbox-0.0.82/lib/musictoolbox/cmd/doreplaygain.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/cmd/fixplaylist.py` & `musictoolbox-0.0.82/lib/musictoolbox/cmd/fixplaylist.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ]:
     filename_to_fullpath: dict[str, list[str]] = collections.defaultdict(list)
     filename_basedir_to_fullpath: dict[str, list[str]] = collections.defaultdict(list)
 
     for base, dirs, files in os.walk(tree_path):
         for fn in files:
             name_without_ext, ext = os.path.splitext(fn)
-            if ext in [".mood"]:
+            if ext in [".mood", ".nfo"]:
                 continue
             fullpath = os.path.join(base, fn)
             filename_to_fullpath[name_without_ext].append(fullpath)
             filename_basedir = os.path.join(os.path.basename(base), name_without_ext)
             filename_basedir_to_fullpath[filename_basedir].append(fullpath)
 
     filename_tokenized_to_fullpath = {
@@ -170,15 +170,17 @@
 
                     try:
                         choice_int = int(newline)
                         newline = choices[choice_int - 1]
                     except Exception:
                         pass
 
-                    newline = os.path.relpath(newline, d)
+                    if os.path.abspath(newline) == newline:
+                        newline = os.path.relpath(newline, d)
+
                     print(f"Replacement selected: {newline}")
                     replacements[fullpath] = newline
                     newlines.append(newline)
 
                     didchange = True
             else:
                 newlines.append(line)
```

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/cmd/genplaylist.py` & `musictoolbox-0.0.82/lib/musictoolbox/cmd/genplaylist.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/cmd/makealbumplaylist.py` & `musictoolbox-0.0.82/lib/musictoolbox/cmd/makealbumplaylist.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/cmd/scanalbumartists.py` & `musictoolbox-0.0.82/lib/musictoolbox/cmd/scanalbumartists.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/cmd/view.py` & `musictoolbox-0.0.82/lib/musictoolbox/cmd/view.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/files.py` & `musictoolbox-0.0.82/lib/musictoolbox/files.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/logging.py` & `musictoolbox-0.0.82/lib/musictoolbox/logging.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/sync/algo.py` & `musictoolbox-0.0.82/lib/musictoolbox/sync/algo.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/sync/cli.py` & `musictoolbox-0.0.82/lib/musictoolbox/sync/cli.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/sync/core.py` & `musictoolbox-0.0.82/lib/musictoolbox/sync/core.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/sync/test_algo.py` & `musictoolbox-0.0.82/lib/musictoolbox/sync/test_algo.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/sync/test_core.py` & `musictoolbox-0.0.82/lib/musictoolbox/sync/test_core.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/tagging.py` & `musictoolbox-0.0.82/lib/musictoolbox/tagging.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/transcoding/cli.py` & `musictoolbox-0.0.82/lib/musictoolbox/transcoding/cli.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/transcoding/codecs/base.py` & `musictoolbox-0.0.82/lib/musictoolbox/transcoding/codecs/base.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/transcoding/codecs/gstreamerffmpeg.py` & `musictoolbox-0.0.82/lib/musictoolbox/transcoding/codecs/gstreamerffmpeg.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/transcoding/codecs/test_codecs.py` & `musictoolbox-0.0.82/lib/musictoolbox/transcoding/codecs/test_codecs.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/transcoding/config.py` & `musictoolbox-0.0.82/lib/musictoolbox/transcoding/config.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/transcoding/interfaces.py` & `musictoolbox-0.0.82/lib/musictoolbox/transcoding/interfaces.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/transcoding/policies.py` & `musictoolbox-0.0.82/lib/musictoolbox/transcoding/policies.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/transcoding/registry.py` & `musictoolbox-0.0.82/lib/musictoolbox/transcoding/registry.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/transcoding/settings.py` & `musictoolbox-0.0.82/lib/musictoolbox/transcoding/settings.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/transcoding/test_policies.py` & `musictoolbox-0.0.82/lib/musictoolbox/transcoding/test_policies.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/transcoding/test_registry.py` & `musictoolbox-0.0.82/lib/musictoolbox/transcoding/test_registry.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox/transcoding/transcoder.py` & `musictoolbox-0.0.82/lib/musictoolbox/transcoding/transcoder.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox.egg-info/PKG-INFO` & `musictoolbox-0.0.82/lib/musictoolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musictoolbox
-Version: 0.0.81
+Version: 0.0.82
 Summary: Utilities to help you groom your music collection
 Home-page: https://github.com/Rudd-O/musictoolbox
 Author: Manuel Amador (Rudd-O)
 Author-email: rudd-o@rudd-o.com
 License: GPLv2
 Keywords: mp3 ogg mkv transcoding aac mp4 video flv flac
 Classifier: Development Status :: 4 - Beta
```

### Comparing `musictoolbox-0.0.81/lib/musictoolbox.egg-info/SOURCES.txt` & `musictoolbox-0.0.82/lib/musictoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/lib/musictoolbox.egg-info/entry_points.txt` & `musictoolbox-0.0.82/lib/musictoolbox.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/musictoolbox.spec` & `musictoolbox-0.0.82/musictoolbox.spec`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 %define debug_package %{nil}
 
 %define _name musictoolbox
 
 %define mybuildnumber %{?build_number}%{?!build_number:1}
 
 Name:           python-%{_name}
-Version:        0.0.81
+Version:        0.0.82
 Release:        %{mybuildnumber}%{?dist}
 Summary:        Utilities to help you groom your music collection
 
 License:        GPLv2
 URL:            https://github.com/Rudd-O/%{_name}
 Source:         %{url}/archive/v%{version}/%{_name}-%{version}.tar.gz
```

### Comparing `musictoolbox-0.0.81/mypy.ini` & `musictoolbox-0.0.82/mypy.ini`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.81/setup.cfg` & `musictoolbox-0.0.82/setup.cfg`

 * *Files identical despite different names*

