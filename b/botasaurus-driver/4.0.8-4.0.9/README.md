# Comparing `tmp/botasaurus_driver-4.0.8.tar.gz` & `tmp/botasaurus_driver-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus_driver-4.0.8.tar", last modified: Wed May 15 15:13:03 2024, max compression
+gzip compressed data, was "botasaurus_driver-4.0.9.tar", last modified: Thu May 16 13:39:29 2024, max compression
```

## Comparing `botasaurus_driver-4.0.8.tar` & `botasaurus_driver-4.0.9.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 15:13:03.433346 botasaurus_driver-4.0.8/
--rw-rw-rw-   0        0        0     1094 2024-03-03 08:47:03.000000 botasaurus_driver-4.0.8/LICENSE
--rw-rw-rw-   0        0        0      139 2024-04-24 09:55:31.000000 botasaurus_driver-4.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     6851 2024-05-15 15:13:03.433346 botasaurus_driver-4.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3984 2024-05-14 14:16:36.000000 botasaurus_driver-4.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 15:13:03.260662 botasaurus_driver-4.0.8/botasaurus_driver/
--rw-rw-rw-   0        0        0      638 2024-05-06 12:43:02.000000 botasaurus_driver-4.0.8/botasaurus_driver/__init__.py
--rw-rw-rw-   0        0        0     3673 2024-04-22 10:12:09.000000 botasaurus_driver-4.0.8/botasaurus_driver/base_data.py
--rw-rw-rw-   0        0        0     1305 2024-04-22 08:12:58.000000 botasaurus_driver-4.0.8/botasaurus_driver/beep_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 15:13:03.406888 botasaurus_driver-4.0.8/botasaurus_driver/cdp/
--rw-rw-rw-   0        0        0      172 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/README.md
--rw-rw-rw-   0        0        0     1011 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/__init__.py
--rw-rw-rw-   0        0        0    25019 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/accessibility.py
--rw-rw-rw-   0        0        0    11919 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/animation.py
--rw-rw-rw-   0        0        0    65075 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/audits.py
--rw-rw-rw-   0        0        0     8168 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/autofill.py
--rw-rw-rw-   0        0        0     6359 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/background_service.py
--rw-rw-rw-   0        0        0    22888 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/browser.py
--rw-rw-rw-   0        0        0     9549 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/cache_storage.py
--rw-rw-rw-   0        0        0     4565 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/cast.py
--rw-rw-rw-   0        0        0     3004 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/console.py
--rw-rw-rw-   0        0        0    80456 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/css.py
--rw-rw-rw-   0        0        0     4358 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/database.py
--rw-rw-rw-   0        0        0    54782 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/debugger.py
--rw-rw-rw-   0        0        0     3497 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/device_access.py
--rw-rw-rw-   0        0        0     1187 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/device_orientation.py
--rw-rw-rw-   0        0        0    66246 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/dom.py
--rw-rw-rw-   0        0        0    10211 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/dom_debugger.py
--rw-rw-rw-   0        0        0    43435 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/dom_snapshot.py
--rw-rw-rw-   0        0        0     6124 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/dom_storage.py
--rw-rw-rw-   0        0        0    34831 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/emulation.py
--rw-rw-rw-   0        0        0     1501 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/event_breakpoints.py
--rw-rw-rw-   0        0        0     7347 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/fed_cm.py
--rw-rw-rw-   0        0        0    21611 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/fetch.py
--rw-rw-rw-   0        0        0     5219 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/headless_experimental.py
--rw-rw-rw-   0        0        0    14457 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/heap_profiler.py
--rw-rw-rw-   0        0        0    18362 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/indexed_db.py
--rw-rw-rw-   0        0        0    29314 2024-04-15 12:04:59.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/input_.py
--rw-rw-rw-   0        0        0     1743 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/inspector.py
--rw-rw-rw-   0        0        0     3120 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/io.py
--rw-rw-rw-   0        0        0    16878 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/layer_tree.py
--rw-rw-rw-   0        0        0     6092 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/log.py
--rw-rw-rw-   0        0        0     8215 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/media.py
--rw-rw-rw-   0        0        0     7279 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/memory.py
--rw-rw-rw-   0        0        0   147161 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/network.py
--rw-rw-rw-   0        0        0    60483 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/overlay.py
--rw-rw-rw-   0        0        0   117573 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/page.py
--rw-rw-rw-   0        0        0     3203 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/performance.py
--rw-rw-rw-   0        0        0     7587 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/performance_timeline.py
--rw-rw-rw-   0        0        0    22524 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/preload.py
--rw-rw-rw-   0        0        0    14302 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/profiler.py
--rw-rw-rw-   0        0        0        0 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/py.typed
--rw-rw-rw-   0        0        0    67631 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/runtime.py
--rw-rw-rw-   0        0        0     1196 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/schema.py
--rw-rw-rw-   0        0        0    18824 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/security.py
--rw-rw-rw-   0        0        0    12358 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/service_worker.py
--rw-rw-rw-   0        0        0    61377 2024-04-17 07:20:04.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/storage.py
--rw-rw-rw-   0        0        0    12914 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/system_info.py
--rw-rw-rw-   0        0        0    25505 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/target.py
--rw-rw-rw-   0        0        0     1533 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/tethering.py
--rw-rw-rw-   0        0        0    14682 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/tracing.py
--rw-rw-rw-   0        0        0      470 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/util.py
--rw-rw-rw-   0        0        0    18513 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/web_audio.py
--rw-rw-rw-   0        0        0    18390 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.8/botasaurus_driver/cdp/web_authn.py
-drwxrwxrwx   0        0        0        0 2024-05-15 15:13:03.428383 botasaurus_driver-4.0.8/botasaurus_driver/core/
--rw-rw-rw-   0        0        0     3344 2024-04-19 06:25:12.000000 botasaurus_driver-4.0.8/botasaurus_driver/core/_contradict.py
--rw-rw-rw-   0        0        0    17760 2024-05-10 15:05:54.000000 botasaurus_driver-4.0.8/botasaurus_driver/core/browser.py
--rw-rw-rw-   0        0        0    12463 2024-05-15 14:53:11.000000 botasaurus_driver-4.0.8/botasaurus_driver/core/config.py
--rw-rw-rw-   0        0        0    17622 2024-05-14 12:40:04.000000 botasaurus_driver-4.0.8/botasaurus_driver/core/connection.py
--rw-rw-rw-   0        0        0     1445 2024-04-22 12:23:38.000000 botasaurus_driver-4.0.8/botasaurus_driver/core/custom_storage_cdp.py
--rw-rw-rw-   0        0        0    33534 2024-04-22 07:27:39.000000 botasaurus_driver-4.0.8/botasaurus_driver/core/element.py
--rw-rw-rw-   0        0        0      729 2024-05-15 14:51:32.000000 botasaurus_driver-4.0.8/botasaurus_driver/core/env.py
--rw-rw-rw-   0        0        0     3185 2024-04-22 11:09:04.000000 botasaurus_driver-4.0.8/botasaurus_driver/core/profiles.py
--rw-rw-rw-   0        0        0    40672 2024-05-10 14:59:53.000000 botasaurus_driver-4.0.8/botasaurus_driver/core/tab.py
--rw-rw-rw-   0        0        0     4748 2024-04-22 11:57:20.000000 botasaurus_driver-4.0.8/botasaurus_driver/core/util.py
--rw-rw-rw-   0        0        0    37106 2024-05-14 05:29:03.000000 botasaurus_driver-4.0.8/botasaurus_driver/driver.py
--rw-rw-rw-   0        0        0     5041 2024-04-22 10:57:19.000000 botasaurus_driver-4.0.8/botasaurus_driver/driver_utils.py
--rw-rw-rw-   0        0        0     4957 2024-05-02 11:54:25.000000 botasaurus_driver-4.0.8/botasaurus_driver/exceptions.py
--rw-rw-rw-   0        0        0     3764 2024-04-22 13:03:42.000000 botasaurus_driver-4.0.8/botasaurus_driver/lang.py
--rw-rw-rw-   0        0        0     1710 2024-04-16 12:10:34.000000 botasaurus_driver-4.0.8/botasaurus_driver/local_storage_driver.py
--rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.000000 botasaurus_driver-4.0.8/botasaurus_driver/opponent.py
--rw-rw-rw-   0        0        0     4153 2024-05-02 11:56:26.000000 botasaurus_driver-4.0.8/botasaurus_driver/profile.py
--rw-rw-rw-   0        0        0     4617 2024-05-12 10:41:42.000000 botasaurus_driver-4.0.8/botasaurus_driver/solve_cloudflare_captcha.py
--rw-rw-rw-   0        0        0     1160 2024-04-22 13:05:31.000000 botasaurus_driver-4.0.8/botasaurus_driver/tiny_profile.py
--rw-rw-rw-   0        0        0     7569 2024-04-22 13:04:27.000000 botasaurus_driver-4.0.8/botasaurus_driver/user_agent.py
--rw-rw-rw-   0        0        0     1203 2024-04-22 13:04:27.000000 botasaurus_driver-4.0.8/botasaurus_driver/window_size.py
-drwxrwxrwx   0        0        0        0 2024-05-15 15:13:03.429450 botasaurus_driver-4.0.8/botasaurus_driver.egg-info/
--rw-rw-rw-   0        0        0     6851 2024-05-15 15:13:02.000000 botasaurus_driver-4.0.8/botasaurus_driver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2952 2024-05-15 15:13:03.000000 botasaurus_driver-4.0.8/botasaurus_driver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 15:13:02.000000 botasaurus_driver-4.0.8/botasaurus_driver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      171 2024-05-15 15:13:02.000000 botasaurus_driver-4.0.8/botasaurus_driver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-15 15:13:02.000000 botasaurus_driver-4.0.8/botasaurus_driver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1941 2024-05-15 15:13:01.000000 botasaurus_driver-4.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       81 2024-05-15 15:13:03.442399 botasaurus_driver-4.0.8/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-24 07:16:00.000000 botasaurus_driver-4.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:39:29.395179 botasaurus_driver-4.0.9/
+-rw-rw-rw-   0        0        0     1094 2024-03-03 08:47:03.000000 botasaurus_driver-4.0.9/LICENSE
+-rw-rw-rw-   0        0        0      139 2024-04-24 09:55:31.000000 botasaurus_driver-4.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6851 2024-05-16 13:39:29.394559 botasaurus_driver-4.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3984 2024-05-14 14:16:36.000000 botasaurus_driver-4.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 13:39:29.184464 botasaurus_driver-4.0.9/botasaurus_driver/
+-rw-rw-rw-   0        0        0      638 2024-05-06 12:43:02.000000 botasaurus_driver-4.0.9/botasaurus_driver/__init__.py
+-rw-rw-rw-   0        0        0     3673 2024-04-22 10:12:09.000000 botasaurus_driver-4.0.9/botasaurus_driver/base_data.py
+-rw-rw-rw-   0        0        0     1305 2024-04-22 08:12:58.000000 botasaurus_driver-4.0.9/botasaurus_driver/beep_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:39:29.363009 botasaurus_driver-4.0.9/botasaurus_driver/cdp/
+-rw-rw-rw-   0        0        0      172 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/README.md
+-rw-rw-rw-   0        0        0     1011 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/__init__.py
+-rw-rw-rw-   0        0        0    25019 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/accessibility.py
+-rw-rw-rw-   0        0        0    11919 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/animation.py
+-rw-rw-rw-   0        0        0    65075 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/audits.py
+-rw-rw-rw-   0        0        0     8168 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/autofill.py
+-rw-rw-rw-   0        0        0     6359 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/background_service.py
+-rw-rw-rw-   0        0        0    22888 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/browser.py
+-rw-rw-rw-   0        0        0     9549 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/cache_storage.py
+-rw-rw-rw-   0        0        0     4565 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/cast.py
+-rw-rw-rw-   0        0        0     3004 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/console.py
+-rw-rw-rw-   0        0        0    80456 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/css.py
+-rw-rw-rw-   0        0        0     4358 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/database.py
+-rw-rw-rw-   0        0        0    54782 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/debugger.py
+-rw-rw-rw-   0        0        0     3497 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/device_access.py
+-rw-rw-rw-   0        0        0     1187 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/device_orientation.py
+-rw-rw-rw-   0        0        0    66246 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/dom.py
+-rw-rw-rw-   0        0        0    10211 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/dom_debugger.py
+-rw-rw-rw-   0        0        0    43435 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/dom_snapshot.py
+-rw-rw-rw-   0        0        0     6124 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/dom_storage.py
+-rw-rw-rw-   0        0        0    34831 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/emulation.py
+-rw-rw-rw-   0        0        0     1501 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/event_breakpoints.py
+-rw-rw-rw-   0        0        0     7347 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/fed_cm.py
+-rw-rw-rw-   0        0        0    21611 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/fetch.py
+-rw-rw-rw-   0        0        0     5219 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/headless_experimental.py
+-rw-rw-rw-   0        0        0    14457 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/heap_profiler.py
+-rw-rw-rw-   0        0        0    18362 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/indexed_db.py
+-rw-rw-rw-   0        0        0    29314 2024-04-15 12:04:59.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/input_.py
+-rw-rw-rw-   0        0        0     1743 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/inspector.py
+-rw-rw-rw-   0        0        0     3120 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/io.py
+-rw-rw-rw-   0        0        0    16878 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/layer_tree.py
+-rw-rw-rw-   0        0        0     6092 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/log.py
+-rw-rw-rw-   0        0        0     8215 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/media.py
+-rw-rw-rw-   0        0        0     7279 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/memory.py
+-rw-rw-rw-   0        0        0   147161 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/network.py
+-rw-rw-rw-   0        0        0    60483 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/overlay.py
+-rw-rw-rw-   0        0        0   117573 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/page.py
+-rw-rw-rw-   0        0        0     3203 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/performance.py
+-rw-rw-rw-   0        0        0     7587 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/performance_timeline.py
+-rw-rw-rw-   0        0        0    22524 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/preload.py
+-rw-rw-rw-   0        0        0    14302 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/profiler.py
+-rw-rw-rw-   0        0        0        0 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/py.typed
+-rw-rw-rw-   0        0        0    67631 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/runtime.py
+-rw-rw-rw-   0        0        0     1196 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/schema.py
+-rw-rw-rw-   0        0        0    18824 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/security.py
+-rw-rw-rw-   0        0        0    12358 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/service_worker.py
+-rw-rw-rw-   0        0        0    61377 2024-04-17 07:20:04.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/storage.py
+-rw-rw-rw-   0        0        0    12914 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/system_info.py
+-rw-rw-rw-   0        0        0    25505 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/target.py
+-rw-rw-rw-   0        0        0     1533 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/tethering.py
+-rw-rw-rw-   0        0        0    14682 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/tracing.py
+-rw-rw-rw-   0        0        0      470 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/util.py
+-rw-rw-rw-   0        0        0    18513 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/web_audio.py
+-rw-rw-rw-   0        0        0    18390 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.9/botasaurus_driver/cdp/web_authn.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:39:29.388008 botasaurus_driver-4.0.9/botasaurus_driver/core/
+-rw-rw-rw-   0        0        0     3344 2024-04-19 06:25:12.000000 botasaurus_driver-4.0.9/botasaurus_driver/core/_contradict.py
+-rw-rw-rw-   0        0        0    17760 2024-05-10 15:05:54.000000 botasaurus_driver-4.0.9/botasaurus_driver/core/browser.py
+-rw-rw-rw-   0        0        0    12463 2024-05-15 14:53:11.000000 botasaurus_driver-4.0.9/botasaurus_driver/core/config.py
+-rw-rw-rw-   0        0        0    17622 2024-05-14 12:40:04.000000 botasaurus_driver-4.0.9/botasaurus_driver/core/connection.py
+-rw-rw-rw-   0        0        0     1445 2024-04-22 12:23:38.000000 botasaurus_driver-4.0.9/botasaurus_driver/core/custom_storage_cdp.py
+-rw-rw-rw-   0        0        0    33534 2024-04-22 07:27:39.000000 botasaurus_driver-4.0.9/botasaurus_driver/core/element.py
+-rw-rw-rw-   0        0        0      729 2024-05-15 14:51:32.000000 botasaurus_driver-4.0.9/botasaurus_driver/core/env.py
+-rw-rw-rw-   0        0        0     3185 2024-04-22 11:09:04.000000 botasaurus_driver-4.0.9/botasaurus_driver/core/profiles.py
+-rw-rw-rw-   0        0        0    40672 2024-05-10 14:59:53.000000 botasaurus_driver-4.0.9/botasaurus_driver/core/tab.py
+-rw-rw-rw-   0        0        0     4748 2024-04-22 11:57:20.000000 botasaurus_driver-4.0.9/botasaurus_driver/core/util.py
+-rw-rw-rw-   0        0        0    37553 2024-05-16 13:36:36.000000 botasaurus_driver-4.0.9/botasaurus_driver/driver.py
+-rw-rw-rw-   0        0        0     5041 2024-04-22 10:57:19.000000 botasaurus_driver-4.0.9/botasaurus_driver/driver_utils.py
+-rw-rw-rw-   0        0        0     4957 2024-05-02 11:54:25.000000 botasaurus_driver-4.0.9/botasaurus_driver/exceptions.py
+-rw-rw-rw-   0        0        0     3764 2024-04-22 13:03:42.000000 botasaurus_driver-4.0.9/botasaurus_driver/lang.py
+-rw-rw-rw-   0        0        0     1710 2024-04-16 12:10:34.000000 botasaurus_driver-4.0.9/botasaurus_driver/local_storage_driver.py
+-rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.000000 botasaurus_driver-4.0.9/botasaurus_driver/opponent.py
+-rw-rw-rw-   0        0        0     4153 2024-05-02 11:56:26.000000 botasaurus_driver-4.0.9/botasaurus_driver/profile.py
+-rw-rw-rw-   0        0        0     4617 2024-05-12 10:41:42.000000 botasaurus_driver-4.0.9/botasaurus_driver/solve_cloudflare_captcha.py
+-rw-rw-rw-   0        0        0     1160 2024-04-22 13:05:31.000000 botasaurus_driver-4.0.9/botasaurus_driver/tiny_profile.py
+-rw-rw-rw-   0        0        0     7569 2024-04-22 13:04:27.000000 botasaurus_driver-4.0.9/botasaurus_driver/user_agent.py
+-rw-rw-rw-   0        0        0     1203 2024-04-22 13:04:27.000000 botasaurus_driver-4.0.9/botasaurus_driver/window_size.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:39:29.390626 botasaurus_driver-4.0.9/botasaurus_driver.egg-info/
+-rw-rw-rw-   0        0        0     6851 2024-05-16 13:39:28.000000 botasaurus_driver-4.0.9/botasaurus_driver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2952 2024-05-16 13:39:28.000000 botasaurus_driver-4.0.9/botasaurus_driver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 13:39:28.000000 botasaurus_driver-4.0.9/botasaurus_driver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      171 2024-05-16 13:39:28.000000 botasaurus_driver-4.0.9/botasaurus_driver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-16 13:39:28.000000 botasaurus_driver-4.0.9/botasaurus_driver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1941 2024-05-16 13:39:27.000000 botasaurus_driver-4.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2024-05-16 13:39:29.399025 botasaurus_driver-4.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-24 07:16:00.000000 botasaurus_driver-4.0.9/setup.py
```

### Comparing `botasaurus_driver-4.0.8/LICENSE` & `botasaurus_driver-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/PKG-INFO` & `botasaurus_driver-4.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus_driver
-Version: 4.0.8
+Version: 4.0.9
 Summary: Super Fast, Super Anti-Detect, and Super Intuitive Web Driver
 Author-email: Chetan <chetan@omkar.cloud>
 Maintainer-email: Chetan <chetan@omkar.cloud>
 License: MIT License
         
         Copyright (c) 2023-2024 Chetan Jain
```

### Comparing `botasaurus_driver-4.0.8/README.md` & `botasaurus_driver-4.0.9/README.md`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/__init__.py` & `botasaurus_driver-4.0.9/botasaurus_driver/__init__.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/base_data.py` & `botasaurus_driver-4.0.9/botasaurus_driver/base_data.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/beep_utils.py` & `botasaurus_driver-4.0.9/botasaurus_driver/beep_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/__init__.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/accessibility.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/accessibility.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/animation.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/animation.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/audits.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/audits.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/autofill.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/autofill.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/background_service.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/background_service.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/browser.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/browser.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/cache_storage.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/cache_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/cast.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/cast.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/console.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/console.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/css.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/css.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/database.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/database.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/debugger.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/debugger.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/device_access.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/device_access.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/device_orientation.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/device_orientation.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/dom.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/dom.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/dom_debugger.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/dom_debugger.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/dom_snapshot.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/dom_snapshot.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/dom_storage.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/dom_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/emulation.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/emulation.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/event_breakpoints.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/event_breakpoints.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/fed_cm.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/fed_cm.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/fetch.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/fetch.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/headless_experimental.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/headless_experimental.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/heap_profiler.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/heap_profiler.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/indexed_db.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/indexed_db.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/input_.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/input_.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/inspector.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/inspector.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/io.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/io.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/layer_tree.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/layer_tree.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/log.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/log.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/media.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/media.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/memory.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/memory.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/network.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/network.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/overlay.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/overlay.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/page.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/page.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/performance.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/performance.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/performance_timeline.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/performance_timeline.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/preload.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/preload.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/profiler.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/profiler.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/runtime.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/runtime.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/schema.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/schema.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/security.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/security.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/service_worker.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/service_worker.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/storage.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/system_info.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/system_info.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/target.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/target.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/tethering.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/tethering.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/tracing.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/tracing.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/web_audio.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/web_audio.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/cdp/web_authn.py` & `botasaurus_driver-4.0.9/botasaurus_driver/cdp/web_authn.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/core/_contradict.py` & `botasaurus_driver-4.0.9/botasaurus_driver/core/_contradict.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/core/browser.py` & `botasaurus_driver-4.0.9/botasaurus_driver/core/browser.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/core/config.py` & `botasaurus_driver-4.0.9/botasaurus_driver/core/config.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/core/connection.py` & `botasaurus_driver-4.0.9/botasaurus_driver/core/connection.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/core/custom_storage_cdp.py` & `botasaurus_driver-4.0.9/botasaurus_driver/core/custom_storage_cdp.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/core/element.py` & `botasaurus_driver-4.0.9/botasaurus_driver/core/element.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/core/env.py` & `botasaurus_driver-4.0.9/botasaurus_driver/core/env.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/core/profiles.py` & `botasaurus_driver-4.0.9/botasaurus_driver/core/profiles.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/core/tab.py` & `botasaurus_driver-4.0.9/botasaurus_driver/core/tab.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/core/util.py` & `botasaurus_driver-4.0.9/botasaurus_driver/core/util.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/driver.py` & `botasaurus_driver-4.0.9/botasaurus_driver/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -902,21 +902,30 @@
         self, target: str
     ) -> bool:
         return self.wait_for_page_to_be(target, None, raise_exception=False)
         
 
     def wait_for_page_to_be(self, expected_url: Union[str, List[str]], wait: Optional[int] = 8, raise_exception: bool = True) -> bool:
         def check_page(driver, expected_url):
-            if isinstance(expected_url, str):
-                return expected_url == driver.current_url
+            if expected_url.startswith('https://') or expected_url.startswith('http://'):
+                if isinstance(expected_url, str):
+                    return expected_url == driver.current_url
+                else:
+                    for url in expected_url:
+                        if url == driver.current_url:
+                            return True
+                return False
             else:
-                for url in expected_url:
-                    if url == driver.current_url:
-                        return True
-            return False
+                if isinstance(expected_url, str):
+                    return expected_url in driver.current_url
+                else:
+                    for x in expected_url:
+                        if x in driver.current_url:
+                            return True
+                    return False
 
         if wait is None:
             if check_page(self, expected_url):
                 wait_till_document_is_ready(self._tab, True)
                 return True
         else:
             time = 0
```

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/driver_utils.py` & `botasaurus_driver-4.0.9/botasaurus_driver/driver_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/exceptions.py` & `botasaurus_driver-4.0.9/botasaurus_driver/exceptions.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/lang.py` & `botasaurus_driver-4.0.9/botasaurus_driver/lang.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/local_storage_driver.py` & `botasaurus_driver-4.0.9/botasaurus_driver/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/profile.py` & `botasaurus_driver-4.0.9/botasaurus_driver/profile.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/solve_cloudflare_captcha.py` & `botasaurus_driver-4.0.9/botasaurus_driver/solve_cloudflare_captcha.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/tiny_profile.py` & `botasaurus_driver-4.0.9/botasaurus_driver/tiny_profile.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/user_agent.py` & `botasaurus_driver-4.0.9/botasaurus_driver/user_agent.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver/window_size.py` & `botasaurus_driver-4.0.9/botasaurus_driver/window_size.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver.egg-info/PKG-INFO` & `botasaurus_driver-4.0.9/botasaurus_driver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus_driver
-Version: 4.0.8
+Version: 4.0.9
 Summary: Super Fast, Super Anti-Detect, and Super Intuitive Web Driver
 Author-email: Chetan <chetan@omkar.cloud>
 Maintainer-email: Chetan <chetan@omkar.cloud>
 License: MIT License
         
         Copyright (c) 2023-2024 Chetan Jain
```

### Comparing `botasaurus_driver-4.0.8/botasaurus_driver.egg-info/SOURCES.txt` & `botasaurus_driver-4.0.9/botasaurus_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.8/pyproject.toml` & `botasaurus_driver-4.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "botasaurus_driver" # Required
-version="4.0.8"  # Required
+version="4.0.9"  # Required
 description = "Super Fast, Super Anti-Detect, and Super Intuitive Web Driver"
 readme = {file = "README.md", content-type = "text/markdown"} # Optional
 requires-python = ">=3.5"
 license = {file = "LICENSE"}
 keywords = [
     "webdriver", "browser", "captcha", "web-scraping",
     "selenium", "navigator", "python3", "cloudflare",
```

