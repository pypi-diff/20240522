# Comparing `tmp/QNodeEditor-1.0.5.tar.gz` & `tmp/qnodeeditor-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QNodeEditor-1.0.5.tar", last modified: Wed Mar 20 23:00:58 2024, max compression
+gzip compressed data, was "qnodeeditor-1.0.6.tar", last modified: Wed May 22 18:04:38 2024, max compression
```

## Comparing `QNodeEditor-1.0.5.tar` & `qnodeeditor-1.0.6.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 23:00:58.421046 QNodeEditor-1.0.5/
--rw-rw-rw-   0        0        0     1516 2023-11-03 22:07:59.000000 QNodeEditor-1.0.5/LICENSE
--rw-rw-rw-   0        0        0       70 2023-11-03 23:01:38.000000 QNodeEditor-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6588 2024-03-20 23:00:58.420048 QNodeEditor-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-20 23:00:58.339739 QNodeEditor-1.0.5/QNodeEditor/
--rw-rw-rw-   0        0        0      299 2024-03-20 22:49:13.000000 QNodeEditor-1.0.5/QNodeEditor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-20 23:00:58.348735 QNodeEditor-1.0.5/QNodeEditor/clipboard/
--rw-rw-rw-   0        0        0      100 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/clipboard/__init__.py
--rw-rw-rw-   0        0        0     7107 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/clipboard/clipboard.py
--rw-rw-rw-   0        0        0     9741 2023-12-01 21:16:08.000000 QNodeEditor-1.0.5/QNodeEditor/dialog.py
--rw-rw-rw-   0        0        0    14308 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/edge.py
--rw-rw-rw-   0        0        0     5470 2023-11-20 18:05:28.000000 QNodeEditor-1.0.5/QNodeEditor/editor.py
-drwxrwxrwx   0        0        0        0 2024-03-20 23:00:58.353736 QNodeEditor-1.0.5/QNodeEditor/entries/
--rw-rw-rw-   0        0        0      230 2024-03-20 21:22:02.000000 QNodeEditor-1.0.5/QNodeEditor/entries/__init__.py
--rw-rw-rw-   0        0        0     3983 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/entries/combo_box.py
--rw-rw-rw-   0        0        0     3782 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/entries/labeled.py
--rw-rw-rw-   0        0        0     3891 2024-03-20 22:56:13.000000 QNodeEditor-1.0.5/QNodeEditor/entries/text_box.py
--rw-rw-rw-   0        0        0     4702 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/entries/value_box.py
--rw-rw-rw-   0        0        0    17170 2024-03-20 21:24:25.000000 QNodeEditor-1.0.5/QNodeEditor/entry.py
-drwxrwxrwx   0        0        0        0 2024-03-20 23:00:58.362735 QNodeEditor-1.0.5/QNodeEditor/graphics/
--rw-rw-rw-   0        0        0      167 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/graphics/__init__.py
--rw-rw-rw-   0        0        0     4943 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/graphics/cutter.py
--rw-rw-rw-   0        0        0     7827 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/graphics/edge.py
--rw-rw-rw-   0        0        0     2342 2023-11-20 18:05:28.000000 QNodeEditor-1.0.5/QNodeEditor/graphics/entry.py
--rw-rw-rw-   0        0        0    10434 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/graphics/node.py
--rw-rw-rw-   0        0        0     3693 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/graphics/scene.py
--rw-rw-rw-   0        0        0     3797 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/graphics/socket.py
--rw-rw-rw-   0        0        0    46106 2024-03-20 21:28:59.000000 QNodeEditor-1.0.5/QNodeEditor/graphics/view.py
-drwxrwxrwx   0        0        0        0 2024-03-20 23:00:58.364735 QNodeEditor-1.0.5/QNodeEditor/history/
--rw-rw-rw-   0        0        0       90 2023-11-01 23:12:06.000000 QNodeEditor-1.0.5/QNodeEditor/history/__init__.py
--rw-rw-rw-   0        0        0     3535 2023-11-03 19:05:55.000000 QNodeEditor-1.0.5/QNodeEditor/history/history.py
-drwxrwxrwx   0        0        0        0 2024-03-20 23:00:58.367738 QNodeEditor-1.0.5/QNodeEditor/metas/
--rw-rw-rw-   0        0        0      159 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/metas/__init__.py
--rw-rw-rw-   0        0        0      370 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/metas/graphics_path_item.py
--rw-rw-rw-   0        0        0      366 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/metas/object.py
--rw-rw-rw-   0        0        0    37022 2024-03-20 22:56:13.000000 QNodeEditor-1.0.5/QNodeEditor/node.py
--rw-rw-rw-   0        0        0    29490 2024-03-20 21:25:59.000000 QNodeEditor-1.0.5/QNodeEditor/scene.py
-drwxrwxrwx   0        0        0        0 2024-03-20 23:00:58.369743 QNodeEditor-1.0.5/QNodeEditor/serialise/
--rw-rw-rw-   0        0        0       86 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/serialise/__init__.py
--rw-rw-rw-   0        0        0     1142 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/serialise/serialise.py
--rw-rw-rw-   0        0        0     4911 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/socket.py
-drwxrwxrwx   0        0        0        0 2024-03-20 23:00:58.374744 QNodeEditor-1.0.5/QNodeEditor/themes/
--rw-rw-rw-   0        0        0     1795 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/themes/__init__.py
--rw-rw-rw-   0        0        0     2978 2023-11-03 19:39:14.000000 QNodeEditor-1.0.5/QNodeEditor/themes/dark.py
-drwxrwxrwx   0        0        0        0 2024-03-20 23:00:58.325739 QNodeEditor-1.0.5/QNodeEditor/themes/fonts/
-drwxrwxrwx   0        0        0        0 2024-03-20 23:00:58.399047 QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/
--rw-rw-rw-   0        0        0   705684 2023-10-27 22:58:59.000000 QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans-Bold.ttf
--rw-rw-rw-   0        0        0   643292 2023-10-27 22:58:59.000000 QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans-BoldOblique.ttf
--rw-rw-rw-   0        0        0   355380 2023-10-27 22:58:59.000000 QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans-ExtraLight.ttf
--rw-rw-rw-   0        0        0   635416 2023-10-27 22:58:59.000000 QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans-Oblique.ttf
--rw-rw-rw-   0        0        0   757076 2023-10-27 22:58:59.000000 QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans.ttf
--rw-rw-rw-   0        0        0   665028 2023-10-27 22:58:59.000000 QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSansCondensed-Bold.ttf
--rw-rw-rw-   0        0        0   611836 2023-10-27 22:58:59.000000 QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSansCondensed-BoldOblique.ttf
--rw-rw-rw-   0        0        0   599292 2023-10-27 22:58:59.000000 QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSansCondensed-Oblique.ttf
--rw-rw-rw-   0        0        0   680264 2023-10-27 22:58:59.000000 QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSansCondensed.ttf
-drwxrwxrwx   0        0        0        0 2024-03-20 23:00:58.402061 QNodeEditor-1.0.5/QNodeEditor/themes/img/
--rw-rw-rw-   0        0        0      366 2023-11-01 12:18:42.000000 QNodeEditor-1.0.5/QNodeEditor/themes/img/arrow_dark.svg
--rw-rw-rw-   0        0        0      366 2023-11-01 12:17:33.000000 QNodeEditor-1.0.5/QNodeEditor/themes/img/arrow_light.svg
--rw-rw-rw-   0        0        0     2910 2023-11-03 19:40:57.000000 QNodeEditor-1.0.5/QNodeEditor/themes/light.py
--rw-rw-rw-   0        0        0     7014 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/themes/theme.py
--rw-rw-rw-   0        0        0     6274 2024-03-20 22:22:44.000000 QNodeEditor-1.0.5/QNodeEditor/util.py
-drwxrwxrwx   0        0        0        0 2024-03-20 23:00:58.410051 QNodeEditor-1.0.5/QNodeEditor/widgets/
--rw-rw-rw-   0        0        0      222 2024-03-20 21:11:03.000000 QNodeEditor-1.0.5/QNodeEditor/widgets/__init__.py
--rw-rw-rw-   0        0        0     9879 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/widgets/combo_box.py
--rw-rw-rw-   0        0        0      508 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/widgets/empty.py
--rw-rw-rw-   0        0        0     1353 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/widgets/label.py
--rw-rw-rw-   0        0        0    10685 2024-03-20 22:56:13.000000 QNodeEditor-1.0.5/QNodeEditor/widgets/text_box.py
--rw-rw-rw-   0        0        0    39704 2023-11-08 20:48:45.000000 QNodeEditor-1.0.5/QNodeEditor/widgets/value_box.py
-drwxrwxrwx   0        0        0        0 2024-03-20 23:00:58.418048 QNodeEditor-1.0.5/QNodeEditor.egg-info/
--rw-rw-rw-   0        0        0     6588 2024-03-20 23:00:58.000000 QNodeEditor-1.0.5/QNodeEditor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2221 2024-03-20 23:00:58.000000 QNodeEditor-1.0.5/QNodeEditor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 23:00:58.000000 QNodeEditor-1.0.5/QNodeEditor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2024-03-20 23:00:58.000000 QNodeEditor-1.0.5/QNodeEditor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-20 23:00:58.000000 QNodeEditor-1.0.5/QNodeEditor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3818 2023-12-01 21:16:08.000000 QNodeEditor-1.0.5/README.md
--rw-rw-rw-   0        0        0     1310 2024-03-20 22:48:01.000000 QNodeEditor-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-20 23:00:58.421046 QNodeEditor-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 18:04:38.271116 qnodeeditor-1.0.6/
+-rw-rw-rw-   0        0        0     1516 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0       70 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     6588 2024-05-22 18:04:38.270116 qnodeeditor-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 18:04:38.014370 qnodeeditor-1.0.6/QNodeEditor/
+-rw-rw-rw-   0        0        0      299 2024-05-22 18:00:01.000000 qnodeeditor-1.0.6/QNodeEditor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:04:38.048405 qnodeeditor-1.0.6/QNodeEditor/clipboard/
+-rw-rw-rw-   0        0        0      100 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/clipboard/__init__.py
+-rw-rw-rw-   0        0        0     7107 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/clipboard/clipboard.py
+-rw-rw-rw-   0        0        0    10034 2024-05-22 17:48:19.000000 qnodeeditor-1.0.6/QNodeEditor/dialog.py
+-rw-rw-rw-   0        0        0    14308 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/edge.py
+-rw-rw-rw-   0        0        0     5825 2024-05-22 17:48:19.000000 qnodeeditor-1.0.6/QNodeEditor/editor.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:04:38.071884 qnodeeditor-1.0.6/QNodeEditor/entries/
+-rw-rw-rw-   0        0        0      230 2024-05-22 17:36:15.000000 qnodeeditor-1.0.6/QNodeEditor/entries/__init__.py
+-rw-rw-rw-   0        0        0     3983 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/entries/combo_box.py
+-rw-rw-rw-   0        0        0     3782 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/entries/labeled.py
+-rw-rw-rw-   0        0        0     3891 2024-05-22 17:36:15.000000 qnodeeditor-1.0.6/QNodeEditor/entries/text_box.py
+-rw-rw-rw-   0        0        0     4702 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/entries/value_box.py
+-rw-rw-rw-   0        0        0    17473 2024-05-22 17:54:42.000000 qnodeeditor-1.0.6/QNodeEditor/entry.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:04:38.123885 qnodeeditor-1.0.6/QNodeEditor/graphics/
+-rw-rw-rw-   0        0        0      167 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/graphics/__init__.py
+-rw-rw-rw-   0        0        0     4943 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/graphics/cutter.py
+-rw-rw-rw-   0        0        0     7827 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/graphics/edge.py
+-rw-rw-rw-   0        0        0     2342 2023-11-12 15:21:43.000000 qnodeeditor-1.0.6/QNodeEditor/graphics/entry.py
+-rw-rw-rw-   0        0        0    10434 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/graphics/node.py
+-rw-rw-rw-   0        0        0     3693 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/graphics/scene.py
+-rw-rw-rw-   0        0        0     3797 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/graphics/socket.py
+-rw-rw-rw-   0        0        0    46472 2024-05-22 17:48:19.000000 qnodeeditor-1.0.6/QNodeEditor/graphics/view.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:04:38.131205 qnodeeditor-1.0.6/QNodeEditor/history/
+-rw-rw-rw-   0        0        0       90 2024-05-22 17:36:15.000000 qnodeeditor-1.0.6/QNodeEditor/history/__init__.py
+-rw-rw-rw-   0        0        0     3535 2024-05-22 17:36:15.000000 qnodeeditor-1.0.6/QNodeEditor/history/history.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:04:38.148239 qnodeeditor-1.0.6/QNodeEditor/metas/
+-rw-rw-rw-   0        0        0      159 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/metas/__init__.py
+-rw-rw-rw-   0        0        0      370 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/metas/graphics_path_item.py
+-rw-rw-rw-   0        0        0      366 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/metas/object.py
+-rw-rw-rw-   0        0        0    37022 2024-05-22 17:36:15.000000 qnodeeditor-1.0.6/QNodeEditor/node.py
+-rw-rw-rw-   0        0        0    29491 2024-05-22 17:54:42.000000 qnodeeditor-1.0.6/QNodeEditor/scene.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:04:38.160280 qnodeeditor-1.0.6/QNodeEditor/serialise/
+-rw-rw-rw-   0        0        0       86 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/serialise/__init__.py
+-rw-rw-rw-   0        0        0     1142 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/serialise/serialise.py
+-rw-rw-rw-   0        0        0     4911 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/socket.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:04:38.181808 qnodeeditor-1.0.6/QNodeEditor/themes/
+-rw-rw-rw-   0        0        0     1795 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/themes/__init__.py
+-rw-rw-rw-   0        0        0     2978 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/themes/dark.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:04:37.987599 qnodeeditor-1.0.6/QNodeEditor/themes/fonts/
+drwxrwxrwx   0        0        0        0 2024-05-22 18:04:38.230978 qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/
+-rw-rw-rw-   0        0        0   705684 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans-Bold.ttf
+-rw-rw-rw-   0        0        0   643292 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans-BoldOblique.ttf
+-rw-rw-rw-   0        0        0   355380 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans-ExtraLight.ttf
+-rw-rw-rw-   0        0        0   635416 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans-Oblique.ttf
+-rw-rw-rw-   0        0        0   757076 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans.ttf
+-rw-rw-rw-   0        0        0   665028 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSansCondensed-Bold.ttf
+-rw-rw-rw-   0        0        0   611836 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSansCondensed-BoldOblique.ttf
+-rw-rw-rw-   0        0        0   599292 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSansCondensed-Oblique.ttf
+-rw-rw-rw-   0        0        0   680264 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSansCondensed.ttf
+drwxrwxrwx   0        0        0        0 2024-05-22 18:04:38.238977 qnodeeditor-1.0.6/QNodeEditor/themes/img/
+-rw-rw-rw-   0        0        0      366 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/themes/img/arrow_dark.svg
+-rw-rw-rw-   0        0        0      366 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/themes/img/arrow_light.svg
+-rw-rw-rw-   0        0        0     2910 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/themes/light.py
+-rw-rw-rw-   0        0        0     7014 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/themes/theme.py
+-rw-rw-rw-   0        0        0     6274 2024-05-22 17:36:15.000000 qnodeeditor-1.0.6/QNodeEditor/util.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:04:38.267056 qnodeeditor-1.0.6/QNodeEditor/widgets/
+-rw-rw-rw-   0        0        0      222 2024-05-22 17:36:15.000000 qnodeeditor-1.0.6/QNodeEditor/widgets/__init__.py
+-rw-rw-rw-   0        0        0     9879 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/widgets/combo_box.py
+-rw-rw-rw-   0        0        0      508 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/widgets/empty.py
+-rw-rw-rw-   0        0        0     1353 2023-11-10 14:31:59.000000 qnodeeditor-1.0.6/QNodeEditor/widgets/label.py
+-rw-rw-rw-   0        0        0    10685 2024-05-22 17:36:15.000000 qnodeeditor-1.0.6/QNodeEditor/widgets/text_box.py
+-rw-rw-rw-   0        0        0    39704 2023-11-12 14:57:08.000000 qnodeeditor-1.0.6/QNodeEditor/widgets/value_box.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:04:38.269115 qnodeeditor-1.0.6/QNodeEditor.egg-info/
+-rw-rw-rw-   0        0        0     6588 2024-05-22 18:04:37.000000 qnodeeditor-1.0.6/QNodeEditor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2047 2024-05-22 18:04:37.000000 qnodeeditor-1.0.6/QNodeEditor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 18:04:37.000000 qnodeeditor-1.0.6/QNodeEditor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2024-05-22 18:04:37.000000 qnodeeditor-1.0.6/QNodeEditor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-22 18:04:37.000000 qnodeeditor-1.0.6/QNodeEditor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3818 2024-05-22 17:36:15.000000 qnodeeditor-1.0.6/README.md
+-rw-rw-rw-   0        0        0     1310 2024-05-22 17:58:34.000000 qnodeeditor-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 18:04:38.271116 qnodeeditor-1.0.6/setup.cfg
```

### Comparing `QNodeEditor-1.0.5/LICENSE` & `qnodeeditor-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/PKG-INFO` & `qnodeeditor-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QNodeEditor
-Version: 1.0.5
+Version: 1.0.6
 Summary: Node editor for PyQt5
 Author: Jasper Jeuken
 License: Copyright (c) 2023, Jasper Jeuken
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -48,15 +48,15 @@
 Requires-Dist: sphinx-toolbox; extra == "docs"
 Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
 Requires-Dist: sphinx-qt-documentation; extra == "docs"
 
 # QNodeEditor
 
-![pylint](https://img.shields.io/badge/pylint-9.82-yellow?logo=python&logoColor=white)
+![pylint](https://img.shields.io/badge/pylint-9.58-yellow?logo=python&logoColor=white)
 [<img src="https://img.shields.io/badge/github--blue?logo=github" alt="Github badge">](https://github.com/JasperJeuken/QNodeEditor)
 [<img src="https://img.shields.io/badge/PyPi--blue?logo=pypi" alt="PyPi badge">](https://pypi.org/project/QNodeEditor/)
 [<img src="https://img.shields.io/badge/Documentation--blue?logo=readthedocs" alt="readthedocs badge">](https://qnodeeditor.readthedocs.io/en/latest/)
 [<img src="https://readthedocs.org/projects/qnodeeditor/badge/" alt="readthedocs badge 2">](https://qnodeeditor.readthedocs.io/en/latest/)
 
 QNodeEditor is a collection of widgets that enables you to easily create 
 and use a node editing environment in PyQt5.
```

### Comparing `QNodeEditor-1.0.5/QNodeEditor/clipboard/clipboard.py` & `qnodeeditor-1.0.6/QNodeEditor/clipboard/clipboard.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/dialog.py` & `qnodeeditor-1.0.6/QNodeEditor/dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,37 +55,42 @@
         Node editor widget that shows an interactive node scene
     result : dict[str, Any] or None
         Result of the evaluated scene (``None`` if not evaluated).
         There is an item in the dictionary for each input of the selected output node. The keys are
         the names of the entries, and the values the input result that they received.
     """
 
-    def __init__(self, parent: QWidget = None, theme: ThemeType = DarkTheme):
+    def __init__(self, parent: QWidget = None,
+                 theme: ThemeType = DarkTheme,
+                 allow_multiple_inputs: bool = False):
         """
         Create a new node editor dialog.
 
         Parameters
         ----------
         parent : QWidget, optional
             Parent widget for this dialog (if any)
         theme : Type[:py:class:`~QNodeEditor.themes.theme.Theme`], optional
             Theme for the dialog (default: :py:class:`~QNodeEditor.themes.dark.DarkTheme`)
+        allow_multiple_inputs : bool
+            If set to True, multiple edges can be connected to the same node input. Otherwise, only
+            a single edge can be connected to any input.
         """
         super().__init__(parent, Qt.WindowCloseButtonHint)
         self.setWindowTitle('Node editor')
         self.setWindowModality(Qt.ApplicationModal)
         self.result: Optional[dict[str, Any]] = None
 
         # Create dialog layout
         layout = QVBoxLayout(self)
         layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(layout)
 
         # Add node editor
-        self.editor: NodeEditor = NodeEditor(self, theme)
+        self.editor: NodeEditor = NodeEditor(self, theme, allow_multiple_inputs)
         self.editor.scene.evaluated.connect(self._handle_result)
         self.editor.scene.errored.connect(self._handle_error)
         layout.addWidget(self.editor, 1)
 
         # Create status display
         self._status_layout = QHBoxLayout()
         self._status_layout.setContentsMargins(0, 0, 0, 0)
```

### Comparing `QNodeEditor-1.0.5/QNodeEditor/edge.py` & `qnodeeditor-1.0.6/QNodeEditor/edge.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/editor.py` & `qnodeeditor-1.0.6/QNodeEditor/editor.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,35 +39,41 @@
     """
 
     evaluated: pyqtSignal = pyqtSignal(dict)
     """pyqtSignal -> dict: Signal that emits the evaluation result if successful"""
     errored: pyqtSignal = pyqtSignal(Exception)
     """pyqtSignal -> Exception: Signal that emits the error if evaluation failed"""
 
-    def __init__(self, parent: QWidget = None, theme: ThemeType = DarkTheme):
+    def __init__(self, parent: QWidget = None,
+                 theme: ThemeType = DarkTheme,
+                 allow_multiple_inputs: bool = False):
         """
         Create a new node editor widget.
 
         Parameters
         ----------
         parent : QWidget, optional
             Parent widget for this node editor (if any)
         theme : Type[:py:class:`~QNodeEditor.themes.theme.Theme`], optional
             Theme for the node editor (default: :py:class:`~QNodeEditor.themes.dark.DarkTheme`)
+        allow_multiple_inputs : bool
+            If set to True, multiple edges can be connected to the same node input. Otherwise, only
+            a single edge can be connected to any input.
         """
         super().__init__(parent)
 
         # Create widget layout
         layout = QVBoxLayout()
         layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(layout)
 
         # Create node scene and view
         self.scene: NodeScene = NodeScene(self)
-        self.view: NodeView = NodeView(self.scene.graphics)
+        self.view: NodeView = NodeView(self.scene.graphics,
+                                       allow_multiple_inputs=allow_multiple_inputs)
         layout.addWidget(self.view)
 
         # Set node editor theme
         self.theme: ThemeType = theme
         self.view.setFocusPolicy(Qt.StrongFocus)
 
         # Pass through scene signals
```

### Comparing `QNodeEditor-1.0.5/QNodeEditor/entries/combo_box.py` & `qnodeeditor-1.0.6/QNodeEditor/entries/combo_box.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/entries/labeled.py` & `qnodeeditor-1.0.6/QNodeEditor/entries/labeled.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/entries/text_box.py` & `qnodeeditor-1.0.6/QNodeEditor/entries/text_box.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/entries/value_box.py` & `qnodeeditor-1.0.6/QNodeEditor/entries/value_box.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/entry.py` & `qnodeeditor-1.0.6/QNodeEditor/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,36 +167,44 @@
         Any
             Value of this entry
         """
         # If this entry is static/output or there are no edges connected, return the widget value
         if self.entry_type in (self.TYPE_STATIC, self.TYPE_OUTPUT) or len(self.socket.edges) == 0:
             return get_widget_value(self.widget)
 
-        # Otherwise, obtain the value from the connected edge
+        # Otherwise, get the vale from the connected edge(s)
         return self._get_connected_value()
 
     def _get_connected_value(self) -> Any:
         """
         Get the value of the output entry that is connected to this input entry.
 
         Returns
         -------
         Any
             Value of the connected output entry.
         """
-        # Get the entry that is connected to the input socket
-        edge = self.socket.edges[0]
-        if edge.start == self.socket:
-            connected_entry = edge.end.entry
-        else:
-            connected_entry = edge.start.entry
-
-        # Get the output from the node the connected entry is in and return the relevant value
-        output = connected_entry.node.output
-        return output[connected_entry.name]
+        # Go through each connected edge to determine its value
+        values = []
+        for edge in self.socket.edges:
+
+            # Get the entry that is connected to the input socket
+            if edge.start == self.socket:
+                connected_entry = edge.end.entry
+            else:
+                connected_entry = edge.start.entry
+
+            # Get the output from the node the connected entry is in and store the relevant value
+            output = connected_entry.node.output
+            values.append(output[connected_entry.name])
+
+        # If there is only one edge, return only its value. Return all values otherwise
+        if len(values) == 1:
+            return values[0]
+        return values
 
     @property
     def theme(self) -> ThemeType:
         """
         Get or set the theme of the entry.
 
         Setting the theme of the entry affects all child elements.
```

### Comparing `QNodeEditor-1.0.5/QNodeEditor/graphics/cutter.py` & `qnodeeditor-1.0.6/QNodeEditor/graphics/cutter.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/graphics/edge.py` & `qnodeeditor-1.0.6/QNodeEditor/graphics/edge.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/graphics/entry.py` & `qnodeeditor-1.0.6/QNodeEditor/graphics/entry.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/graphics/node.py` & `qnodeeditor-1.0.6/QNodeEditor/graphics/node.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/graphics/scene.py` & `qnodeeditor-1.0.6/QNodeEditor/graphics/scene.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/graphics/socket.py` & `qnodeeditor-1.0.6/QNodeEditor/graphics/socket.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/graphics/view.py` & `qnodeeditor-1.0.6/QNodeEditor/graphics/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,24 +35,28 @@
     STATE_CUTTING: int = 1
     """int: Cutting state (a :py:class:`~.cutter.Cutter` is being drawn)"""
     STATE_DRAGGING: int = 2
     """int: Dragging state (a new edge is being dragged)"""
     STATE_PLACING: int = 3
     """int: Placing state (a item or group of items is being placed)"""
 
-    def __init__(self, scene_graphics: NodeSceneGraphics, theme: ThemeType = DarkTheme):
+    def __init__(self, scene_graphics: NodeSceneGraphics, theme: ThemeType = DarkTheme,
+                 allow_multiple_inputs: bool = False):
         """
         Create a new node view.
 
         Parameters
         ----------
         scene_graphics : :py:class:`~.scene.NodeSceneGraphics`
             Scene graphics this view is for.
         theme :  Type[:py:class:`~QNodeEditor.themes.theme.Theme`], optional
             Theme for the node view (default: :py:class:`~QNodeEditor.themes.dark.DarkTheme`)
+        allow_multiple_inputs: bool
+            If True, multiple edges can be connected to a single input, otherwise only a single
+            edge can be connected to any input.
         """
         super().__init__(scene_graphics)
         self.scene_graphics: NodeSceneGraphics = scene_graphics
 
         # Create cutting line
         self._cutter: Cutter = Cutter(self.scene_graphics.scene)
         self.scene_graphics.addItem(self._cutter)
@@ -90,14 +94,15 @@
         self._started_place: bool = False
 
         # Set other tracking variables
         self.prev_mouse_pos: QPoint = QPoint()
         self._last_left_click: QPoint = QPoint()
         self._last_right_click: QPoint = QPoint()
         self._editing: bool = False
+        self._allow_multiple_inputs: bool = allow_multiple_inputs
 
     @property
     def theme(self) -> ThemeType:
         """
         Get or set the node view theme.
         """
         return self._theme
@@ -577,18 +582,19 @@
         # Check if an edge already exists between these two sockets
         for edge in self.scene_graphics.scene.edges:
             if ((edge.start == self._drag_start and edge.end == item.socket) or
                     (edge.end == self._drag_start and edge.start == item.socket)):
                 return
 
         # Remove all present edges from input sockets (only single edge allowed)
-        if item.socket.entry.entry_type == Entry.TYPE_INPUT:
-            item.socket.remove_all_edges()
-        if self._drag_start.entry.entry_type == Entry.TYPE_INPUT:
-            self._drag_start.remove_all_edges()
+        if not self._allow_multiple_inputs:
+            if item.socket.entry.entry_type == Entry.TYPE_INPUT:
+                item.socket.remove_all_edges()
+            if self._drag_start.entry.entry_type == Entry.TYPE_INPUT:
+                self._drag_start.remove_all_edges()
 
         # Create a new edge to connect the start and end sockets
         Edge(self._drag_start, item.socket, self.scene_graphics.scene, self.theme)
         self._drag_start = None
 
     def calculate_drag_pos(self, mouse_pos: QPoint) -> QPoint:
         """
```

### Comparing `QNodeEditor-1.0.5/QNodeEditor/history/history.py` & `qnodeeditor-1.0.6/QNodeEditor/history/history.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/node.py` & `qnodeeditor-1.0.6/QNodeEditor/node.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/scene.py` & `qnodeeditor-1.0.6/QNodeEditor/scene.py`

 * *Files 0% similar despite different names*

```diff
@@ -848,15 +848,15 @@
             None
         """
         try:
             # Prevent infinite recursion when cycles exist in the scene
             if scene.has_cycles():
                 raise ValueError('Cannot evaluate scene since there are cycles in the connections')
 
-            # Rest all node outputs
+            # Reset all node outputs
             for node in scene.nodes:
                 node.output = None
 
             # Get the value for each input socket of the output node
             output_node = scene.find_output_node()
             result = {}
             for entry in output_node.entries:
```

### Comparing `QNodeEditor-1.0.5/QNodeEditor/serialise/serialise.py` & `qnodeeditor-1.0.6/QNodeEditor/serialise/serialise.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/socket.py` & `qnodeeditor-1.0.6/QNodeEditor/socket.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/themes/__init__.py` & `qnodeeditor-1.0.6/QNodeEditor/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/themes/dark.py` & `qnodeeditor-1.0.6/QNodeEditor/themes/dark.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans-Bold.ttf` & `qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans-BoldOblique.ttf` & `qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans-ExtraLight.ttf` & `qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans-Oblique.ttf` & `qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans.ttf` & `qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSansCondensed-Bold.ttf` & `qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSansCondensed-Bold.ttf`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSansCondensed-BoldOblique.ttf` & `qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSansCondensed-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSansCondensed-Oblique.ttf` & `qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSansCondensed-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSansCondensed.ttf` & `qnodeeditor-1.0.6/QNodeEditor/themes/fonts/DejaVuSans/DejaVuSansCondensed.ttf`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/themes/light.py` & `qnodeeditor-1.0.6/QNodeEditor/themes/light.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/themes/theme.py` & `qnodeeditor-1.0.6/QNodeEditor/themes/theme.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/util.py` & `qnodeeditor-1.0.6/QNodeEditor/util.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/widgets/combo_box.py` & `qnodeeditor-1.0.6/QNodeEditor/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/widgets/label.py` & `qnodeeditor-1.0.6/QNodeEditor/widgets/label.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/widgets/text_box.py` & `qnodeeditor-1.0.6/QNodeEditor/widgets/text_box.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor/widgets/value_box.py` & `qnodeeditor-1.0.6/QNodeEditor/widgets/value_box.py`

 * *Files identical despite different names*

### Comparing `QNodeEditor-1.0.5/QNodeEditor.egg-info/PKG-INFO` & `qnodeeditor-1.0.6/QNodeEditor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QNodeEditor
-Version: 1.0.5
+Version: 1.0.6
 Summary: Node editor for PyQt5
 Author: Jasper Jeuken
 License: Copyright (c) 2023, Jasper Jeuken
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -48,15 +48,15 @@
 Requires-Dist: sphinx-toolbox; extra == "docs"
 Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
 Requires-Dist: sphinx-qt-documentation; extra == "docs"
 
 # QNodeEditor
 
-![pylint](https://img.shields.io/badge/pylint-9.82-yellow?logo=python&logoColor=white)
+![pylint](https://img.shields.io/badge/pylint-9.58-yellow?logo=python&logoColor=white)
 [<img src="https://img.shields.io/badge/github--blue?logo=github" alt="Github badge">](https://github.com/JasperJeuken/QNodeEditor)
 [<img src="https://img.shields.io/badge/PyPi--blue?logo=pypi" alt="PyPi badge">](https://pypi.org/project/QNodeEditor/)
 [<img src="https://img.shields.io/badge/Documentation--blue?logo=readthedocs" alt="readthedocs badge">](https://qnodeeditor.readthedocs.io/en/latest/)
 [<img src="https://readthedocs.org/projects/qnodeeditor/badge/" alt="readthedocs badge 2">](https://qnodeeditor.readthedocs.io/en/latest/)
 
 QNodeEditor is a collection of widgets that enables you to easily create 
 and use a node editing environment in PyQt5.
```

### Comparing `QNodeEditor-1.0.5/QNodeEditor.egg-info/SOURCES.txt` & `qnodeeditor-1.0.6/QNodeEditor.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -54,13 +54,8 @@
 QNodeEditor/themes/img/arrow_dark.svg
 QNodeEditor/themes/img/arrow_light.svg
 QNodeEditor/widgets/__init__.py
 QNodeEditor/widgets/combo_box.py
 QNodeEditor/widgets/empty.py
 QNodeEditor/widgets/label.py
 QNodeEditor/widgets/text_box.py
-QNodeEditor/widgets/value_box.py
-qnodeeditor.egg-info/PKG-INFO
-qnodeeditor.egg-info/SOURCES.txt
-qnodeeditor.egg-info/dependency_links.txt
-qnodeeditor.egg-info/requires.txt
-qnodeeditor.egg-info/top_level.txt
+QNodeEditor/widgets/value_box.py
```

### Comparing `QNodeEditor-1.0.5/README.md` & `qnodeeditor-1.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # QNodeEditor
 
-![pylint](https://img.shields.io/badge/pylint-9.82-yellow?logo=python&logoColor=white)
+![pylint](https://img.shields.io/badge/pylint-9.58-yellow?logo=python&logoColor=white)
 [<img src="https://img.shields.io/badge/github--blue?logo=github" alt="Github badge">](https://github.com/JasperJeuken/QNodeEditor)
 [<img src="https://img.shields.io/badge/PyPi--blue?logo=pypi" alt="PyPi badge">](https://pypi.org/project/QNodeEditor/)
 [<img src="https://img.shields.io/badge/Documentation--blue?logo=readthedocs" alt="readthedocs badge">](https://qnodeeditor.readthedocs.io/en/latest/)
 [<img src="https://readthedocs.org/projects/qnodeeditor/badge/" alt="readthedocs badge 2">](https://qnodeeditor.readthedocs.io/en/latest/)
 
 QNodeEditor is a collection of widgets that enables you to easily create 
 and use a node editing environment in PyQt5.
```

### Comparing `QNodeEditor-1.0.5/pyproject.toml` & `qnodeeditor-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "QNodeEditor"
-version = "1.0.5"
+version = "1.0.6"
 description = "Node editor for PyQt5"
 readme = "README.md"
 authors = [{ name = "Jasper Jeuken" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

