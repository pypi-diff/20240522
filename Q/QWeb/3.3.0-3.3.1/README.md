# Comparing `tmp/QWeb-3.3.0.tar.gz` & `tmp/QWeb-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QWeb-3.3.0.tar", last modified: Wed May 15 06:40:07 2024, max compression
+gzip compressed data, was "QWeb-3.3.1.tar", last modified: Wed May 22 14:43:29 2024, max compression
```

## Comparing `QWeb-3.3.0.tar` & `QWeb-3.3.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 06:40:07.543135 QWeb-3.3.0/
--rw-rw-rw-   0        0        0    11558 2021-09-04 19:02:10.000000 QWeb-3.3.0/LICENSE
--rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-3.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0    11340 2024-05-15 06:40:07.543635 QWeb-3.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 06:40:07.553430 QWeb-3.3.0/QWeb/
--rw-rw-rw-   0        0        0    16938 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/__init__.py
--rw-rw-rw-   0        0        0     2259 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/__main__.py
--rw-rw-rw-   0        0        0      519 2024-05-15 06:40:07.553947 QWeb-3.3.0/QWeb/_version.py
--rw-rw-rw-   0        0        0     1408 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/custom_config.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:40:06.801869 QWeb-3.3.0/QWeb/internal/
--rw-rw-rw-   0        0        0       64 2021-09-04 19:02:10.000000 QWeb-3.3.0/QWeb/internal/__init__.py
--rw-rw-rw-   0        0        0    21711 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/internal/actions.py
--rw-rw-rw-   0        0        0     3671 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/ajax.py
--rw-rw-rw-   0        0        0     1709 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/alert.py
--rw-rw-rw-   0        0        0     3691 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/blocks.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:40:06.993141 QWeb-3.3.0/QWeb/internal/browser/
--rw-rw-rw-   0        0        0     4879 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/browser/__init__.py
--rw-rw-rw-   0        0        0     1548 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/browser/android.py
--rw-rw-rw-   0        0        0     3426 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/browser/bs_desktop.py
--rw-rw-rw-   0        0        0     2166 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/browser/bs_mobile.py
--rw-rw-rw-   0        0        0     6072 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/browser/chrome.py
--rw-rw-rw-   0        0        0     4308 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/internal/browser/edge.py
--rw-rw-rw-   0        0        0     5093 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/internal/browser/firefox.py
--rw-rw-rw-   0        0        0     1884 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/browser/safari.py
--rw-rw-rw-   0        0        0     6141 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/checkbox.py
--rw-rw-rw-   0        0        0     4314 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/config.py
--rw-rw-rw-   0        0        0     4442 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/config_defaults.py
--rw-rw-rw-   0        0        0     1294 2022-11-22 10:56:24.000000 QWeb-3.3.0/QWeb/internal/cookies.py
--rw-rw-rw-   0        0        0     9703 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/decorators.py
--rw-rw-rw-   0        0        0     5625 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/download.py
--rw-rw-rw-   0        0        0     3096 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/dragdrop.py
--rw-rw-rw-   0        0        0     7881 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/dropdown.py
--rw-rw-rw-   0        0        0    29827 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/element.py
--rw-rw-rw-   0        0        0     3105 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/exceptions.py
--rw-rw-rw-   0        0        0     3550 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/file.py
--rw-rw-rw-   0        0        0    11694 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/frame.py
--rw-rw-rw-   0        0        0     1960 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/frame_checker.py
--rw-rw-rw-   0        0        0    21185 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/internal/icon.py
--rw-rw-rw-   0        0        0    10845 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/internal/input_.py
--rw-rw-rw-   0        0        0     7292 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/input_handler.py
--rw-rw-rw-   0        0        0    21147 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/javascript.py
--rw-rw-rw-   0        0        0     9115 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/lists.py
--rw-rw-rw-   0        0        0     3180 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/meas.py
--rw-rw-rw-   0        0        0      833 2022-06-16 12:12:06.000000 QWeb-3.3.0/QWeb/internal/platform.py
--rw-rw-rw-   0        0        0    13285 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/screenshot.py
--rw-rw-rw-   0        0        0     7236 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/search_strategy.py
--rw-rw-rw-   0        0        0     8613 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/secrets.py
--rw-rw-rw-   0        0        0    16553 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/table.py
--rw-rw-rw-   0        0        0    18247 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/text.py
--rw-rw-rw-   0        0        0     1373 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/user.py
--rw-rw-rw-   0        0        0    13801 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/internal/util.py
--rw-rw-rw-   0        0        0     4233 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/window.py
--rw-rw-rw-   0        0        0     3303 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/xhr.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:40:07.540136 QWeb-3.3.0/QWeb/keywords/
--rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-3.3.0/QWeb/keywords/__init__.py
--rw-rw-rw-   0        0        0     4473 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/ajax.py
--rw-rw-rw-   0        0        0     4920 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/alert.py
--rw-rw-rw-   0        0        0     5920 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/blocks.py
--rw-rw-rw-   0        0        0    24523 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/keywords/browser.py
--rw-rw-rw-   0        0        0    12198 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/checkbox.py
--rw-rw-rw-   0        0        0    37935 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/config.py
--rw-rw-rw-   0        0        0     3055 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/cookies.py
--rw-rw-rw-   0        0        0     2508 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/debug.py
--rw-rw-rw-   0        0        0     4028 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/download.py
--rw-rw-rw-   0        0        0     6151 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/dragdrop.py
--rw-rw-rw-   0        0        0    14990 2024-05-15 06:11:38.000000 QWeb-3.3.0/QWeb/keywords/dropdown.py
--rw-rw-rw-   0        0        0    27779 2024-05-15 06:11:38.000000 QWeb-3.3.0/QWeb/keywords/element.py
--rw-rw-rw-   0        0        0    14394 2024-05-15 06:11:38.000000 QWeb-3.3.0/QWeb/keywords/file.py
--rw-rw-rw-   0        0        0     4624 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/frame.py
--rw-rw-rw-   0        0        0    11998 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/keywords/icon.py
--rw-rw-rw-   0        0        0    35769 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/keywords/input_.py
--rw-rw-rw-   0        0        0     1887 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/javascript.py
--rw-rw-rw-   0        0        0     8630 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/lists.py
--rw-rw-rw-   0        0        0     2968 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/screenshot.py
--rw-rw-rw-   0        0        0     8480 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/search_strategy.py
--rw-rw-rw-   0        0        0    20397 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/keywords/table.py
--rw-rw-rw-   0        0        0    66946 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/keywords/text.py
--rw-rw-rw-   0        0        0    17192 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/window.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:40:05.890885 QWeb-3.3.0/QWeb.egg-info/
--rw-rw-rw-   0        0        0    11340 2024-05-15 06:40:05.000000 QWeb-3.3.0/QWeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2018 2024-05-15 06:40:05.000000 QWeb-3.3.0/QWeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 06:40:05.000000 QWeb-3.3.0/QWeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-09-08 09:34:25.000000 QWeb-3.3.0/QWeb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      351 2024-05-15 06:40:05.000000 QWeb-3.3.0/QWeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-15 06:40:05.000000 QWeb-3.3.0/QWeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10600 2023-10-20 07:45:42.000000 QWeb-3.3.0/README.md
--rw-rw-rw-   0        0        0     1209 2024-05-15 06:40:07.550763 QWeb-3.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2532 2024-04-05 12:00:29.000000 QWeb-3.3.0/setup.py
--rw-rw-rw-   0        0        0    70433 2021-09-04 19:02:10.000000 QWeb-3.3.0/versioneer.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:43:29.053859 QWeb-3.3.1/
+-rw-rw-rw-   0        0        0    11558 2021-09-04 19:02:10.000000 QWeb-3.3.1/LICENSE
+-rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-3.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    11340 2024-05-22 14:43:29.054852 QWeb-3.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 14:43:29.070668 QWeb-3.3.1/QWeb/
+-rw-rw-rw-   0        0        0    16938 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/__init__.py
+-rw-rw-rw-   0        0        0     2259 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/__main__.py
+-rw-rw-rw-   0        0        0      519 2024-05-22 14:43:29.071253 QWeb-3.3.1/QWeb/_version.py
+-rw-rw-rw-   0        0        0     1408 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/custom_config.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:43:28.915728 QWeb-3.3.1/QWeb/internal/
+-rw-rw-rw-   0        0        0       64 2021-09-04 19:02:10.000000 QWeb-3.3.1/QWeb/internal/__init__.py
+-rw-rw-rw-   0        0        0    21711 2024-05-06 12:35:56.000000 QWeb-3.3.1/QWeb/internal/actions.py
+-rw-rw-rw-   0        0        0     3671 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/ajax.py
+-rw-rw-rw-   0        0        0     1709 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/alert.py
+-rw-rw-rw-   0        0        0     3691 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/blocks.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:43:28.944619 QWeb-3.3.1/QWeb/internal/browser/
+-rw-rw-rw-   0        0        0     4879 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/browser/__init__.py
+-rw-rw-rw-   0        0        0     1548 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/browser/android.py
+-rw-rw-rw-   0        0        0     3426 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/browser/bs_desktop.py
+-rw-rw-rw-   0        0        0     2166 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/browser/bs_mobile.py
+-rw-rw-rw-   0        0        0     6072 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/browser/chrome.py
+-rw-rw-rw-   0        0        0     4308 2024-05-06 12:35:56.000000 QWeb-3.3.1/QWeb/internal/browser/edge.py
+-rw-rw-rw-   0        0        0     5093 2024-05-06 12:35:56.000000 QWeb-3.3.1/QWeb/internal/browser/firefox.py
+-rw-rw-rw-   0        0        0     1884 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/browser/safari.py
+-rw-rw-rw-   0        0        0     6141 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/checkbox.py
+-rw-rw-rw-   0        0        0     4314 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/config.py
+-rw-rw-rw-   0        0        0     4442 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/config_defaults.py
+-rw-rw-rw-   0        0        0     1294 2022-11-22 10:56:24.000000 QWeb-3.3.1/QWeb/internal/cookies.py
+-rw-rw-rw-   0        0        0     9703 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/decorators.py
+-rw-rw-rw-   0        0        0     5625 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/download.py
+-rw-rw-rw-   0        0        0     3096 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/dragdrop.py
+-rw-rw-rw-   0        0        0     7881 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/dropdown.py
+-rw-rw-rw-   0        0        0    29827 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/element.py
+-rw-rw-rw-   0        0        0     3105 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/exceptions.py
+-rw-rw-rw-   0        0        0     3550 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/file.py
+-rw-rw-rw-   0        0        0    11694 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/frame.py
+-rw-rw-rw-   0        0        0     1960 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/frame_checker.py
+-rw-rw-rw-   0        0        0    21185 2024-05-06 12:35:56.000000 QWeb-3.3.1/QWeb/internal/icon.py
+-rw-rw-rw-   0        0        0    10845 2024-05-06 12:35:56.000000 QWeb-3.3.1/QWeb/internal/input_.py
+-rw-rw-rw-   0        0        0     7292 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/input_handler.py
+-rw-rw-rw-   0        0        0    21147 2024-05-20 06:34:29.000000 QWeb-3.3.1/QWeb/internal/javascript.py
+-rw-rw-rw-   0        0        0     9115 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/lists.py
+-rw-rw-rw-   0        0        0     3180 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/meas.py
+-rw-rw-rw-   0        0        0      833 2022-06-16 12:12:06.000000 QWeb-3.3.1/QWeb/internal/platform.py
+-rw-rw-rw-   0        0        0    13285 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/screenshot.py
+-rw-rw-rw-   0        0        0     7236 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/search_strategy.py
+-rw-rw-rw-   0        0        0     8613 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/secrets.py
+-rw-rw-rw-   0        0        0    16553 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/table.py
+-rw-rw-rw-   0        0        0    19349 2024-05-22 11:39:49.000000 QWeb-3.3.1/QWeb/internal/text.py
+-rw-rw-rw-   0        0        0     1373 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/user.py
+-rw-rw-rw-   0        0        0    13801 2024-05-17 11:06:51.000000 QWeb-3.3.1/QWeb/internal/util.py
+-rw-rw-rw-   0        0        0     4233 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/window.py
+-rw-rw-rw-   0        0        0     3303 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/internal/xhr.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:43:29.048826 QWeb-3.3.1/QWeb/keywords/
+-rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-3.3.1/QWeb/keywords/__init__.py
+-rw-rw-rw-   0        0        0     4473 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/keywords/ajax.py
+-rw-rw-rw-   0        0        0     4920 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/keywords/alert.py
+-rw-rw-rw-   0        0        0     5920 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/keywords/blocks.py
+-rw-rw-rw-   0        0        0    24523 2024-05-06 12:35:56.000000 QWeb-3.3.1/QWeb/keywords/browser.py
+-rw-rw-rw-   0        0        0    12198 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/keywords/checkbox.py
+-rw-rw-rw-   0        0        0    37935 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/keywords/config.py
+-rw-rw-rw-   0        0        0     3055 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/keywords/cookies.py
+-rw-rw-rw-   0        0        0     2508 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/keywords/debug.py
+-rw-rw-rw-   0        0        0     4028 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/keywords/download.py
+-rw-rw-rw-   0        0        0     6151 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/keywords/dragdrop.py
+-rw-rw-rw-   0        0        0    14990 2024-05-15 06:11:38.000000 QWeb-3.3.1/QWeb/keywords/dropdown.py
+-rw-rw-rw-   0        0        0    27779 2024-05-15 06:11:38.000000 QWeb-3.3.1/QWeb/keywords/element.py
+-rw-rw-rw-   0        0        0    14394 2024-05-15 06:11:38.000000 QWeb-3.3.1/QWeb/keywords/file.py
+-rw-rw-rw-   0        0        0     4624 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/keywords/frame.py
+-rw-rw-rw-   0        0        0    11998 2024-05-06 12:35:56.000000 QWeb-3.3.1/QWeb/keywords/icon.py
+-rw-rw-rw-   0        0        0    35769 2024-05-06 12:35:56.000000 QWeb-3.3.1/QWeb/keywords/input_.py
+-rw-rw-rw-   0        0        0     1887 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/keywords/javascript.py
+-rw-rw-rw-   0        0        0     8630 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/keywords/lists.py
+-rw-rw-rw-   0        0        0     2968 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/keywords/screenshot.py
+-rw-rw-rw-   0        0        0     8480 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/keywords/search_strategy.py
+-rw-rw-rw-   0        0        0    20397 2024-05-06 12:35:56.000000 QWeb-3.3.1/QWeb/keywords/table.py
+-rw-rw-rw-   0        0        0    66946 2024-05-06 12:35:56.000000 QWeb-3.3.1/QWeb/keywords/text.py
+-rw-rw-rw-   0        0        0    17192 2024-04-24 06:29:20.000000 QWeb-3.3.1/QWeb/keywords/window.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:43:28.791624 QWeb-3.3.1/QWeb.egg-info/
+-rw-rw-rw-   0        0        0    11340 2024-05-22 14:43:28.000000 QWeb-3.3.1/QWeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2018 2024-05-22 14:43:28.000000 QWeb-3.3.1/QWeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 14:43:28.000000 QWeb-3.3.1/QWeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-09-08 09:34:25.000000 QWeb-3.3.1/QWeb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      351 2024-05-22 14:43:28.000000 QWeb-3.3.1/QWeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-22 14:43:28.000000 QWeb-3.3.1/QWeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10600 2023-10-20 07:45:42.000000 QWeb-3.3.1/README.md
+-rw-rw-rw-   0        0        0     1209 2024-05-22 14:43:29.069170 QWeb-3.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2532 2024-04-05 12:00:29.000000 QWeb-3.3.1/setup.py
+-rw-rw-rw-   0        0        0    70433 2021-09-04 19:02:10.000000 QWeb-3.3.1/versioneer.py
```

### Comparing `QWeb-3.3.0/LICENSE` & `QWeb-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/PKG-INFO` & `QWeb-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QWeb
-Version: 3.3.0
+Version: 3.3.1
 Summary: Keyword driven automation for the web
 Home-page: https://github.com/qentinelqi/qweb/
 Author: Qentinel Group
 Author-email: libraries@qentinel.com
 License: Apache License 2.0
 Keywords: test automation robot framework
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `QWeb-3.3.0/QWeb/__init__.py` & `QWeb-3.3.1/QWeb/__init__.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/__main__.py` & `QWeb-3.3.1/QWeb/__main__.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/custom_config.py` & `QWeb-3.3.1/QWeb/custom_config.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/actions.py` & `QWeb-3.3.1/QWeb/internal/actions.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/ajax.py` & `QWeb-3.3.1/QWeb/internal/ajax.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/alert.py` & `QWeb-3.3.1/QWeb/internal/alert.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/blocks.py` & `QWeb-3.3.1/QWeb/internal/blocks.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/browser/__init__.py` & `QWeb-3.3.1/QWeb/internal/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/browser/android.py` & `QWeb-3.3.1/QWeb/internal/browser/android.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/browser/bs_desktop.py` & `QWeb-3.3.1/QWeb/internal/browser/bs_desktop.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/browser/bs_mobile.py` & `QWeb-3.3.1/QWeb/internal/browser/bs_mobile.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/browser/chrome.py` & `QWeb-3.3.1/QWeb/internal/browser/chrome.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/browser/edge.py` & `QWeb-3.3.1/QWeb/internal/browser/edge.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/browser/firefox.py` & `QWeb-3.3.1/QWeb/internal/browser/firefox.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/browser/safari.py` & `QWeb-3.3.1/QWeb/internal/browser/safari.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/checkbox.py` & `QWeb-3.3.1/QWeb/internal/checkbox.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/config.py` & `QWeb-3.3.1/QWeb/internal/config.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/config_defaults.py` & `QWeb-3.3.1/QWeb/internal/config_defaults.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/cookies.py` & `QWeb-3.3.1/QWeb/internal/cookies.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/decorators.py` & `QWeb-3.3.1/QWeb/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/download.py` & `QWeb-3.3.1/QWeb/internal/download.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/dragdrop.py` & `QWeb-3.3.1/QWeb/internal/dragdrop.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/dropdown.py` & `QWeb-3.3.1/QWeb/internal/dropdown.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/element.py` & `QWeb-3.3.1/QWeb/internal/element.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/exceptions.py` & `QWeb-3.3.1/QWeb/internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/file.py` & `QWeb-3.3.1/QWeb/internal/file.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/frame.py` & `QWeb-3.3.1/QWeb/internal/frame.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/frame_checker.py` & `QWeb-3.3.1/QWeb/internal/frame_checker.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/icon.py` & `QWeb-3.3.1/QWeb/internal/icon.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/input_.py` & `QWeb-3.3.1/QWeb/internal/input_.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/input_handler.py` & `QWeb-3.3.1/QWeb/internal/input_handler.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/javascript.py` & `QWeb-3.3.1/QWeb/internal/javascript.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/lists.py` & `QWeb-3.3.1/QWeb/internal/lists.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/meas.py` & `QWeb-3.3.1/QWeb/internal/meas.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/platform.py` & `QWeb-3.3.1/QWeb/internal/platform.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/screenshot.py` & `QWeb-3.3.1/QWeb/internal/screenshot.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/search_strategy.py` & `QWeb-3.3.1/QWeb/internal/search_strategy.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/secrets.py` & `QWeb-3.3.1/QWeb/internal/secrets.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/table.py` & `QWeb-3.3.1/QWeb/internal/table.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/text.py` & `QWeb-3.3.1/QWeb/internal/text.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     if all_text_nodes:
         web_elements = check_all_nodes(text, **kwargs)
         if web_elements:
             return web_elements
 
     if "css" not in kwargs:
         try:
-            web_elements = get_clickable_element_by_js(text, shadow_dom=shadow_dom, **kwargs)
+            web_elements = get_clickable_elements(text, shadow_dom=shadow_dom, **kwargs)
         except (
             JavascriptException,
             WebDriverException,
             NoSuchFrameException,
             QWebStalingElementError,
         ) as e:
             logger.debug("got {}. Syntax might be invalid".format(e))
@@ -424,29 +424,59 @@
         inner_text = el.get_attribute("innerText") or ""
         if (exact_match and anchor == inner_text) or (not exact_match and anchor in inner_text):
             return el
     return None
 
 
 @frame.all_frames
-def get_clickable_element_by_js(
+def get_clickable_elements(
     locator: str, shadow_dom: bool = False, **kwargs
 ) -> Optional[list[WebElement]]:
+    """
+    Retrieve clickable elements based on a locator string.
+
+    Args:
+        locator (str): The string to locate elements by.
+        shadow_dom (bool): Whether to search within shadow DOM.
+        partial_match (bool): Whether to use partial matching.
+        **kwargs: Additional keyword arguments.
+
+    Returns:
+        Optional[List[WebElement]]: List of clickable WebElement objects, or None if none found.
+    """
     partial = kwargs["partial_match"]
+
+    # find parent <a> from slots with direct text
+    if partial:
+        xpath = f"//a[descendant::slot[contains(., '{locator}')]]"
+    else:
+        xpath = f"//a[descendant::slot[text()='{locator}']]"
+
+    # Find slots with text and get their parent link
+    driver = browser.get_current_browser()
+    xpath_elements = driver.find_elements(By.XPATH, xpath)
+    # Find normal elements via javascript
     if shadow_dom:
-        web_elements = element.get_visible_elements_from_elements(
-            javascript.get_clickable_from_shadow_dom(locator, partial)
-        )
+        js_elements = javascript.get_clickable_from_shadow_dom(locator, partial)
     else:
-        web_elements = element.get_visible_elements_from_elements(
-            javascript.get_clickable(locator), **kwargs
-        )
-    if web_elements:
-        logger.debug("Found elements by js: {}".format(web_elements))
-        return web_elements
+        js_elements = javascript.get_clickable(locator)
+
+    if js_elements:
+        logger.debug(f"Found elements by js: {js_elements}")
+
+    # merge found elements and check visibility
+    if not xpath_elements:
+        xpath_elements = []
+    else:
+        logger.debug(f"Found elements by xpath: {xpath_elements}")
+    if js_elements:
+        util.remove_duplicates_from_list(js_elements, xpath_elements)
+        # util.remove_stale_elements(xpath_elements)
+    if xpath_elements:
+        return element.get_visible_elements_from_elements(xpath_elements, **kwargs)
     return None
 
 
 @frame.all_frames
 def get_texts_including_shadow_dom(locator: str, partial: bool, **kwargs) -> list[WebElement]:
     web_elements = element.get_visible_elements_from_elements(
         javascript.get_text_elements_from_shadow_dom(locator, partial), **kwargs
```

### Comparing `QWeb-3.3.0/QWeb/internal/user.py` & `QWeb-3.3.1/QWeb/internal/user.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/util.py` & `QWeb-3.3.1/QWeb/internal/util.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/window.py` & `QWeb-3.3.1/QWeb/internal/window.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/internal/xhr.py` & `QWeb-3.3.1/QWeb/internal/xhr.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/ajax.py` & `QWeb-3.3.1/QWeb/keywords/ajax.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/alert.py` & `QWeb-3.3.1/QWeb/keywords/alert.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/blocks.py` & `QWeb-3.3.1/QWeb/keywords/blocks.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/browser.py` & `QWeb-3.3.1/QWeb/keywords/browser.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/checkbox.py` & `QWeb-3.3.1/QWeb/keywords/checkbox.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/config.py` & `QWeb-3.3.1/QWeb/keywords/config.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/cookies.py` & `QWeb-3.3.1/QWeb/keywords/cookies.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/debug.py` & `QWeb-3.3.1/QWeb/keywords/debug.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/download.py` & `QWeb-3.3.1/QWeb/keywords/download.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/dragdrop.py` & `QWeb-3.3.1/QWeb/keywords/dragdrop.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/dropdown.py` & `QWeb-3.3.1/QWeb/keywords/dropdown.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/element.py` & `QWeb-3.3.1/QWeb/keywords/element.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/file.py` & `QWeb-3.3.1/QWeb/keywords/file.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/frame.py` & `QWeb-3.3.1/QWeb/keywords/frame.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/icon.py` & `QWeb-3.3.1/QWeb/keywords/icon.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/input_.py` & `QWeb-3.3.1/QWeb/keywords/input_.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/javascript.py` & `QWeb-3.3.1/QWeb/keywords/javascript.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/lists.py` & `QWeb-3.3.1/QWeb/keywords/lists.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/screenshot.py` & `QWeb-3.3.1/QWeb/keywords/screenshot.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/search_strategy.py` & `QWeb-3.3.1/QWeb/keywords/search_strategy.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/table.py` & `QWeb-3.3.1/QWeb/keywords/table.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/text.py` & `QWeb-3.3.1/QWeb/keywords/text.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb/keywords/window.py` & `QWeb-3.3.1/QWeb/keywords/window.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/QWeb.egg-info/PKG-INFO` & `QWeb-3.3.1/QWeb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QWeb
-Version: 3.3.0
+Version: 3.3.1
 Summary: Keyword driven automation for the web
 Home-page: https://github.com/qentinelqi/qweb/
 Author: Qentinel Group
 Author-email: libraries@qentinel.com
 License: Apache License 2.0
 Keywords: test automation robot framework
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `QWeb-3.3.0/QWeb.egg-info/SOURCES.txt` & `QWeb-3.3.1/QWeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/README.md` & `QWeb-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/setup.cfg` & `QWeb-3.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/setup.py` & `QWeb-3.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.3.0/versioneer.py` & `QWeb-3.3.1/versioneer.py`

 * *Files identical despite different names*

