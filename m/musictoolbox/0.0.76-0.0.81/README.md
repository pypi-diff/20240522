# Comparing `tmp/musictoolbox-0.0.76.tar.gz` & `tmp/musictoolbox-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musictoolbox-0.0.76.tar", last modified: Tue Aug 22 01:52:16 2023, max compression
+gzip compressed data, was "musictoolbox-0.0.81.tar", last modified: Tue May 21 22:36:00 2024, max compression
```

## Comparing `musictoolbox-0.0.76.tar` & `musictoolbox-0.0.81.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-22 01:52:16.400000 musictoolbox-0.0.76/
--rw-rw-r--   0 user      (1000) user      (1000)       90 2023-08-22 00:00:59.000000 musictoolbox-0.0.76/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     3173 2023-08-22 01:52:16.400000 musictoolbox-0.0.76/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2496 2022-12-04 13:26:51.000000 musictoolbox-0.0.76/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     1662 2022-01-26 01:46:12.000000 musictoolbox-0.0.76/TODO
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-22 01:52:16.392000 musictoolbox-0.0.76/lib/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-22 01:52:16.394000 musictoolbox-0.0.76/lib/musictoolbox/
--rw-rw-r--   0 user      (1000) user      (1000)       73 2023-08-22 01:00:41.000000 musictoolbox-0.0.76/lib/musictoolbox/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     6562 2023-08-21 15:18:18.000000 musictoolbox-0.0.76/lib/musictoolbox/cache.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-22 01:52:16.396000 musictoolbox-0.0.76/lib/musictoolbox/cmd/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-01-26 01:40:28.000000 musictoolbox-0.0.76/lib/musictoolbox/cmd/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-21 23:40:00.000000 musictoolbox-0.0.76/lib/musictoolbox/cmd/cpm3u.py
--rw-rw-r--   0 user      (1000) user      (1000)      979 2023-08-22 00:22:32.000000 musictoolbox-0.0.76/lib/musictoolbox/cmd/detect.py
--rw-rw-r--   0 user      (1000) user      (1000)     6960 2023-08-22 00:39:38.000000 musictoolbox-0.0.76/lib/musictoolbox/cmd/doreplaygain.py
--rw-rw-r--   0 user      (1000) user      (1000)     1456 2023-08-21 23:43:44.000000 musictoolbox-0.0.76/lib/musictoolbox/cmd/fixplaylist.py
--rw-rw-r--   0 user      (1000) user      (1000)     6151 2023-08-21 23:43:36.000000 musictoolbox-0.0.76/lib/musictoolbox/cmd/genplaylist.py
--rw-rw-r--   0 user      (1000) user      (1000)     2507 2023-08-22 00:44:26.000000 musictoolbox-0.0.76/lib/musictoolbox/cmd/makealbumplaylist.py
--rw-rw-r--   0 user      (1000) user      (1000)      421 2023-08-22 00:44:11.000000 musictoolbox-0.0.76/lib/musictoolbox/cmd/removemusicbrainz.py
--rw-rw-r--   0 user      (1000) user      (1000)     6737 2023-08-22 00:39:45.000000 musictoolbox-0.0.76/lib/musictoolbox/cmd/scanalbumartists.py
--rw-rw-r--   0 user      (1000) user      (1000)     2777 2023-08-22 00:39:42.000000 musictoolbox-0.0.76/lib/musictoolbox/cmd/view.py
--rw-rw-r--   0 user      (1000) user      (1000)     2124 2023-08-21 15:03:05.000000 musictoolbox-0.0.76/lib/musictoolbox/files.py
--rw-rw-r--   0 user      (1000) user      (1000)      881 2022-01-26 01:40:28.000000 musictoolbox-0.0.76/lib/musictoolbox/logging.py
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-08-21 23:17:09.000000 musictoolbox-0.0.76/lib/musictoolbox/py.typed
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-22 01:52:16.397000 musictoolbox-0.0.76/lib/musictoolbox/sync/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-01-26 01:40:28.000000 musictoolbox-0.0.76/lib/musictoolbox/sync/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    10157 2023-08-22 00:13:43.000000 musictoolbox-0.0.76/lib/musictoolbox/sync/algo.py
--rw-rw-r--   0 user      (1000) user      (1000)    11079 2023-08-21 23:49:07.000000 musictoolbox-0.0.76/lib/musictoolbox/sync/cli.py
--rw-rw-r--   0 user      (1000) user      (1000)    12537 2022-12-04 13:18:42.000000 musictoolbox-0.0.76/lib/musictoolbox/sync/core.py
--rw-rw-r--   0 user      (1000) user      (1000)      299 2022-01-26 01:40:28.000000 musictoolbox-0.0.76/lib/musictoolbox/sync/interfaces.py
--rw-rw-r--   0 user      (1000) user      (1000)    12909 2022-12-04 12:36:14.000000 musictoolbox-0.0.76/lib/musictoolbox/sync/test_algo.py
--rw-rw-r--   0 user      (1000) user      (1000)    13977 2022-12-04 13:19:54.000000 musictoolbox-0.0.76/lib/musictoolbox/sync/test_core.py
--rw-rw-r--   0 user      (1000) user      (1000)     4574 2023-08-21 22:23:46.000000 musictoolbox-0.0.76/lib/musictoolbox/tagging.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-22 01:52:16.399000 musictoolbox-0.0.76/lib/musictoolbox/transcoding/
--rw-rw-r--   0 user      (1000) user      (1000)       98 2022-01-26 01:40:28.000000 musictoolbox-0.0.76/lib/musictoolbox/transcoding/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     4266 2023-08-22 01:22:29.000000 musictoolbox-0.0.76/lib/musictoolbox/transcoding/cli.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-22 01:52:16.400000 musictoolbox-0.0.76/lib/musictoolbox/transcoding/codecs/
--rw-rw-r--   0 user      (1000) user      (1000)       45 2023-08-21 23:04:16.000000 musictoolbox-0.0.76/lib/musictoolbox/transcoding/codecs/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1704 2022-01-26 01:40:28.000000 musictoolbox-0.0.76/lib/musictoolbox/transcoding/codecs/base.py
--rw-rw-r--   0 user      (1000) user      (1000)      443 2023-08-21 23:34:54.000000 musictoolbox-0.0.76/lib/musictoolbox/transcoding/codecs/basic.py
--rw-rw-r--   0 user      (1000) user      (1000)    10190 2023-08-22 00:10:35.000000 musictoolbox-0.0.76/lib/musictoolbox/transcoding/codecs/gstreamerffmpeg.py
--rw-rw-r--   0 user      (1000) user      (1000)     2695 2022-01-26 01:40:28.000000 musictoolbox-0.0.76/lib/musictoolbox/transcoding/codecs/test_codecs.py
--rw-rw-r--   0 user      (1000) user      (1000)     6202 2023-08-21 13:05:57.000000 musictoolbox-0.0.76/lib/musictoolbox/transcoding/config.py
--rw-rw-r--   0 user      (1000) user      (1000)     1166 2022-01-26 01:40:28.000000 musictoolbox-0.0.76/lib/musictoolbox/transcoding/interfaces.py
--rw-rw-r--   0 user      (1000) user      (1000)     5962 2023-08-22 01:40:30.000000 musictoolbox-0.0.76/lib/musictoolbox/transcoding/policies.py
--rw-rw-r--   0 user      (1000) user      (1000)     6912 2023-08-22 00:23:32.000000 musictoolbox-0.0.76/lib/musictoolbox/transcoding/registry.py
--rw-rw-r--   0 user      (1000) user      (1000)      810 2022-01-26 01:40:28.000000 musictoolbox-0.0.76/lib/musictoolbox/transcoding/settings.py
--rw-rw-r--   0 user      (1000) user      (1000)     3260 2022-01-26 01:40:28.000000 musictoolbox-0.0.76/lib/musictoolbox/transcoding/test_policies.py
--rw-rw-r--   0 user      (1000) user      (1000)     2079 2022-01-26 01:40:28.000000 musictoolbox-0.0.76/lib/musictoolbox/transcoding/test_registry.py
--rw-rw-r--   0 user      (1000) user      (1000)     4223 2023-08-22 00:23:10.000000 musictoolbox-0.0.76/lib/musictoolbox/transcoding/transcoder.py
--rw-rw-r--   0 user      (1000) user      (1000)      370 2022-01-26 01:40:28.000000 musictoolbox-0.0.76/lib/musictoolbox/util.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-22 01:52:16.395000 musictoolbox-0.0.76/lib/musictoolbox.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3173 2023-08-22 01:52:16.000000 musictoolbox-0.0.76/lib/musictoolbox.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1762 2023-08-22 01:52:16.000000 musictoolbox-0.0.76/lib/musictoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-08-22 01:52:16.000000 musictoolbox-0.0.76/lib/musictoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)     1315 2023-08-22 01:52:16.000000 musictoolbox-0.0.76/lib/musictoolbox.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       47 2023-08-22 01:52:16.000000 musictoolbox-0.0.76/lib/musictoolbox.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       13 2023-08-22 01:52:16.000000 musictoolbox-0.0.76/lib/musictoolbox.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)     1453 2023-08-22 01:00:34.000000 musictoolbox-0.0.76/musictoolbox.spec
--rw-rw-r--   0 user      (1000) user      (1000)      622 2023-08-22 00:40:13.000000 musictoolbox-0.0.76/mypy.ini
--rw-r--r--   0 user      (1000) user      (1000)       85 2023-08-21 23:23:51.000000 musictoolbox-0.0.76/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)     2282 2023-08-22 01:52:16.400000 musictoolbox-0.0.76/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      135 2023-08-22 01:51:14.000000 musictoolbox-0.0.76/tox.ini
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:36:00.103833 musictoolbox-0.0.81/
+-rw-rw-r--   0 user      (1000) user      (1000)       90 2023-08-22 00:00:59.000000 musictoolbox-0.0.81/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     3332 2024-05-21 22:36:00.103833 musictoolbox-0.0.81/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2496 2022-12-04 13:26:51.000000 musictoolbox-0.0.81/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     1662 2022-01-26 01:46:12.000000 musictoolbox-0.0.81/TODO
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:36:00.093833 musictoolbox-0.0.81/lib/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:36:00.096833 musictoolbox-0.0.81/lib/musictoolbox/
+-rw-rw-r--   0 user      (1000) user      (1000)       73 2024-05-21 22:22:52.000000 musictoolbox-0.0.81/lib/musictoolbox/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6562 2023-08-21 15:18:18.000000 musictoolbox-0.0.81/lib/musictoolbox/cache.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:36:00.098832 musictoolbox-0.0.81/lib/musictoolbox/cmd/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-21 23:40:00.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/cpm3u.py
+-rw-rw-r--   0 user      (1000) user      (1000)      979 2023-08-22 00:22:32.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/detect.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9272 2024-01-08 01:39:12.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/doreplaygain.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6395 2024-05-21 22:22:22.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/fixplaylist.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6151 2023-08-21 23:43:36.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/genplaylist.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2507 2023-08-22 00:44:26.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/makealbumplaylist.py
+-rw-rw-r--   0 user      (1000) user      (1000)      421 2023-08-22 00:44:11.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/removemusicbrainz.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6737 2023-08-22 00:39:45.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/scanalbumartists.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2777 2023-08-22 00:39:42.000000 musictoolbox-0.0.81/lib/musictoolbox/cmd/view.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2124 2023-08-21 15:03:05.000000 musictoolbox-0.0.81/lib/musictoolbox/files.py
+-rw-rw-r--   0 user      (1000) user      (1000)      881 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/logging.py
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-08-21 23:17:09.000000 musictoolbox-0.0.81/lib/musictoolbox/py.typed
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:36:00.099833 musictoolbox-0.0.81/lib/musictoolbox/sync/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/sync/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10257 2024-01-06 03:13:55.000000 musictoolbox-0.0.81/lib/musictoolbox/sync/algo.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11079 2023-08-21 23:49:07.000000 musictoolbox-0.0.81/lib/musictoolbox/sync/cli.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12537 2022-12-04 13:18:42.000000 musictoolbox-0.0.81/lib/musictoolbox/sync/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)      299 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/sync/interfaces.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12909 2022-12-04 12:36:14.000000 musictoolbox-0.0.81/lib/musictoolbox/sync/test_algo.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13977 2022-12-04 13:19:54.000000 musictoolbox-0.0.81/lib/musictoolbox/sync/test_core.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4574 2023-08-21 22:23:46.000000 musictoolbox-0.0.81/lib/musictoolbox/tagging.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:36:00.101832 musictoolbox-0.0.81/lib/musictoolbox/transcoding/
+-rw-rw-r--   0 user      (1000) user      (1000)       98 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4266 2023-08-22 01:22:29.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/cli.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:36:00.102833 musictoolbox-0.0.81/lib/musictoolbox/transcoding/codecs/
+-rw-rw-r--   0 user      (1000) user      (1000)       45 2023-08-21 23:04:16.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/codecs/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1704 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/codecs/base.py
+-rw-rw-r--   0 user      (1000) user      (1000)      443 2023-08-21 23:34:54.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/codecs/basic.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10190 2023-08-22 00:10:35.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/codecs/gstreamerffmpeg.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2695 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/codecs/test_codecs.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6202 2023-08-21 13:05:57.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1166 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/interfaces.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5962 2023-08-22 01:40:30.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/policies.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6912 2023-08-22 00:23:32.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/registry.py
+-rw-rw-r--   0 user      (1000) user      (1000)      810 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/settings.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3260 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/test_policies.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2079 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/test_registry.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4223 2023-08-22 00:23:10.000000 musictoolbox-0.0.81/lib/musictoolbox/transcoding/transcoder.py
+-rw-rw-r--   0 user      (1000) user      (1000)      370 2022-01-26 01:40:28.000000 musictoolbox-0.0.81/lib/musictoolbox/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-21 22:36:00.102833 musictoolbox-0.0.81/lib/musictoolbox.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3332 2024-05-21 22:36:00.000000 musictoolbox-0.0.81/lib/musictoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1762 2024-05-21 22:36:00.000000 musictoolbox-0.0.81/lib/musictoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-05-21 22:36:00.000000 musictoolbox-0.0.81/lib/musictoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)     1315 2024-05-21 22:36:00.000000 musictoolbox-0.0.81/lib/musictoolbox.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)       54 2024-05-21 22:36:00.000000 musictoolbox-0.0.81/lib/musictoolbox.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       13 2024-05-21 22:36:00.000000 musictoolbox-0.0.81/lib/musictoolbox.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)     1453 2024-05-21 22:22:36.000000 musictoolbox-0.0.81/musictoolbox.spec
+-rw-rw-r--   0 user      (1000) user      (1000)      622 2023-08-22 00:40:13.000000 musictoolbox-0.0.81/mypy.ini
+-rw-r--r--   0 user      (1000) user      (1000)       85 2023-08-21 23:23:51.000000 musictoolbox-0.0.81/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)     2290 2024-05-21 22:36:00.103833 musictoolbox-0.0.81/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      135 2023-08-22 01:51:14.000000 musictoolbox-0.0.81/tox.ini
```

### Comparing `musictoolbox-0.0.76/PKG-INFO` & `musictoolbox-0.0.81/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: musictoolbox
-Version: 0.0.76
+Version: 0.0.81
 Summary: Utilities to help you groom your music collection
 Home-page: https://github.com/Rudd-O/musictoolbox
 Author: Manuel Amador (Rudd-O)
 Author-email: rudd-o@rudd-o.com
 License: GPLv2
 Keywords: mp3 ogg mkv transcoding aac mp4 video flv flac
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+Requires-Dist: mutagen
+Requires-Dist: networkx
+Requires-Dist: pyxdg
+Requires-Dist: psutil
+Requires-Dist: PyYAML
+Requires-Dist: packaging
+Requires-Dist: rgain3
 
 # Music toolbox
 
 This is a small toolbox of utilities written in Python 2 that help users groom their music collection.
 
 ## What's in the box
```

### Comparing `musictoolbox-0.0.76/README.md` & `musictoolbox-0.0.81/README.md`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/TODO` & `musictoolbox-0.0.81/TODO`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/cache.py` & `musictoolbox-0.0.81/lib/musictoolbox/cache.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/cmd/cpm3u.py` & `musictoolbox-0.0.81/lib/musictoolbox/cmd/cpm3u.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/cmd/detect.py` & `musictoolbox-0.0.81/lib/musictoolbox/cmd/detect.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/cmd/genplaylist.py` & `musictoolbox-0.0.81/lib/musictoolbox/cmd/genplaylist.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/cmd/makealbumplaylist.py` & `musictoolbox-0.0.81/lib/musictoolbox/cmd/makealbumplaylist.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/cmd/scanalbumartists.py` & `musictoolbox-0.0.81/lib/musictoolbox/cmd/scanalbumartists.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/cmd/view.py` & `musictoolbox-0.0.81/lib/musictoolbox/cmd/view.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/files.py` & `musictoolbox-0.0.81/lib/musictoolbox/files.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/logging.py` & `musictoolbox-0.0.81/lib/musictoolbox/logging.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/sync/algo.py` & `musictoolbox-0.0.81/lib/musictoolbox/sync/algo.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,36 +105,40 @@
     if x >= 2:
         return 1
     elif x <= -2:
         return -1
     return 0
 
 
+def default_timestamp_comparator(s: int | float, t: int | float) -> int:
+    return 1 if s > t else (-1 if s < t else 0)
+
+
 class SourceAlwaysNewer(object):
     def compare(self, __arg1: AbsolutePath, __arg2: AbsolutePath) -> int:
         return 1
 
 
 class ModTimestampComparer(object):
     def __init__(self) -> None:
         self.mptypes = get_mptypes()
 
     def compare(self, path1: AbsolutePath, path2: AbsolutePath) -> int:
-        fstypes = set(get_fstype(p, self.mptypes)[0] for p in [path1, path2])
-        if "vfat" in fstypes:
-            comparator = vfatcompare
-        else:
-            comparator = lambda x, y: (1 if x > y else (-1 if x < y else 0))
-
         try:
             st2 = path2.stat()
         except FileNotFoundError:
             # The target file does not exist, so we always return the
             # source file as newer.
             return 1
+
+        fstypes = set(get_fstype(p, self.mptypes)[0] for p in [path1, path2])
+        if "vfat" in fstypes:
+            comparator = vfatcompare
+        else:
+            comparator = default_timestamp_comparator
         st1 = path1.stat()
 
         try:
             t1 = st1.st_mtime_ns / 1000000000
             t2 = st2.st_mtime_ns / 1000000000
         except AttributeError:
             t1 = st1.st_mtime
```

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/sync/cli.py` & `musictoolbox-0.0.81/lib/musictoolbox/sync/cli.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/sync/core.py` & `musictoolbox-0.0.81/lib/musictoolbox/sync/core.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/sync/test_algo.py` & `musictoolbox-0.0.81/lib/musictoolbox/sync/test_algo.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/sync/test_core.py` & `musictoolbox-0.0.81/lib/musictoolbox/sync/test_core.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/tagging.py` & `musictoolbox-0.0.81/lib/musictoolbox/tagging.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/transcoding/cli.py` & `musictoolbox-0.0.81/lib/musictoolbox/transcoding/cli.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/transcoding/codecs/base.py` & `musictoolbox-0.0.81/lib/musictoolbox/transcoding/codecs/base.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/transcoding/codecs/gstreamerffmpeg.py` & `musictoolbox-0.0.81/lib/musictoolbox/transcoding/codecs/gstreamerffmpeg.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/transcoding/codecs/test_codecs.py` & `musictoolbox-0.0.81/lib/musictoolbox/transcoding/codecs/test_codecs.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/transcoding/config.py` & `musictoolbox-0.0.81/lib/musictoolbox/transcoding/config.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/transcoding/interfaces.py` & `musictoolbox-0.0.81/lib/musictoolbox/transcoding/interfaces.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/transcoding/policies.py` & `musictoolbox-0.0.81/lib/musictoolbox/transcoding/policies.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/transcoding/registry.py` & `musictoolbox-0.0.81/lib/musictoolbox/transcoding/registry.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/transcoding/settings.py` & `musictoolbox-0.0.81/lib/musictoolbox/transcoding/settings.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/transcoding/test_policies.py` & `musictoolbox-0.0.81/lib/musictoolbox/transcoding/test_policies.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/transcoding/test_registry.py` & `musictoolbox-0.0.81/lib/musictoolbox/transcoding/test_registry.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox/transcoding/transcoder.py` & `musictoolbox-0.0.81/lib/musictoolbox/transcoding/transcoder.py`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox.egg-info/PKG-INFO` & `musictoolbox-0.0.81/lib/musictoolbox.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: musictoolbox
-Version: 0.0.76
+Version: 0.0.81
 Summary: Utilities to help you groom your music collection
 Home-page: https://github.com/Rudd-O/musictoolbox
 Author: Manuel Amador (Rudd-O)
 Author-email: rudd-o@rudd-o.com
 License: GPLv2
 Keywords: mp3 ogg mkv transcoding aac mp4 video flv flac
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+Requires-Dist: mutagen
+Requires-Dist: networkx
+Requires-Dist: pyxdg
+Requires-Dist: psutil
+Requires-Dist: PyYAML
+Requires-Dist: packaging
+Requires-Dist: rgain3
 
 # Music toolbox
 
 This is a small toolbox of utilities written in Python 2 that help users groom their music collection.
 
 ## What's in the box
```

### Comparing `musictoolbox-0.0.76/lib/musictoolbox.egg-info/SOURCES.txt` & `musictoolbox-0.0.81/lib/musictoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/lib/musictoolbox.egg-info/entry_points.txt` & `musictoolbox-0.0.81/lib/musictoolbox.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/musictoolbox.spec` & `musictoolbox-0.0.81/musictoolbox.spec`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 %define debug_package %{nil}
 
 %define _name musictoolbox
 
 %define mybuildnumber %{?build_number}%{?!build_number:1}
 
 Name:           python-%{_name}
-Version:        0.0.76
+Version:        0.0.81
 Release:        %{mybuildnumber}%{?dist}
 Summary:        Utilities to help you groom your music collection
 
 License:        GPLv2
 URL:            https://github.com/Rudd-O/%{_name}
 Source:         %{url}/archive/v%{version}/%{_name}-%{version}.tar.gz
```

### Comparing `musictoolbox-0.0.76/mypy.ini` & `musictoolbox-0.0.81/mypy.ini`

 * *Files identical despite different names*

### Comparing `musictoolbox-0.0.76/setup.cfg` & `musictoolbox-0.0.81/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 install_requires = 
 	mutagen
 	networkx
 	pyxdg
 	psutil
 	PyYAML
 	packaging
+	rgain3
 
 [options.packages.find]
 where = lib
 
 [options.package_data]
 musictoolbox = py.typed
```

