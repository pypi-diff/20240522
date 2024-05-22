# Comparing `tmp/libreflow_launcher-1.0.8.tar.gz` & `tmp/libreflow_launcher-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreflow_launcher-1.0.8.tar", last modified: Thu May 16 10:30:53 2024, max compression
+gzip compressed data, was "libreflow_launcher-1.0.9.tar", last modified: Wed May 22 16:39:45 2024, max compression
```

## Comparing `libreflow_launcher-1.0.8.tar` & `libreflow_launcher-1.0.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:30:53.412345 libreflow_launcher-1.0.8/
--rw-rw-rw-   0 root         (0) root         (0)     2295 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3084 2024-05-16 10:30:53.412345 libreflow_launcher-1.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      839 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-05-16 10:30:53.412345 libreflow_launcher-1.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1691 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:30:53.396345 libreflow_launcher-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:30:53.400345 libreflow_launcher-1.0.8/src/libreflow_launcher/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-16 10:30:53.412345 libreflow_launcher-1.0.8/src/libreflow_launcher/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    21600 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:30:53.401345 libreflow_launcher-1.0.8/src/libreflow_launcher/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:30:53.402345 libreflow_launcher-1.0.8/src/libreflow_launcher/data/servers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/data/servers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1894 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/gui.py
--rw-rw-rw-   0 root         (0) root         (0)     6211 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/model.py
--rw-rw-rw-   0 root         (0) root         (0)     7983 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:30:53.402345 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:30:53.405345 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   503824 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf
--rw-rw-rw-   0 root         (0) root         (0)   445528 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf
--rw-rw-rw-   0 root         (0) root         (0)   579296 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf
--rw-rw-rw-   0 root         (0) root         (0)   528976 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/fonts/OpenSans.ttf
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/fonts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:30:53.406345 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:30:53.410345 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5628 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/arrow-down.png
--rw-rw-rw-   0 root         (0) root         (0)     5667 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/arrow-right.png
--rw-rw-rw-   0 root         (0) root         (0)     1177 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png
--rw-rw-rw-   0 root         (0) root         (0)     9732 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/close.png
--rw-rw-rw-   0 root         (0) root         (0)     9850 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/gitlab.svg
--rw-rw-rw-   0 root         (0) root         (0)     1719 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/kitsu.svg
--rw-rw-rw-   0 root         (0) root         (0)     8760 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/log-out.png
--rw-rw-rw-   0 root         (0) root         (0)     6277 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/log-out_hover.png
--rw-rw-rw-   0 root         (0) root         (0)     6277 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/log-out_normal.png
--rw-rw-rw-   0 root         (0) root         (0)     7267 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/open.png
--rw-rw-rw-   0 root         (0) root         (0)    10491 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/pypi.svg
--rw-rw-rw-   0 root         (0) root         (0)    17905 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/server.png
--rw-rw-rw-   0 root         (0) root         (0)    13119 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/settings.png
--rw-rw-rw-   0 root         (0) root         (0)    19182 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/settings_outline.png
--rw-rw-rw-   0 root         (0) root         (0)     5851 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/start.png
--rw-rw-rw-   0 root         (0) root         (0)     7946 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/trash.png
--rw-rw-rw-   0 root         (0) root         (0)     8358 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/trash_hover.png
--rw-rw-rw-   0 root         (0) root         (0)     7996 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/trash_normal.png
--rw-rw-rw-   0 root         (0) root         (0)    11968 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/user.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:30:53.411345 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/styles/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/styles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:30:53.411345 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/styles/default/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/styles/default/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5049 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/ui/styles/default/default_style.css
--rw-rw-rw-   0 root         (0) root         (0)    57247 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/src/libreflow_launcher/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:30:53.411345 libreflow_launcher-1.0.8/src/libreflow_launcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3084 2024-05-16 10:30:53.000000 libreflow_launcher-1.0.8/src/libreflow_launcher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2191 2024-05-16 10:30:53.000000 libreflow_launcher-1.0.8/src/libreflow_launcher.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 10:30:53.000000 libreflow_launcher-1.0.8/src/libreflow_launcher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-05-16 10:30:53.000000 libreflow_launcher-1.0.8/src/libreflow_launcher.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-16 10:30:53.000000 libreflow_launcher-1.0.8/src/libreflow_launcher.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    86677 2024-05-16 10:30:43.000000 libreflow_launcher-1.0.8/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:39:45.497096 libreflow_launcher-1.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3197 2024-05-22 16:39:45.496096 libreflow_launcher-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      839 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-05-22 16:39:45.497096 libreflow_launcher-1.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1795 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:39:45.479096 libreflow_launcher-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:39:45.484096 libreflow_launcher-1.0.9/src/libreflow_launcher/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-22 16:39:45.497096 libreflow_launcher-1.0.9/src/libreflow_launcher/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    22291 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:39:45.486096 libreflow_launcher-1.0.9/src/libreflow_launcher/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:39:45.486096 libreflow_launcher-1.0.9/src/libreflow_launcher/data/servers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/data/servers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)     6211 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     7983 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:39:45.486096 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:39:45.490096 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   503824 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   445528 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   579296 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   528976 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/fonts/OpenSans.ttf
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/fonts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:39:45.490096 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:39:45.495096 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5628 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/arrow-down.png
+-rw-rw-rw-   0 root         (0) root         (0)     5667 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/arrow-right.png
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png
+-rw-rw-rw-   0 root         (0) root         (0)     9732 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/close.png
+-rw-rw-rw-   0 root         (0) root         (0)     9850 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/gitlab.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/kitsu.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8760 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/log-out.png
+-rw-rw-rw-   0 root         (0) root         (0)     6277 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/log-out_hover.png
+-rw-rw-rw-   0 root         (0) root         (0)     6277 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/log-out_normal.png
+-rw-rw-rw-   0 root         (0) root         (0)     7267 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/open.png
+-rw-rw-rw-   0 root         (0) root         (0)    10491 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/pypi.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17905 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/server.png
+-rw-rw-rw-   0 root         (0) root         (0)    13119 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/settings.png
+-rw-rw-rw-   0 root         (0) root         (0)    19182 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/settings_outline.png
+-rw-rw-rw-   0 root         (0) root         (0)     5851 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/start.png
+-rw-rw-rw-   0 root         (0) root         (0)     7946 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/trash.png
+-rw-rw-rw-   0 root         (0) root         (0)     8358 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/trash_hover.png
+-rw-rw-rw-   0 root         (0) root         (0)     7996 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/trash_normal.png
+-rw-rw-rw-   0 root         (0) root         (0)    11968 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/user.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:39:45.495096 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/styles/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/styles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:39:45.496096 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/styles/default/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/styles/default/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5049 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/ui/styles/default/default_style.css
+-rw-rw-rw-   0 root         (0) root         (0)    57247 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/src/libreflow_launcher/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:39:45.496096 libreflow_launcher-1.0.9/src/libreflow_launcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3197 2024-05-22 16:39:45.000000 libreflow_launcher-1.0.9/src/libreflow_launcher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2191 2024-05-22 16:39:45.000000 libreflow_launcher-1.0.9/src/libreflow_launcher.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 16:39:45.000000 libreflow_launcher-1.0.9/src/libreflow_launcher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-22 16:39:45.000000 libreflow_launcher-1.0.9/src/libreflow_launcher.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-22 16:39:45.000000 libreflow_launcher-1.0.9/src/libreflow_launcher.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    86677 2024-05-22 16:39:35.000000 libreflow_launcher-1.0.9/versioneer.py
```

### Comparing `libreflow_launcher-1.0.8/CHANGELOG.md` & `libreflow_launcher-1.0.9/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [1.0.9] - 2024-05-22
+
+### Added
+
+* MacOS support to manage installation and execution of Libreflow instances
+
 ## [1.0.8] - 2024-05-16
 
 ### Added
 
 * Support project environment variables
 * Issue #9
   * Indentation on user settings json files
```

### Comparing `libreflow_launcher-1.0.8/PKG-INFO` & `libreflow_launcher-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow_launcher
-Version: 1.0.8
+Version: 1.0.9
 Summary: Launcher for instances of Libreflow asset-manager
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow_launcher
 Author: Valentin Braem
 Author-email: valentin.braem@les-fees-speciales.coop
 License: LGPLv3+
 Keywords: kabaret kitsu gazu animation pipeline libreflow launcher lfs overseer asset-manager
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [1.0.9] - 2024-05-22
+
+### Added
+
+* MacOS support to manage installation and execution of Libreflow instances
+
 ## [1.0.8] - 2024-05-16
 
 ### Added
 
 * Support project environment variables
 * Issue #9
   * Indentation on user settings json files
```

### Comparing `libreflow_launcher-1.0.8/README.md` & `libreflow_launcher-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/setup.py` & `libreflow_launcher-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 import setuptools
 import versioneer
 import os
+import platform
 
 readme = os.path.normpath(os.path.join(__file__, '..', 'README.md'))
 with open(readme, "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 long_description += '\n\n'
 
 changelog = os.path.normpath(os.path.join(__file__, '..', 'CHANGELOG.md'))
 with open(changelog, "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
+
+requierements = ["pyside2~=5.0",
+                  "qtpy",
+                  "requests",
+                  "poetry",
+                  "toml"
+                  ]
+if platform.system() == 'Darwin':
+    requierements.extend(["applescript"])
+
 setuptools.setup(
     cmdclass=versioneer.get_cmdclass(),
     name="libreflow_launcher", # Replace with your own username
     version=versioneer.get_version(),
     author="Valentin Braem",
     author_email="valentin.braem@les-fees-speciales.coop",
     description="Launcher for instances of Libreflow asset-manager",
@@ -27,20 +38,15 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
         "Operating System :: OS Independent",
     ],
     keywords="kabaret kitsu gazu animation pipeline libreflow launcher lfs overseer asset-manager",
-    install_requires=["pyside2~=5.0",
-                      "qtpy",
-                      "requests",
-                      "poetry",
-                      "toml"
-                      ],
+    install_requires=requierements,
     python_requires='>=3.7',
     packages=setuptools.find_packages("src"),
     package_dir={"": "src"},
     package_data={
         '': [
             "*.css",
             '*.png',
```

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/controller.py` & `libreflow_launcher-1.0.9/src/libreflow_launcher/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,14 +499,20 @@
                 f.write(' '.join(cmd))
 
         if platform.system() == "Windows":
             subprocess.Popen(exec_path, creationflags=subprocess.CREATE_NEW_CONSOLE)
         elif platform.system() == "Linux":
             subprocess.Popen(('chmod', '+x', exec_path)) 
             subprocess.Popen(('gnome-terminal', '--', exec_path))
+        elif platform.system() == 'Darwin':
+            from applescript import tell
+            macCommand = f'cd {os.path.dirname(exec_path)}; sh {exec_path}'
+            tell.app( 'Terminal', 'do script "' + macCommand + '"')
+        else:
+            print("ERROR os %s not supported" % platform.system())
         
         os.chdir(store_base_path)
 
 
     def fetch_settings(self):
         return self._settings.fetch_settings()
     
@@ -556,17 +562,23 @@
         
         return sorted(versions, key=lambda d: d['version'])
 
     def fetch_poetry_path(self):
         if os.getenv('LF_LAUNCHER_POETRY_PATH', None) is not None:
             self.poetry_path = os.getenv('LF_LAUNCHER_POETRY_PATH')
         elif platform.system() == "Windows":
-            self.poetry_path = f"{pathlib.Path.home()}/AppData/Roaming/Python/Scripts/poetry"
+            self.poetry_path = os.path.normpath(f"{pathlib.Path.home()}/AppData/Roaming/Python/Scripts/poetry.exe")
         elif platform.system() == "Linux":
-            self.poetry_path = f"{pathlib.Path.home()}/.local/bin/poetry"
+            self.poetry_path = os.path.normpath(f"{pathlib.Path.home()}/.local/bin/poetry")
+        elif platform.system() == "Darwin":
+            self.poetry_path = os.path.normpath(f"{pathlib.Path.home()}/Library/Application Support/pypoetry/venv/bin/poetry")
+
+        # test_command = shutil.which(self.poetry_path)
+        # if not test_command:
+        #     print("INFO: Could not find poetry? at %s" % str(self.poetry_path))
 
     def user_settings_folder(self):
         return os.path.join(pathlib.Path.home(), '.libreflow_launcher')
 
     def resolve_value(self, value, project={}):
         resolved = value.format(
             user_settings=self.user_settings_folder(),
```

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/gui.py` & `libreflow_launcher-1.0.9/src/libreflow_launcher/gui.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/model.py` & `libreflow_launcher-1.0.9/src/libreflow_launcher/model.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/resources.py` & `libreflow_launcher-1.0.9/src/libreflow_launcher/resources.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/fonts/OpenSans.ttf` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/fonts/OpenSans.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/arrow-down.png` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/arrow-down.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/arrow-right.png` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/arrow-right.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/close.png` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/close.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/gitlab.svg` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/gitlab.svg`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/kitsu.svg` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/kitsu.svg`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/log-out.png` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/log-out.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/log-out_hover.png` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/log-out_hover.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/log-out_normal.png` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/log-out_normal.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/open.png` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/open.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/pypi.svg` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/pypi.svg`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/server.png` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/server.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/settings.png` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/settings.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/settings_outline.png` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/settings_outline.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/start.png` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/start.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/trash.png` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/trash.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/trash_hover.png` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/trash_hover.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/trash_normal.png` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/trash_normal.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/icons/gui/user.png` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/icons/gui/user.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/ui/styles/default/default_style.css` & `libreflow_launcher-1.0.9/src/libreflow_launcher/ui/styles/default/default_style.css`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher/view.py` & `libreflow_launcher-1.0.9/src/libreflow_launcher/view.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher.egg-info/PKG-INFO` & `libreflow_launcher-1.0.9/src/libreflow_launcher.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow_launcher
-Version: 1.0.8
+Version: 1.0.9
 Summary: Launcher for instances of Libreflow asset-manager
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow_launcher
 Author: Valentin Braem
 Author-email: valentin.braem@les-fees-speciales.coop
 License: LGPLv3+
 Keywords: kabaret kitsu gazu animation pipeline libreflow launcher lfs overseer asset-manager
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [1.0.9] - 2024-05-22
+
+### Added
+
+* MacOS support to manage installation and execution of Libreflow instances
+
 ## [1.0.8] - 2024-05-16
 
 ### Added
 
 * Support project environment variables
 * Issue #9
   * Indentation on user settings json files
```

### Comparing `libreflow_launcher-1.0.8/src/libreflow_launcher.egg-info/SOURCES.txt` & `libreflow_launcher-1.0.9/src/libreflow_launcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.8/versioneer.py` & `libreflow_launcher-1.0.9/versioneer.py`

 * *Files identical despite different names*

