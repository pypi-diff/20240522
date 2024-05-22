# Comparing `tmp/tentacletk-0.9.8.tar.gz` & `tmp/tentacletk-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tentacletk-0.9.8.tar", last modified: Sun Dec 17 23:29:16 2023, max compression
+gzip compressed data, was "tentacletk-0.9.9.tar", last modified: Wed Dec 20 15:33:05 2023, max compression
```

## Comparing `tentacletk-0.9.8.tar` & `tentacletk-0.9.9.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxrwxrwx   0        0        0        0 2023-12-17 23:29:16.986529 tentacletk-0.9.8/
--rw-rw-rw-   0        0        0     7815 2023-04-16 12:18:04.000000 tentacletk-0.9.8/COPYING.LESSER
--rw-rw-rw-   0        0        0       24 2023-09-06 12:44:05.000000 tentacletk-0.9.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3723 2023-12-17 23:29:16.985525 tentacletk-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-12-17 23:29:16.986529 tentacletk-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1549 2023-12-17 22:46:39.000000 tentacletk-0.9.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-17 23:29:16.861634 tentacletk-0.9.8/tentacle/
--rw-rw-rw-   0        0        0     1553 2023-12-17 23:29:12.000000 tentacletk-0.9.8/tentacle/__init__.py
--rw-rw-rw-   0        0        0    14612 2023-09-18 18:03:25.000000 tentacletk-0.9.8/tentacle/overlay.py
-drwxrwxrwx   0        0        0        0 2023-12-17 23:29:16.861634 tentacletk-0.9.8/tentacle/slots/
--rw-rw-rw-   0        0        0     1757 2023-11-07 15:42:46.000000 tentacletk-0.9.8/tentacle/slots/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-17 23:29:16.884660 tentacletk-0.9.8/tentacle/slots/maya/
--rw-rw-rw-   0        0        0      608 2023-11-07 15:24:19.000000 tentacletk-0.9.8/tentacle/slots/maya/__init__.py
--rw-rw-rw-   0        0        0     5859 2023-12-10 18:55:19.000000 tentacletk-0.9.8/tentacle/slots/maya/animation.py
--rw-rw-rw-   0        0        0     8355 2023-10-03 14:15:12.000000 tentacletk-0.9.8/tentacle/slots/maya/cameras.py
--rw-rw-rw-   0        0        0     4281 2023-11-06 16:13:22.000000 tentacletk-0.9.8/tentacle/slots/maya/convert.py
--rw-rw-rw-   0        0        0     2904 2023-12-14 21:09:48.000000 tentacletk-0.9.8/tentacle/slots/maya/crease.py
--rw-rw-rw-   0        0        0     9703 2023-09-06 12:44:05.000000 tentacletk-0.9.8/tentacle/slots/maya/create.py
--rw-rw-rw-   0        0        0      531 2023-09-06 12:44:05.000000 tentacletk-0.9.8/tentacle/slots/maya/deformation.py
--rw-rw-rw-   0        0        0     5031 2023-11-09 02:25:30.000000 tentacletk-0.9.8/tentacle/slots/maya/display.py
--rw-rw-rw-   0        0        0     3226 2023-10-23 15:52:33.000000 tentacletk-0.9.8/tentacle/slots/maya/duplicate.py
--rw-rw-rw-   0        0        0    16099 2023-11-08 12:58:42.000000 tentacletk-0.9.8/tentacle/slots/maya/edit.py
--rw-rw-rw-   0        0        0    11666 2023-10-11 15:40:49.000000 tentacletk-0.9.8/tentacle/slots/maya/editors.py
--rw-rw-rw-   0        0        0     9413 2023-12-17 16:36:46.000000 tentacletk-0.9.8/tentacle/slots/maya/file.py
--rw-rw-rw-   0        0        0     6860 2023-09-06 12:44:05.000000 tentacletk-0.9.8/tentacle/slots/maya/init.py
--rw-rw-rw-   0        0        0      626 2023-09-06 12:44:05.000000 tentacletk-0.9.8/tentacle/slots/maya/lighting.py
--rw-rw-rw-   0        0        0     1663 2023-10-03 14:15:57.000000 tentacletk-0.9.8/tentacle/slots/maya/main.py
--rw-rw-rw-   0        0        0     9987 2023-10-24 22:16:45.000000 tentacletk-0.9.8/tentacle/slots/maya/materials.py
--rw-rw-rw-   0        0        0     7893 2023-11-15 17:22:57.000000 tentacletk-0.9.8/tentacle/slots/maya/normals.py
--rw-rw-rw-   0        0        0    30556 2023-10-24 23:07:00.000000 tentacletk-0.9.8/tentacle/slots/maya/nurbs.py
--rw-rw-rw-   0        0        0     3853 2023-10-23 14:26:15.000000 tentacletk-0.9.8/tentacle/slots/maya/pivot.py
--rw-rw-rw-   0        0        0    20904 2023-10-29 12:57:23.000000 tentacletk-0.9.8/tentacle/slots/maya/polygons.py
--rw-rw-rw-   0        0        0     5005 2023-12-17 19:40:35.000000 tentacletk-0.9.8/tentacle/slots/maya/preferences.py
--rw-rw-rw-   0        0        0     3471 2023-10-24 13:34:24.000000 tentacletk-0.9.8/tentacle/slots/maya/rendering.py
--rw-rw-rw-   0        0        0    18130 2023-10-24 23:07:16.000000 tentacletk-0.9.8/tentacle/slots/maya/rigging.py
--rw-rw-rw-   0        0        0     4632 2023-10-11 13:52:04.000000 tentacletk-0.9.8/tentacle/slots/maya/scene.py
--rw-rw-rw-   0        0        0    22495 2023-11-23 14:16:46.000000 tentacletk-0.9.8/tentacle/slots/maya/selection.py
--rw-rw-rw-   0        0        0     6432 2023-10-24 23:07:45.000000 tentacletk-0.9.8/tentacle/slots/maya/subdivision.py
--rw-rw-rw-   0        0        0     2486 2023-10-23 14:26:15.000000 tentacletk-0.9.8/tentacle/slots/maya/symmetry.py
--rw-rw-rw-   0        0        0    16213 2023-11-15 14:21:00.000000 tentacletk-0.9.8/tentacle/slots/maya/transform.py
--rw-rw-rw-   0        0        0      954 2023-09-06 12:44:06.000000 tentacletk-0.9.8/tentacle/slots/maya/utilities.py
--rw-rw-rw-   0        0        0    24991 2023-11-10 18:16:54.000000 tentacletk-0.9.8/tentacle/slots/maya/uv.py
--rw-rw-rw-   0        0        0      621 2023-09-06 12:44:06.000000 tentacletk-0.9.8/tentacle/slots/maya/vfx.py
--rw-rw-rw-   0        0        0    22206 2023-12-17 15:06:24.000000 tentacletk-0.9.8/tentacle/tcl.py
--rw-rw-rw-   0        0        0     2354 2023-12-13 14:18:39.000000 tentacletk-0.9.8/tentacle/tcl_blender.py
--rw-rw-rw-   0        0        0     3132 2023-12-13 14:19:46.000000 tentacletk-0.9.8/tentacle/tcl_max.py
--rw-rw-rw-   0        0        0     1631 2023-12-13 14:17:16.000000 tentacletk-0.9.8/tentacle/tcl_maya.py
-drwxrwxrwx   0        0        0        0 2023-12-17 23:29:16.941273 tentacletk-0.9.8/tentacle/ui/
--rw-rw-rw-   0        0        0      514 2023-09-18 18:03:25.000000 tentacletk-0.9.8/tentacle/ui/__init__.py
--rw-rw-rw-   0        0        0     6509 2023-09-18 18:03:25.000000 tentacletk-0.9.8/tentacle/ui/animation#submenu.ui
--rw-rw-rw-   0        0        0    10216 2023-12-10 18:51:08.000000 tentacletk-0.9.8/tentacle/ui/animation.ui
--rw-rw-rw-   0        0        0     3539 2023-09-06 12:44:06.000000 tentacletk-0.9.8/tentacle/ui/cameras#lower#submenu.ui
--rw-rw-rw-   0        0        0    15922 2023-10-23 14:26:15.000000 tentacletk-0.9.8/tentacle/ui/cameras#startmenu.ui
--rw-rw-rw-   0        0        0     5596 2023-09-18 18:03:25.000000 tentacletk-0.9.8/tentacle/ui/convert#submenu.ui
--rw-rw-rw-   0        0        0     4359 2023-10-04 16:04:17.000000 tentacletk-0.9.8/tentacle/ui/convert.ui
--rw-rw-rw-   0        0        0     3755 2023-12-14 17:32:46.000000 tentacletk-0.9.8/tentacle/ui/crease#submenu.ui
--rw-rw-rw-   0        0        0     8158 2023-12-14 17:32:35.000000 tentacletk-0.9.8/tentacle/ui/crease.ui
--rw-rw-rw-   0        0        0     5843 2023-09-18 18:03:25.000000 tentacletk-0.9.8/tentacle/ui/create#submenu.ui
--rw-rw-rw-   0        0        0     9164 2023-10-04 16:08:18.000000 tentacletk-0.9.8/tentacle/ui/create.ui
--rw-rw-rw-   0        0        0     2684 2023-09-18 18:03:25.000000 tentacletk-0.9.8/tentacle/ui/deformation#submenu.ui
--rw-rw-rw-   0        0        0     4440 2023-10-04 16:12:14.000000 tentacletk-0.9.8/tentacle/ui/deformation.ui
--rw-rw-rw-   0        0        0     6613 2023-10-23 14:26:15.000000 tentacletk-0.9.8/tentacle/ui/display#submenu.ui
--rw-rw-rw-   0        0        0    12538 2023-10-23 14:26:15.000000 tentacletk-0.9.8/tentacle/ui/display.ui
--rw-rw-rw-   0        0        0    11053 2023-10-23 14:26:15.000000 tentacletk-0.9.8/tentacle/ui/duplicate#submenu.ui
--rw-rw-rw-   0        0        0    10050 2023-10-23 14:26:15.000000 tentacletk-0.9.8/tentacle/ui/duplicate.ui
--rw-rw-rw-   0        0        0    10050 2023-11-08 14:23:54.000000 tentacletk-0.9.8/tentacle/ui/edit#submenu.ui
--rw-rw-rw-   0        0        0    20019 2023-11-08 11:39:01.000000 tentacletk-0.9.8/tentacle/ui/edit.ui
--rw-rw-rw-   0        0        0     3636 2023-09-06 12:44:06.000000 tentacletk-0.9.8/tentacle/ui/editors#lower#submenu.ui
--rw-rw-rw-   0        0        0    12338 2023-09-18 18:03:25.000000 tentacletk-0.9.8/tentacle/ui/editors#startmenu.ui
--rw-rw-rw-   0        0        0     5487 2023-11-09 00:25:14.000000 tentacletk-0.9.8/tentacle/ui/file#submenu.ui
--rw-rw-rw-   0        0        0    10454 2023-10-23 14:26:15.000000 tentacletk-0.9.8/tentacle/ui/file.ui
-drwxrwxrwx   0        0        0        0 2023-12-17 23:29:16.943829 tentacletk-0.9.8/tentacle/ui/icons/
--rw-rw-rw-   0        0        0     1492 2023-09-06 12:44:06.000000 tentacletk-0.9.8/tentacle/ui/icons/Dolly Mode.png
--rw-rw-rw-   0        0        0     1679 2023-09-06 12:44:06.000000 tentacletk-0.9.8/tentacle/ui/icons/Orbit View Mode.png
--rw-rw-rw-   0        0        0     1403 2023-09-06 12:44:06.000000 tentacletk-0.9.8/tentacle/ui/icons/Pan Non-Camera View Mode.png
--rw-rw-rw-   0        0        0     3861 2023-09-06 12:44:06.000000 tentacletk-0.9.8/tentacle/ui/icons/Select and Rotate.png
--rw-rw-rw-   0        0        0     5565 2023-09-18 18:03:25.000000 tentacletk-0.9.8/tentacle/ui/init#startmenu.ui
--rw-rw-rw-   0        0        0     2682 2023-09-18 18:03:25.000000 tentacletk-0.9.8/tentacle/ui/lighting#submenu.ui
--rw-rw-rw-   0        0        0     4434 2023-10-04 16:05:08.000000 tentacletk-0.9.8/tentacle/ui/lighting.ui
--rw-rw-rw-   0        0        0     3630 2023-09-06 12:44:06.000000 tentacletk-0.9.8/tentacle/ui/main#lower#submenu.ui
--rw-rw-rw-   0        0        0    12608 2023-10-23 14:26:15.000000 tentacletk-0.9.8/tentacle/ui/main#startmenu.ui
--rw-rw-rw-   0        0        0     8362 2023-10-23 16:24:09.000000 tentacletk-0.9.8/tentacle/ui/materials#submenu.ui
--rw-rw-rw-   0        0        0    10631 2023-10-13 02:50:55.000000 tentacletk-0.9.8/tentacle/ui/materials.ui
--rw-rw-rw-   0        0        0     7867 2023-09-18 18:03:25.000000 tentacletk-0.9.8/tentacle/ui/normals#submenu.ui
--rw-rw-rw-   0        0        0    15831 2023-10-04 16:07:45.000000 tentacletk-0.9.8/tentacle/ui/normals.ui
--rw-rw-rw-   0        0        0    10681 2023-09-18 18:03:25.000000 tentacletk-0.9.8/tentacle/ui/nurbs#submenu.ui
--rw-rw-rw-   0        0        0    34110 2023-10-04 16:05:01.000000 tentacletk-0.9.8/tentacle/ui/nurbs.ui
--rw-rw-rw-   0        0        0     7188 2023-10-23 14:26:15.000000 tentacletk-0.9.8/tentacle/ui/pivot#submenu.ui
--rw-rw-rw-   0        0        0     6377 2023-10-04 16:11:59.000000 tentacletk-0.9.8/tentacle/ui/pivot.ui
--rw-rw-rw-   0        0        0    15520 2023-10-23 14:26:15.000000 tentacletk-0.9.8/tentacle/ui/polygons#component#submenu.ui
--rw-rw-rw-   0        0        0     5016 2023-09-06 12:44:06.000000 tentacletk-0.9.8/tentacle/ui/polygons#edge#submenu.ui
--rw-rw-rw-   0        0        0     5323 2023-09-06 12:44:06.000000 tentacletk-0.9.8/tentacle/ui/polygons#face#submenu.ui
--rw-rw-rw-   0        0        0     6146 2023-10-23 14:26:15.000000 tentacletk-0.9.8/tentacle/ui/polygons#mesh#submenu.ui
--rw-rw-rw-   0        0        0     5874 2023-10-24 12:11:59.000000 tentacletk-0.9.8/tentacle/ui/polygons#submenu.ui
--rw-rw-rw-   0        0        0     5312 2023-09-12 18:43:04.000000 tentacletk-0.9.8/tentacle/ui/polygons#vertex#submenu.ui
--rw-rw-rw-   0        0        0    47868 2023-10-04 16:39:38.000000 tentacletk-0.9.8/tentacle/ui/polygons.ui
--rw-rw-rw-   0        0        0     4547 2023-09-18 18:03:25.000000 tentacletk-0.9.8/tentacle/ui/preferences#submenu.ui
--rw-rw-rw-   0        0        0    13278 2023-12-17 16:47:41.000000 tentacletk-0.9.8/tentacle/ui/preferences.ui
--rw-rw-rw-   0        0        0     3462 2023-09-18 18:03:25.000000 tentacletk-0.9.8/tentacle/ui/rendering#submenu.ui
--rw-rw-rw-   0        0        0    10912 2023-10-04 16:12:29.000000 tentacletk-0.9.8/tentacle/ui/rendering.ui
--rw-rw-rw-   0        0        0     7450 2023-09-18 18:03:25.000000 tentacletk-0.9.8/tentacle/ui/rigging#submenu.ui
--rw-rw-rw-   0        0        0    20295 2023-10-04 16:12:43.000000 tentacletk-0.9.8/tentacle/ui/rigging.ui
--rw-rw-rw-   0        0        0     7631 2023-10-23 14:26:15.000000 tentacletk-0.9.8/tentacle/ui/scene#submenu.ui
--rw-rw-rw-   0        0        0    10303 2023-10-04 16:01:23.000000 tentacletk-0.9.8/tentacle/ui/scene.ui
--rw-rw-rw-   0        0        0     9784 2023-10-23 14:26:15.000000 tentacletk-0.9.8/tentacle/ui/selection#submenu.ui
--rw-rw-rw-   0        0        0    12348 2023-10-23 14:26:15.000000 tentacletk-0.9.8/tentacle/ui/selection.ui
--rw-rw-rw-   0        0        0     7692 2023-10-10 18:12:46.000000 tentacletk-0.9.8/tentacle/ui/subdivision#submenu.ui
--rw-rw-rw-   0        0        0    11766 2023-10-10 18:05:55.000000 tentacletk-0.9.8/tentacle/ui/subdivision.ui
--rw-rw-rw-   0        0        0     5199 2023-09-18 18:03:25.000000 tentacletk-0.9.8/tentacle/ui/symmetry#submenu.ui
--rw-rw-rw-   0        0        0     8873 2023-10-04 16:12:35.000000 tentacletk-0.9.8/tentacle/ui/symmetry.ui
--rw-rw-rw-   0        0        0    13382 2023-11-15 14:21:11.000000 tentacletk-0.9.8/tentacle/ui/transform#submenu.ui
--rw-rw-rw-   0        0        0     6891 2023-10-04 16:08:09.000000 tentacletk-0.9.8/tentacle/ui/transform.constrain.ui
--rw-rw-rw-   0        0        0     4495 2023-10-04 16:04:01.000000 tentacletk-0.9.8/tentacle/ui/transform.snap.ui
--rw-rw-rw-   0        0        0    20267 2023-10-23 14:26:15.000000 tentacletk-0.9.8/tentacle/ui/transform.ui
--rw-rw-rw-   0        0        0     2776 2023-09-18 18:03:25.000000 tentacletk-0.9.8/tentacle/ui/utilities#submenu.ui
--rw-rw-rw-   0        0        0     7470 2023-10-04 16:04:44.000000 tentacletk-0.9.8/tentacle/ui/utilities.ui
--rw-rw-rw-   0        0        0     6866 2023-09-18 18:03:25.000000 tentacletk-0.9.8/tentacle/ui/uv#submenu.ui
--rw-rw-rw-   0        0        0    35970 2023-11-10 17:45:16.000000 tentacletk-0.9.8/tentacle/ui/uv.ui
--rw-rw-rw-   0        0        0     2672 2023-09-18 18:03:25.000000 tentacletk-0.9.8/tentacle/ui/vfx#submenu.ui
--rw-rw-rw-   0        0        0     4044 2023-10-04 16:01:55.000000 tentacletk-0.9.8/tentacle/ui/vfx.ui
-drwxrwxrwx   0        0        0        0 2023-12-17 23:29:16.985525 tentacletk-0.9.8/tentacletk.egg-info/
--rw-rw-rw-   0        0        0     3723 2023-12-17 23:29:16.000000 tentacletk-0.9.8/tentacletk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3404 2023-12-17 23:29:16.000000 tentacletk-0.9.8/tentacletk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-17 23:29:16.000000 tentacletk-0.9.8/tentacletk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-12-17 23:29:16.000000 tentacletk-0.9.8/tentacletk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-12-17 23:29:16.000000 tentacletk-0.9.8/tentacletk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-12-20 15:33:05.683218 tentacletk-0.9.9/
+-rw-rw-rw-   0        0        0     7815 2023-04-16 12:18:04.000000 tentacletk-0.9.9/COPYING.LESSER
+-rw-rw-rw-   0        0        0       24 2023-09-06 12:44:05.000000 tentacletk-0.9.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3735 2023-12-20 15:33:05.682221 tentacletk-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-12-20 15:33:05.683218 tentacletk-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1549 2023-12-17 22:46:39.000000 tentacletk-0.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-20 15:33:04.649386 tentacletk-0.9.9/tentacle/
+-rw-rw-rw-   0        0        0     1553 2023-12-20 15:32:57.000000 tentacletk-0.9.9/tentacle/__init__.py
+-rw-rw-rw-   0        0        0    14612 2023-09-18 18:03:25.000000 tentacletk-0.9.9/tentacle/overlay.py
+drwxrwxrwx   0        0        0        0 2023-12-20 15:33:04.657384 tentacletk-0.9.9/tentacle/slots/
+-rw-rw-rw-   0        0        0     1757 2023-11-07 15:42:46.000000 tentacletk-0.9.9/tentacle/slots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-20 15:33:05.102437 tentacletk-0.9.9/tentacle/slots/maya/
+-rw-rw-rw-   0        0        0      608 2023-11-07 15:24:19.000000 tentacletk-0.9.9/tentacle/slots/maya/__init__.py
+-rw-rw-rw-   0        0        0     5851 2023-12-18 13:48:05.000000 tentacletk-0.9.9/tentacle/slots/maya/animation.py
+-rw-rw-rw-   0        0        0     8355 2023-10-03 14:15:12.000000 tentacletk-0.9.9/tentacle/slots/maya/cameras.py
+-rw-rw-rw-   0        0        0     4281 2023-11-06 16:13:22.000000 tentacletk-0.9.9/tentacle/slots/maya/convert.py
+-rw-rw-rw-   0        0        0     2904 2023-12-14 21:09:48.000000 tentacletk-0.9.9/tentacle/slots/maya/crease.py
+-rw-rw-rw-   0        0        0     9703 2023-09-06 12:44:05.000000 tentacletk-0.9.9/tentacle/slots/maya/create.py
+-rw-rw-rw-   0        0        0      531 2023-09-06 12:44:05.000000 tentacletk-0.9.9/tentacle/slots/maya/deformation.py
+-rw-rw-rw-   0        0        0     5031 2023-11-09 02:25:30.000000 tentacletk-0.9.9/tentacle/slots/maya/display.py
+-rw-rw-rw-   0        0        0     3226 2023-10-23 15:52:33.000000 tentacletk-0.9.9/tentacle/slots/maya/duplicate.py
+-rw-rw-rw-   0        0        0    16099 2023-11-08 12:58:42.000000 tentacletk-0.9.9/tentacle/slots/maya/edit.py
+-rw-rw-rw-   0        0        0    11666 2023-10-11 15:40:49.000000 tentacletk-0.9.9/tentacle/slots/maya/editors.py
+-rw-rw-rw-   0        0        0     9468 2023-12-19 15:25:09.000000 tentacletk-0.9.9/tentacle/slots/maya/file.py
+-rw-rw-rw-   0        0        0     6860 2023-09-06 12:44:05.000000 tentacletk-0.9.9/tentacle/slots/maya/init.py
+-rw-rw-rw-   0        0        0      626 2023-09-06 12:44:05.000000 tentacletk-0.9.9/tentacle/slots/maya/lighting.py
+-rw-rw-rw-   0        0        0     1663 2023-10-03 14:15:57.000000 tentacletk-0.9.9/tentacle/slots/maya/main.py
+-rw-rw-rw-   0        0        0     9987 2023-10-24 22:16:45.000000 tentacletk-0.9.9/tentacle/slots/maya/materials.py
+-rw-rw-rw-   0        0        0     7893 2023-11-15 17:22:57.000000 tentacletk-0.9.9/tentacle/slots/maya/normals.py
+-rw-rw-rw-   0        0        0    30556 2023-10-24 23:07:00.000000 tentacletk-0.9.9/tentacle/slots/maya/nurbs.py
+-rw-rw-rw-   0        0        0     3853 2023-10-23 14:26:15.000000 tentacletk-0.9.9/tentacle/slots/maya/pivot.py
+-rw-rw-rw-   0        0        0    20904 2023-10-29 12:57:23.000000 tentacletk-0.9.9/tentacle/slots/maya/polygons.py
+-rw-rw-rw-   0        0        0     5005 2023-12-17 19:40:35.000000 tentacletk-0.9.9/tentacle/slots/maya/preferences.py
+-rw-rw-rw-   0        0        0     3471 2023-10-24 13:34:24.000000 tentacletk-0.9.9/tentacle/slots/maya/rendering.py
+-rw-rw-rw-   0        0        0    18130 2023-10-24 23:07:16.000000 tentacletk-0.9.9/tentacle/slots/maya/rigging.py
+-rw-rw-rw-   0        0        0     4820 2023-12-20 14:28:40.000000 tentacletk-0.9.9/tentacle/slots/maya/scene.py
+-rw-rw-rw-   0        0        0    22495 2023-11-23 14:16:46.000000 tentacletk-0.9.9/tentacle/slots/maya/selection.py
+-rw-rw-rw-   0        0        0     6432 2023-10-24 23:07:45.000000 tentacletk-0.9.9/tentacle/slots/maya/subdivision.py
+-rw-rw-rw-   0        0        0     2486 2023-10-23 14:26:15.000000 tentacletk-0.9.9/tentacle/slots/maya/symmetry.py
+-rw-rw-rw-   0        0        0    16213 2023-11-15 14:21:00.000000 tentacletk-0.9.9/tentacle/slots/maya/transform.py
+-rw-rw-rw-   0        0        0      954 2023-09-06 12:44:06.000000 tentacletk-0.9.9/tentacle/slots/maya/utilities.py
+-rw-rw-rw-   0        0        0    24991 2023-11-10 18:16:54.000000 tentacletk-0.9.9/tentacle/slots/maya/uv.py
+-rw-rw-rw-   0        0        0      621 2023-09-06 12:44:06.000000 tentacletk-0.9.9/tentacle/slots/maya/vfx.py
+-rw-rw-rw-   0        0        0    22206 2023-12-17 15:06:24.000000 tentacletk-0.9.9/tentacle/tcl.py
+-rw-rw-rw-   0        0        0     2354 2023-12-13 14:18:39.000000 tentacletk-0.9.9/tentacle/tcl_blender.py
+-rw-rw-rw-   0        0        0     3132 2023-12-13 14:19:46.000000 tentacletk-0.9.9/tentacle/tcl_max.py
+-rw-rw-rw-   0        0        0     1631 2023-12-13 14:17:16.000000 tentacletk-0.9.9/tentacle/tcl_maya.py
+drwxrwxrwx   0        0        0        0 2023-12-20 15:33:05.609853 tentacletk-0.9.9/tentacle/ui/
+-rw-rw-rw-   0        0        0      514 2023-09-18 18:03:25.000000 tentacletk-0.9.9/tentacle/ui/__init__.py
+-rw-rw-rw-   0        0        0     6509 2023-09-18 18:03:25.000000 tentacletk-0.9.9/tentacle/ui/animation#submenu.ui
+-rw-rw-rw-   0        0        0    10216 2023-12-10 18:51:08.000000 tentacletk-0.9.9/tentacle/ui/animation.ui
+-rw-rw-rw-   0        0        0     3539 2023-09-06 12:44:06.000000 tentacletk-0.9.9/tentacle/ui/cameras#lower#submenu.ui
+-rw-rw-rw-   0        0        0    15922 2023-10-23 14:26:15.000000 tentacletk-0.9.9/tentacle/ui/cameras#startmenu.ui
+-rw-rw-rw-   0        0        0     5596 2023-09-18 18:03:25.000000 tentacletk-0.9.9/tentacle/ui/convert#submenu.ui
+-rw-rw-rw-   0        0        0     4359 2023-10-04 16:04:17.000000 tentacletk-0.9.9/tentacle/ui/convert.ui
+-rw-rw-rw-   0        0        0     3755 2023-12-14 17:32:46.000000 tentacletk-0.9.9/tentacle/ui/crease#submenu.ui
+-rw-rw-rw-   0        0        0     8158 2023-12-14 17:32:35.000000 tentacletk-0.9.9/tentacle/ui/crease.ui
+-rw-rw-rw-   0        0        0     5843 2023-09-18 18:03:25.000000 tentacletk-0.9.9/tentacle/ui/create#submenu.ui
+-rw-rw-rw-   0        0        0     9164 2023-10-04 16:08:18.000000 tentacletk-0.9.9/tentacle/ui/create.ui
+-rw-rw-rw-   0        0        0     2684 2023-09-18 18:03:25.000000 tentacletk-0.9.9/tentacle/ui/deformation#submenu.ui
+-rw-rw-rw-   0        0        0     4440 2023-10-04 16:12:14.000000 tentacletk-0.9.9/tentacle/ui/deformation.ui
+-rw-rw-rw-   0        0        0     6613 2023-10-23 14:26:15.000000 tentacletk-0.9.9/tentacle/ui/display#submenu.ui
+-rw-rw-rw-   0        0        0    12538 2023-10-23 14:26:15.000000 tentacletk-0.9.9/tentacle/ui/display.ui
+-rw-rw-rw-   0        0        0    11053 2023-10-23 14:26:15.000000 tentacletk-0.9.9/tentacle/ui/duplicate#submenu.ui
+-rw-rw-rw-   0        0        0    10050 2023-10-23 14:26:15.000000 tentacletk-0.9.9/tentacle/ui/duplicate.ui
+-rw-rw-rw-   0        0        0    10050 2023-11-08 14:23:54.000000 tentacletk-0.9.9/tentacle/ui/edit#submenu.ui
+-rw-rw-rw-   0        0        0    20019 2023-11-08 11:39:01.000000 tentacletk-0.9.9/tentacle/ui/edit.ui
+-rw-rw-rw-   0        0        0     3636 2023-09-06 12:44:06.000000 tentacletk-0.9.9/tentacle/ui/editors#lower#submenu.ui
+-rw-rw-rw-   0        0        0    12338 2023-09-18 18:03:25.000000 tentacletk-0.9.9/tentacle/ui/editors#startmenu.ui
+-rw-rw-rw-   0        0        0     5487 2023-11-09 00:25:14.000000 tentacletk-0.9.9/tentacle/ui/file#submenu.ui
+-rw-rw-rw-   0        0        0    10986 2023-12-19 13:33:17.000000 tentacletk-0.9.9/tentacle/ui/file.ui
+drwxrwxrwx   0        0        0        0 2023-12-20 15:33:05.640136 tentacletk-0.9.9/tentacle/ui/icons/
+-rw-rw-rw-   0        0        0     1492 2023-09-06 12:44:06.000000 tentacletk-0.9.9/tentacle/ui/icons/Dolly Mode.png
+-rw-rw-rw-   0        0        0     1679 2023-09-06 12:44:06.000000 tentacletk-0.9.9/tentacle/ui/icons/Orbit View Mode.png
+-rw-rw-rw-   0        0        0     1403 2023-09-06 12:44:06.000000 tentacletk-0.9.9/tentacle/ui/icons/Pan Non-Camera View Mode.png
+-rw-rw-rw-   0        0        0     3861 2023-09-06 12:44:06.000000 tentacletk-0.9.9/tentacle/ui/icons/Select and Rotate.png
+-rw-rw-rw-   0        0        0     5565 2023-09-18 18:03:25.000000 tentacletk-0.9.9/tentacle/ui/init#startmenu.ui
+-rw-rw-rw-   0        0        0     2682 2023-09-18 18:03:25.000000 tentacletk-0.9.9/tentacle/ui/lighting#submenu.ui
+-rw-rw-rw-   0        0        0     4434 2023-10-04 16:05:08.000000 tentacletk-0.9.9/tentacle/ui/lighting.ui
+-rw-rw-rw-   0        0        0     3630 2023-09-06 12:44:06.000000 tentacletk-0.9.9/tentacle/ui/main#lower#submenu.ui
+-rw-rw-rw-   0        0        0    12608 2023-10-23 14:26:15.000000 tentacletk-0.9.9/tentacle/ui/main#startmenu.ui
+-rw-rw-rw-   0        0        0     8362 2023-10-23 16:24:09.000000 tentacletk-0.9.9/tentacle/ui/materials#submenu.ui
+-rw-rw-rw-   0        0        0    10631 2023-10-13 02:50:55.000000 tentacletk-0.9.9/tentacle/ui/materials.ui
+-rw-rw-rw-   0        0        0     7867 2023-09-18 18:03:25.000000 tentacletk-0.9.9/tentacle/ui/normals#submenu.ui
+-rw-rw-rw-   0        0        0    15831 2023-10-04 16:07:45.000000 tentacletk-0.9.9/tentacle/ui/normals.ui
+-rw-rw-rw-   0        0        0    10681 2023-09-18 18:03:25.000000 tentacletk-0.9.9/tentacle/ui/nurbs#submenu.ui
+-rw-rw-rw-   0        0        0    34110 2023-10-04 16:05:01.000000 tentacletk-0.9.9/tentacle/ui/nurbs.ui
+-rw-rw-rw-   0        0        0     7188 2023-10-23 14:26:15.000000 tentacletk-0.9.9/tentacle/ui/pivot#submenu.ui
+-rw-rw-rw-   0        0        0     6377 2023-10-04 16:11:59.000000 tentacletk-0.9.9/tentacle/ui/pivot.ui
+-rw-rw-rw-   0        0        0    15520 2023-10-23 14:26:15.000000 tentacletk-0.9.9/tentacle/ui/polygons#component#submenu.ui
+-rw-rw-rw-   0        0        0     5016 2023-09-06 12:44:06.000000 tentacletk-0.9.9/tentacle/ui/polygons#edge#submenu.ui
+-rw-rw-rw-   0        0        0     5323 2023-09-06 12:44:06.000000 tentacletk-0.9.9/tentacle/ui/polygons#face#submenu.ui
+-rw-rw-rw-   0        0        0     6146 2023-10-23 14:26:15.000000 tentacletk-0.9.9/tentacle/ui/polygons#mesh#submenu.ui
+-rw-rw-rw-   0        0        0     5874 2023-10-24 12:11:59.000000 tentacletk-0.9.9/tentacle/ui/polygons#submenu.ui
+-rw-rw-rw-   0        0        0     5312 2023-09-12 18:43:04.000000 tentacletk-0.9.9/tentacle/ui/polygons#vertex#submenu.ui
+-rw-rw-rw-   0        0        0    47868 2023-10-04 16:39:38.000000 tentacletk-0.9.9/tentacle/ui/polygons.ui
+-rw-rw-rw-   0        0        0     4547 2023-09-18 18:03:25.000000 tentacletk-0.9.9/tentacle/ui/preferences#submenu.ui
+-rw-rw-rw-   0        0        0    13278 2023-12-17 16:47:41.000000 tentacletk-0.9.9/tentacle/ui/preferences.ui
+-rw-rw-rw-   0        0        0     3462 2023-09-18 18:03:25.000000 tentacletk-0.9.9/tentacle/ui/rendering#submenu.ui
+-rw-rw-rw-   0        0        0    10912 2023-10-04 16:12:29.000000 tentacletk-0.9.9/tentacle/ui/rendering.ui
+-rw-rw-rw-   0        0        0     7450 2023-09-18 18:03:25.000000 tentacletk-0.9.9/tentacle/ui/rigging#submenu.ui
+-rw-rw-rw-   0        0        0    20295 2023-10-04 16:12:43.000000 tentacletk-0.9.9/tentacle/ui/rigging.ui
+-rw-rw-rw-   0        0        0     7631 2023-10-23 14:26:15.000000 tentacletk-0.9.9/tentacle/ui/scene#submenu.ui
+-rw-rw-rw-   0        0        0    10303 2023-10-04 16:01:23.000000 tentacletk-0.9.9/tentacle/ui/scene.ui
+-rw-rw-rw-   0        0        0     9784 2023-10-23 14:26:15.000000 tentacletk-0.9.9/tentacle/ui/selection#submenu.ui
+-rw-rw-rw-   0        0        0    12348 2023-10-23 14:26:15.000000 tentacletk-0.9.9/tentacle/ui/selection.ui
+-rw-rw-rw-   0        0        0     7692 2023-10-10 18:12:46.000000 tentacletk-0.9.9/tentacle/ui/subdivision#submenu.ui
+-rw-rw-rw-   0        0        0    11766 2023-10-10 18:05:55.000000 tentacletk-0.9.9/tentacle/ui/subdivision.ui
+-rw-rw-rw-   0        0        0     5199 2023-09-18 18:03:25.000000 tentacletk-0.9.9/tentacle/ui/symmetry#submenu.ui
+-rw-rw-rw-   0        0        0     8873 2023-10-04 16:12:35.000000 tentacletk-0.9.9/tentacle/ui/symmetry.ui
+-rw-rw-rw-   0        0        0    13382 2023-11-15 14:21:11.000000 tentacletk-0.9.9/tentacle/ui/transform#submenu.ui
+-rw-rw-rw-   0        0        0     6891 2023-10-04 16:08:09.000000 tentacletk-0.9.9/tentacle/ui/transform.constrain.ui
+-rw-rw-rw-   0        0        0     4495 2023-10-04 16:04:01.000000 tentacletk-0.9.9/tentacle/ui/transform.snap.ui
+-rw-rw-rw-   0        0        0    20267 2023-10-23 14:26:15.000000 tentacletk-0.9.9/tentacle/ui/transform.ui
+-rw-rw-rw-   0        0        0     2776 2023-09-18 18:03:25.000000 tentacletk-0.9.9/tentacle/ui/utilities#submenu.ui
+-rw-rw-rw-   0        0        0     7470 2023-10-04 16:04:44.000000 tentacletk-0.9.9/tentacle/ui/utilities.ui
+-rw-rw-rw-   0        0        0     6866 2023-09-18 18:03:25.000000 tentacletk-0.9.9/tentacle/ui/uv#submenu.ui
+-rw-rw-rw-   0        0        0    35970 2023-11-10 17:45:16.000000 tentacletk-0.9.9/tentacle/ui/uv.ui
+-rw-rw-rw-   0        0        0     2672 2023-09-18 18:03:25.000000 tentacletk-0.9.9/tentacle/ui/vfx#submenu.ui
+-rw-rw-rw-   0        0        0     4044 2023-10-04 16:01:55.000000 tentacletk-0.9.9/tentacle/ui/vfx.ui
+drwxrwxrwx   0        0        0        0 2023-12-20 15:33:05.681220 tentacletk-0.9.9/tentacletk.egg-info/
+-rw-rw-rw-   0        0        0     3735 2023-12-20 15:33:04.000000 tentacletk-0.9.9/tentacletk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3404 2023-12-20 15:33:04.000000 tentacletk-0.9.9/tentacletk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-20 15:33:04.000000 tentacletk-0.9.9/tentacletk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-12-20 15:33:04.000000 tentacletk-0.9.9/tentacletk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-12-20 15:33:04.000000 tentacletk-0.9.9/tentacletk.egg-info/top_level.txt
```

### Comparing `tentacletk-0.9.8/COPYING.LESSER` & `tentacletk-0.9.9/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/PKG-INFO` & `tentacletk-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tentacletk
-Version: 0.9.8
+Version: 0.9.9
 Home-page: https://github.com/m3trik/tentacle
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 Requires-Dist: shiboken2
 Requires-Dist: pymel
 Requires-Dist: pythontk==0.7.10
 Requires-Dist: uitk==1.0.7
 Requires-Dist: mayatk==0.9.8
 
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.en.html)
-[![Version](https://img.shields.io/badge/Version-0.9.8-blue.svg)](https://pypi.org/project/tentacletk/)
+[![Version](https://img.shields.io/badge/Version-0.9.9-blue.svg)](https://pypi.org/project/tentacletk/)
 
 
 # Tentacle: A Python3/PySide2 Marking Menu and DCC Toolkit
 Tentacle is a Python3/PySide2 marking menu implemented using Qt's QStackedWidget. It is designed for use with Maya, 3ds Max, Blender, and any other DCC app that supports the PySide2 framework. It allows easy management of various user interfaces (UIs) and provides functionality related to key events and mouse interactions. This is an ongoing personal project and is currently a work in progress. At the moment, I have stopped developing for Max and Blender and am solely focused on Maya, as it proved too much of an undertaking at this stage to support all three apps, especially since I am still somewhat in the experimental stage. However, this can be easily extended to work with those apps. If you have any questions or thoughts about that, feel like collaborating on something, or anything else, just drop me message.
 
 ## Design
 Tentacle runs on top of [uitk](https://github.com/m3trik/uitk.git), a PySide2 dynamic UI loader and management package, which allows for the creation of fully-featured UI with less time and code.
@@ -46,15 +46,15 @@
 | [ui](https://github.com/m3trik/uitk/blob/main/tentacle/events.py) | Location of the dynamic UI files. |
 | [slots](https://github.com/m3trik/uitk/blob/main/tentacle/slots) | Location of the various slot modules. |
 
 ## Installation
 Install via pip in a command line window using:
 
 ```bash
-python -m pip install tentacletk
+path/to/mayapy.exe -m pip install tentacletk
 ```
 ## Usage
 To launch the marking menu:
 
 For Maya, add a macro to a hotkey similar to the following:
 ```python
 from tentacle import tcl_maya
```

### Comparing `tentacletk-0.9.8/setup.py` & `tentacletk-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/__init__.py` & `tentacletk-0.9.9/tentacle/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # !/usr/bin/python
 # coding=utf-8
 import sys
 
 __package__ = "tentacle"
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 
 
 def greeting(string, outputToConsole=True):
     """Format a string using preset variables.
 
     Parameters:
         string (str): The greeting to format as a string with placeholders using the below keywords.
```

### Comparing `tentacletk-0.9.8/tentacle/overlay.py` & `tentacletk-0.9.9/tentacle/overlay.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/__init__.py` & `tentacletk-0.9.9/tentacle/slots/__init__.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/__init__.py` & `tentacletk-0.9.9/tentacle/slots/maya/__init__.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/animation.py` & `tentacletk-0.9.9/tentacle/slots/maya/animation.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class Animation(SlotsMaya):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def tb000_init(self, widget):
         """ """
-        widget.menu.setTitle("Set Current Frame")
+        widget.menu.setTitle("Move To Frame")
         widget.menu.add(
             "QSpinBox",
             setPrefix="Frame: ",
             setObjectName="s000",
             set_limits=[0, 10000],
             setValue=0,
             setToolTip="The desired frame number.",
@@ -35,15 +35,15 @@
             setText="Relative",
             setObjectName="chk000",
             setChecked=True,
             setToolTip="Move relative to the current position.",
         )
 
     def tb000(self, widget):
-        """Set Current Frame"""
+        """Move To Frame"""
         time = widget.menu.s000.value()
         update = widget.menu.chk001.isChecked()
         relative = widget.menu.chk000.isChecked()
 
         mtk.setCurrentFrame(time=time, update=update, relative=relative)
 
     def tb001_init(self, widget):
```

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/cameras.py` & `tentacletk-0.9.9/tentacle/slots/maya/cameras.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/convert.py` & `tentacletk-0.9.9/tentacle/slots/maya/convert.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/crease.py` & `tentacletk-0.9.9/tentacle/slots/maya/crease.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/create.py` & `tentacletk-0.9.9/tentacle/slots/maya/create.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/deformation.py` & `tentacletk-0.9.9/tentacle/slots/maya/deformation.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/display.py` & `tentacletk-0.9.9/tentacle/slots/maya/display.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/duplicate.py` & `tentacletk-0.9.9/tentacle/slots/maya/duplicate.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/edit.py` & `tentacletk-0.9.9/tentacle/slots/maya/edit.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/editors.py` & `tentacletk-0.9.9/tentacle/slots/maya/editors.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/file.py` & `tentacletk-0.9.9/tentacle/slots/maya/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,29 +134,29 @@
     def cmb006_init(self, widget):
         """ """
         widget.refresh = True
         if not widget.is_initialized:
             widget.menu.add(
                 self.sb.Label,
                 setObjectName="lbl000",
-                setText="Set",
+                setText="Set Project Directory",
                 setToolTip="Set the project directory.",
             )
             widget.menu.add(
                 self.sb.Label,
                 setObjectName="lbl004",
-                setText="Root",
-                setToolTip="Open the project directory.",
+                setText="Open Project Directory",
+                setToolTip="Open the project root directory.",
             )
 
         workspace = mtk.get_maya_info("workspace_dir")
         project = ptk.format_path(workspace, "dir")
         # Add each dir in the workspace as well as its full path as data
         items = {d: f"{workspace}/{d}" for d in os.listdir(workspace)}
-        widget.add(items, header=project, clear=True)
+        widget.add(items, header=f"Project: {project}", clear=True)
 
     def cmb006(self, index, widget):
         """Workspace"""
         try:
             item = widget.items[index]
             os.startfile(item)
         except Exception as e:
```

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/init.py` & `tentacletk-0.9.9/tentacle/slots/maya/init.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/lighting.py` & `tentacletk-0.9.9/tentacle/slots/maya/lighting.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/main.py` & `tentacletk-0.9.9/tentacle/slots/maya/main.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/materials.py` & `tentacletk-0.9.9/tentacle/slots/maya/materials.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/normals.py` & `tentacletk-0.9.9/tentacle/slots/maya/normals.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/nurbs.py` & `tentacletk-0.9.9/tentacle/slots/maya/nurbs.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/pivot.py` & `tentacletk-0.9.9/tentacle/slots/maya/pivot.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/polygons.py` & `tentacletk-0.9.9/tentacle/slots/maya/polygons.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/preferences.py` & `tentacletk-0.9.9/tentacle/slots/maya/preferences.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/rendering.py` & `tentacletk-0.9.9/tentacle/slots/maya/rendering.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/rigging.py` & `tentacletk-0.9.9/tentacle/slots/maya/rigging.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/scene.py` & `tentacletk-0.9.9/tentacle/slots/maya/scene.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # !/usr/bin/python
 # coding=utf-8
 try:
     import pymel.core as pm
 except ImportError as error:
     print(__file__, error)
+import pythontk as ptk
 import mayatk as mtk
 from uitk import Signals
 from tentacle.slots.maya import SlotsMaya
 
 
 class Scene(SlotsMaya):
     def __init__(self, *args, **kwargs):
@@ -27,19 +28,22 @@
         widget.menu.add(
             "QCheckBox",
             setText="Regular Expression",
             setObjectName="chk001",
             setToolTip="When checked, regular expression syntax is used instead of the default '*' and '|' wildcards.",
         )
 
+    @Signals("textChanged", "returnPressed")
     def txt000(self, text, widget):
-        """Select By Name"""
+        """Find"""
         # An asterisk denotes startswith*, *endswith, *contains*
         if text:
-            pm.select(pm.ls(text))
+            object_names = [str(i) for i in pm.ls()]
+            found_object_names = ptk.find_str(text, object_names)
+            pm.select(found_object_names)
 
     # The LineEdit text parameter is not emitted on `returnPressed`
     @Signals("returnPressed")
     def txt001(self, widget):
         """Rename"""
         # An asterisk denotes startswith*, *endswith, *contains*
         find = widget.ui.txt000.text()
```

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/selection.py` & `tentacletk-0.9.9/tentacle/slots/maya/selection.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/subdivision.py` & `tentacletk-0.9.9/tentacle/slots/maya/subdivision.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/symmetry.py` & `tentacletk-0.9.9/tentacle/slots/maya/symmetry.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/transform.py` & `tentacletk-0.9.9/tentacle/slots/maya/transform.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/utilities.py` & `tentacletk-0.9.9/tentacle/slots/maya/utilities.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/uv.py` & `tentacletk-0.9.9/tentacle/slots/maya/uv.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/slots/maya/vfx.py` & `tentacletk-0.9.9/tentacle/slots/maya/vfx.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/tcl.py` & `tentacletk-0.9.9/tentacle/tcl.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/tcl_blender.py` & `tentacletk-0.9.9/tentacle/tcl_blender.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/tcl_max.py` & `tentacletk-0.9.9/tentacle/tcl_max.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/tcl_maya.py` & `tentacletk-0.9.9/tentacle/tcl_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/__init__.py` & `tentacletk-0.9.9/tentacle/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/animation#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/animation#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/animation.ui` & `tentacletk-0.9.9/tentacle/ui/animation.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/cameras#lower#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/cameras#lower#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/cameras#startmenu.ui` & `tentacletk-0.9.9/tentacle/ui/cameras#startmenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/convert#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/convert#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/convert.ui` & `tentacletk-0.9.9/tentacle/ui/convert.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/crease#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/crease#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/crease.ui` & `tentacletk-0.9.9/tentacle/ui/crease.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/create#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/create#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/create.ui` & `tentacletk-0.9.9/tentacle/ui/create.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/deformation#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/deformation#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/deformation.ui` & `tentacletk-0.9.9/tentacle/ui/deformation.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/display#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/display#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/display.ui` & `tentacletk-0.9.9/tentacle/ui/display.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/duplicate#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/duplicate#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/duplicate.ui` & `tentacletk-0.9.9/tentacle/ui/duplicate.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/edit#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/edit#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/edit.ui` & `tentacletk-0.9.9/tentacle/ui/edit.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/editors#lower#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/editors#lower#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/editors#startmenu.ui` & `tentacletk-0.9.9/tentacle/ui/editors#startmenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/file#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/file#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/file.ui` & `tentacletk-0.9.9/tentacle/ui/file.ui`

 * *Files 3% similar despite different names*

#### Comparing `tentacletk-0.9.8/tentacle/ui/file.ui` & `tentacletk-0.9.9/tentacle/ui/file.ui`

```diff
@@ -85,14 +85,17 @@
                       </property>
                       <property name="maximumSize">
                         <size>
                           <width>16777215</width>
                           <height>20</height>
                         </size>
                       </property>
+                      <property name="toolTip">
+                        <string>Any recent workspaces will appear here.</string>
+                      </property>
                       <property name="maxVisibleItems">
                         <number>30</number>
                       </property>
                       <property name="sizeAdjustPolicy">
                         <enum>QComboBox::AdjustToContentsOnFirstShow</enum>
                       </property>
                       <property name="frame">
@@ -115,14 +118,17 @@
                       </property>
                       <property name="maximumSize">
                         <size>
                           <width>16777215</width>
                           <height>20</height>
                         </size>
                       </property>
+                      <property name="toolTip">
+                        <string>Open a workspace folder, or set a new workspace.</string>
+                      </property>
                       <property name="maxVisibleItems">
                         <number>40</number>
                       </property>
                       <property name="sizeAdjustPolicy">
                         <enum>QComboBox::AdjustToContents</enum>
                       </property>
                       <property name="frame">
@@ -169,14 +175,17 @@
                       </property>
                       <property name="maximumSize">
                         <size>
                           <width>16777215</width>
                           <height>20</height>
                         </size>
                       </property>
+                      <property name="toolTip">
+                        <string>Any recent scenes will appear here.</string>
+                      </property>
                       <property name="maxVisibleItems">
                         <number>30</number>
                       </property>
                       <property name="sizeAdjustPolicy">
                         <enum>QComboBox::AdjustToContentsOnFirstShow</enum>
                       </property>
                       <property name="frame">
@@ -199,14 +208,17 @@
                       </property>
                       <property name="maximumSize">
                         <size>
                           <width>16777215</width>
                           <height>20</height>
                         </size>
                       </property>
+                      <property name="toolTip">
+                        <string>Any recent autosaves will appear here.</string>
+                      </property>
                       <property name="maxVisibleItems">
                         <number>30</number>
                       </property>
                       <property name="sizeAdjustPolicy">
                         <enum>QComboBox::AdjustToContentsOnFirstShow</enum>
                       </property>
                       <property name="frame">
```

### Comparing `tentacletk-0.9.8/tentacle/ui/icons/Dolly Mode.png` & `tentacletk-0.9.9/tentacle/ui/icons/Dolly Mode.png`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/icons/Orbit View Mode.png` & `tentacletk-0.9.9/tentacle/ui/icons/Orbit View Mode.png`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/icons/Pan Non-Camera View Mode.png` & `tentacletk-0.9.9/tentacle/ui/icons/Pan Non-Camera View Mode.png`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/icons/Select and Rotate.png` & `tentacletk-0.9.9/tentacle/ui/icons/Select and Rotate.png`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/init#startmenu.ui` & `tentacletk-0.9.9/tentacle/ui/init#startmenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/lighting#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/lighting#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/lighting.ui` & `tentacletk-0.9.9/tentacle/ui/lighting.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/main#lower#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/main#lower#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/main#startmenu.ui` & `tentacletk-0.9.9/tentacle/ui/main#startmenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/materials#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/materials#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/materials.ui` & `tentacletk-0.9.9/tentacle/ui/materials.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/normals#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/normals#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/normals.ui` & `tentacletk-0.9.9/tentacle/ui/normals.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/nurbs#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/nurbs#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/nurbs.ui` & `tentacletk-0.9.9/tentacle/ui/nurbs.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/pivot#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/pivot#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/pivot.ui` & `tentacletk-0.9.9/tentacle/ui/pivot.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/polygons#component#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/polygons#component#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/polygons#edge#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/polygons#edge#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/polygons#face#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/polygons#face#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/polygons#mesh#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/polygons#mesh#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/polygons#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/polygons#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/polygons#vertex#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/polygons#vertex#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/polygons.ui` & `tentacletk-0.9.9/tentacle/ui/polygons.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/preferences#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/preferences#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/preferences.ui` & `tentacletk-0.9.9/tentacle/ui/preferences.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/rendering#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/rendering#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/rendering.ui` & `tentacletk-0.9.9/tentacle/ui/rendering.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/rigging#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/rigging#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/rigging.ui` & `tentacletk-0.9.9/tentacle/ui/rigging.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/scene#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/scene#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/scene.ui` & `tentacletk-0.9.9/tentacle/ui/scene.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/selection#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/selection#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/selection.ui` & `tentacletk-0.9.9/tentacle/ui/selection.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/subdivision#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/subdivision#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/subdivision.ui` & `tentacletk-0.9.9/tentacle/ui/subdivision.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/symmetry#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/symmetry#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/symmetry.ui` & `tentacletk-0.9.9/tentacle/ui/symmetry.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/transform#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/transform#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/transform.constrain.ui` & `tentacletk-0.9.9/tentacle/ui/transform.constrain.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/transform.snap.ui` & `tentacletk-0.9.9/tentacle/ui/transform.snap.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/transform.ui` & `tentacletk-0.9.9/tentacle/ui/transform.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/utilities#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/utilities#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/utilities.ui` & `tentacletk-0.9.9/tentacle/ui/utilities.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/uv#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/uv#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/uv.ui` & `tentacletk-0.9.9/tentacle/ui/uv.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/vfx#submenu.ui` & `tentacletk-0.9.9/tentacle/ui/vfx#submenu.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacle/ui/vfx.ui` & `tentacletk-0.9.9/tentacle/ui/vfx.ui`

 * *Files identical despite different names*

### Comparing `tentacletk-0.9.8/tentacletk.egg-info/PKG-INFO` & `tentacletk-0.9.9/tentacletk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tentacletk
-Version: 0.9.8
+Version: 0.9.9
 Home-page: https://github.com/m3trik/tentacle
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 Requires-Dist: shiboken2
 Requires-Dist: pymel
 Requires-Dist: pythontk==0.7.10
 Requires-Dist: uitk==1.0.7
 Requires-Dist: mayatk==0.9.8
 
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.en.html)
-[![Version](https://img.shields.io/badge/Version-0.9.8-blue.svg)](https://pypi.org/project/tentacletk/)
+[![Version](https://img.shields.io/badge/Version-0.9.9-blue.svg)](https://pypi.org/project/tentacletk/)
 
 
 # Tentacle: A Python3/PySide2 Marking Menu and DCC Toolkit
 Tentacle is a Python3/PySide2 marking menu implemented using Qt's QStackedWidget. It is designed for use with Maya, 3ds Max, Blender, and any other DCC app that supports the PySide2 framework. It allows easy management of various user interfaces (UIs) and provides functionality related to key events and mouse interactions. This is an ongoing personal project and is currently a work in progress. At the moment, I have stopped developing for Max and Blender and am solely focused on Maya, as it proved too much of an undertaking at this stage to support all three apps, especially since I am still somewhat in the experimental stage. However, this can be easily extended to work with those apps. If you have any questions or thoughts about that, feel like collaborating on something, or anything else, just drop me message.
 
 ## Design
 Tentacle runs on top of [uitk](https://github.com/m3trik/uitk.git), a PySide2 dynamic UI loader and management package, which allows for the creation of fully-featured UI with less time and code.
@@ -46,15 +46,15 @@
 | [ui](https://github.com/m3trik/uitk/blob/main/tentacle/events.py) | Location of the dynamic UI files. |
 | [slots](https://github.com/m3trik/uitk/blob/main/tentacle/slots) | Location of the various slot modules. |
 
 ## Installation
 Install via pip in a command line window using:
 
 ```bash
-python -m pip install tentacletk
+path/to/mayapy.exe -m pip install tentacletk
 ```
 ## Usage
 To launch the marking menu:
 
 For Maya, add a macro to a hotkey similar to the following:
 ```python
 from tentacle import tcl_maya
```

### Comparing `tentacletk-0.9.8/tentacletk.egg-info/SOURCES.txt` & `tentacletk-0.9.9/tentacletk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

