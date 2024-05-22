# Comparing `tmp/babelwidget-2024.2.tar.gz` & `tmp/babelwidget-2024.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "babelwidget-2024.2.tar", last modified: Tue May 14 09:40:06 2024, max compression
+gzip compressed data, was "babelwidget-2024.3.tar", last modified: Wed May 22 07:39:55 2024, max compression
```

## Comparing `babelwidget-2024.2.tar` & `babelwidget-2024.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-14 09:40:06.759451 babelwidget-2024.2/
--rwx------   0 eric      (1000) users      (984)      114 2022-10-14 06:42:17.000000 babelwidget-2024.2/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     5305 2024-05-14 09:40:06.759451 babelwidget-2024.2/PKG-INFO
--rwx------   0 eric      (1000) users      (984)      636 2023-10-05 13:15:24.000000 babelwidget-2024.2/README-COPYRIGHT-utf8.txt
--rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 babelwidget-2024.2/README-LICENCE-utf8.txt
--rwx------   0 eric      (1000) users      (984)     4473 2023-10-05 13:22:38.000000 babelwidget-2024.2/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-14 09:40:06.746117 babelwidget-2024.2/babelwidget/
--rwx------   0 eric      (1000) users      (984)     1596 2023-10-05 13:15:54.000000 babelwidget-2024.2/babelwidget/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-14 09:40:06.749451 babelwidget-2024.2/babelwidget/backend/
--rwx------   0 eric      (1000) users      (984)     2647 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/builder.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-14 09:40:06.749451 babelwidget-2024.2/babelwidget/backend/generic/
--rwx------   0 eric      (1000) users      (984)     7639 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/generic/path_chooser.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-14 09:40:06.749451 babelwidget-2024.2/babelwidget/backend/pyqt5/
--rwx------   0 eric      (1000) users      (984)     2700 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt5/constant.py
--rw-r--r--   0 eric      (1000) users      (984)     2025 2024-05-14 09:38:31.000000 babelwidget-2024.2/babelwidget/backend/pyqt5/function.py
--rwx------   0 eric      (1000) users      (984)     2115 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt5/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-14 09:40:06.752784 babelwidget-2024.2/babelwidget/backend/pyqt5/widget/
--rwx------   0 eric      (1000) users      (984)     1777 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt5/widget/button.py
--rwx------   0 eric      (1000) users      (984)     2119 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt5/widget/choices.py
--rwx------   0 eric      (1000) users      (984)     2143 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt5/widget/image.py
--rwx------   0 eric      (1000) users      (984)     1755 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt5/widget/label.py
--rwx------   0 eric      (1000) users      (984)     1787 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt5/widget/menu.py
--rwx------   0 eric      (1000) users      (984)     1964 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt5/widget/path_chooser.py
--rwx------   0 eric      (1000) users      (984)     1815 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt5/widget/scroll_container.py
--rwx------   0 eric      (1000) users      (984)     1767 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt5/widget/text_box.py
--rwx------   0 eric      (1000) users      (984)     1770 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt5/widget/text_line.py
--rwx------   0 eric      (1000) users      (984)     1780 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt5/widget/unchanged.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-14 09:40:06.752784 babelwidget-2024.2/babelwidget/backend/pyqt6/
--rwx------   0 eric      (1000) users      (984)     2809 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt6/constant.py
--rw-r--r--   0 eric      (1000) users      (984)     2025 2024-05-14 09:38:14.000000 babelwidget-2024.2/babelwidget/backend/pyqt6/function.py
--rwx------   0 eric      (1000) users      (984)     2115 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt6/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-14 09:40:06.756117 babelwidget-2024.2/babelwidget/backend/pyqt6/widget/
--rwx------   0 eric      (1000) users      (984)     1777 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt6/widget/button.py
--rwx------   0 eric      (1000) users      (984)     2119 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt6/widget/choices.py
--rwx------   0 eric      (1000) users      (984)     2157 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt6/widget/image.py
--rwx------   0 eric      (1000) users      (984)     1755 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt6/widget/label.py
--rwx------   0 eric      (1000) users      (984)     1787 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt6/widget/menu.py
--rwx------   0 eric      (1000) users      (984)     1964 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt6/widget/path_chooser.py
--rwx------   0 eric      (1000) users      (984)     1815 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt6/widget/scroll_container.py
--rwx------   0 eric      (1000) users      (984)     1767 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt6/widget/text_box.py
--rwx------   0 eric      (1000) users      (984)     1770 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt6/widget/text_line.py
--rwx------   0 eric      (1000) users      (984)     1780 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqt6/widget/unchanged.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-14 09:40:06.759451 babelwidget-2024.2/babelwidget/backend/pyqtx/
--rwx------   0 eric      (1000) users      (984)     1678 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqtx/button.py
--rwx------   0 eric      (1000) users      (984)     2094 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqtx/choices.py
--rwx------   0 eric      (1000) users      (984)     3358 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqtx/image.py
--rwx------   0 eric      (1000) users      (984)     1612 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqtx/label.py
--rwx------   0 eric      (1000) users      (984)     3079 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqtx/main.py
--rwx------   0 eric      (1000) users      (984)     1841 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqtx/menu.py
--rwx------   0 eric      (1000) users      (984)     2136 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqtx/path_chooser.py
--rwx------   0 eric      (1000) users      (984)     1732 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqtx/scroll_container.py
--rwx------   0 eric      (1000) users      (984)     1627 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqtx/text_box.py
--rwx------   0 eric      (1000) users      (984)     1620 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/backend/pyqtx/text_line.py
--rwx------   0 eric      (1000) users      (984)     5411 2024-04-15 11:10:59.000000 babelwidget-2024.2/babelwidget/main.py
--rwx------   0 eric      (1000) users      (984)     1575 2024-05-14 09:39:41.000000 babelwidget-2024.2/babelwidget/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-14 09:40:06.759451 babelwidget-2024.2/babelwidget.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     5305 2024-05-14 09:40:06.000000 babelwidget-2024.2/babelwidget.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     1916 2024-05-14 09:40:06.000000 babelwidget-2024.2/babelwidget.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2024-05-14 09:40:06.000000 babelwidget-2024.2/babelwidget.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       12 2024-05-14 09:40:06.000000 babelwidget-2024.2/babelwidget.egg-info/top_level.txt
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-14 09:40:06.746117 babelwidget-2024.2/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-14 09:40:06.759451 babelwidget-2024.2/documentation/wiki/
--rwx------   0 eric      (1000) users      (984)     1912 2023-10-05 13:23:51.000000 babelwidget-2024.2/documentation/wiki/description.asciidoc
--rwx------   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 babelwidget-2024.2/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2024-05-14 09:40:06.759451 babelwidget-2024.2/setup.cfg
--rwx------   0 eric      (1000) users      (984)     5932 2023-11-07 14:56:02.000000 babelwidget-2024.2/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:39:55.022201 babelwidget-2024.3/
+-rwx------   0 eric      (1000) users      (984)      114 2022-10-14 06:42:17.000000 babelwidget-2024.3/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     5305 2024-05-22 07:39:55.022201 babelwidget-2024.3/PKG-INFO
+-rwx------   0 eric      (1000) users      (984)      636 2023-10-05 13:15:24.000000 babelwidget-2024.3/README-COPYRIGHT-utf8.txt
+-rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 babelwidget-2024.3/README-LICENCE-utf8.txt
+-rwx------   0 eric      (1000) users      (984)     4473 2023-10-05 13:22:38.000000 babelwidget-2024.3/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:39:55.015535 babelwidget-2024.3/babelwidget/
+-rwx------   0 eric      (1000) users      (984)     1596 2023-10-05 13:15:54.000000 babelwidget-2024.3/babelwidget/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:39:55.015535 babelwidget-2024.3/babelwidget/backend/
+-rwx------   0 eric      (1000) users      (984)     2647 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/builder.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:39:55.015535 babelwidget-2024.3/babelwidget/backend/generic/
+-rwx------   0 eric      (1000) users      (984)     7639 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/generic/path_chooser.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:39:55.015535 babelwidget-2024.3/babelwidget/backend/pyqt5/
+-rwx------   0 eric      (1000) users      (984)     2700 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt5/constant.py
+-rw-r--r--   0 eric      (1000) users      (984)     2095 2024-05-21 15:20:36.000000 babelwidget-2024.3/babelwidget/backend/pyqt5/function.py
+-rwx------   0 eric      (1000) users      (984)     2115 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt5/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:39:55.018868 babelwidget-2024.3/babelwidget/backend/pyqt5/widget/
+-rwx------   0 eric      (1000) users      (984)     1777 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt5/widget/button.py
+-rwx------   0 eric      (1000) users      (984)     2119 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt5/widget/choices.py
+-rwx------   0 eric      (1000) users      (984)     2143 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt5/widget/image.py
+-rwx------   0 eric      (1000) users      (984)     1755 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt5/widget/label.py
+-rwx------   0 eric      (1000) users      (984)     1787 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt5/widget/menu.py
+-rwx------   0 eric      (1000) users      (984)     1964 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt5/widget/path_chooser.py
+-rwx------   0 eric      (1000) users      (984)     1815 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt5/widget/scroll_container.py
+-rwx------   0 eric      (1000) users      (984)     1767 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt5/widget/text_box.py
+-rwx------   0 eric      (1000) users      (984)     1770 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt5/widget/text_line.py
+-rwx------   0 eric      (1000) users      (984)     1780 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt5/widget/unchanged.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:39:55.018868 babelwidget-2024.3/babelwidget/backend/pyqt6/
+-rwx------   0 eric      (1000) users      (984)     2809 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt6/constant.py
+-rw-r--r--   0 eric      (1000) users      (984)     2095 2024-05-21 15:20:31.000000 babelwidget-2024.3/babelwidget/backend/pyqt6/function.py
+-rwx------   0 eric      (1000) users      (984)     2115 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt6/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:39:55.018868 babelwidget-2024.3/babelwidget/backend/pyqt6/widget/
+-rwx------   0 eric      (1000) users      (984)     1777 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt6/widget/button.py
+-rwx------   0 eric      (1000) users      (984)     2119 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt6/widget/choices.py
+-rwx------   0 eric      (1000) users      (984)     2157 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt6/widget/image.py
+-rwx------   0 eric      (1000) users      (984)     1755 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt6/widget/label.py
+-rwx------   0 eric      (1000) users      (984)     1787 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt6/widget/menu.py
+-rwx------   0 eric      (1000) users      (984)     1964 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt6/widget/path_chooser.py
+-rwx------   0 eric      (1000) users      (984)     1815 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt6/widget/scroll_container.py
+-rwx------   0 eric      (1000) users      (984)     1767 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt6/widget/text_box.py
+-rwx------   0 eric      (1000) users      (984)     1770 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt6/widget/text_line.py
+-rwx------   0 eric      (1000) users      (984)     1780 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqt6/widget/unchanged.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:39:55.018868 babelwidget-2024.3/babelwidget/backend/pyqtx/
+-rwx------   0 eric      (1000) users      (984)     1678 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqtx/button.py
+-rwx------   0 eric      (1000) users      (984)     2094 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqtx/choices.py
+-rwx------   0 eric      (1000) users      (984)     3358 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqtx/image.py
+-rwx------   0 eric      (1000) users      (984)     1612 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqtx/label.py
+-rwx------   0 eric      (1000) users      (984)     3079 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqtx/main.py
+-rwx------   0 eric      (1000) users      (984)     1841 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqtx/menu.py
+-rwx------   0 eric      (1000) users      (984)     2136 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqtx/path_chooser.py
+-rwx------   0 eric      (1000) users      (984)     1732 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqtx/scroll_container.py
+-rwx------   0 eric      (1000) users      (984)     1627 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqtx/text_box.py
+-rwx------   0 eric      (1000) users      (984)     1620 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/backend/pyqtx/text_line.py
+-rwx------   0 eric      (1000) users      (984)     5411 2024-04-15 11:10:59.000000 babelwidget-2024.3/babelwidget/main.py
+-rwx------   0 eric      (1000) users      (984)     1575 2024-05-21 15:28:45.000000 babelwidget-2024.3/babelwidget/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:39:55.022201 babelwidget-2024.3/babelwidget.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     5305 2024-05-22 07:39:55.000000 babelwidget-2024.3/babelwidget.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     1916 2024-05-22 07:39:55.000000 babelwidget-2024.3/babelwidget.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2024-05-22 07:39:55.000000 babelwidget-2024.3/babelwidget.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       12 2024-05-22 07:39:55.000000 babelwidget-2024.3/babelwidget.egg-info/top_level.txt
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:39:55.012201 babelwidget-2024.3/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:39:55.022201 babelwidget-2024.3/documentation/wiki/
+-rwx------   0 eric      (1000) users      (984)     1912 2023-10-05 13:23:51.000000 babelwidget-2024.3/documentation/wiki/description.asciidoc
+-rwx------   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 babelwidget-2024.3/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2024-05-22 07:39:55.022201 babelwidget-2024.3/setup.cfg
+-rwx------   0 eric      (1000) users      (984)     5932 2023-11-07 14:56:02.000000 babelwidget-2024.3/setup.py
```

### Comparing `babelwidget-2024.2/PKG-INFO` & `babelwidget-2024.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: babelwidget
-Version: 2024.2
+Version: 2024.3
 Summary: A Meta Widget Library That Speaks Several Backends
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/babelwidget/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/babelwidget//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/babelwidget/
```

### Comparing `babelwidget-2024.2/README-COPYRIGHT-utf8.txt` & `babelwidget-2024.3/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/README-LICENCE-utf8.txt` & `babelwidget-2024.3/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/README.rst` & `babelwidget-2024.3/README.rst`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/__init__.py` & `babelwidget-2024.3/babelwidget/__init__.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/builder.py` & `babelwidget-2024.3/babelwidget/backend/builder.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/generic/path_chooser.py` & `babelwidget-2024.3/babelwidget/backend/generic/path_chooser.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt5/constant.py` & `babelwidget-2024.3/babelwidget/backend/pyqt5/constant.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt5/function.py` & `babelwidget-2024.3/babelwidget/backend/pyqt6/function.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import typing as h
 
-import PyQt5.QtCore as core
+import PyQt6.QtCore as core
 
 NewMessage = core.pyqtSignal
 
 
 def CreateMessageCanal(
     messenger: core.QObject,
     message: str,
@@ -43,9 +43,11 @@
     /,
     *args,
     **kwargs,
 ) -> None:
     """"""
     signal: core.pyqtBoundSignal = getattr(messenger, message)
     if (args.__len__() > 0) or (kwargs.__len__() > 0):
-        AcknowledgeMessage = lambda: AcknowledgeMessage(*args, **kwargs)
-    signal.connect(AcknowledgeMessage)
+        AcknowledgeMessage_ = lambda *_, **__: AcknowledgeMessage(*args, **kwargs)
+    else:
+        AcknowledgeMessage_ = AcknowledgeMessage
+    signal.connect(AcknowledgeMessage_)
```

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt5/main.py` & `babelwidget-2024.3/babelwidget/backend/pyqt5/main.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt5/widget/button.py` & `babelwidget-2024.3/babelwidget/backend/pyqt5/widget/button.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt5/widget/choices.py` & `babelwidget-2024.3/babelwidget/backend/pyqt5/widget/choices.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt5/widget/image.py` & `babelwidget-2024.3/babelwidget/backend/pyqt5/widget/image.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt5/widget/label.py` & `babelwidget-2024.3/babelwidget/backend/pyqt5/widget/label.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt5/widget/menu.py` & `babelwidget-2024.3/babelwidget/backend/pyqt5/widget/menu.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt5/widget/path_chooser.py` & `babelwidget-2024.3/babelwidget/backend/pyqt5/widget/path_chooser.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt5/widget/scroll_container.py` & `babelwidget-2024.3/babelwidget/backend/pyqt5/widget/scroll_container.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt5/widget/text_box.py` & `babelwidget-2024.3/babelwidget/backend/pyqt5/widget/text_box.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt5/widget/text_line.py` & `babelwidget-2024.3/babelwidget/backend/pyqt5/widget/text_line.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt5/widget/unchanged.py` & `babelwidget-2024.3/babelwidget/backend/pyqt5/widget/unchanged.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt6/constant.py` & `babelwidget-2024.3/babelwidget/backend/pyqt6/constant.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt6/function.py` & `babelwidget-2024.3/babelwidget/backend/pyqt5/function.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import typing as h
 
-import PyQt6.QtCore as core
+import PyQt5.QtCore as core
 
 NewMessage = core.pyqtSignal
 
 
 def CreateMessageCanal(
     messenger: core.QObject,
     message: str,
@@ -43,9 +43,11 @@
     /,
     *args,
     **kwargs,
 ) -> None:
     """"""
     signal: core.pyqtBoundSignal = getattr(messenger, message)
     if (args.__len__() > 0) or (kwargs.__len__() > 0):
-        AcknowledgeMessage = lambda: AcknowledgeMessage(*args, **kwargs)
-    signal.connect(AcknowledgeMessage)
+        AcknowledgeMessage_ = lambda *_, **__: AcknowledgeMessage(*args, **kwargs)
+    else:
+        AcknowledgeMessage_ = AcknowledgeMessage
+    signal.connect(AcknowledgeMessage_)
```

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt6/main.py` & `babelwidget-2024.3/babelwidget/backend/pyqt6/main.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt6/widget/button.py` & `babelwidget-2024.3/babelwidget/backend/pyqt6/widget/button.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt6/widget/choices.py` & `babelwidget-2024.3/babelwidget/backend/pyqt6/widget/choices.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt6/widget/image.py` & `babelwidget-2024.3/babelwidget/backend/pyqt6/widget/image.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt6/widget/label.py` & `babelwidget-2024.3/babelwidget/backend/pyqt6/widget/label.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt6/widget/menu.py` & `babelwidget-2024.3/babelwidget/backend/pyqt6/widget/menu.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt6/widget/path_chooser.py` & `babelwidget-2024.3/babelwidget/backend/pyqt6/widget/path_chooser.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt6/widget/scroll_container.py` & `babelwidget-2024.3/babelwidget/backend/pyqt6/widget/scroll_container.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt6/widget/text_box.py` & `babelwidget-2024.3/babelwidget/backend/pyqt6/widget/text_box.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt6/widget/text_line.py` & `babelwidget-2024.3/babelwidget/backend/pyqt6/widget/text_line.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqt6/widget/unchanged.py` & `babelwidget-2024.3/babelwidget/backend/pyqt6/widget/unchanged.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqtx/button.py` & `babelwidget-2024.3/babelwidget/backend/pyqtx/button.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqtx/choices.py` & `babelwidget-2024.3/babelwidget/backend/pyqtx/choices.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqtx/image.py` & `babelwidget-2024.3/babelwidget/backend/pyqtx/image.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqtx/label.py` & `babelwidget-2024.3/babelwidget/backend/pyqtx/label.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqtx/main.py` & `babelwidget-2024.3/babelwidget/backend/pyqtx/main.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqtx/menu.py` & `babelwidget-2024.3/babelwidget/backend/pyqtx/menu.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqtx/path_chooser.py` & `babelwidget-2024.3/babelwidget/backend/pyqtx/path_chooser.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqtx/scroll_container.py` & `babelwidget-2024.3/babelwidget/backend/pyqtx/scroll_container.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqtx/text_box.py` & `babelwidget-2024.3/babelwidget/backend/pyqtx/text_box.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/backend/pyqtx/text_line.py` & `babelwidget-2024.3/babelwidget/backend/pyqtx/text_line.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/main.py` & `babelwidget-2024.3/babelwidget/main.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/babelwidget/version.py` & `babelwidget-2024.3/babelwidget/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2024.2"
+__version__ = "2024.3"
```

### Comparing `babelwidget-2024.2/babelwidget.egg-info/PKG-INFO` & `babelwidget-2024.3/babelwidget.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: babelwidget
-Version: 2024.2
+Version: 2024.3
 Summary: A Meta Widget Library That Speaks Several Backends
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/babelwidget/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/babelwidget//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/babelwidget/
```

### Comparing `babelwidget-2024.2/babelwidget.egg-info/SOURCES.txt` & `babelwidget-2024.3/babelwidget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/documentation/wiki/description.asciidoc` & `babelwidget-2024.3/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `babelwidget-2024.2/setup.py` & `babelwidget-2024.3/setup.py`

 * *Files identical despite different names*

