# Comparing `tmp/qtile-0.9.0.tar.gz` & `tmp/qtile-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qtile-0.9.0.tar", last modified: Sat Feb 21 16:20:08 2015, max compression
+gzip compressed data, was "dist/qtile-0.9.1.tar", last modified: Sat Feb 21 16:21:29 2015, max compression
```

## Comparing `qtile-0.9.0.tar` & `qtile-0.9.1.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2015-02-21 16:20:08.000000 qtile-0.9.0/
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     2313 2015-02-21 16:19:53.000000 qtile-0.9.0/setup.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)       59 2015-02-21 16:20:08.000000 qtile-0.9.0/setup.cfg
-drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2015-02-21 16:20:08.000000 qtile-0.9.0/bin/
--rwxrwxr-x   0 tycho     (1000) tycho     (1000)     1856 2014-05-15 12:39:01.000000 qtile-0.9.0/bin/qtile-run
--rwxrwxr-x   0 tycho     (1000) tycho     (1000)     2239 2015-02-01 04:36:23.000000 qtile-0.9.0/bin/qtile-session
--rwxrwxr-x   0 tycho     (1000) tycho     (1000)     2213 2015-02-01 04:36:23.000000 qtile-0.9.0/bin/qsh
--rwxrwxr-x   0 tycho     (1000) tycho     (1000)     4171 2015-02-21 16:19:53.000000 qtile-0.9.0/bin/qtile
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     1187 2015-02-21 16:20:08.000000 qtile-0.9.0/PKG-INFO
--rw-r--r--   0 tycho     (1000) tycho     (1000)     1079 2014-01-10 20:09:17.000000 qtile-0.9.0/LICENSE
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     1916 2015-02-21 16:19:53.000000 qtile-0.9.0/README.rst
-drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2015-02-21 16:20:08.000000 qtile-0.9.0/libqtile/
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     4405 2015-02-01 04:36:23.000000 qtile-0.9.0/libqtile/utils.py
-drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2015-02-21 16:20:08.000000 qtile-0.9.0/libqtile/layout/
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    12751 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/layout/stack.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     6406 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/layout/tile.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    11967 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/layout/ratiotile.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    18087 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/layout/tree.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    10393 2015-02-08 15:39:59.000000 qtile-0.9.0/libqtile/layout/verticaltile.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     8560 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/layout/base.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     3472 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/layout/slice.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     5835 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/layout/matrix.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     3962 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/layout/max.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    26020 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/layout/xmonad.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     5215 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/layout/floating.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     4146 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/layout/zoomy.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)      470 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/layout/__init__.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     3458 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/confreader.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    12246 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/group.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    16066 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/config.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     7075 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/ipc.py
-drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2015-02-21 16:20:08.000000 qtile-0.9.0/libqtile/widget/
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     5242 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/mpris2widget.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     4412 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/keyboardlayout.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     1851 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/debuginfo.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)      963 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/currentlayout.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     1131 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/sep.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     5693 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/launchbar.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     2527 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/net.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)      925 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/wlan.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     2091 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/image.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     7183 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/tasklist.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     1133 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/canto.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     2496 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/maildir.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    12047 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/graph.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     1053 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/crashme.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)      893 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/windowname.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     3062 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/notify.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     1763 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/backlight.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     1861 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/pacman.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     6119 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/volume.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     5324 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/systray.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    12875 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/base.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    13023 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/prompt.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     2961 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/sensors.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     1135 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/countdown.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     1451 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/bitcoin_ticker.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     2449 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/imapwidget.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     1812 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/clock.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     4022 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/yahoo_weather.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     2487 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/df.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     1616 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/gmail_checker.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)      988 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/textbox.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)      991 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/she.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     9850 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/battery.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     9286 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/mpdwidget.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     7680 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/groupbox.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     1631 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/windowtabs.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)      564 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/spacer.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     2351 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/__init__.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     4876 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/mpriswidget.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     2988 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/widget/clipboard.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     7634 2015-02-08 15:39:59.000000 qtile-0.9.0/libqtile/widget/google_calendar.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     8719 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/pangocffi.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     2967 2015-02-01 04:36:23.000000 qtile-0.9.0/libqtile/configurable.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    12399 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/drawer.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    13439 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/command.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     9020 2015-02-01 04:36:23.000000 qtile-0.9.0/libqtile/bar.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     2237 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/log_utils.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     2906 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/notify.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    62328 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/xkeysyms.py
-drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2015-02-21 16:20:08.000000 qtile-0.9.0/libqtile/resources/
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     3246 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/resources/default_config.py
-drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2015-02-21 16:20:08.000000 qtile-0.9.0/libqtile/resources/__pycache__/
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     2259 2015-02-09 06:27:08.000000 qtile-0.9.0/libqtile/resources/__pycache__/default_config.cpython-34.pyc
--rw-r--r--   0 tycho     (1000) tycho     (1000)      140 2014-10-11 22:30:07.000000 qtile-0.9.0/libqtile/resources/__pycache__/__init__.cpython-34.pyc
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     2469 2015-02-12 01:20:29.000000 qtile-0.9.0/libqtile/resources/default_config.pyc
--rw-r--r--   0 tycho     (1000) tycho     (1000)      144 2014-03-11 15:58:08.000000 qtile-0.9.0/libqtile/resources/__init__.pyc
-drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2015-02-21 16:20:08.000000 qtile-0.9.0/libqtile/resources/battery-icons/
--rw-r--r--   0 tycho     (1000) tycho     (1000)      707 2014-01-10 20:09:17.000000 qtile-0.9.0/libqtile/resources/battery-icons/battery-full.png
--rw-r--r--   0 tycho     (1000) tycho     (1000)     1250 2014-01-10 20:09:17.000000 qtile-0.9.0/libqtile/resources/battery-icons/battery-full-charging.png
--rw-r--r--   0 tycho     (1000) tycho     (1000)     1315 2014-01-10 20:09:17.000000 qtile-0.9.0/libqtile/resources/battery-icons/battery-caution-charging.png
--rw-r--r--   0 tycho     (1000) tycho     (1000)      743 2014-01-10 20:09:17.000000 qtile-0.9.0/libqtile/resources/battery-icons/battery-empty.png
--rw-r--r--   0 tycho     (1000) tycho     (1000)      780 2014-01-10 20:09:17.000000 qtile-0.9.0/libqtile/resources/battery-icons/battery-low.png
--rw-r--r--   0 tycho     (1000) tycho     (1000)      882 2014-01-10 20:09:17.000000 qtile-0.9.0/libqtile/resources/battery-icons/battery-missing.png
--rw-r--r--   0 tycho     (1000) tycho     (1000)     1308 2014-01-10 20:09:17.000000 qtile-0.9.0/libqtile/resources/battery-icons/battery-low-charging.png
--rw-r--r--   0 tycho     (1000) tycho     (1000)     1283 2014-01-10 20:09:17.000000 qtile-0.9.0/libqtile/resources/battery-icons/battery-good-charging.png
--rw-r--r--   0 tycho     (1000) tycho     (1000)     1138 2014-01-10 20:09:17.000000 qtile-0.9.0/libqtile/resources/battery-icons/battery-caution.png
--rw-r--r--   0 tycho     (1000) tycho     (1000)     1077 2014-01-10 20:09:17.000000 qtile-0.9.0/libqtile/resources/battery-icons/battery-full-charged.png
--rw-r--r--   0 tycho     (1000) tycho     (1000)      762 2014-01-10 20:09:17.000000 qtile-0.9.0/libqtile/resources/battery-icons/battery-good.png
--rw-r--r--   0 tycho     (1000) tycho     (1000)        0 2014-01-10 20:09:17.000000 qtile-0.9.0/libqtile/resources/__init__.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    40737 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/window.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    57856 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/manager.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     6938 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/hook.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     6955 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/dgroups.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     8873 2015-02-01 04:36:23.000000 qtile-0.9.0/libqtile/sh.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    29379 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/xcbq.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)      702 2015-02-21 16:19:53.000000 qtile-0.9.0/libqtile/__init__.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     2415 2015-02-01 04:36:23.000000 qtile-0.9.0/libqtile/state.py
-drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2015-02-21 16:20:08.000000 qtile-0.9.0/qtile.egg-info/
--rw-rw-r--   0 tycho     (1000) tycho     (1000)       62 2015-02-21 16:20:08.000000 qtile-0.9.0/qtile.egg-info/requires.txt
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     1187 2015-02-21 16:20:08.000000 qtile-0.9.0/qtile.egg-info/PKG-INFO
--rw-rw-r--   0 tycho     (1000) tycho     (1000)        9 2015-02-21 16:20:08.000000 qtile-0.9.0/qtile.egg-info/top_level.txt
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     2977 2015-02-21 16:20:08.000000 qtile-0.9.0/qtile.egg-info/SOURCES.txt
--rw-rw-r--   0 tycho     (1000) tycho     (1000)        1 2015-02-21 16:20:08.000000 qtile-0.9.0/qtile.egg-info/dependency_links.txt
--rw-rw-r--   0 tycho     (1000) tycho     (1000)      127 2015-02-01 04:36:23.000000 qtile-0.9.0/MANIFEST.in
+drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2015-02-21 16:21:29.000000 qtile-0.9.1/
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     3606 2015-02-21 16:20:25.000000 qtile-0.9.1/setup.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)       59 2015-02-21 16:21:29.000000 qtile-0.9.1/setup.cfg
+drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2015-02-21 16:21:29.000000 qtile-0.9.1/bin/
+-rwxrwxr-x   0 tycho     (1000) tycho     (1000)     1856 2014-05-15 12:39:01.000000 qtile-0.9.1/bin/qtile-run
+-rwxrwxr-x   0 tycho     (1000) tycho     (1000)     2239 2015-02-01 04:36:23.000000 qtile-0.9.1/bin/qtile-session
+-rwxrwxr-x   0 tycho     (1000) tycho     (1000)     2213 2015-02-01 04:36:23.000000 qtile-0.9.1/bin/qsh
+-rwxrwxr-x   0 tycho     (1000) tycho     (1000)     4172 2015-02-21 16:20:25.000000 qtile-0.9.1/bin/qtile
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     1187 2015-02-21 16:21:29.000000 qtile-0.9.1/PKG-INFO
+-rw-r--r--   0 tycho     (1000) tycho     (1000)     1079 2014-01-10 20:09:17.000000 qtile-0.9.1/LICENSE
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     1916 2015-02-21 16:20:25.000000 qtile-0.9.1/README.rst
+drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2015-02-21 16:21:29.000000 qtile-0.9.1/libqtile/
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     4405 2015-02-01 04:36:23.000000 qtile-0.9.1/libqtile/utils.py
+drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2015-02-21 16:21:29.000000 qtile-0.9.1/libqtile/layout/
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    12663 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/layout/stack.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     7820 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/layout/tile.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    13320 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/layout/ratiotile.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    19534 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/layout/tree.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    10393 2015-02-08 15:39:59.000000 qtile-0.9.1/libqtile/layout/verticaltile.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     8714 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/layout/base.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     4949 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/layout/slice.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     7113 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/layout/matrix.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     4054 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/layout/max.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    27569 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/layout/xmonad.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     6621 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/layout/floating.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     5630 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/layout/zoomy.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     1630 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/layout/__init__.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     3436 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/confreader.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    13598 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/group.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    17398 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/config.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     7243 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/ipc.py
+drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2015-02-21 16:21:29.000000 qtile-0.9.1/libqtile/widget/
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     6437 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/mpris2widget.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     5603 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/keyboardlayout.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     3016 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/debuginfo.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2324 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/currentlayout.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2399 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/sep.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     9223 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/launchbar.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     3621 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/net.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2194 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/wlan.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     3239 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/image.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     8439 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/tasklist.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2393 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/canto.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     3722 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/maildir.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    13616 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/graph.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2304 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/crashme.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2187 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/windowname.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     4396 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/notify.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2959 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/backlight.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     1836 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/pacman.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     7726 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/volume.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     6723 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/systray.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    14763 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/base.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    14516 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/prompt.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     4108 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/sensors.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2318 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/countdown.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2532 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/bitcoin_ticker.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     3546 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/imapwidget.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     3007 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/clock.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     5080 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/yahoo_weather.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2909 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/df.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2813 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/gmail_checker.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2262 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/textbox.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2131 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/she.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    11292 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/battery.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2112 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/generic_poll_text.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    10772 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/mpdwidget.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     9181 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/groupbox.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2859 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/windowtabs.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     1864 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/spacer.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     3576 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/__init__.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     6115 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/mpriswidget.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     4171 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/widget/clipboard.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     7634 2015-02-08 15:39:59.000000 qtile-0.9.1/libqtile/widget/google_calendar.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     9916 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/pangocffi.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2967 2015-02-01 04:36:23.000000 qtile-0.9.1/libqtile/configurable.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    13262 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/drawer.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    13473 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/command.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     9020 2015-02-01 04:36:23.000000 qtile-0.9.1/libqtile/bar.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     3427 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/log_utils.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     4134 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/notify.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    63517 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/xkeysyms.py
+drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2015-02-21 16:21:29.000000 qtile-0.9.1/libqtile/resources/
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     4540 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/resources/default_config.py
+drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2015-02-21 16:21:29.000000 qtile-0.9.1/libqtile/resources/__pycache__/
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2259 2015-02-09 06:27:08.000000 qtile-0.9.1/libqtile/resources/__pycache__/default_config.cpython-34.pyc
+-rw-r--r--   0 tycho     (1000) tycho     (1000)      140 2014-10-11 22:30:07.000000 qtile-0.9.1/libqtile/resources/__pycache__/__init__.cpython-34.pyc
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2469 2015-02-12 01:20:29.000000 qtile-0.9.1/libqtile/resources/default_config.pyc
+-rw-r--r--   0 tycho     (1000) tycho     (1000)      144 2014-03-11 15:58:08.000000 qtile-0.9.1/libqtile/resources/__init__.pyc
+drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2015-02-21 16:21:29.000000 qtile-0.9.1/libqtile/resources/battery-icons/
+-rw-r--r--   0 tycho     (1000) tycho     (1000)      707 2014-01-10 20:09:17.000000 qtile-0.9.1/libqtile/resources/battery-icons/battery-full.png
+-rw-r--r--   0 tycho     (1000) tycho     (1000)     1250 2014-01-10 20:09:17.000000 qtile-0.9.1/libqtile/resources/battery-icons/battery-full-charging.png
+-rw-r--r--   0 tycho     (1000) tycho     (1000)     1315 2014-01-10 20:09:17.000000 qtile-0.9.1/libqtile/resources/battery-icons/battery-caution-charging.png
+-rw-r--r--   0 tycho     (1000) tycho     (1000)      743 2014-01-10 20:09:17.000000 qtile-0.9.1/libqtile/resources/battery-icons/battery-empty.png
+-rw-r--r--   0 tycho     (1000) tycho     (1000)      780 2014-01-10 20:09:17.000000 qtile-0.9.1/libqtile/resources/battery-icons/battery-low.png
+-rw-r--r--   0 tycho     (1000) tycho     (1000)      882 2014-01-10 20:09:17.000000 qtile-0.9.1/libqtile/resources/battery-icons/battery-missing.png
+-rw-r--r--   0 tycho     (1000) tycho     (1000)     1308 2014-01-10 20:09:17.000000 qtile-0.9.1/libqtile/resources/battery-icons/battery-low-charging.png
+-rw-r--r--   0 tycho     (1000) tycho     (1000)     1283 2014-01-10 20:09:17.000000 qtile-0.9.1/libqtile/resources/battery-icons/battery-good-charging.png
+-rw-r--r--   0 tycho     (1000) tycho     (1000)     1138 2014-01-10 20:09:17.000000 qtile-0.9.1/libqtile/resources/battery-icons/battery-caution.png
+-rw-r--r--   0 tycho     (1000) tycho     (1000)     1077 2014-01-10 20:09:17.000000 qtile-0.9.1/libqtile/resources/battery-icons/battery-full-charged.png
+-rw-r--r--   0 tycho     (1000) tycho     (1000)      762 2014-01-10 20:09:17.000000 qtile-0.9.1/libqtile/resources/battery-icons/battery-good.png
+-rw-r--r--   0 tycho     (1000) tycho     (1000)        0 2014-01-10 20:09:17.000000 qtile-0.9.1/libqtile/resources/__init__.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    40809 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/window.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    57994 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/manager.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     8443 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/hook.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     8292 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/dgroups.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     8873 2015-02-01 04:36:23.000000 qtile-0.9.1/libqtile/sh.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    31290 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/xcbq.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     1758 2015-02-21 16:20:25.000000 qtile-0.9.1/libqtile/__init__.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2415 2015-02-01 04:36:23.000000 qtile-0.9.1/libqtile/state.py
+drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2015-02-21 16:21:29.000000 qtile-0.9.1/qtile.egg-info/
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)       62 2015-02-21 16:21:29.000000 qtile-0.9.1/qtile.egg-info/requires.txt
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     1187 2015-02-21 16:21:29.000000 qtile-0.9.1/qtile.egg-info/PKG-INFO
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)        9 2015-02-21 16:21:29.000000 qtile-0.9.1/qtile.egg-info/top_level.txt
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     3014 2015-02-21 16:21:29.000000 qtile-0.9.1/qtile.egg-info/SOURCES.txt
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)        1 2015-02-21 16:21:29.000000 qtile-0.9.1/qtile.egg-info/dependency_links.txt
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)      127 2015-02-01 04:36:23.000000 qtile-0.9.1/MANIFEST.in
```

### Comparing `qtile-0.9.0/bin/qtile-run` & `qtile-0.9.1/bin/qtile-run`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/bin/qtile-session` & `qtile-0.9.1/bin/qtile-session`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/bin/qsh` & `qtile-0.9.1/bin/qsh`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/bin/qtile` & `qtile-0.9.1/bin/qtile`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,21 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 # Set the locale before any widgets or anything are imported, so any widget
 # whose defaults depend on a reasonable locale sees something reasonable.
 import locale
-locale.setlocale(locale.LC_ALL, locale.getdefaultlocale())
-
 import logging
+
 from libqtile.log_utils import init_log
 from libqtile import confreader
 
+locale.setlocale(locale.LC_ALL, locale.getdefaultlocale())
+
 try:
     import pkg_resources
     VERSION = pkg_resources.require("qtile")[0].version
 except (pkg_resources.DistributionNotFound, ImportError):
     VERSION = 'dev'
 
 def rename_process():
```

### Comparing `qtile-0.9.0/PKG-INFO` & `qtile-0.9.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: qtile
-Version: 0.9.0
+Version: 0.9.1
 Summary: A pure-Python tiling window manager.
 Home-page: http://qtile.org
 Author: Tycho Andersen
 Author-email: tycho@tycho.ws
 License: MIT
 Description: 
         A pure-Python tiling window manager.
```

### Comparing `qtile-0.9.0/LICENSE` & `qtile-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/README.rst` & `qtile-0.9.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   manipulate windows, update status bar widgets and more.
 * Qtile's remote scriptability makes it one of the most thoroughly
   unit-tested window managers around.
 
 Current Release
 ===============
 
-The current stable version of qtile is 0.9.0, released 2015-01-20. See the
+The current stable version of qtile is 0.9.1, released 2015-02-13. See the
 `documentation <http://docs.qtile.org/en/latest/manual/install/index.html>`_
 for installation instructions.
 
 Community
 =========
 
 Qtile is supported by a dedicated group of users. If you need any help, please
```

### Comparing `qtile-0.9.0/libqtile/utils.py` & `qtile-0.9.1/libqtile/utils.py`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/layout/stack.py` & `qtile-0.9.1/libqtile/layout/stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 from .base import Layout
 from .. import utils
 
 
 class _WinStack(object):
-    split = False
-    _current = 0
+    def __init__(self, autosplit=False):
+        self.split = autosplit
+        self._current = 0
+        self.lst = []
 
     @property
     def current(self):
         return self._current
 
     @current.setter
     def current(self, x):
@@ -38,17 +40,14 @@
 
     @property
     def cw(self):
         if not self.lst:
             return None
         return self.lst[self.current]
 
-    def __init__(self):
-        self.lst = []
-
     def toggleSplit(self):
         self.split = False if self.split else True
 
     def join(self, ws):
         # FIXME: This buggers up window order -
         # windows should be injected BEFORE
         # the current offset.
@@ -104,16 +103,16 @@
 
     def __getitem__(self, i):
         return self.lst[i]
 
     def __contains__(self, client):
         return client in self.lst
 
-    def __repr__(self):
-        return "_WinStack(%s, %s)" % (
+    def __str__(self):
+        return "_WinStack: %s, %s" % (
             self.current, str([i.name for i in self])
         )
 
     def info(self):
         return dict(
             clients=[x.name for x in self],
             split=self.split,
@@ -139,18 +138,15 @@
         ("fair", False, "Add new windows to the stacks in a round robin way."),
         ("margin", 0, "Margin of the layout"),
     ]
 
     def __init__(self, **config):
         Layout.__init__(self, **config)
         self.add_defaults(Stack.defaults)
-        self.stacks = [_WinStack() for i in range(self.num_stacks)]
-        for stack in self.stacks:
-            if self.autosplit:
-                stack.split = True
+        self.stacks = [_WinStack(autosplit=self.autosplit) for i in range(self.num_stacks)]
 
     @property
     def currentStack(self):
         return self.stacks[self.currentStackOffset]
 
     @property
     def currentStackOffset(self):
@@ -165,18 +161,15 @@
         for stack in self.stacks:
             client_list.extend(list(stack))
         return client_list
 
     def clone(self, group):
         c = Layout.clone(self, group)
         # These are mutable
-        c.stacks = [_WinStack() for i in self.stacks]
-        for stack in c.stacks:
-            if self.autosplit:
-                stack.split = True
+        c.stacks = [_WinStack(autosplit=self.autosplit) for i in self.stacks]
         return c
 
     def _findNext(self, lst, offset):
         for i in lst[offset + 1:]:
             if i:
                 return i
         else:
@@ -379,15 +372,15 @@
         """
         self.deleteCurrentStack()
 
     def cmd_add(self):
         """
             Add another stack to the layout.
         """
-        newstack = _WinStack()
+        newstack = _WinStack(autosplit=self.autosplit)
         if self.autosplit:
             newstack.split = True
         self.stacks.append(newstack)
         self.group.layoutAll()
 
     def cmd_rotate(self):
         """
```

### Comparing `qtile-0.9.0/libqtile/layout/tile.py` & `qtile-0.9.1/libqtile/layout/zoomy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,213 +1,171 @@
-from __future__ import division
-
-from .base import Layout
-from .. import utils
-
-
-class Tile(Layout):
+# Copyright (c) 2011 Mounier Florian
+# Copyright (c) 2011 Paul Colomiets
+# Copyright (c) 2012 Craig Barnes
+# Copyright (c) 2012, 2014 Tycho Andersen
+# Copyright (c) 2013 Tao Sauvage
+# Copyright (c) 2014 ramnes
+# Copyright (c) 2014 Sean Vig
+# Copyright (c) 2014 dmpayton
+# Copyright (c) 2014 dequis
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+from .base import SingleWindow
+
+
+class Zoomy(SingleWindow):
+    """
+        A layout with single active windows, and few other previews at the
+        right
+    """
     defaults = [
-        ("border_focus", "#0000ff", "Border colour for the focused window."),
-        ("border_normal", "#000000", "Border colour for un-focused winows."),
-        ("border_width", 1, "Border width."),
-        ("name", "tile", "Name of this layout."),
+        ("columnwidth", 150, "Width of the right column"),
+        ("property_name", "ZOOM", "Property to set on zoomed window"),
+        ("property_small", "0.1", "Property value to set on zoomed window"),
+        ("property_big", "1.0", "Property value to set on normal window"),
         ("margin", 0, "Margin of the layout"),
     ]
 
-    def __init__(self, ratio=0.618, masterWindows=1, expand=True,
-                 ratio_increment=0.05, add_on_top=True, shift_windows=False,
-                 master_match=None, **config):
-        Layout.__init__(self, **config)
-        self.add_defaults(Tile.defaults)
+    def __init__(self, **config):
+        SingleWindow.__init__(self, **config)
+        self.add_defaults(Zoomy.defaults)
         self.clients = []
-        self.ratio = ratio
-        self.master = masterWindows
         self.focused = None
-        self.expand = expand
-        self.ratio_increment = ratio_increment
-        self.add_on_top = add_on_top
-        self.shift_windows = shift_windows
-        self.master_match = master_match
-
-    @property
-    def master_windows(self):
-        return self.clients[:self.master]
-
-    @property
-    def slave_windows(self):
-        return self.clients[self.master:]
-
-    def up(self):
-        if self.shift_windows:
-            self.shift_up()
-        else:
-            self.shuffle(utils.shuffleUp)
-
-    def down(self):
-        if self.shift_windows:
-            self.shift_down()
-        else:
-            self.shuffle(utils.shuffleDown)
-
-    def shift_up(self):
-        if self.clients:
-            currentindex = self.clients.index(self.focused)
-            nextindex = (currentindex + 1) % len(self.clients)
-            self.shift(currentindex, nextindex)
 
-    def shift_down(self):
-        if self.clients:
-            currentindex = self.clients.index(self.focused)
-            previndex = (currentindex - 1) % len(self.clients)
-            self.shift(currentindex, previndex)
+    def _get_window(self):
+        return self.focused
 
     def focus_first(self):
         if self.clients:
             return self.clients[0]
 
+    def focus_last(self):
+        if self.clients:
+            return self.clients[len(self.clients) - 1]
+
     def focus_next(self, client):
         if client not in self.clients:
             return
         idx = self.clients.index(client)
         if len(self.clients) > idx + 1:
             return self.clients[idx + 1]
 
-    def focus_last(self):
-        if self.clients:
-            return self.clients[-1]
-
     def focus_previous(self, client):
-        if client not in self.clients:
+        if not self.clients:
             return
         idx = self.clients.index(client)
         if idx > 0:
             return self.clients[idx - 1]
 
-    def shuffle(self, function):
-        if self.clients:
-            function(self.clients)
-            self.group.layoutAll(True)
-
-    def resetMaster(self, match=None):
-        if not match and self.master_match:
-            match = self.master_match
-        else:
-            return
-        if self.clients:
-            masters = [c for c in self.clients if match.compare(c)]
-            self.clients = masters + [
-                c for c in self.clients if c not in masters
-            ]
-
-    def shift(self, idx1, idx2):
-        if self.clients:
-            self.clients[idx1], self.clients[idx2] = \
-                self.clients[idx2], self.clients[idx1]
-            self.group.layoutAll(True)
-
     def clone(self, group):
-        c = Layout.clone(self, group)
+        c = SingleWindow.clone(self, group)
         c.clients = []
         return c
 
-    def focus(self, client):
-        self.focused = client
-
-    def blur(self):
-        self.focused = None
-
     def add(self, client):
-        index = 0
-        if not self.add_on_top and self.clients and self.focused:
-            index = self.clients.index(self.focused)
-        self.clients.insert(index, client)
-        self.resetMaster()
+        self.clients.insert(0, client)
+        self.focus(client)
 
     def remove(self, client):
         if client not in self.clients:
             return
-
-        if self.focused is client:
-            self.focused = None
-
+        if self.focused == client:
+            self.cmd_previous()
         self.clients.remove(client)
-        if self.clients and client is self.focused:
-            self.focused = self.clients[0]
         return self.focused
 
     def configure(self, client, screen):
-        screenWidth = screen.width
-        screenHeight = screen.height
-        x = 0
-        y = 0
-        w = 0
-        h = 0
-        borderWidth = self.border_width
-        if self.clients and client in self.clients:
-            pos = self.clients.index(client)
-            if client in self.master_windows:
-                w = int(screenWidth * self.ratio) \
-                    if len(self.slave_windows) or not self.expand \
-                    else screenWidth
-                h = screenHeight // self.master
-                x = screen.x
-                y = screen.y + pos * h
-            else:
-                w = screenWidth - int(screenWidth * self.ratio)
-                h = screenHeight // (len(self.slave_windows))
-                x = screen.x + int(screenWidth * self.ratio)
-                y = screen.y + self.clients[self.master:].index(client) * h
-            if client is self.focused:
-                bc = self.group.qtile.colorPixel(self.border_focus)
-            else:
-                bc = self.group.qtile.colorPixel(self.border_normal)
+        left, right = screen.hsplit(screen.width - self.columnwidth)
+        if client is self.focused:
             client.place(
-                x,
-                y,
-                w - borderWidth * 2,
-                h - borderWidth * 2,
-                borderWidth,
-                bc,
+                left.x,
+                left.y,
+                left.width,
+                left.height,
+                0,
+                None,
                 margin=self.margin,
             )
-            client.unhide()
         else:
-            client.hide()
+            h = int(right.width * left.height / left.width)
+            client_index = self.clients.index(client)
+            focused_index = self.clients.index(self.focused)
+            offset = client_index - focused_index - 1
+            if offset < 0:
+                offset += len(self.clients)
+            if h * (len(self.clients) - 1) < right.height:
+                client.place(
+                    right.x,
+                    right.y + h * offset,
+                    right.width,
+                    h,
+                    0,
+                    None,
+                    margin=self.margin,
+                )
+            else:
+                hh = int((right.height - h) / (len(self.clients) - 1))
+                client.place(
+                    right.x,
+                    right.y + hh * offset,
+                    right.width,
+                    h,
+                    0,
+                    None,
+                    margin=self.margin,
+                )
+        client.unhide()
 
     def info(self):
-        return dict(
-            clients=[c.name for c in self.clients],
-            master=[c.name for c in self.master_windows],
-            slave=[c.name for c in self.slave_windows],
-        )
-
-    def cmd_down(self):
-        self.down()
-
-    def cmd_up(self):
-        self.up()
+        d = SingleWindow.info(self)
+        d["clients"] = [x.name for x in self.clients]
+        return d
+
+    def focus(self, win):
+        if self.focused and self.property_name and self.focused.window.get_property(
+            self.property_name,
+            "UTF8_STRING"
+        ) is not None:
+            self.focused.window.set_property(
+                self.property_name,
+                self.property_small,
+                "UTF8_STRING",
+                format=8
+            )
+        SingleWindow.focus(self, win)
+        if self.property_name:
+            self.focused = win
+            win.window.set_property(
+                self.property_name,
+                self.property_big,
+                "UTF8_STRING",
+                format=8
+            )
 
     def cmd_next(self):
         client = self.focus_next(self.focused) or self.focus_first()
         self.group.focus(client, False)
 
+    cmd_down = cmd_next
+
     def cmd_previous(self):
         client = self.focus_previous(self.focused) or self.focus_last()
         self.group.focus(client, False)
 
-    def cmd_decrease_ratio(self):
-        self.ratio -= self.ratio_increment
-        self.group.layoutAll()
-
-    def cmd_increase_ratio(self):
-        self.ratio += self.ratio_increment
-        self.group.layoutAll()
-
-    def cmd_decrease_nmaster(self):
-        self.master -= 1
-        if self.master <= 0:
-            self.master = 1
-        self.group.layoutAll()
-
-    def cmd_increase_nmaster(self):
-        self.master += 1
-        self.group.layoutAll()
+    cmd_up = cmd_previous
```

### Comparing `qtile-0.9.0/libqtile/layout/ratiotile.py` & `qtile-0.9.1/libqtile/layout/ratiotile.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+# -*- coding:utf-8 -*-
+# Copyright (c) 2011 Florian Mounier
+# Copyright (c) 2012-2013, 2015 Tycho Andersen
+# Copyright (c) 2013 Björn Lindström
+# Copyright (c) 2013 Tao Sauvage
+# Copyright (c) 2014 ramnes
+# Copyright (c) 2014 Sean Vig
+# Copyright (c) 2014 dmpayton
+# Copyright (c) 2014 dequis
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 from __future__ import division
 
 import math
 
 from .base import Layout
 from .. import utils
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qtile-0.9.0/libqtile/layout/tree.py` & `qtile-0.9.1/libqtile/layout/tree.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,38 @@
+# -*- coding:utf-8 -*-
+# Copyright (c) 2011 Mounier Florian
+# Copyright (c) 2011 Paul Colomiets
+# Copyright (c) 2012 roger
+# Copyright (c) 2012-2014 Tycho Andersen
+# Copyright (c) 2013 Tao Sauvage
+# Copyright (c) 2013 Arnas Udovicius
+# Copyright (c) 2014 ramnes
+# Copyright (c) 2014 Sean Vig
+# Copyright (c) 2014 Nathan Hoad
+# Copyright (c) 2014 dequis
+# Copyright (c) 2014 Thomas Sarboni
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 # -*- coding: utf-8 -*-
 from .base import SingleWindow
 from .. import drawer, hook, window
 
 import six
 
 to_superscript = dict(zip(map(ord, six.u('0123456789')), map(ord, six.u('⁰¹²³⁴⁵⁶⁷⁸⁹'))))
```

### Comparing `qtile-0.9.0/libqtile/layout/verticaltile.py` & `qtile-0.9.1/libqtile/layout/verticaltile.py`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/layout/base.py` & `qtile-0.9.1/libqtile/layout/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,7 +294,13 @@
 
         For ``cmd_``-methods that don't exist on the Delegate subclass, this
         looks for an implementation on the active layout.
         """
         if name.startswith('cmd_'):
             return getattr(self._get_active_layout(), name)
         return super(Delegate, self).__getattr__(name)
+
+    def info(self):
+        d = Layout.info(self)
+        for layout in self._get_layouts():
+            d[layout.name] = layout.info()
+        return d
```

### Comparing `qtile-0.9.0/libqtile/layout/max.py` & `qtile-0.9.1/libqtile/layout/max.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,23 +49,27 @@
     def focus_last(self):
         if self.clients:
             return self.clients[-1]
 
     def focus_next(self, window):
         if not self.clients:
             return
+        if window is None:
+            return
         if window != self._get_window():
             self.focus(window)
         idx = self.clients.index(window)
         if idx + 1 < len(self.clients):
             return self.clients[idx + 1]
 
     def focus_previous(self, window):
         if not self.clients:
             return
+        if window is None:
+            return
         if window != self._get_window():
             self.focus(window)
         idx = self.clients.index(window)
         if idx > 0:
             return self.clients[idx - 1]
 
     def up(self):
```

### Comparing `qtile-0.9.0/libqtile/layout/xmonad.py` & `qtile-0.9.1/libqtile/layout/xmonad.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,41 @@
+# -*- coding:utf-8 -*-
+# Copyright (c) 2011-2012 Dustin Lacewell
+# Copyright (c) 2011 Mounier Florian
+# Copyright (c) 2012 Craig Barnes
+# Copyright (c) 2012 Maximilian Köhl
+# Copyright (c) 2012, 2014-2015 Tycho Andersen
+# Copyright (c) 2013 jpic
+# Copyright (c) 2013 babadoo
+# Copyright (c) 2013 Jure Ham
+# Copyright (c) 2013 Tao Sauvage
+# Copyright (c) 2014 ramnes
+# Copyright (c) 2014 Sean Vig
+# Copyright (c) 2014 dmpayton
+# Copyright (c) 2014 dequis
+# Copyright (c) 2014 Florian Scherf
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 from .base import SingleWindow
 import math
 
 
 class MonadTall(SingleWindow):
     """
     This layout attempts to emulate the behavior of XMonad's default
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qtile-0.9.0/libqtile/confreader.py` & `qtile-0.9.1/libqtile/confreader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 # coding: utf-8
 #
 # Copyright (c) 2008, Aldo Cortesi <aldo@corte.si>
 # Copyright (c) 2011, Andrew Grigorev <andrew@ei-grad.ru>
 #
 # All rights reserved.
 #
```

### Comparing `qtile-0.9.0/libqtile/group.py` & `qtile-0.9.1/libqtile/group.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+# Copyright (c) 2012-2014 Tycho Andersen
+# Copyright (c) 2013 xarvh
+# Copyright (c) 2013 roger
+# Copyright (c) 2013 Tao Sauvage
+# Copyright (c) 2014 ramnes
+# Copyright (c) 2014 Sean Vig
+# Copyright (c) 2014 dequis
+# Copyright (c) 2015 Dario Giovannetti
+# Copyright (c) 2015 Alexander Lozovskoy
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 import contextlib
 import xcffib
 import xcffib.xproto
 
 from . import command
 from . import hook
 from . import window
@@ -319,20 +347,20 @@
 
     def prevGroup(self, skip_empty=False, skip_managed=False):
         return self._dirGroup(-1, skip_empty, skip_managed)
 
     def nextGroup(self, skip_empty=False, skip_managed=False):
         return self._dirGroup(1, skip_empty, skip_managed)
 
-    def cmd_unminimise_all(self):
+    def cmd_unminimize_all(self):
         """
             Unminimise all windows in this group.
         """
         for w in self.windows:
-            w.minimised = False
+            w.minimized = False
         self.layoutAll()
 
     def cmd_next_window(self):
         if not self.windows:
             return
         if self.currentWindow.floating:
             nxt = self.floating_layout.focus_next(self.currentWindow) or \
```

### Comparing `qtile-0.9.0/libqtile/config.py` & `qtile-0.9.1/libqtile/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+# Copyright (c) 2012-2015 Tycho Andersen
+# Copyright (c) 2013 xarvh
+# Copyright (c) 2013 horsik
+# Copyright (c) 2013-2014 roger
+# Copyright (c) 2013 Tao Sauvage
+# Copyright (c) 2014 ramnes
+# Copyright (c) 2014 Sean Vig
+# Copyright (c) 2014 Adi Sieker
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 from . import command
 from . import hook
 from . import utils
 from . import xcbq
 
 from six import MAXSIZE
 
@@ -439,15 +466,16 @@
         self._rules += [('wm_type', r) for r in wm_type]
         self._rules += [('wm_instance_class', w) for w in wm_instance_class]
         self._rules += [('net_wm_pid', w) for w in net_wm_pid]
 
     def compare(self, client):
         for _type, rule in self._rules:
             if _type == "net_wm_pid":
-                match_func = lambda value: rule == value
+                def match_func(value):
+                    return rule == value
             else:
                 match_func = getattr(rule, 'match', None) or \
                     getattr(rule, 'count')
 
             if _type == 'title':
                 value = client.name
             elif _type == 'wm_class':
```

### Comparing `qtile-0.9.0/libqtile/ipc.py` & `qtile-0.9.1/libqtile/ipc.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,19 @@
     def connection_made(self, transport):
         self.transport = transport
         self.recv = b''
         self.reply = asyncio.Future()
 
     def send(self, msg):
         self.transport.write(self._pack(msg))
-        self.transport.write_eof()
+        try:
+            self.transport.write_eof()
+        except AttributeError:
+            log = logging.getLogger('qtile')
+            log.exception('Swallowing AttributeError due to asyncio bug!')
 
     def data_received(self, data):
         self.recv += data
 
     def eof_received(self):
         # The server sends EOF when there is data ready to be processed
         try:
```

### Comparing `qtile-0.9.0/libqtile/widget/launchbar.py` & `qtile-0.9.1/libqtile/widget/mpriswidget.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,155 +1,179 @@
-"""
-This module define a widget that displays icons to launch softwares or commands
-when clicked -- a launchbar.
-Only png icon files are displayed, not xpm because cairo doesn't support
-loading of xpm file.
+# Copyright (c) 2011 Mounier Florian
+# Copyright (c) 2011, 2014 Tycho Andersen
+# Copyright (c) 2012-2013 Craig Barnes
+# Copyright (c) 2013 Tao Sauvage
+# Copyright (c) 2014 Sean Vig
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+import dbus
 
-To execute a software:
- - ('thunderbird', 'thunderbird -safe-mode', 'launch thunderbird in safe mode')
-To execute a python command in qtile, begin with by 'qsh:'
- - ('logout', 'qsh:self.qtile.cmd_shutdown()', 'logout from qtile')
+from dbus.mainloop.glib import DBusGMainLoop
 
+from . import base
+from .. import bar
 
-"""
 
-from libqtile import bar
-from libqtile.widget import base
-
-import os.path
-import cairocffi
-from xdg.IconTheme import getIconPath
-
-
-class LaunchBar(base._Widget):
+class Mpris(base._TextBox):
     """
-    A widget that display icons to launch the associated command
+    A widget which displays the current track/artist of your favorite MPRIS
+    player. It should work with all players which implement a reasonably
+    correct version of MPRIS, though I have only tested it with clementine.
     """
 
-    defaults = [
-        ('padding', 2, 'Padding between icons'),
-        ('default_icon', '/usr/share/icons/oxygen/256x256/mimetypes/'
-        'application-x-executable.png', 'Default icon not found'),
-    ]
+    def __init__(self, name="clementine", width=bar.CALCULATED,
+                 objname='org.mpris.clementine', **config):
+        base._TextBox.__init__(self, " ", width, **config)
+
+        self.dbus_loop = None
+
+        self.objname = objname
+        self.connected = False
+        self.name = name
+
+    def _configure(self, qtile, bar):
+        base._TextBox._configure(self, qtile, bar)
+
+        # we don't need to reconnect all the dbus stuff if we already
+        # connected it.
+        if self.dbus_loop is not None:
+            return
+
+        # we need a main loop to get event signals
+        # we just piggyback on qtile's main loop
+        self.dbus_loop = DBusGMainLoop()
+        self.bus = dbus.SessionBus(mainloop=self.dbus_loop)
+
+        # watch for our player to start up
+        deebus = self.bus.get_object(
+            'org.freedesktop.DBus',
+            '/org/freedesktop/DBus'
+        )
+        deebus.connect_to_signal(
+            "NameOwnerChanged",
+            self.handle_name_owner_change
+        )
+
+        # try to connect for grins
+        self._connect()
+
+    def _connect(self):
+        """ Try to connect to the player if it exists. """
+        try:
+            self.player = self.bus.get_object(self.objname, '/Player')
+            self.iface = dbus.Interface(
+                self.player,
+                dbus_interface='org.freedesktop.MediaPlayer'
+            )
+            # See: http://xmms2.org/wiki/MPRIS for info on signals
+            # and what they mean.
+            self.iface.connect_to_signal(
+                "TrackChange",
+                self.handle_track_change
+            )
+            self.iface.connect_to_signal(
+                "StatusChange",
+                self.handle_status_change
+            )
+            self.connected = True
+        except dbus.exceptions.DBusException:
+            self.qtile.log.exception("exception initalizing mpris")
+            self.connected = False
+
+    def handle_track_change(self, metadata):
+        self.update()
+
+    def handle_status_change(self, *args):
+        self.update()
+
+    def handle_name_owner_change(self, name, old_owner, new_owner):
+        if name == self.objname:
+            if old_owner == '':
+                # Our player started, so connect to it
+                self._connect()
+            elif new_owner == '':
+                # It disconnected :-(
+                self.connected = False
+            self.update()
 
-    def __init__(self, progs=None, width=bar.CALCULATED, **config):
-        """
-        @progs: a list of tuple (software_name, command_to_execute, comment)
-        for example:
-        ('thunderbird', 'thunderbird -safe-mode', 'launch thunderbird in safe\
-        mode')
-        ('logout', 'qsh:self.qtile.cmd_shutdown()', 'logout from qtile')
+    def ensure_connected(f):
         """
-        base._Widget.__init__(self, width, *config)
-        if progs is None:
-            progs = []
-        self.add_defaults(LaunchBar.defaults)
-        self.surfaces = {}
-        self.icons_files = {}
-        self.icons_widths = {}
-        self.icons_offsets = {}
-        # For now, ignore the comments but may be one day it will be useful
-        self.commands = dict((prg[0], prg[1]) for prg in progs)
-
-    def _configure(self, qtile, pbar):
-        base._Widget._configure(self, qtile, pbar)
-        self.lookup_icons()
-        self.setup_images()
-        self.width = self.calculate_width()
-
-    def setup_images(self):
-        """ Create image structures for each icon files. """
-        for img_name, iconfile in self.icons_files.items():
+        Tries to connect to the player. It *should* be succesful if the player
+        is alive. """
+        def wrapper(*args, **kwargs):
+            self = args[0]
             try:
-                img = cairocffi.ImageSurface.create_from_png(iconfile)
-            except cairocffi.Error:
-                self.qtile.log.exception('No icon found for application ' +
-                                         img_name + '(' + iconfile + ')')
-                return
-
-            input_width = img.get_width()
-            input_height = img.get_height()
-
-            sp = input_height / float(self.bar.height - 4)
-
-            width = input_width / sp
-            if width > self.width:
-                self.width = int(width) + self.padding * 2
-
-            imgpat = cairocffi.SurfacePattern(img)
-
-            scaler = cairocffi.Matrix()
-
-            scaler.scale(sp, sp)
-            scaler.translate(self.padding * -1, -2)
-            imgpat.set_matrix(scaler)
-
-            imgpat.set_filter(cairocffi.FILTER_BEST)
-            self.surfaces[img_name] = imgpat
-            self.icons_widths[img_name] = width
-
-    def _lookup_icon(self, name):
-        """ Search for the icon corresponding to one command. """
-
-        # if the software_name is directly an abslolute path icon file
-        if os.path.isabs(name):
-            # name start with '/' thus it's an absolute path
-            root, ext = os.path.splitext(name)
-            if ext == '.png':
-                self.icons_files[name] = name if os.path.isfile(name) else None
-            else:
-                # try to add the extension
-                self.icons_files[name] = name + '.png' if os.path.isfile(name +
-                                                '.png') else None
+                self.iface.GetMetadata()
+            except (dbus.exceptions.DBusException, AttributeError):
+                # except AttributeError because
+                # self.iface won't exist if we haven't
+                # _connect()ed yet
+                self._connect()
+            return f(*args, **kwargs)
+        return wrapper
+
+    @ensure_connected
+    def update(self):
+        self.qtile.call_soon_threadsafe(self.real_update)
+
+    @ensure_connected
+    def real_update(self):
+        if not self.configured:
+            playing = 'Not configured'
+        if not self.connected:
+            playing = 'Not Connected'
+        elif not self.is_playing():
+            playing = 'Stopped'
+        else:
+            try:
+                metadata = self.iface.GetMetadata()
+
+                # TODO: Make this configurable?
+                playing = metadata["title"] + ' - ' + metadata["artist"]
+            except dbus.exceptions.DBusException:
+                self.connected = False
+                playing = ''
+
+        if playing != self.text:
+            self.text = playing
+            self.bar.draw()
+
+    @ensure_connected
+    def is_playing(self):
+        """ Returns true if we are connected to the player and it is playing
+        something, false otherwise. """
+        if self.connected:
+            (playing, random, repeat, stop_after_last) = self.iface.GetStatus()
+            return playing == 0
         else:
-            self.icons_files[name] = getIconPath(name)
+            return False
 
-        if self.icons_files[name] is None:
-            self.icons_files[name] = self.default_icon
+    def cmd_info(self):
+        """ What's the current state of the widget? """
+        return dict(
+            connected=self.connected,
+            nowplaying=self.text,
+            isplaying=self.is_playing(),
+        )
+
+    def cmd_update(self):
+        """ Force the widget to update. Mostly used for testing. """
+        self.update()
 
-    def lookup_icons(self):
-        """ Search for the icons corresponding to the commands to execute. """
-        if not os.path.isfile(self.default_icon):
-            self.default_icon = None
-        for name in self.commands:
-            self._lookup_icon(name)
-
-    def get_icon_in_position(self, x, y):
-        """ Retreive the wich icon is clicked according to its position. """
-        for i in self.commands:
-            if x < self.icons_offsets[i] + self.icons_widths[i] + self.padding\
-               / 2:
-                return i
-
-    def button_press(self, x, y, button):
-        """ Launch the associated command to the clicked icon. """
-        if button == 1:
-            icon = self.get_icon_in_position(x, y)
-            if icon:
-                cmd = self.commands[icon]
-                if cmd.startswith('qsh:'):
-                    eval(cmd[4:])
-                else:
-                    self.qtile.cmd_spawn(cmd)
-            self.draw()
-
-    def draw(self):
-        """ Draw the icons in the widget. """
-        width = self.calculate_width()
-        self.width = width
-        self.drawer.clear(self.background or self.bar.background)
-        xoffset = 0
-        for i in self.commands:
-            self.icons_offsets[i] = xoffset + self.padding
-            self.drawer.ctx.move_to(self.offset + xoffset,
-                                    self.icons_widths[i])
-            self.drawer.clear(self.background or self.bar.background)
-            self.drawer.ctx.set_source(self.surfaces[i])
-            self.drawer.ctx.paint()
-            self.drawer.draw(self.offset + xoffset,
-                             self.icons_widths[i] + self.padding)
-            xoffset += self.icons_widths[i] + self.padding
-
-    def calculate_width(self):
-        """ Compute the width of the widget according to each icon width. """
-        return sum(self.icons_widths.values()) + self.padding * (
-            len(self.icons_files.values()) + 1)
+# vim: tabstop=4 shiftwidth=4 expandtab
```

### Comparing `qtile-0.9.0/libqtile/widget/graph.py` & `qtile-0.9.1/libqtile/drawer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,386 +1,391 @@
+# Copyright (c) 2010 Aldo Cortesi
+# Copyright (c) 2011 Florian Mounier
+# Copyright (c) 2011 oitel
+# Copyright (c) 2011 Kenji_Takahashi
+# Copyright (c) 2011 Paul Colomiets
+# Copyright (c) 2012, 2014 roger
+# Copyright (c) 2012 nullzion
+# Copyright (c) 2013 Tao Sauvage
+# Copyright (c) 2014-2015 Sean Vig
+# Copyright (c) 2014 Nathan Hoad
+# Copyright (c) 2014 dequis
+# Copyright (c) 2014 Tycho Andersen
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+import collections
+import math
 import cairocffi
+import xcffib.xproto
 
-from . import base
-from os import statvfs
-import time
-
-__all__ = [
-    'CPUGraph',
-    'MemoryGraph',
-    'SwapGraph',
-    'NetGraph',
-    'HDDGraph',
-    'HDDBusyGraph',
-]
-
-
-class _Graph(base._Widget):
-    fixed_upper_bound = False
-    defaults = [
-        ("graph_color", "18BAEB", "Graph color"),
-        ("fill_color", "1667EB.3", "Fill color for linefill graph"),
-        ("border_color", "215578", "Widget border color"),
-        ("border_width", 2, "Widget border width"),
-        ("margin_x", 3, "Margin X"),
-        ("margin_y", 3, "Margin Y"),
-        ("samples", 100, "Count of graph samples."),
-        ("frequency", 1, "Update frequency in seconds"),
-        ("type", "linefill", "'box', 'line', 'linefill'"),
-        ("line_width", 3, "Line width"),
-        ("start_pos", "bottom", "Drawer starting position ('bottom'/'top')"),
-    ]
-
-    def __init__(self, width=100, **config):
-        base._Widget.__init__(self, width, **config)
-        self.add_defaults(_Graph.defaults)
-        self.values = [0] * self.samples
-        self.maxvalue = 0
-        self.oldtime = time.time()
-        self.lag_cycles = 0
+from . import pangocffi
+from . import utils
 
-    def timer_setup(self):
-        self.timeout_add(self.frequency, self.update)
 
-    @property
-    def graphwidth(self):
-        return self.width - self.border_width * 2 - self.margin_x * 2
+class TextLayout(object):
+    def __init__(self, drawer, text, colour, font_family, font_size,
+                 font_shadow, wrap=True, markup=False):
+        self.drawer, self.colour = drawer, colour
+        layout = drawer.ctx.create_layout()
+        layout.set_alignment(pangocffi.ALIGN_CENTER)
+        if not wrap:  # pango wraps by default
+            layout.set_ellipsize(pangocffi.ELLIPSIZE_END)
+        desc = pangocffi.FontDescription()
+        desc.set_family(font_family)
+        desc.set_absolute_size(pangocffi.units_from_double(font_size))
+        layout.set_font_description(desc)
+        self.font_shadow = font_shadow
+        self.layout = layout
+        self.markup = markup
+        self.text = text
+        self._width = None
 
     @property
-    def graphheight(self):
-        return self.bar.height - self.margin_y * 2 - self.border_width * 2
-
-    def draw_box(self, x, y, values):
-        step = self.graphwidth / float(self.samples)
-        self.drawer.set_source_rgb(self.graph_color)
-        for val in values:
-            val = self.val(val)
-            self.drawer.fillrect(x, y - val, step, val)
-            x += step
-
-    def draw_line(self, x, y, values):
-        step = self.graphwidth / float(self.samples - 1)
-        self.drawer.ctx.set_line_join(cairocffi.LINE_JOIN_ROUND)
-        self.drawer.set_source_rgb(self.graph_color)
-        self.drawer.ctx.set_line_width(self.line_width)
-        for val in values:
-            self.drawer.ctx.line_to(x, y - self.val(val))
-            x += step
-        self.drawer.ctx.stroke()
+    def text(self):
+        return self.layout.get_text()
 
-    def draw_linefill(self, x, y, values):
-        step = self.graphwidth / float(self.samples - 2)
-        self.drawer.ctx.set_line_join(cairocffi.LINE_JOIN_ROUND)
-        self.drawer.set_source_rgb(self.graph_color)
-        self.drawer.ctx.set_line_width(self.line_width)
-        for index, val in enumerate(values):
-            self.drawer.ctx.line_to(x + index * step, y - self.val(val))
-        self.drawer.ctx.stroke_preserve()
-        self.drawer.ctx.line_to(
-            x + (len(values) - 1) * step,
-            y - 1 + self.line_width / 2.0
-        )
-        self.drawer.ctx.line_to(x, y - 1 + self.line_width / 2.0)
-        self.drawer.set_source_rgb(self.fill_color)
-        self.drawer.ctx.fill()
-
-    def val(self, val):
-        if self.start_pos == 'bottom':
-            return val
-        elif self.start_pos == 'top':
-            return -val
-        else:
-            raise ValueError("Unknown starting position: %s." % self.start_pos)
+    @text.setter
+    def text(self, value):
+        if self.markup:
+            # pangocffi doesn't like None here, so we use "".
+            if value is None:
+                value = ''
+            attrlist, value, accel_char = pangocffi.parse_markup(value)
+            self.layout.set_attributes(attrlist)
+        return self.layout.set_text(utils.scrub_to_utf8(value))
 
-    def draw(self):
-        self.drawer.clear(self.background or self.bar.background)
-        if self.border_width:
-            self.drawer.set_source_rgb(self.border_color)
-            self.drawer.ctx.set_line_width(self.border_width)
-            self.drawer.ctx.rectangle(
-                self.margin_x + self.border_width / 2.0,
-                self.margin_y + self.border_width / 2.0,
-                self.graphwidth + self.border_width,
-                self.bar.height - self.margin_y * 2 - self.border_width,
-            )
-            self.drawer.ctx.stroke()
-        x = self.margin_x + self.border_width
-        y = self.margin_y + self.border_width
-        if self.start_pos == 'bottom':
-            y += self.graphheight
-        elif not self.start_pos == 'top':
-            raise ValueError("Unknown starting position: %s." % self.start_pos)
-        k = 1.0 / (self.maxvalue or 1)
-        scaled = [self.graphheight * val * k for val in reversed(self.values)]
-
-        if self.type == "box":
-            self.draw_box(x, y, scaled)
-        elif self.type == "line":
-            self.draw_line(x, y, scaled)
-        elif self.type == "linefill":
-            self.draw_linefill(x, y, scaled)
+    @property
+    def width(self):
+        if self._width is not None:
+            return self._width
         else:
-            raise ValueError("Unknown graph type: %s." % self.type)
-
-        self.drawer.draw(self.offset, self.width)
-
-    def push(self, value):
-        if self.lag_cycles > self.samples:
-            # compensate lag by sending the same value up to
-            # the graph samples limit
-            self.lag_cycles = 1
-
-        self.values = ([value] * min(self.samples, self.lag_cycles)) + self.values
-        self.values = self.values[:self.samples]
-
-        if not self.fixed_upper_bound:
-            self.maxvalue = max(self.values)
-        self.draw()
+            return self.layout.get_pixel_size()[0]
 
-    def update(self):
-        # lag detection
-        newtime = time.time()
-        self.lag_cycles = int((newtime - self.oldtime) / self.frequency)
-        self.oldtime = newtime
+    @width.setter
+    def width(self, value):
+        self._width = value
+        self.layout.set_width(pangocffi.units_from_double(value))
+
+    @width.deleter
+    def width(self):
+        self._width = None
+        self.layout.set_width(-1)
 
-        self.update_graph()
-        self.timeout_add(self.frequency, self.update)
+    @property
+    def height(self):
+        return self.layout.get_pixel_size()[1]
 
-    def fullfill(self, value):
-        self.values = [value] * len(self.values)
+    def fontdescription(self):
+        return self.layout.get_font_description()
 
+    @property
+    def font_family(self):
+        d = self.fontdescription()
+        return d.get_family()
+
+    @font_family.setter
+    def font_family(self, font):
+        d = self.fontdescription()
+        d.set_family(font)
+        self.layout.set_font_description(d)
 
-class CPUGraph(_Graph):
-    """
-        Display CPU usage graph.
-    """
-    defaults = [
-        ("core", "all", "Which core to show (all/0/1/2/...)"),
-    ]
-
-    fixed_upper_bound = True
-
-    def __init__(self, **config):
-        _Graph.__init__(self, **config)
-        self.add_defaults(CPUGraph.defaults)
-        self.maxvalue = 100
-        self.oldvalues = self._getvalues()
-
-    def _getvalues(self):
-        with open('/proc/stat') as file:
-            lines = file.readlines()
-
-            # default to all cores (first line)
-            line = lines.pop(0)
-
-            # core specified, grab the corresponding line
-            if isinstance(self.core, int):
-                # we already removed the first line from the list,
-                # so it's 0 indexed now :D
-                line = lines[self.core]
-
-                if not line.startswith("cpu%s" % self.core):
-                    raise ValueError("No such core: %s" % self.core)
-
-            name, user, nice, sys, idle, iowait, tail = line.split(None, 6)
-
-            return (int(user), int(nice), int(sys), int(idle))
-
-    def update_graph(self):
-        nval = self._getvalues()
-        oval = self.oldvalues
-        busy = nval[0] + nval[1] + nval[2] - oval[0] - oval[1] - oval[2]
-        total = busy + nval[3] - oval[3]
-        # sometimes this value is zero for unknown reason (time shift?)
-        # we just sent the previous value, because it gives us no info about
-        # cpu load, if it's zero.
-
-        if total:
-            push_value = busy * 100.0 / total
-            self.push(push_value)
+    @property
+    def font_size(self):
+        d = self.fontdescription()
+        return d.get_size()
+
+    @font_size.setter
+    def font_size(self, size):
+        d = self.fontdescription()
+        d.set_size(size)
+        d.set_absolute_size(pangocffi.units_from_double(size))
+        self.layout.set_font_description(d)
+
+    def draw(self, x, y):
+        if self.font_shadow is not None:
+            self.drawer.set_source_rgb(self.font_shadow)
+            self.drawer.ctx.move_to(x + 1, y + 1)
+            self.drawer.ctx.show_layout(self.layout)
+
+        self.drawer.set_source_rgb(self.colour)
+        self.drawer.ctx.move_to(x, y)
+        self.drawer.ctx.show_layout(self.layout)
+
+    def framed(self, border_width, border_color, pad_x, pad_y):
+        return TextFrame(self, border_width, border_color, pad_x, pad_y)
+
+
+class TextFrame:
+    def __init__(self, layout, border_width, border_color, pad_x, pad_y):
+        self.layout = layout
+        self.border_width = border_width
+        self.border_color = border_color
+        self.drawer = self.layout.drawer
+
+        if isinstance(pad_x, collections.Iterable):
+            self.pad_left = pad_x[0]
+            self.pad_right = pad_x[1]
         else:
-            self.push(self.values[0])
-        self.oldvalues = nval
-
+            self.pad_left = self.pad_right = pad_x
 
-def get_meminfo():
-    with open('/proc/meminfo') as file:
-        val = {}
-        for line in file:
-            key, tail = line.split(':')
-            uv = tail.split()
-            val[key] = int(uv[0])
-    return val
-
-
-class MemoryGraph(_Graph):
-    """
-        Displays a memory usage graph.
-    """
-    fixed_upper_bound = True
+        if isinstance(pad_y, collections.Iterable):
+            self.pad_top = pad_y[0]
+            self.pad_bottom = pad_y[1]
+        else:
+            self.pad_top = self.pad_bottom = pad_y
 
-    def __init__(self, **config):
-        _Graph.__init__(self, **config)
-        val = self._getvalues()
-        self.maxvalue = val['MemTotal']
-
-        mem = val['MemTotal'] - val['MemFree'] - val['Buffers'] - val['Cached']
-        self.fullfill(mem)
-
-    def _getvalues(self):
-        return get_meminfo()
-
-    def update_graph(self):
-        val = self._getvalues()
-        self.push(
-            val['MemTotal'] - val['MemFree'] - val['Buffers'] - val['Cached']
+    def draw(self, x, y, rounded=True, fill=False):
+        self.drawer.set_source_rgb(self.border_color)
+        opts = [
+            x, y,
+            self.layout.width + self.pad_left + self.pad_right,
+            self.layout.height + self.pad_top + self.pad_bottom,
+            self.border_width
+        ]
+        if fill:
+            if rounded:
+                self.drawer.rounded_fillrect(*opts)
+            else:
+                self.drawer.fillrect(*opts)
+        else:
+            if rounded:
+                self.drawer.rounded_rectangle(*opts)
+            else:
+                self.drawer.rectangle(*opts)
+        self.drawer.ctx.stroke()
+        self.layout.draw(
+            x + self.pad_left,
+            y + self.pad_top
         )
 
+    def draw_fill(self, x, y, rounded=True):
+        self.draw(x, y, rounded, fill=True)
 
-class SwapGraph(_Graph):
-    """
-        Display a swap info graph.
-    """
-    fixed_upper_bound = True
-
-    def __init__(self, **config):
-        _Graph.__init__(self, **config)
-        val = self._getvalues()
-        self.maxvalue = val['SwapTotal']
-        swap = val['SwapTotal'] - val['SwapFree'] - val.get('SwapCached', 0)
-        self.fullfill(swap)
-
-    def _getvalues(self):
-        return get_meminfo()
-
-    def update_graph(self):
-        val = self._getvalues()
-
-        swap = val['SwapTotal'] - val['SwapFree'] - val.get('SwapCached', 0)
+    @property
+    def height(self):
+        return self.layout.height + self.pad_top + self.pad_bottom
 
-        # can change, swapon/off
-        if self.maxvalue != val['SwapTotal']:
-            self.maxvalue = val['SwapTotal']
-            self.fullfill(swap)
-        self.push(swap)
+    @property
+    def width(self):
+        return self.layout.width + self.pad_left + self.pad_right
 
 
-class NetGraph(_Graph):
-    """
-        Display a network usage graph.
+class Drawer:
     """
-    defaults = [
-        (
-            "interface",
-            "auto",
-            "Interface to display info for ('auto' for detection)"
-        ),
-        ("bandwidth_type", "down", "down(load)/up(load)"),
-    ]
-
-    def __init__(self, **config):
-        _Graph.__init__(self, **config)
-        self.add_defaults(NetGraph.defaults)
-        if self.interface == "auto":
-            try:
-                self.interface = self.get_main_iface()
-            except RuntimeError:
-                self.log.warning(
-                    "NetGraph - Automatic interface detection failed, "
-                    "falling back to 'eth0'"
-                )
-                self.interface = "eth0"
-        self.filename = '/sys/class/net/{interface}/statistics/{type}'.format(
-            interface=self.interface,
-            type=self.bandwidth_type == 'down' and 'rx_bytes' or 'tx_bytes'
-        )
-        self.bytes = 0
-        self.bytes = self._getValues()
-
-    def _getValues(self):
-        try:
-            with open(self.filename) as file:
-                val = int(file.read())
-                rval = val - self.bytes
-                self.bytes = val
-                return rval
-        except IOError:
-            return 0
-
-    def update_graph(self):
-        val = self._getValues()
-        self.push(val)
-
-    @staticmethod
-    def get_main_iface():
-        filename = "/proc/net/route"
-        make_route = lambda line: dict(zip(['iface', 'dest'], line.split()))
-        routes = [make_route(line) for line in list(open(filename))[1:]]
-        try:
-            return next(
-                (r for r in routes if not int(r['dest'], 16)),
-                routes[0]
-            )['iface']
-        except (KeyError, IndexError, ValueError):
-            raise RuntimeError('No valid interfaces available')
-
+        A helper class for drawing and text layout.
 
-class HDDGraph(_Graph):
+        We have a drawer object for each widget in the bar. The underlying
+        surface is a pixmap with the same size as the bar itself. We draw to
+        the pixmap starting at offset 0, 0, and when the time comes to display
+        to the window, we copy the appropriate portion of the pixmap onto the
+        window.
     """
-        Display HDD free or used space graph.
-    """
-    fixed_upper_bound = True
-    defaults = [
-        ("path", "/", "Partition mount point."),
-        ("space_type", "used", "free/used")
-    ]
-
-    def __init__(self, **config):
-        _Graph.__init__(self, **config)
-        self.add_defaults(HDDGraph.defaults)
-        stats = statvfs(self.path)
-        self.maxvalue = stats.f_blocks * stats.f_frsize
-        values = self._getValues()
-        self.fullfill(values)
-
-    def _getValues(self):
-        stats = statvfs(self.path)
-        if self.space_type == 'used':
-            return (stats.f_blocks - stats.f_bfree) * stats.f_frsize
-        else:
-            return stats.f_bavail * stats.f_frsize
+    def __init__(self, qtile, wid, width, height):
+        self.qtile = qtile
+        self.wid, self.width, self.height = wid, width, height
 
-    def update_graph(self):
-        val = self._getValues()
-        self.push(val)
+        self.pixmap = self.qtile.conn.conn.generate_id()
+        self.gc = self.qtile.conn.conn.generate_id()
 
+        self.qtile.conn.conn.core.CreatePixmap(
+            self.qtile.conn.default_screen.root_depth,
+            self.pixmap,
+            self.wid,
+            self.width,
+            self.height
+        )
+        self.qtile.conn.conn.core.CreateGC(
+            self.gc,
+            self.wid,
+            xcffib.xproto.GC.Foreground | xcffib.xproto.GC.Background,
+            [
+                self.qtile.conn.default_screen.black_pixel,
+                self.qtile.conn.default_screen.white_pixel
+            ]
+        )
+        self.surface = cairocffi.XCBSurface(
+            qtile.conn.conn,
+            self.pixmap,
+            self.find_root_visual(),
+            self.width,
+            self.height,
+        )
+        self.ctx = self.new_ctx()
+        self.clear((0, 0, 1))
 
-class HDDBusyGraph(_Graph):
-    """
-        Parses /sys/block/<dev>/stat file and extracts overall device
-        IO usage, based on ``io_ticks``'s value.
-        See https://www.kernel.org/doc/Documentation/block/stat.txt
-    """
-    defaults = [
-        ("device", "sda", "Block device to display info for")
-    ]
-
-    def __init__(self, **config):
-        _Graph.__init__(self, **config)
-        self.add_defaults(HDDBusyGraph.defaults)
-        self.path = '/sys/block/{dev}/stat'.format(
-            dev=self.device
+    def __del__(self):
+        self.qtile.conn.conn.core.FreeGC(self.gc)
+        self.qtile.conn.conn.core.FreePixmap(self.pixmap)
+
+    def _rounded_rect(self, x, y, width, height, linewidth):
+        aspect = 1.0
+        corner_radius = height / 10.0
+        radius = corner_radius / aspect
+        degrees = math.pi / 180.0
+
+        self.ctx.new_sub_path()
+
+        delta = radius + linewidth / 2
+        self.ctx.arc(x + width - delta, y + delta, radius,
+                     -90 * degrees, 0 * degrees)
+        self.ctx.arc(x + width - delta, y + height - delta,
+                     radius, 0 * degrees, 90 * degrees)
+        self.ctx.arc(x + delta, y + height - delta, radius,
+                     90 * degrees, 180 * degrees)
+        self.ctx.arc(x + delta, y + delta, radius,
+                     180 * degrees, 270 * degrees)
+        self.ctx.close_path()
+
+    def rounded_rectangle(self, x, y, width, height, linewidth):
+        self._rounded_rect(x, y, width, height, linewidth)
+        self.ctx.set_line_width(linewidth)
+        self.ctx.stroke()
+
+    def rounded_fillrect(self, x, y, width, height, linewidth):
+        self._rounded_rect(x, y, width, height, linewidth)
+        self.ctx.fill()
+
+    def rectangle(self, x, y, width, height, linewidth=2):
+        self.ctx.set_line_width(linewidth)
+        self.ctx.rectangle(x, y, width, height)
+        self.ctx.stroke()
+
+    def fillrect(self, x, y, width, height, linewidth=2):
+        self.ctx.set_line_width(linewidth)
+        self.ctx.rectangle(x, y, width, height)
+        self.ctx.fill()
+        self.ctx.stroke()
+
+    def draw(self, offset, width):
+        """
+            offset: the X offset to start drawing at.
+            width: the portion of the canvas to draw at the starting point.
+        """
+        self.qtile.conn.conn.core.CopyArea(
+            self.pixmap,
+            self.wid,
+            self.gc,
+            0, 0,  # srcx, srcy
+            offset, 0,  # dstx, dsty
+            width, self.height
         )
-        self._prev = 0
 
-    def _getActivity(self):
-        try:
-            # io_ticks is field number 9
-            io_ticks = int(open(self.path).read().split()[9])
-        except IOError:
-            return 0
-        activity = io_ticks - self._prev
-        self._prev = io_ticks
-        return activity
+    def find_root_visual(self):
+        for i in self.qtile.conn.default_screen.allowed_depths:
+            for v in i.visuals:
+                if v.visual_id == self.qtile.conn.default_screen.root_visual:
+                    return v
+
+    def new_ctx(self):
+        return pangocffi.CairoContext(cairocffi.Context(self.surface))
+
+    def set_source_rgb(self, colour):
+        if type(colour) == list:
+            linear = cairocffi.LinearGradient(0.0, 0.0, 0.0, self.height)
+            step_size = 1.0 / (len(colour) - 1)
+            step = 0.0
+            for c in colour:
+                rgb_col = utils.rgb(c)
+                if len(rgb_col) < 4:
+                    rgb_col[3] = 1
+                linear.add_color_stop_rgba(step, *rgb_col)
+                step += step_size
+            self.ctx.set_source(linear)
+        else:
+            self.ctx.set_source_rgba(*utils.rgb(colour))
 
-    def update_graph(self):
-        self.push(self._getActivity())
+    def clear(self, colour):
+        self.set_source_rgb(colour)
+        self.ctx.rectangle(0, 0, self.width, self.height)
+        self.ctx.fill()
+        self.ctx.stroke()
+
+    def textlayout(self, text, colour, font_family, font_size, font_shadow,
+                   markup=False, **kw):
+        """
+            Get a text layout.
+        """
+        return TextLayout(self, text, colour, font_family, font_size,
+                          font_shadow, markup=markup, **kw)
+
+    def max_layout_size(self, texts, font_family, font_size):
+        sizelayout = self.textlayout(
+            "", "ffffff", font_family, font_size, None)
+        widths, heights = [], []
+        for i in texts:
+            sizelayout.text = i
+            widths.append(sizelayout.width)
+            heights.append(sizelayout.height)
+        return max(widths), max(heights)
+
+    # Old text layout functions, to be deprectated.
+    def set_font(self, fontface, size, antialias=True):
+        self.ctx.select_font_face(fontface)
+        self.ctx.set_font_size(size)
+        fo = self.ctx.get_font_options()
+        fo.set_antialias(cairocffi.ANTIALIAS_SUBPIXEL)
+
+    def text_extents(self, text):
+        return self.ctx.text_extents(utils.scrub_to_utf8(text))
+
+    def font_extents(self):
+        return self.ctx.font_extents()
+
+    def fit_fontsize(self, heightlimit):
+        """
+            Try to find a maximum font size that fits any strings within the
+            height.
+        """
+        self.ctx.set_font_size(heightlimit)
+        asc, desc, height, _, _ = self.font_extents()
+        self.ctx.set_font_size(
+            int(heightlimit * (heightlimit / float(height))))
+        return self.font_extents()
+
+    def fit_text(self, strings, heightlimit):
+        """
+            Try to find a maximum font size that fits all strings within the
+            height.
+        """
+        self.ctx.set_font_size(heightlimit)
+        _, _, _, maxheight, _, _ = self.ctx.text_extents("".join(strings))
+        if not maxheight:
+            return 0, 0
+        self.ctx.set_font_size(
+            int(heightlimit * (heightlimit / float(maxheight))))
+        maxwidth, maxheight = 0, 0
+        for i in strings:
+            _, _, x, y, _, _ = self.ctx.text_extents(i)
+            maxwidth = max(maxwidth, x)
+            maxheight = max(maxheight, y)
+        return maxwidth, maxheight
+
+    def draw_vbar(self, color, x, y1, y2, linewidth=1):
+        self.set_source_rgb(color)
+        self.ctx.move_to(x, y1)
+        self.ctx.line_to(x, y2)
+        self.ctx.set_line_width(linewidth)
+        self.ctx.stroke()
+
+    def draw_hbar(self, color, x1, x2, y, linewidth=1):
+        self.set_source_rgb(color)
+        self.ctx.move_to(x1, y)
+        self.ctx.line_to(x2, y)
+        self.ctx.set_line_width(linewidth)
+        self.ctx.stroke()
```

### Comparing `qtile-0.9.0/libqtile/widget/pacman.py` & `qtile-0.9.1/libqtile/widget/pacman.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 import subprocess
 
 
 class Pacman(base.ThreadedPollText):
     """
     Shows number of available updates.
-    Needs the pacman package manager installed. So will only work in Arch Linux installation.
+    Needs the pacman package manager installed. So will only work in Arch Linux
+    installation.
     """
     defaults = [
         ('unavailable', 'ffffff', 'Unavailable Color - no updates.'),
         ('execute', None, 'Command to execute on click'),
         ('update_interval', 60, "The update interval."),
     ]
 
@@ -39,14 +40,14 @@
         if self.text == '0':
             self.layout.colour = self.unavailable
         else:
             self.layout.colour = self.foreground
         base.ThreadedPollText.draw(self)
 
     def poll(self):
-        pacman = subprocess.Popen(['checkupdates'], stdout=subprocess.PIPE)
-        return str(len(pacman.stdout.readlines()))
+        pacman = self.call_process(['checkupdates'])
+        return str(len(pacman.splitlines()))
 
     def button_press(self, x, y, button):
         base.ThreadedPollText.button_press(self, x, y, button)
         if button == 1 and self.execute is not None:
             subprocess.Popen([self.execute], shell=True)
```

### Comparing `qtile-0.9.0/libqtile/widget/systray.py` & `qtile-0.9.1/libqtile/widget/systray.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+# Copyright (c) 2010 Aldo Cortesi
+# Copyright (c) 2010-2011 dequis
+# Copyright (c) 2010, 2012 roger
+# Copyright (c) 2011 Mounier Florian
+# Copyright (c) 2011-2012, 2014 Tycho Andersen
+# Copyright (c) 2012 dmpayton
+# Copyright (c) 2012-2013 Craig Barnes
+# Copyright (c) 2013 hbc
+# Copyright (c) 2013 Tao Sauvage
+# Copyright (c) 2014 Sean Vig
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 from __future__ import division
 
 from .. import bar, xcbq, window
 from . import base
 
 import xcffib
 from xcffib.xproto import ClientMessageEvent, ClientMessageData, EventMask, SetMode
```

### Comparing `qtile-0.9.0/libqtile/widget/base.py` & `qtile-0.9.1/libqtile/widget/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,41 @@
+# Copyright (c) 2008-2010 Aldo Cortesi
+# Copyright (c) 2011 Florian Mounier
+# Copyright (c) 2011 Kenji_Takahashi
+# Copyright (c) 2011 Paul Colomiets
+# Copyright (c) 2012 roger
+# Copyright (c) 2012 Craig Barnes
+# Copyright (c) 2012-2015 Tycho Andersen
+# Copyright (c) 2013 dequis
+# Copyright (c) 2013 David R. Andersen
+# Copyright (c) 2013 Tao Sauvage
+# Copyright (c) 2014-2015 Sean Vig
+# Copyright (c) 2014 Justin Bronder
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 from .. import command, bar, configurable, drawer
 import six
+import subprocess
 import logging
 import threading
 import warnings
 
 LEFT = object()
 CENTER = object()
 
@@ -132,14 +164,25 @@
 
     def timeout_add(self, seconds, method, method_args=()):
         """
             This method calls either ``.call_later`` with given arguments.
         """
         return self.qtile.call_later(seconds, self._wrapper, method, *method_args)
 
+    def call_process(self, command, **kwargs):
+        """
+            This method uses `subprocess.check_output` to run the given command
+            and return the string from stdout, which is decoded when using
+            Python 3.
+        """
+        output = subprocess.check_output(command, **kwargs)
+        if six.PY3:
+            output = output.decode()
+        return output
+
     def _wrapper(self, method, *method_args):
         try:
             method(*method_args)
         except:
             self.log.exception('got exception from widget timer')
 
 
@@ -389,14 +432,15 @@
             self.bar.draw()
 
     def poll(self):
         pass
 
 # these two classes below look SUSPICIOUSLY similar
 
+
 class PaddingMixin(object):
     """
         Mixin that provides padding(_x|_y|)
 
         To use it, subclass and add this to __init__:
 
             self.add_defaults(base.PaddingMixin.defaults)
@@ -426,9 +470,10 @@
         ("margin_x", None, "X Margin. Overrides 'margin' if set"),
         ("margin_y", None, "Y Margin. Overrides 'margin' if set"),
     ]
 
     margin_x = configurable.ExtraFallback('margin_x', 'margin')
     margin_y = configurable.ExtraFallback('margin_y', 'margin')
 
+
 def deprecated(msg):
     warnings.warn(msg, DeprecationWarning)
```

### Comparing `qtile-0.9.0/libqtile/widget/prompt.py` & `qtile-0.9.1/libqtile/widget/battery.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,417 +1,344 @@
-import glob
+# Copyright (c) 2011 matt
+# Copyright (c) 2011 Paul Colomiets
+# Copyright (c) 2011-2014 Tycho Andersen
+# Copyright (c) 2012 dmpayton
+# Copyright (c) 2012 hbc
+# Copyright (c) 2012 Tim Neumann
+# Copyright (c) 2012 uberj
+# Copyright (c) 2012-2013 Craig Barnes
+# Copyright (c) 2013 Tao Sauvage
+# Copyright (c) 2014 Sean Vig
+# Copyright (c) 2014 dequis
+# Copyright (c) 2014 Sebastien Blot
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+import cairocffi
 import os
-import string
-from .. import bar, xkeysyms, xcbq, command
+from libqtile import bar
 from . import base
 
+BAT_DIR = '/sys/class/power_supply'
+CHARGED = 'Full'
+CHARGING = 'Charging'
+DISCHARGING = 'Discharging'
+UNKNOWN = 'Unknown'
+
+BATTERY_INFO_FILES = {
+    'energy_now_file': ['energy_now', 'charge_now'],
+    'energy_full_file': ['energy_full', 'charge_full'],
+    'power_now_file': ['power_now', 'current_now'],
+    'status_file': ['status'],
+}
+
+
+def default_icon_path():
+    # default icons are in libqtile/resources/battery-icons
+    root = os.sep.join(os.path.abspath(__file__).split(os.sep)[:-2])
+    return os.path.join(root, 'resources', 'battery-icons')
+
+
+class _Battery(base._TextBox):
+    ''' Base battery class '''
+
+    filenames = {}
+
+    defaults = [
+        ('battery_name', 'BAT0', 'ACPI name of a battery, usually BAT0'),
+        (
+            'status_file',
+            'status',
+            'Name of status file in'
+            ' /sys/class/power_supply/battery_name'
+        ),
+        (
+            'energy_now_file',
+            None,
+            'Name of file with the '
+            'current energy in /sys/class/power_supply/battery_name'
+        ),
+        (
+            'energy_full_file',
+            None,
+            'Name of file with the maximum'
+            ' energy in /sys/class/power_supply/battery_name'
+        ),
+        (
+            'power_now_file',
+            None,
+            'Name of file with the current'
+            ' power draw in /sys/class/power_supply/battery_name'
+        ),
+        ('update_delay', 1, 'The delay in seconds between updates'),
+    ]
+
+    def __init__(self, **config):
+        base._TextBox.__init__(self, "BAT", bar.CALCULATED, **config)
+        self.add_defaults(_Battery.defaults)
+
+    def _load_file(self, name):
+        try:
+            path = os.path.join(BAT_DIR, self.battery_name, name)
+            with open(path, 'r') as f:
+                return f.read().strip()
+        except IOError:
+            if name == 'current_now':
+                return 0
+            return False
+        except Exception:
+            self.log.exception("Failed to get %s" % name)
+
+    def _get_param(self, name):
+        if name in self.filenames and self.filenames[name]:
+            return self._load_file(self.filenames[name])
+        elif name not in self.filenames:
+            # Don't have the file name cached, figure it out
+
+            # Don't modify the global list! Copy with [:]
+            file_list = BATTERY_INFO_FILES.get(name, [])[:]
+
+            if getattr(self, name, None):
+                # If a file is manually specified, check it first
+                file_list.insert(0, getattr(self, name))
+
+            # Iterate over the possibilities, and return the first valid value
+            for file in file_list:
+                value = self._load_file(file)
+                if not (value in (False, None)):
+                    self.filenames[name] = file
+                    return value
+
+        # If we made it this far, we don't have a valid file.
+        # Set it to None to avoid trying the next time.
+        self.filenames[name] = None
+
+        return None
+
+    def _get_info(self):
+        try:
+            info = {
+                'stat': self._get_param('status_file'),
+                'now': float(self._get_param('energy_now_file')),
+                'full': float(self._get_param('energy_full_file')),
+                'power': float(self._get_param('power_now_file')),
+            }
+        except TypeError:
+            return False
+        return info
 
-class NullCompleter:
-    def __init__(self, qtile):
-        self.qtile = qtile
-        self.thisfinal = ""
-
-    def actual(self):
-        return self.thisfinal
-
-    def reset(self):
-        pass
-
-    def complete(self, txt):
-        return txt
-
-
-class FileCompleter:
-    def __init__(self, qtile, _testing=False):
-        self._testing = _testing
-        self.qtile = qtile
-        self.thisfinal = None
-        self.reset()
-
-    def actual(self):
-        return self.thisfinal
-
-    def reset(self):
-        self.lookup = None
-
-    def complete(self, txt):
-        """
-        Returns the next completion for txt, or None if there is no completion.
-        """
-        if not self.lookup:
-            self.lookup = []
-            if txt == "" or txt[0] not in "~/":
-                txt = "~/" + txt
-            path = os.path.expanduser(txt)
-            if os.path.isdir(path):
-                files = glob.glob(os.path.join(path, "*"))
-                prefix = txt
-            else:
-                files = glob.glob(path + "*")
-                prefix = os.path.dirname(txt)
-                prefix = prefix.rstrip("/") or "/"
-            for f in files:
-                display = os.path.join(prefix, os.path.basename(f))
-                if os.path.isdir(f):
-                    display += "/"
-                self.lookup.append((display, f))
-                self.lookup.sort()
-            self.offset = -1
-            self.lookup.append((txt, txt))
-        self.offset += 1
-        if self.offset >= len(self.lookup):
-            self.offset = 0
-        ret = self.lookup[self.offset]
-        self.thisfinal = ret[1]
-        return ret[0]
-
-
-class QshCompleter:
-    def __init__(self, qtile):
-        self.qtile = qtile
-        self.client = command.CommandRoot(self.qtile)
-        self.thisfinal = None
-        self.reset()
-
-    def actual(self):
-        return self.thisfinal
-
-    def reset(self):
-        self.lookup = None
-        self.path = ''
-        self.offset = -1
-
-    def complete(self, txt):
-        txt = txt.lower()
-        if not self.lookup:
-            self.lookup = []
-            path = txt.split('.')[:-1]
-            self.path = '.'.join(path)
-            term = txt.split('.')[-1]
-            if len(self.path) > 0:
-                self.path += '.'
 
-            contains_cmd = 'self.client.%s_contains' % self.path
-            try:
-                contains = eval(contains_cmd)
-            except AttributeError:
-                contains = []
-            for obj in contains:
-                if obj.lower().startswith(term):
-                    self.lookup.append((obj, obj))
+class Battery(_Battery):
+    """
+        A simple but flexible text-based battery widget.
+    """
+    defaults = [
+        ('low_foreground', 'FF0000', 'font color when battery is low'),
+        (
+            'format',
+            '{char} {percent:2.0%} {hour:d}:{min:02d}',
+            'Display format'
+        ),
+        ('charge_char', '^', 'Character to indicate the battery is charging'),
+        (
+            'discharge_char',
+            'V',
+            'Character to indicate the battery'
+            ' is discharging'
+        ),
+        (
+            'low_percentage',
+            0.10,
+            "0 < x < 1 at which to indicate battery is low with low_foreground"
+        ),
+        ('hide_threshold', None, 'Hide the text when there is enough energy'),
+    ]
+
+    def __init__(self, **config):
+        _Battery.__init__(self, **config)
+        self.add_defaults(Battery.defaults)
+
+    def timer_setup(self):
+        update_delay = self.update()
+        if update_delay is None and self.update_delay is not None:
+            self.timeout_add(self.update_delay, self.timer_setup)
+        elif update_delay:
+            self.timeout_add(update_delay, self.timer_setup)
 
-            commands_cmd = 'self.client.%scommands()' % self.path
-            try:
-                commands = eval(commands_cmd)
-            except (command.CommandError, AttributeError):
-                commands = []
-            for cmd in commands:
-                if cmd.lower().startswith(term):
-                    self.lookup.append((cmd + '()', cmd + '()'))
-
-            self.offset = -1
-            self.lookup.append((term, term))
-
-        self.offset += 1
-        if self.offset >= len(self.lookup):
-            self.offset = 0
-        ret = self.lookup[self.offset]
-        self.thisfinal = self.path + ret[0]
-        return self.path + ret[0]
-
-
-class GroupCompleter:
-    def __init__(self, qtile):
-        self.qtile = qtile
-        self.thisfinal = None
-        self.lookup = None
-        self.offset = None
-
-    def actual(self):
-        """
-            Returns the current actual value.
-        """
-        return self.thisfinal
-
-    def reset(self):
-        self.lookup = None
-        self.offset = -1
-
-    def complete(self, txt):
-        """
-        Returns the next completion for txt, or None if there is no completion.
-        """
-        txt = txt.lower()
-        if not self.lookup:
-            self.lookup = []
-            for group in self.qtile.groupMap.keys():
-                if group.lower().startswith(txt):
-                    self.lookup.append((group, group))
-
-            self.lookup.sort()
-            self.offset = -1
-            self.lookup.append((txt, txt))
-
-        self.offset += 1
-        if self.offset >= len(self.lookup):
-            self.offset = 0
-        ret = self.lookup[self.offset]
-        self.thisfinal = ret[1]
-        return ret[0]
-
-
-class WindowCompleter:
-    def __init__(self, qtile):
-        self.qtile = qtile
-        self.thisfinal = None
-        self.lookup = None
-        self.offset = None
-
-    def actual(self):
-        """
-            Returns the current actual value.
-        """
-        return self.thisfinal
-
-    def reset(self):
-        self.lookup = None
-        self.offset = -1
-
-    def complete(self, txt):
-        """
-        Returns the next completion for txt, or None if there is no completion.
-        """
-        if not self.lookup:
-            self.lookup = []
-            for wid, window in self.qtile.windowMap.items():
-                if window.group and window.name.lower().startswith(txt):
-                    self.lookup.append((window.name, wid))
-
-            self.lookup.sort()
-            self.offset = -1
-            self.lookup.append((txt, txt))
-
-        self.offset += 1
-        if self.offset >= len(self.lookup):
-            self.offset = 0
-        ret = self.lookup[self.offset]
-        self.thisfinal = ret[1]
-        return ret[0]
-
-
-class CommandCompleter:
-    DEFAULTPATH = "/bin:/usr/bin:/usr/local/bin"
-
-    def __init__(self, qtile, _testing=False):
-        """
-        _testing: disables reloading of the lookup table
-                  to make testing possible.
-        """
-        self.lookup = None
-        self.offset = None
-        self.thisfinal = None
-        self._testing = _testing
-
-    def actual(self):
-        """
-            Returns the current actual value.
-        """
-        return self.thisfinal
-
-    def executable(self, fpath):
-        return os.access(fpath, os.X_OK)
-
-    def reset(self):
-        self.lookup = None
-        self.offset = -1
-
-    def complete(self, txt):
-        """
-        Returns the next completion for txt, or None if there is no completion.
-        """
-        if not self.lookup:
-            if not self._testing:
-                # Lookup is a set of (display value, actual value) tuples.
-                self.lookup = []
-                if txt and txt[0] in "~/":
-                    path = os.path.expanduser(txt)
-                    if os.path.isdir(path):
-                        files = glob.glob(os.path.join(path, "*"))
-                        prefix = txt
-                    else:
-                        files = glob.glob(path + "*")
-                        prefix = os.path.dirname(txt)
-                    prefix = prefix.rstrip("/") or "/"
-                    for f in files:
-                        if self.executable(f):
-                            display = os.path.join(prefix, os.path.basename(f))
-                            if os.path.isdir(f):
-                                display += "/"
-                            self.lookup.append((display, f))
-                else:
-                    dirs = os.environ.get("PATH", self.DEFAULTPATH).split(":")
-                    for didx, d in enumerate(dirs):
-                        try:
-                            for cmd in glob.glob(os.path.join(d, "%s*" % txt)):
-                                if self.executable(cmd):
-                                    self.lookup.append(
-                                        (
-                                            os.path.basename(cmd),
-                                            cmd
-                                        ),
-                                    )
-                        except OSError:
-                            pass
-            self.lookup.sort()
-            self.offset = -1
-            self.lookup.append((txt, txt))
-        self.offset += 1
-        if self.offset >= len(self.lookup):
-            self.offset = 0
-        ret = self.lookup[self.offset]
-        self.thisfinal = ret[1]
-        return ret[0]
+    def _configure(self, qtile, bar):
+        if self.configured:
+            self.update()
+        _Battery._configure(self, qtile, bar)
+
+    def _get_text(self):
+        info = self._get_info()
+        if info is False:
+            return 'Error'
+
+        # Set the charging character
+        try:
+            # hide the text when it's higher than threshold, but still
+            # display `full` when the battery is fully charged.
+            if self.hide_threshold and \
+                    info['now'] / info['full'] * 100.0 >= \
+                    self.hide_threshold and \
+                    info['stat'] != CHARGED:
+                return ''
+            elif info['stat'] == DISCHARGING:
+                char = self.discharge_char
+                time = info['now'] / info['power']
+            elif info['stat'] == CHARGING:
+                char = self.charge_char
+                time = (info['full'] - info['now']) / info['power']
+            else:
+                return 'Full'
+        except ZeroDivisionError:
+            time = -1
+
+        # Calculate the battery percentage and time left
+        if time >= 0:
+            hour = int(time)
+            min = int(time * 60) % 60
+        else:
+            hour = -1
+            min = -1
+        percent = info['now'] / info['full']
+        if info['stat'] == DISCHARGING and percent < self.low_percentage:
+            self.layout.colour = self.low_foreground
+        else:
+            self.layout.colour = self.foreground
 
+        return self.format.format(
+            char=char,
+            percent=percent,
+            hour=hour,
+            min=min
+        )
 
-class Prompt(base._TextBox):
-    """
-        A widget that prompts for user input. Input should be started using the
-        .startInput method on this class.
-    """
-    completers = {
-        "file": FileCompleter,
-        "qsh": QshCompleter,
-        "cmd": CommandCompleter,
-        "group": GroupCompleter,
-        "window": WindowCompleter,
-        None: NullCompleter
-    }
-    defaults = [("cursorblink", 0.5, "Cursor blink rate. 0 to disable."),
-                ("prompt", "{prompt}: ", "Text displayed at the prompt")]
-
-    def __init__(self, name="prompt", **config):
-        base._TextBox.__init__(self, "", bar.CALCULATED, **config)
-        self.add_defaults(Prompt.defaults)
-        self.name = name
-        self.active = False
-        self.blink = False
-        self.completer = None
+    def update(self):
+        ntext = self._get_text()
+        if ntext != self.text:
+            self.text = ntext
+            self.bar.draw()
+
+
+class BatteryIcon(_Battery):
+    ''' Battery life indicator widget '''
+
+    defaults = [
+        ('theme_path', default_icon_path(), 'Path of the icons'),
+        ('custom_icons', {}, 'dict containing key->filename icon map'),
+    ]
+
+    def __init__(self, **config):
+        _Battery.__init__(self, **config)
+        self.add_defaults(BatteryIcon.defaults)
+
+        if self.theme_path:
+            self.width_type = bar.STATIC
+            self.width = 0
+        self.surfaces = {}
+        self.current_icon = 'battery-missing'
+        self.icons = dict([(x, '{0}.png'.format(x)) for x in (
+            'battery-missing',
+            'battery-caution',
+            'battery-low',
+            'battery-good',
+            'battery-full',
+            'battery-caution-charging',
+            'battery-low-charging',
+            'battery-good-charging',
+            'battery-full-charging',
+            'battery-full-charged',
+        )])
+        self.icons.update(self.custom_icons)
+
+    def timer_setup(self):
+        self.update()
+        self.timeout_add(self.update_delay, self.timer_setup)
 
     def _configure(self, qtile, bar):
         base._TextBox._configure(self, qtile, bar)
+        self.setup_images()
 
-    def startInput(self, prompt, callback,
-                   complete=None, strict_completer=False):
-        """
-            complete: Tab-completion. Can be None, or "cmd".
-
-            Displays a prompt and starts to take one line of keyboard input
-            from the user. When done, calls the callback with the input string
-            as argument.
-
-            prompt = text displayed at the prompt, e.g. "spawn: "
-            callback = function to call with returned value.
-            complete = completer to use.
-            strict_completer = When True the retuen value wil be the exact
-                               completer result where available.
-        """
-
-        if self.cursorblink and not self.active:
-            self.timeout_add(self.cursorblink, self._blink)
-        self.display = self.prompt.format(prompt=prompt)
-        self.active = True
-        self.userInput = ""
-        self.callback = callback
-        self.completer = self.completers[complete](self.qtile)
-        self.strict_completer = strict_completer
-        self._update()
-        self.bar.widget_grab_keyboard(self)
-
-    def _calculate_real_width(self):
-        if self.blink:
-            return min(
-                self.layout.width,
-                self.bar.width
-            ) + self.actual_padding * 2
+    def _get_icon_key(self):
+        key = 'battery'
+        info = self._get_info()
+        if info is False or not info.get('full'):
+            key += '-missing'
         else:
-            _text = self.text
-            self.text = _text + "_"
-            width = min(
-                self.layout.width,
-                self.bar.width
-            ) + self.actual_padding * 2
-            self.text = _text
-            return width
-
-    def calculate_width(self):
-        if self.text:
-            return self._calculate_real_width()
-        else:
-            return 0
-
-    def _blink(self):
-        self.blink = not self.blink
-        self._update()
-        if self.active:
-            self.timeout_add(self.cursorblink, self._blink)
-
-    def _update(self):
-        if self.active:
-            self.text = "%s%s" % (self.display, self.userInput)
-            if self.blink:
-                self.text = self.text + "_"
+            percent = info['now'] / info['full']
+            if percent < .2:
+                key += '-caution'
+            elif percent < .4:
+                key += '-low'
+            elif percent < .8:
+                key += '-good'
             else:
-                self.text = self.text
-        else:
-            self.text = ""
-        self.bar.draw()
+                key += '-full'
 
-    def handle_KeyPress(self, e):
-        """
-            KeyPress handler for the minibuffer.
-            Currently only supports ASCII characters.
-        """
-        state = e.state & ~(self.qtile.numlockMask)
-        keysym = self.qtile.conn.keycode_to_keysym(e.detail, state)
-        if keysym == xkeysyms.keysyms['Tab']:
-            self.userInput = self.completer.complete(self.userInput)
+            if info['stat'] == CHARGING:
+                key += '-charging'
+            elif info['stat'] == CHARGED:
+                key += '-charged'
+        return key
+
+    def update(self):
+        icon = self._get_icon_key()
+        if icon != self.current_icon:
+            self.current_icon = icon
+            self.draw()
+
+    def draw(self):
+        if self.theme_path:
+            self.drawer.clear(self.background or self.bar.background)
+            self.drawer.ctx.set_source(self.surfaces[self.current_icon])
+            self.drawer.ctx.paint()
+            self.drawer.draw(self.offset, self.width)
         else:
-            actual_value = self.completer.actual()
-            self.completer.reset()
-            if keysym < 127 and chr(keysym) in string.printable:
-                # No LookupString in XCB... oh,
-                # the shame! Unicode users beware!
-                self.userInput += chr(keysym)
-            elif (keysym == xkeysyms.keysyms['BackSpace'] and
-                  len(self.userInput) > 0):
-                self.userInput = self.userInput[:-1]
-            elif keysym == xkeysyms.keysyms['Escape']:
-                self.active = False
-                self.bar.widget_ungrab_keyboard()
-            elif keysym == xkeysyms.keysyms['Return']:
-                self.active = False
-                self.bar.widget_ungrab_keyboard()
-                if self.strict_completer:
-                    self.callback(actual_value or self.userInput)
-                else:
-                    self.callback(self.userInput)
-        self._update()
-
-    def cmd_fake_keypress(self, key):
-        class Dummy:
-            pass
-        d = Dummy()
-        keysym = xcbq.keysyms[key]
-        d.detail = self.qtile.conn.keysym_to_keycode(keysym)
-        d.state = 0
-        self.handle_KeyPress(d)
-
-    def cmd_info(self):
-        """
-            Returns a dictionary of info for this object.
-        """
-        return dict(
-            name=self.name,
-            width=self.width,
-            text=self.text,
-            active=self.active,
-        )
+            self.text = self.current_icon[8:]
+            base._TextBox.draw(self)
+
+    def setup_images(self):
+        for key, name in self.icons.items():
+            try:
+                path = os.path.join(self.theme_path, name)
+                img = cairocffi.ImageSurface.create_from_png(path)
+            except cairocffi.Error:
+                self.theme_path = None
+                self.qtile.log.warning('Battery Icon switching to text mode')
+                return
+            input_width = img.get_width()
+            input_height = img.get_height()
+
+            sp = input_height / float(self.bar.height - 1)
+
+            width = input_width / sp
+            if width > self.width:
+                self.width = int(width) + self.actual_padding * 2
+
+            imgpat = cairocffi.SurfacePattern(img)
+
+            scaler = cairocffi.Matrix()
+
+            scaler.scale(sp, sp)
+            scaler.translate(self.actual_padding * -1, 0)
+            imgpat.set_matrix(scaler)
+
+            imgpat.set_filter(cairocffi.FILTER_BEST)
+            self.surfaces[key] = imgpat
```

### Comparing `qtile-0.9.0/libqtile/widget/df.py` & `qtile-0.9.1/libqtile/widget/df.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # -*- coding:utf-8 -*-
 #
-# Copyright (C) 2013, Roger Duran <rogerduran@gmail.com>
+# Copyright (c) 2015, Roger Duran. All rights reserved.
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-# GNU General Public License for more details.
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
 
 import os
 from . import base
 
 class DF(base.ThreadedPollText):
     """
     Disk Free Widget
```

### Comparing `qtile-0.9.0/libqtile/widget/mpdwidget.py` & `qtile-0.9.1/libqtile/widget/mpdwidget.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,38 @@
+# Copyright (c) 2010 matt
+# Copyright (c) 2010 Dieter Plaetinck
+# Copyright (c) 2010, 2012 roger
+# Copyright (c) 2011-2012 Florian Mounier
+# Copyright (c) 2011 Mounier Florian
+# Copyright (c) 2011 Timo Schmiade
+# Copyright (c) 2012 Mikkel Oscar Lyderik
+# Copyright (c) 2012, 2014 Tycho Andersen
+# Copyright (c) 2012 Craig Barnes
+# Copyright (c) 2013 Tao Sauvage
+# Copyright (c) 2013 Tom Hunt
+# Copyright (c) 2014 Justin Bronder
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 # -*- coding: utf-8 -*-
 # depends on python-mpd
 
 
 # TODO: check if UI hangs in case of network issues and such
 # TODO: some kind of templating to make shown info configurable
 # TODO: best practice to handle failures? just write to stderr?
```

### Comparing `qtile-0.9.0/libqtile/widget/groupbox.py` & `qtile-0.9.1/libqtile/widget/volume.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,235 +1,230 @@
-from .. import bar, hook
-from . import base
-
-
-class _GroupBase(base._TextBox, base.PaddingMixin, base.MarginMixin):
-    defaults = [
-        ("borderwidth", 3, "Current group border width"),
-    ]
+# Copyright (c) 2010, 2012, 2014 roger
+# Copyright (c) 2011 Kirk Strauser
+# Copyright (c) 2011 Florian Mounier
+# Copyright (c) 2011 Mounier Florian
+# Copyright (c) 2011 Roger Duran
+# Copyright (c) 2012-2015 Tycho Andersen
+# Copyright (c) 2013 Tao Sauvage
+# Copyright (c) 2013 Craig Barnes
+# Copyright (c) 2014-2015 Sean Vig
+# Copyright (c) 2014 Adi Sieker
+# Copyright (c) 2014 dmpayton
+# Copyright (c) 2014 Jody Frankowski
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+import os
+import re
+import subprocess
 
-    def __init__(self, **config):
-        base._TextBox.__init__(self, width=bar.CALCULATED, **config)
-        self.add_defaults(_GroupBase.defaults)
-        self.add_defaults(base.PaddingMixin.defaults)
-        self.add_defaults(base.MarginMixin.defaults)
-
-    def box_width(self, groups):
-        width, height = self.drawer.max_layout_size(
-            [i.name for i in groups],
-            self.font,
-            self.fontsize
-        )
-        return width + self.padding_x * 2 + self.margin_x * 2 + \
-            self.borderwidth * 2
-
-    def _configure(self, qtile, bar):
-        base._Widget._configure(self, qtile, bar)
-
-        if self.fontsize is None:
-            calc = self.bar.height - self.margin_y * 2 - \
-                self.borderwidth * 2 - self.padding_y * 2
-            self.fontsize = max(calc, 1)
-
-        self.layout = self.drawer.textlayout(
-            "",
-            "ffffff",
-            self.font,
-            self.fontsize,
-            self.fontshadow
-        )
-        self.setup_hooks()
+import cairocffi
 
-    def setup_hooks(self):
-        def hook_response(*args, **kwargs):
-            self.bar.draw()
-        hook.subscribe.client_managed(hook_response)
-        hook.subscribe.client_urgent_hint_changed(hook_response)
-        hook.subscribe.client_killed(hook_response)
-        hook.subscribe.setgroup(hook_response)
-        hook.subscribe.group_window_add(hook_response)
-        hook.subscribe.current_screen_change(hook_response)
-        hook.subscribe.changegroup(hook_response)
-
-    def drawbox(self, offset, text, bordercolor, textcolor, rounded=False,
-                block=False, width=None):
-        self.layout.text = text
-        self.layout.font_family = self.font
-        self.layout.font_size = self.fontsize
-        self.layout.colour = textcolor
-        if width is not None:
-            self.layout.width = width
-        framed = self.layout.framed(
-            self.borderwidth,
-            bordercolor,
-            self.padding_x,
-            self.padding_y
-        )
-        if block:
-            framed.draw_fill(offset, self.margin_y, rounded)
-        else:
-            framed.draw(offset, self.margin_y, rounded)
-
-
-class AGroupBox(_GroupBase):
-    """
-        A widget that graphically displays the current group.
-    """
-    defaults = [("border", "000000", "group box border color")]
-
-    def __init__(self, **config):
-        _GroupBase.__init__(self, **config)
-        self.add_defaults(AGroupBox.defaults)
+from . import base
+from .. import bar
+from six import u
 
-    def button_press(self, x, y, button):
-        self.bar.screen.cmd_nextgroup()
+__all__ = [
+    'Volume',
+]
 
-    def calculate_width(self):
-        return self.box_width(self.qtile.groups)
+re_vol = re.compile('\[(\d?\d?\d?)%\]')
 
-    def draw(self):
-        self.drawer.clear(self.background or self.bar.background)
-        e = next(
-            i for i in self.qtile.groups
-            if i.name == self.bar.screen.group.name
-        )
-        self.drawbox(self.margin_x, e.name, self.border, self.foreground)
-        self.drawer.draw(self.offset, self.width)
 
-
-class GroupBox(_GroupBase):
-    """
-        A widget that graphically displays the current group.
-    """
+class Volume(base._TextBox):
+    ''' Widget that display and change volume
+        if theme_path is set it draw widget as
+        icons '''
     defaults = [
-        ("active", "FFFFFF", "Active group font colour"),
-        ("inactive", "404040", "Inactive group font colour"),
-        ("urgent_text", "FF0000", "Urgent group font color"),
-        (
-            "highlight_method",
-            "border",
-            "Method of highlighting (one of 'border' or 'block') "
-            "Uses \*_border color settings"
-        ),
-        ("rounded", True, "To round or not to round borders"),
-        (
-            "this_current_screen_border",
-            "215578",
-            "Border colour for group on this screen when focused."
-        ),
-        (
-            "urgent_alert_method",
-            "border",
-            "Method for alerting you of WM urgent "
-            "hints (one of 'border', 'text' or 'block')"
-        ),
-        (
-            "disable_drag",
-            False,
-            "Disable dragging and dropping of group names on widget"
-        ),
-        (
-            "this_screen_border",
-            "215578",
-            "Border colour for group on this screen."
-        ),
-        (
-            "other_screen_border",
-            "404040",
-            "Border colour for group on other screen."
-        ),
-        ("urgent_border", "FF0000", "Urgent border color"),
-        ("invert_mouse_wheel", False, "Whether to invert mouse wheel group movement")
+        ("cardid", 0, "Card Id"),
+        ("channel", "Master", "Channel"),
+        ("padding", 3, "Padding left and right. Calculated if None."),
+        ("theme_path", None, "Path of the icons"),
+        ("update_interval", 0.2, "Update time in seconds."),
+        ("emoji", False, "Use emoji to display volume states, only if ``theme_path`` is not set."
+                         "The specified font needs to contain the correct unicode characters."),
+        ("mute_command", None, "Mute command"),
+        ("volume_up_command", None, "Volume up command"),
+        ("volume_down_command", None, "Volume down command"),
+        ("get_volume_command", None, "Command to get the current volume"),
     ]
 
     def __init__(self, **config):
-        _GroupBase.__init__(self, **config)
-        self.add_defaults(GroupBox.defaults)
-        self.clicked = None
-
-    def get_clicked_group(self, x, y):
-        group = None
-        new_width = 0
-        width = 0
-        for g in self.qtile.groups:
-            new_width += self.box_width([g])
-            if x >= width and x <= new_width:
-                group = g
-                break
-            width = new_width
-        return group
+        base._TextBox.__init__(self, '0', width=bar.CALCULATED, **config)
+        self.add_defaults(Volume.defaults)
+        if self.theme_path:
+            self.width_type = bar.STATIC
+            self.width = 0
+        self.surfaces = {}
+        self.volume = None
+
+    def timer_setup(self):
+        self.timeout_add(self.update_interval, self.update)
+        if self.theme_path:
+            self.setup_images()
 
     def button_press(self, x, y, button):
-        self.clicked = None
-        group = None
-        curGroup = self.qtile.currentGroup
-
-        if button == (5 if not self.invert_mouse_wheel else 4):
-            group = curGroup.prevGroup()
-        elif button == (4 if not self.invert_mouse_wheel else 5):
-            group = curGroup.nextGroup()
-        else:
-            group = self.get_clicked_group(x, y)
-            if not self.disable_drag:
-                self.clicked = group
-
-        if group:
-            self.bar.screen.setGroup(group)
-
-    def button_release(self, x, y, button):
-        if button not in (5, 4):
-            group = self.get_clicked_group(x, y)
-            if group and self.clicked:
-                group.cmd_switch_groups(self.clicked.name)
-                self.clicked = None
-
-    def calculate_width(self):
-        width = 0
-        for g in self.qtile.groups:
-            width += self.box_width([g])
-        return width
-
-    def group_has_urgent(self, group):
-        return len([w for w in group.windows if w.urgent]) > 0
-
-    def draw(self):
-        self.drawer.clear(self.background or self.bar.background)
-
-        offset = 0
-        for i, g in enumerate(self.qtile.groups):
-            is_block = (self.highlight_method == 'block')
-
-            bw = self.box_width([g])
-            if g.screen:
-                if self.bar.screen.group.name == g.name:
-                    if self.qtile.currentScreen == self.bar.screen:
-                        border = self.this_current_screen_border
-                    else:
-                        border = self.this_screen_border
-                else:
-                    border = self.other_screen_border
-            elif self.group_has_urgent(g) and \
-                    self.urgent_alert_method in ('border', 'block'):
-                border = self.urgent_border
-                if self.urgent_alert_method == 'block':
-                    is_block = True
+        if button == 5:
+            if self.volume_down_command is not None:
+                subprocess.call(self.volume_down_command)
+            else:
+                subprocess.call([
+                    'amixer',
+                    '-q',
+                    '-c',
+                    str(self.cardid),
+                    'sset',
+                    self.channel,
+                    '2dB-'
+                ])
+        elif button == 4:
+            if self.volume_up_command is not None:
+                subprocess.call(self.volume_up_command)
             else:
-                border = self.background or self.bar.background
+                subprocess.call([
+                    'amixer',
+                    '-q',
+                    '-c',
+                    str(self.cardid),
+                    'sset',
+                    self.channel,
+                    '2dB+'
+                ])
+        elif button == 1:
+            if self.mute_command is not None:
+                subprocess.call(self.mute_command)
+            else:
+                subprocess.call([
+                    'amixer',
+                    '-q',
+                    '-c',
+                    str(self.cardid),
+                    'sset',
+                    self.channel,
+                    'toggle'
+                ])
+        self.draw()
+
+    def update(self):
+        vol = self.get_volume()
+        if vol != self.volume:
+            self.volume = vol
+            # Update the underlying canvas size before actually attempting
+            # to figure out how big it is and draw it.
+            self._update_drawer()
+            self.bar.draw()
+        self.timeout_add(self.update_interval, self.update)
 
-            if self.group_has_urgent(g) and self.urgent_alert_method == "text":
-                text = self.urgent_text
-            elif g.windows:
-                text = self.active
+    def _update_drawer(self):
+        if self.theme_path:
+            self.drawer.clear(self.background or self.bar.background)
+            if self.volume <= 0:
+                img_name = 'audio-volume-muted'
+            elif self.volume <= 30:
+                img_name = 'audio-volume-low'
+            elif self.volume < 80:
+                img_name = 'audio-volume-medium'
+            elif self.volume >= 80:
+                img_name = 'audio-volume-high'
+
+            self.drawer.ctx.set_source(self.surfaces[img_name])
+            self.drawer.ctx.paint()
+        elif self.emoji:
+            if self.volume <= 0:
+                self.text = u('\U0001f507')
+            elif self.volume <= 30:
+                self.text = u('\U0001f508')
+            elif self.volume < 80:
+                self.text = u('\U0001f509')
+            elif self.volume >= 80:
+                self.text = u('\U0001f50a')
+        else:
+            if self.volume == -1:
+                self.text = 'M'
             else:
-                text = self.inactive
+                self.text = '%s%%' % self.volume
 
-            self.drawbox(
-                self.margin_x + offset,
-                g.name,
-                border,
-                text,
-                self.rounded,
-                is_block,
-                bw - self.margin_x * 2 - self.padding_x * 2
-            )
-            offset += bw
-        self.drawer.draw(self.offset, self.width)
+    def setup_images(self):
+        for img_name in (
+            'audio-volume-high',
+            'audio-volume-low',
+            'audio-volume-medium',
+            'audio-volume-muted'
+        ):
+
+            try:
+                img = cairocffi.ImageSurface.create_from_png(
+                    os.path.join(self.theme_path, '%s.png' % img_name)
+                )
+            except cairocffi.Error:
+                self.theme_path = None
+                self.width_type = bar.CALCULATED
+                self.qtile.log.exception('Volume switching to text mode')
+                return
+            input_width = img.get_width()
+            input_height = img.get_height()
+
+            sp = input_height / float(self.bar.height - 1)
+
+            width = input_width / sp
+            if width > self.width:
+                self.width = int(width) + self.actual_padding * 2
+
+            imgpat = cairocffi.SurfacePattern(img)
+
+            scaler = cairocffi.Matrix()
+
+            scaler.scale(sp, sp)
+            scaler.translate(self.actual_padding * -1, 0)
+            imgpat.set_matrix(scaler)
+
+            imgpat.set_filter(cairocffi.FILTER_BEST)
+            self.surfaces[img_name] = imgpat
+
+    def get_volume(self):
+        try:
+            get_volume_cmd = [
+                'amixer',
+                '-c',
+                str(self.cardid),
+                'sget',
+                self.channel
+            ]
+
+            if self.get_volume_command:
+                get_volume_cmd = self.get_volume_command
+
+            mixer_out = self.call_process(get_volume_cmd)
+        except subprocess.CalledProcessError:
+            return -1
+
+        if '[off]' in mixer_out:
+            return -1
+
+        volgroups = re_vol.search(mixer_out)
+        if volgroups:
+            return int(volgroups.groups()[0])
+        else:
+            # this shouldn't happend
+            return -1
+
+    def draw(self):
+        if self.theme_path:
+            self.drawer.draw(self.offset, self.width)
+        else:
+            base._TextBox.draw(self)
```

### Comparing `qtile-0.9.0/libqtile/widget/windowtabs.py` & `qtile-0.9.1/libqtile/widget/windowtabs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+# Copyright (c) 2012-2013 Craig Barnes
+# Copyright (c) 2012 roger
+# Copyright (c) 2012, 2014 Tycho Andersen
+# Copyright (c) 2014 Sean Vig
+# Copyright (c) 2014 Adi Sieker
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 from .. import hook, bar
 from . import base
 
 
 class WindowTabs(base._TextBox):
     """
         Displays the name of each window in the current group.
```

### Comparing `qtile-0.9.0/libqtile/widget/google_calendar.py` & `qtile-0.9.1/libqtile/widget/google_calendar.py`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/pangocffi.py` & `qtile-0.9.1/libqtile/pangocffi.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+# Copyright (c) 2014-2015 Sean Vig
+# Copyright (c) 2014 roger
+# Copyright (c) 2014 Tycho Andersen
+# Copyright (c) 2015 Craig Barnes
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 # This module is kind of a hack; you've been warned :-). Some upstream work
 # needs to happen in order to avoid doing this, though.
 #
 # The problem is that we want to use pango to draw stuff. We need to create a
 # cairo surface, in particular an XCB surface. Since we're using xcffib as the
 # XCB binding and there is no portable way to go from cffi's PyObject* cdata
 # wrappers to the wrapped type [1], we can't add support to pycairo for XCB
@@ -145,14 +168,15 @@
                          gssize length);
 """)
 
 gobject = ffi.dlopen('gobject-2.0')
 pango = ffi.dlopen('pango-1.0')
 pangocairo = ffi.dlopen('pangocairo-1.0')
 
+
 def CairoContext(cairo_t):
     def create_layout():
         return PangoLayout(cairo_t._pointer)
     cairo_t.create_layout = create_layout
 
     def show_layout(layout):
         pangocairo.pango_cairo_show_layout(cairo_t._pointer, layout._pointer)
@@ -160,21 +184,24 @@
 
     return cairo_t
 
 ALIGN_CENTER = pango.PANGO_ALIGN_CENTER
 ELLIPSIZE_END = pango.PANGO_ELLIPSIZE_END
 units_from_double = pango.pango_units_from_double
 
+
 def _const_char_to_py_str(cc):
     return ''.join(ffi.buffer(cc, len(cc)))
 
+
 class PangoLayout(object):
     def __init__(self, cairo_t):
         self._cairo_t = cairo_t
         self._pointer = pangocairo.pango_cairo_create_layout(cairo_t)
+
         def free(p):
             p = ffi.cast("gpointer", p)
             gobject.g_object_unref(p)
         self._pointer = ffi.gc(self._pointer, free)
 
     def set_font_description(self, desc):
         # save a pointer so it doesn't get GC'd out from under us
@@ -212,14 +239,15 @@
         pango.pango_layout_get_pixel_size(self._pointer, width, height)
 
         return width[0], height[0]
 
     def set_width(self, width):
         pango.pango_layout_set_width(self._pointer, width)
 
+
 class FontDescription(object):
     def __init__(self, pointer=None):
         if pointer is None:
             self._pointer = pango.pango_font_description_new()
             self._pointer = ffi.gc(self._pointer, pango.pango_font_description_free)
         else:
             self._pointer = pointer
@@ -236,26 +264,28 @@
 
     def set_size(self, size):
         pango.pango_font_description_set_size(self._pointer, size)
 
     def get_size(self, size):
         return pango.pango_font_description_get_size(self._pointer, size)
 
+
 def parse_markup(value, accel_marker=0):
     attr_list = ffi.new("PangoAttrList**")
     text = ffi.new("char**")
     error = ffi.new("GError**")
     if six.PY3:
         value = value.encode()
 
     ret = pango.pango_parse_markup(value, -1, accel_marker, attr_list, text, ffi.NULL, error)
 
     if ret == 0:
         raise Exception("parse_markup() failed for %s" % value)
 
     return attr_list[0], ffi.string(text[0]), six.unichr(accel_marker)
 
+
 def markup_escape_text(text):
     ret = gobject.g_markup_escape_text(text.encode(), -1)
     if six.PY3:
         return ffi.string(ret).decode()
     return ffi.string(ret)
```

### Comparing `qtile-0.9.0/libqtile/configurable.py` & `qtile-0.9.1/libqtile/configurable.py`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/command.py` & `qtile-0.9.1/libqtile/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,14 +426,14 @@
             except SyntaxError:
                 exec(code)
                 return (True, None)
         except:
             error = traceback.format_exc().strip().split("\n")[-1]
             return (False, error)
 
-    def cmd_function(self, function):
+    def cmd_function(self, function, *args, **kwargs):
         """Call a function with current object as argument"""
         try:
-            function(self)
+            function(self, *args, **kwargs)
         except Exception:
             error = traceback.format_exc()
             self.log.error('Exception calling "%s":\n%s' % (function, error))
```

### Comparing `qtile-0.9.0/libqtile/bar.py` & `qtile-0.9.1/libqtile/bar.py`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/xkeysyms.py` & `qtile-0.9.1/libqtile/xkeysyms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+# -*- coding: utf-8 -*-
+#
+# Copyright (c) 2010 Aldo Cortesi
+# Copyright (c) 2012 Julian Berman
+# Copyright (c) 2014 Björn Lässig
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 keysyms = {
     'XF86ModeLock': 0x1008FF01,
     'XF86MonBrightnessUp': 0x1008FF02,
     'XF86MonBrightnessDown': 0x1008FF03,
     'XF86KbdLightOnOff': 0x1008FF04,
     'XF86KbdBrightnessUp': 0x1008FF05,
     'XF86KbdBrightnessDown': 0x1008FF06,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qtile-0.9.0/libqtile/resources/__pycache__/default_config.cpython-34.pyc` & `qtile-0.9.1/libqtile/resources/__pycache__/default_config.cpython-34.pyc`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/resources/default_config.pyc` & `qtile-0.9.1/libqtile/resources/default_config.pyc`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/resources/battery-icons/battery-full.png` & `qtile-0.9.1/libqtile/resources/battery-icons/battery-full.png`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/resources/battery-icons/battery-full-charging.png` & `qtile-0.9.1/libqtile/resources/battery-icons/battery-full-charging.png`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/resources/battery-icons/battery-caution-charging.png` & `qtile-0.9.1/libqtile/resources/battery-icons/battery-caution-charging.png`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/resources/battery-icons/battery-empty.png` & `qtile-0.9.1/libqtile/resources/battery-icons/battery-empty.png`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/resources/battery-icons/battery-low.png` & `qtile-0.9.1/libqtile/resources/battery-icons/battery-low.png`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/resources/battery-icons/battery-missing.png` & `qtile-0.9.1/libqtile/resources/battery-icons/battery-missing.png`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/resources/battery-icons/battery-low-charging.png` & `qtile-0.9.1/libqtile/resources/battery-icons/battery-low-charging.png`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/resources/battery-icons/battery-good-charging.png` & `qtile-0.9.1/libqtile/resources/battery-icons/battery-good-charging.png`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/resources/battery-icons/battery-caution.png` & `qtile-0.9.1/libqtile/resources/battery-icons/battery-caution.png`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/resources/battery-icons/battery-full-charged.png` & `qtile-0.9.1/libqtile/resources/battery-icons/battery-full-charged.png`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/resources/battery-icons/battery-good.png` & `qtile-0.9.1/libqtile/resources/battery-icons/battery-good.png`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/window.py` & `qtile-0.9.1/libqtile/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -871,40 +871,43 @@
         else:
             # make sure x, y is on the screen
             screen = self.qtile.find_closest_screen(self.x, self.y)
             if screen is not None and \
                     self.group is not None and \
                     self.group.screen is not None and \
                     screen != self.group.screen:
-                self.x = self.group.screen.x
-                self.y = self.group.screen.y
+                x = self.group.screen.x
+                y = self.group.screen.y
+            else:
+                x = self.x
+                y = self.y
 
             if self.width < self.hints.get('min_width', 0):
-                self.width = self.hints['min_width']
+                width = self.hints['min_width']
+            else:
+                width = self.width
 
             if self.height < self.hints.get('min_height', 0):
                 self.height = self.hints['min_height']
+            else:
+                height = self.height
 
-            width = self.width
             if self.hints.get('width_inc', 0):
                 width = (width -
-                    ((width - self.hints['base_width']) %
-                    self.hints['width_inc']))
+                         ((width - self.hints['base_width']) %
+                          self.hints['width_inc']))
 
-            height = self.height
             if self.hints.get('height_inc', 0):
                 height = (height -
-                    ((height - self.hints['base_height'])
-                    % self.hints['height_inc']))
+                          ((height - self.hints['base_height'])
+                           % self.hints['height_inc']))
 
             self.place(
-                self.x,
-                self.y,
-                width,
-                height,
+                x, y,
+                width, height,
                 self.borderwidth,
                 self.bordercolor,
                 above=True,
             )
         if self._float_state != new_float_state:
             self._float_state = new_float_state
             if self.group:  # may be not, if it's called from hook
@@ -1001,31 +1004,26 @@
     def handle_ConfigureRequest(self, e):
         if self.qtile._drag and self.qtile.currentWindow == self:
             # ignore requests while user is dragging window
             return
         if getattr(self, 'floating', False):
             # only obey resize for floating windows
             cw = xcffib.xproto.ConfigWindow
-            if e.value_mask & cw.Width:
-                self.width = e.width
-            if e.value_mask & cw.Height:
-                self.height = e.height
-            if e.value_mask & cw.X:
-                self.x = e.x
-            if e.value_mask & cw.Y:
-                self.y = e.y
+            width = e.width if e.value_mask & cw.Width else self.width
+            height = e.height if e.value_mask & cw.Height else self.height
+            x = e.x if e.value_mask & cw.X else self.x
+            y = e.y if e.value_mask & cw.Y else self.y
+        else:
+            width, height, x, y = self.width, self.height, self.x, self.y
 
         if self.group and self.group.screen:
             self.place(
-                self.x,
-                self.y,
-                self.width,
-                self.height,
-                self.borderwidth,
-                self.bordercolor,
+                x, y,
+                width, height,
+                self.borderwidth, self.bordercolor,
             )
         self.updateState()
         return False
 
     def update_wm_net_icon(self):
         """
             Set a dict with the icons of the window
```

### Comparing `qtile-0.9.0/libqtile/manager.py` & `qtile-0.9.1/libqtile/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,19 +241,19 @@
         # us via calls to asyncio's call_soon_threadsafe.
         try:
             # We import dbus here to thrown an ImportError if it isn't
             # available. Since the only reason we're running this thread is
             # because of dbus, if dbus isn't around there's no need to run
             # this thread.
             import dbus  # noqa
-            from six.moves import gobject
+            from gi.repository import GObject
 
-            gobject.threads_init()
+            GObject.threads_init()
             def gobject_thread():
-                ctx = gobject.main_context_default()
+                ctx = GObject.main_context_default()
                 while not self._eventloop.is_closed():
                     try:
                         ctx.iteration(True)
                     except Exception:
                         self.qtile.exception("got exception from gobject")
             t = threading.Thread(target=gobject_thread, name="gobject_thread")
             t.start()
@@ -686,30 +686,32 @@
             pass
 
     def loop(self):
         self.server.start()
 
         self._eventloop.add_signal_handler(signal.SIGINT, self._eventloop.stop)
         self._eventloop.add_signal_handler(signal.SIGTERM, self._eventloop.stop)
+        self._eventloop.set_exception_handler(
+            lambda x, y: self.log.exception("Got an exception in poll loop"))
 
         self.log.info('Adding io watch')
         fd = self.conn.conn.get_file_descriptor()
         self._eventloop.add_reader(fd, self._xpoll)
 
         try:
             self._eventloop.run_forever()
         finally:
             self.server.close()
             self.log.info('Removing io watch')
             self._eventloop.remove_reader(fd)
             self._eventloop.close()
             self.conn.conn.disconnect()
             try:
-                from six.moves import gobject
-                gobject.idle_add(lambda: None)
+                from gi.repository import GObject
+                GObject.idle_add(lambda: None)
             except ImportError:
                 pass
 
     def find_screen(self, x, y):
         """
             Find a screen based on the x and y offset.
         """
@@ -804,15 +806,15 @@
         # it's the selection property
         if name in ("PRIMARY", "CLIPBOARD"):
             assert e.window == self.selection_window.wid
             prop = self.selection_window.get_property(e.atom, "UTF8_STRING")
 
             # If the selection property is None, it is unset, which means the
             # clipboard is empty.
-            value = prop and prop.value.to_string() or ""
+            value = prop and prop.value.to_utf8() or six.u("")
 
             self.selection[name]["selection"] = value
             hook.fire("selection_change", name, self.selection[name])
 
     def handle_EnterNotify(self, e):
         if e.event in self.windowMap:
             return True
```

### Comparing `qtile-0.9.0/libqtile/sh.py` & `qtile-0.9.1/libqtile/sh.py`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/libqtile/xcbq.py` & `qtile-0.9.1/libqtile/xcbq.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+# Copyright (c) 2009-2010 Aldo Cortesi
+# Copyright (c) 2010 matt
+# Copyright (c) 2010, 2012, 2014 dequis
+# Copyright (c) 2010 Philip Kranz
+# Copyright (c) 2010-2011 Paul Colomiets
+# Copyright (c) 2011 osebelin
+# Copyright (c) 2011 Mounier Florian
+# Copyright (c) 2011 Kenji_Takahashi
+# Copyright (c) 2011 Tzbob
+# Copyright (c) 2012, 2014 roger
+# Copyright (c) 2012, 2014-2015 Tycho Andersen
+# Copyright (c) 2013 Tao Sauvage
+# Copyright (c) 2014-2015 Sean Vig
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
     A minimal EWMH-aware OO layer over xpyb. This is NOT intended to be
     complete - it only implements the subset of functionalty needed by qtile.
 """
 from __future__ import print_function, division
 
 import six
@@ -65,14 +97,15 @@
     "IconPositionHint": 16,  # icon_x & icon_y
     "IconMaskHint": 32,      # icon_mask
     "WindowGroupHint": 64,   # window_group
     "MessageHint": 128,      # (this bit is obsolete)
     "UrgencyHint": 256,      # urgency
 }
 
+# http://standards.freedesktop.org/wm-spec/latest/ar01s05.html#idm139870830002400
 WindowTypes = {
     '_NET_WM_WINDOW_TYPE_DESKTOP': "desktop",
     '_NET_WM_WINDOW_TYPE_DOCK': "dock",
     '_NET_WM_WINDOW_TYPE_TOOLBAR': "toolbar",
     '_NET_WM_WINDOW_TYPE_MENU': "menu",
     '_NET_WM_WINDOW_TYPE_UTILITY': "utility",
     '_NET_WM_WINDOW_TYPE_SPLASH': "splash",
@@ -82,14 +115,15 @@
     '_NET_WM_WINDOW_TYPE_TOOLTIP': "tooltip",
     '_NET_WM_WINDOW_TYPE_NOTIFICATION': "notification",
     '_NET_WM_WINDOW_TYPE_COMBO': "combo",
     '_NET_WM_WINDOW_TYPE_DND': "dnd",
     '_NET_WM_WINDOW_TYPE_NORMAL': "normal",
 }
 
+# http://standards.freedesktop.org/wm-spec/latest/ar01s05.html#idm139870829988448
 WindowStates = {
     None: 'normal',
     '_NET_WM_STATE_FULLSCREEN': 'fullscreen',
 }
 
 # Maps property names to types and formats.
 PropertyMap = {
@@ -126,53 +160,49 @@
 
     # ICCCM
     "WM_STATE": ("WM_STATE", 32),
     # Qtile-specific properties
     "QTILE_INTERNAL": ("CARDINAL", 32)
 }
 
-# TODO add everything required here
-# http://standards.freedesktop.org/wm-spec/1.4/ar01s03.html
+# TODO add everything required here:
+# http://standards.freedesktop.org/wm-spec/latest/ar01s03.html
 SUPPORTED_ATOMS = [
-    '_NET_WM_PID',
-    '_NET_ACTIVE_WINDOW',
-    '_NET_WM_DESKTOP',
-    '_NET_CURRENT_DESKTOP',
+    # From http://standards.freedesktop.org/wm-spec/latest/ar01s03.html
+    '_NET_SUPPORTED',
     '_NET_CLIENT_LIST',
     '_NET_CLIENT_LIST_STACKING',
-    '_NET_SUPPORTED',
-    '_NET_WM_STATE',
-    '_NET_WM_STATE_FULLSCREEN',
+    '_NET_CURRENT_DESKTOP',
+    '_NET_ACTIVE_WINDOW',
+    # '_NET_WORKAREA',
     '_NET_SUPPORTING_WM_CHECK',
+    # From http://standards.freedesktop.org/wm-spec/latest/ar01s05.html
     '_NET_WM_NAME',
+    '_NET_WM_VISIBLE_NAME',
+    '_NET_WM_ICON_NAME',
+    '_NET_WM_DESKTOP',
+    '_NET_WM_WINDOW_TYPE',
+    '_NET_WM_STATE',
     '_NET_WM_STRUT',
     '_NET_WM_STRUT_PARTIAL',
-    '_NET_WM_WINDOW_TYPE',
-    'WM_WINDOW_ROLE',
-    'WM_TAKE_FOCUS',
-    'WM_PROTOCOLS',
-    'WM_DELETE_WINDOW',
-    'UTF8_STRING',
+    '_NET_WM_PID',
 ]
-SUPPORTED_ATOMS += WindowTypes.keys()
+SUPPORTED_ATOMS.extend(WindowTypes.keys())
+SUPPORTED_ATOMS.extend(key for key in WindowStates.keys() if key)
 
 XCB_CONN_ERRORS = {
     1: 'XCB_CONN_ERROR',
     2: 'XCB_CONN_CLOSED_EXT_NOTSUPPORTED',
     3: 'XCB_CONN_CLOSED_MEM_INSUFFICIENT',
     4: 'XCB_CONN_CLOSED_REQ_LEN_EXCEED',
     5: 'XCB_CONN_CLOSED_PARSE_ERR',
     6: 'XCB_CONN_CLOSED_INVALID_SCREEN',
     7: 'XCB_CONN_CLOSED_FDPASSING_FAILED',
 }
 
-def toStr(s):
-    # return "".join([chr(i) for i in s.name])
-    return s.name.to_string()
-
 
 class MaskMap:
     """
         A general utility class that encapsulates the way the mask/value idiom
         works in xpyb. It understands a special attribute _maskvalue on
         objects, which will be used instead of the object value if present.
         This lets us passin a Font object, rather than Font.fid, for example.
@@ -385,57 +415,52 @@
         self.conn.conn.core.SetInputFocus(
             xcffib.xproto.InputFocus.PointerRoot,
             self.wid,
             xcffib.xproto.Time.CurrentTime
         )
 
     def warp_pointer(self, x, y):
+        """
+            Warps the pointer to the location `x`, `y` on the window
+        """
         self.conn.conn.core.WarpPointer(
-            0,
-            self.wid,
-            0,
-            0,
-            0,
-            0,
-            x,
-            y
+            0, self.wid,  # src_window, dst_window
+            0, 0,         # src_x, src_y
+            0, 0,         # src_width, src_height
+            x, y          # dest_x, dest_y
         )
 
     def get_name(self):
         """
             Tries to retrieve a canonical window name. We test the following
-            properties in order of preference: _NET_WM_VISIBLE_NAME,
-            _NET_WM_NAME, WM_NAME.
+            properties in order of preference:
+                - _NET_WM_VISIBLE_NAME
+                - _NET_WM_NAME
+                - WM_NAME.
         """
-        r = self.get_property(
-            "_NET_WM_VISIBLE_NAME",
-            xcffib.xproto.GetPropertyType.Any
-        )
+        r = self.get_property("_NET_WM_VISIBLE_NAME", "UTF8_STRING")
         if r:
             return self._propertyUTF8(r)
 
-        r = self.get_property("_NET_WM_NAME", xcffib.xproto.GetPropertyType.Any)
+        r = self.get_property("_NET_WM_NAME", "UTF8_STRING")
         if r:
             return self._propertyUTF8(r)
 
         r = self.get_property(
             xcffib.xproto.Atom.WM_NAME,
             xcffib.xproto.GetPropertyType.Any
         )
         if r:
             return self._propertyString(r)
 
     def get_wm_hints(self):
         r = self.get_property("WM_HINTS", xcffib.xproto.GetPropertyType.Any)
         if r:
             l = r.value.to_atoms()
-            flags = set()
-            for k, v in HintsFlags.items():
-                if l[0] & v:
-                    flags.add(k)
+            flags = set(k for k, v in HintsFlags.items() if l[0] & v)
             return dict(
                 flags=flags,
                 input=l[1],
                 initial_state=l[2],
                 icon_pixmap=l[3],
                 icon_window=l[4],
                 icon_x=l[5],
@@ -447,18 +472,15 @@
     def get_wm_normal_hints(self):
         r = self.get_property(
             "WM_NORMAL_HINTS",
             xcffib.xproto.GetPropertyType.Any
         )
         if r:
             l = r.value.to_atoms()
-            flags = set()
-            for k, v in NormalHintsFlags.items():
-                if l[0] & v:
-                    flags.add(k)
+            flags = set(k for k, v in NormalHintsFlags.items() if l[0] & v)
             return dict(
                 flags=flags,
                 min_width=l[1 + 4],
                 min_height=l[2 + 4],
                 max_width=l[3 + 4],
                 max_height=l[4 + 4],
                 width_inc=l[5 + 4],
@@ -467,25 +489,19 @@
                 max_aspect=l[8 + 4],
                 base_width=l[9 + 4],
                 base_height=l[9 + 4],
                 win_gravity=l[9 + 4],
             )
 
     def get_wm_protocols(self):
-        r = self.get_property("WM_PROTOCOLS", xcffib.xproto.GetPropertyType.Any)
-        if r:
-            l = r.value.to_atoms()
-            return set([self.conn.atoms.get_name(i) for i in l])
-        else:
-            return set()
+        l = self.get_property("WM_PROTOCOLS", "ATOM", unpack=int)
+        return set(self.conn.atoms.get_name(i) for i in l)
 
     def get_wm_state(self):
-        r = self.get_property("WM_STATE", xcffib.xproto.GetPropertyType.Any)
-        if r:
-            return r.value.to_atoms()
+        return self.get_property("WM_STATE", xcffib.xproto.GetPropertyType.Any, unpack=int)
 
     def get_wm_class(self):
         """
             Return an (instance, class) tuple if WM_CLASS exists, or None.
         """
         r = self.get_property("WM_CLASS", "STRING")
         if r:
@@ -499,22 +515,26 @@
 
     def get_wm_transient_for(self):
         r = self.get_property("WM_TRANSIENT_FOR", "ATOM")
         if r:
             return list(r.value)
 
     def get_wm_icon_name(self):
-        r = self.get_property("WM_ICON_NAME", "UTF8_STRING")
+        r = self.get_property("_NET_WM_ICON_NAME", "UTF8_STRING")
         if r:
-            return self._propertyString(r)
+            return self._propertyUTF8(r)
+
+        r = self.get_property("WM_ICON_NAME", "STRING")
+        if r:
+            return self._propertyUTF8(r)
 
     def get_wm_client_machine(self):
-        r = self.get_property("WM_CLIENT_MACHINE", "UTF8_STRING")
+        r = self.get_property("WM_CLIENT_MACHINE", "STRING")
         if r:
-            return self._propertyString(r)
+            return self._propertyUTF8(r)
 
     def get_geometry(self):
         q = self.conn.conn.core.GetGeometry(self.wid)
         return q.reply()
 
     def get_wm_desktop(self):
         r = self.get_property("_NET_WM_DESKTOP", "CARDINAL", unpack=int)
@@ -584,16 +604,22 @@
             if None in (type, format):
                 raise ValueError(
                     "Must specify type and format for unknown property."
                 )
 
         try:
             if isinstance(value, six.string_types):
-                # xcffib will pack the strings
-                pass
+                # xcffib will pack the bytes, but we should encode them properly
+                if six.PY3:
+                    value = value.encode()
+                elif not isinstance(value, str):
+                    # This will only run for Python 2 unicode strings, can't
+                    # use 'isinstance(value, unicode)' because Py 3 does not
+                    # have unicode and pyflakes complains
+                    value = value.encode('utf-8')
             else:
                 # if this runs without error, the value is already a list, don't wrap it
                 six.next(iter(value))
         except StopIteration:
             # The value was an iterable, just empty
             value = []
         except TypeError:
@@ -811,27 +837,18 @@
 
     def refresh_keymap(self, first=None, count=None):
         if first is None:
             first = self.setup.min_keycode
             count = self.setup.max_keycode - self.setup.min_keycode + 1
         q = self.conn.core.GetKeyboardMapping(first, count).reply()
 
-        l = []
-        for i, v in enumerate(q.keysyms):
-            if not i % q.keysyms_per_keycode:
-                if l:
-                    self.code_to_syms[
-                        (i // q.keysyms_per_keycode) + first - 1
-                    ] = l
-                l = []
-                l.append(v)
-            else:
-                l.append(v)
-        assert len(l) == q.keysyms_per_keycode
-        self.code_to_syms[first + count - 1] = l
+        assert len(q.keysyms) % q.keysyms_per_keycode == 0
+        for i in range(len(q.keysyms) // q.keysyms_per_keycode):
+            self.code_to_syms[first + i] = \
+                q.keysyms[i * q.keysyms_per_keycode:(i + 1) * q.keysyms_per_keycode]
 
         first_sym_to_code = {}
         for k, s in self.code_to_syms.items():
             if s[0] and not s[0] in first_sym_to_code:
                 first_sym_to_code[s[0]] = k
 
         self.first_sym_to_code = first_sym_to_code
@@ -884,35 +901,35 @@
         self._connected = False
 
     def flush(self):
         if self._connected:
             return self.conn.flush()
 
     def xsync(self):
-        # The idea here is that pushing an innocuous request through
-        # the queue and waiting for a response "syncs" the connection, since
-        # requests are serviced in order.
+        # The idea here is that pushing an innocuous request through the queue
+        # and waiting for a response "syncs" the connection, since requests are
+        # serviced in order.
         self.conn.core.GetInputFocus().reply()
 
     def grab_server(self):
         return self.conn.core.GrabServer()
 
     def get_setup(self):
         return self.conn.get_setup()
 
     def open_font(self, name):
         fid = self.conn.generate_id()
         self.conn.core.OpenFont(fid, len(name), name)
         return Font(self, fid)
 
     def extensions(self):
-        return set([
-            toStr(i).lower()
+        return set(
+            i.name.to_string().lower()
             for i in self.conn.core.ListExtensions().reply().names
-        ])
+        )
 
 
 # Stolen from samurai-x
 # (Don't know where to put it, so I'll put it here)
 # XCB cursors doesn't want to be themed, libxcursor
 # would be better choice I think
 # and we (indirectly) depend on it anyway...
```

### Comparing `qtile-0.9.0/libqtile/state.py` & `qtile-0.9.1/libqtile/state.py`

 * *Files identical despite different names*

### Comparing `qtile-0.9.0/qtile.egg-info/PKG-INFO` & `qtile-0.9.1/qtile.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: qtile
-Version: 0.9.0
+Version: 0.9.1
 Summary: A pure-Python tiling window manager.
 Home-page: http://qtile.org
 Author: Tycho Andersen
 Author-email: tycho@tycho.ws
 License: MIT
 Description: 
         A pure-Python tiling window manager.
```

### Comparing `qtile-0.9.0/qtile.egg-info/SOURCES.txt` & `qtile-0.9.1/qtile.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 libqtile/widget/clipboard.py
 libqtile/widget/clock.py
 libqtile/widget/countdown.py
 libqtile/widget/crashme.py
 libqtile/widget/currentlayout.py
 libqtile/widget/debuginfo.py
 libqtile/widget/df.py
+libqtile/widget/generic_poll_text.py
 libqtile/widget/gmail_checker.py
 libqtile/widget/google_calendar.py
 libqtile/widget/graph.py
 libqtile/widget/groupbox.py
 libqtile/widget/image.py
 libqtile/widget/imapwidget.py
 libqtile/widget/keyboardlayout.py
```

