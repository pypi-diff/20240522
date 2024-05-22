# Comparing `tmp/bootlace-0.2.2.tar.gz` & `tmp/bootlace-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat May 18 16:54:05 2024, max compression
+gzip compressed data, last modified: Tue May 21 04:09:54 2024, max compression
```

## Comparing `bootlace-0.2.2.tar` & `bootlace-0.2.3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0      247 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/__about__.py
--rw-r--r--   0        0        0      384 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/__init__.py
--rw-r--r--   0        0        0      411 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/_version.py
--rw-r--r--   0        0        0     6490 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/breadcrumbs.py
--rw-r--r--   0        0        0     3278 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/endpoint.py
--rw-r--r--   0        0        0     1179 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/extension.py
--rw-r--r--   0        0        0     1042 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/icon.py
--rw-r--r--   0        0        0      465 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/image.py
--rw-r--r--   0        0        0     1777 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/links.py
--rw-r--r--   0        0        0        0 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/py.typed
--rw-r--r--   0        0        0     1207 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/resources.py
--rw-r--r--   0        0        0      669 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/size.py
--rw-r--r--   0        0        0     1217 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/style.py
--rw-r--r--   0        0        0    11020 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/util.py
--rw-r--r--   0        0        0        0 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/forms/__init__.py
--rw-r--r--   0        0        0     3037 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/forms/fields.py
--rw-r--r--   0        0        0      661 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/forms/widgets.py
--rw-r--r--   0        0        0     1571 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/forms/templates/bootlace/_form.html
--rw-r--r--   0        0        0      109 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/nav/__init__.py
--rw-r--r--   0        0        0     5161 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/nav/bar.py
--rw-r--r--   0        0        0     5781 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/nav/core.py
--rw-r--r--   0        0        0      427 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/nav/elements.py
--rw-r--r--   0        0        0     3197 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/nav/nav.py
--rw-r--r--   0        0        0    70330 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.css
--rw-r--r--   0        0        0   203179 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.css.map
--rw-r--r--   0        0        0    51796 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.min.css
--rw-r--r--   0        0        0   115988 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.min.css.map
--rw-r--r--   0        0        0    70404 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.rtl.css
--rw-r--r--   0        0        0   203183 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0        0        0    51871 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0        0        0   116065 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0        0        0    12066 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.css
--rw-r--r--   0        0        0   129328 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.css.map
--rw-r--r--   0        0        0    10127 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.min.css
--rw-r--r--   0        0        0    51370 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.min.css.map
--rw-r--r--   0        0        0    12059 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.rtl.css
--rw-r--r--   0        0        0   129343 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0        0        0    10199 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0        0        0    63944 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0        0        0   107824 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.css
--rw-r--r--   0        0        0   267492 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.css.map
--rw-r--r--   0        0        0    85353 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.min.css
--rw-r--r--   0        0        0   180382 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.min.css.map
--rw-r--r--   0        0        0   107692 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.rtl.css
--rw-r--r--   0        0        0   267433 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0        0        0    85282 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0        0        0   180218 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0        0        0   280814 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap.css
--rw-r--r--   0        0        0   679012 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap.css.map
--rw-r--r--   0        0        0   232949 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap.min.css
--rw-r--r--   0        0        0   589162 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap.min.css.map
--rw-r--r--   0        0        0   280393 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap.rtl.css
--rw-r--r--   0        0        0   678857 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap.rtl.css.map
--rw-r--r--   0        0        0   233056 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap.rtl.min.css
--rw-r--r--   0        0        0   588696 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap.rtl.min.css.map
--rw-r--r--   0        0        0    88585 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/icons/bootstrap-icons.css
--rw-r--r--   0        0        0    47188 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/icons/bootstrap-icons.json
--rw-r--r--   0        0        0   211136 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/icons/bootstrap-icons.scss
--rw-r--r--   0        0        0   972584 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/icons/bootstrap-icons.svg
--rw-r--r--   0        0        0   207731 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   444287 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    80664 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   331887 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   135747 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.esm.js
--rw-r--r--   0        0        0   305153 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    74155 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   222463 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   145313 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.js
--rw-r--r--   0        0        0   306321 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.js.map
--rw-r--r--   0        0        0    60578 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.min.js
--rw-r--r--   0        0        0   220351 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.min.js.map
--rw-r--r--   0        0        0      303 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/table/__init__.py
--rw-r--r--   0        0        0     5552 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/table/base.py
--rw-r--r--   0        0        0     2862 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/table/columns.py
--rw-r--r--   0        0        0       67 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/testing/__init__.py
--rw-r--r--   0        0        0     4939 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/testing/html.py
--rw-r--r--   0        0        0     1222 2024-05-18 16:54:05.000000 bootlace-0.2.2/.gitignore
--rw-r--r--   0        0        0     1096 2024-05-18 16:54:05.000000 bootlace-0.2.2/LICENSE.txt
--rw-r--r--   0        0        0      478 2024-05-18 16:54:05.000000 bootlace-0.2.2/README.md
--rw-r--r--   0        0        0     2687 2024-05-18 16:54:05.000000 bootlace-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1323 2024-05-18 16:54:05.000000 bootlace-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      247 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/__about__.py
+-rw-r--r--   0        0        0      384 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/__init__.py
+-rw-r--r--   0        0        0      411 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/_version.py
+-rw-r--r--   0        0        0     6490 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/breadcrumbs.py
+-rw-r--r--   0        0        0     3278 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/endpoint.py
+-rw-r--r--   0        0        0     1179 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/extension.py
+-rw-r--r--   0        0        0     1042 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/icon.py
+-rw-r--r--   0        0        0      465 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/image.py
+-rw-r--r--   0        0        0     1777 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/links.py
+-rw-r--r--   0        0        0        0 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/py.typed
+-rw-r--r--   0        0        0     1207 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/resources.py
+-rw-r--r--   0        0        0      669 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/size.py
+-rw-r--r--   0        0        0     1217 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/style.py
+-rw-r--r--   0        0        0    11020 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/util.py
+-rw-r--r--   0        0        0        0 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/forms/__init__.py
+-rw-r--r--   0        0        0     3037 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/forms/fields.py
+-rw-r--r--   0        0        0      661 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/forms/widgets.py
+-rw-r--r--   0        0        0     1571 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/forms/templates/bootlace/_form.html
+-rw-r--r--   0        0        0      109 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/nav/__init__.py
+-rw-r--r--   0        0        0     5161 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/nav/bar.py
+-rw-r--r--   0        0        0     5781 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/nav/core.py
+-rw-r--r--   0        0        0      427 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/nav/elements.py
+-rw-r--r--   0        0        0     3197 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/nav/nav.py
+-rw-r--r--   0        0        0    70330 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-grid.css
+-rw-r--r--   0        0        0   203179 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    51796 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0   115988 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0    70404 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-grid.rtl.css
+-rw-r--r--   0        0        0   203183 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0        0        0    51871 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0        0        0   116065 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0        0        0    12066 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0   129328 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0    10127 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    51370 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0    12059 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0        0        0   129343 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0        0        0    10199 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0        0        0    63944 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0        0        0   107824 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-utilities.css
+-rw-r--r--   0        0        0   267492 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-utilities.css.map
+-rw-r--r--   0        0        0    85353 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-utilities.min.css
+-rw-r--r--   0        0        0   180382 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0        0        0   107692 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0        0        0   267433 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0        0        0    85282 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0        0        0   180218 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0        0        0   280814 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap.css
+-rw-r--r--   0        0        0   679012 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap.css.map
+-rw-r--r--   0        0        0   232949 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0   589162 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0   280393 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap.rtl.css
+-rw-r--r--   0        0        0   678857 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap.rtl.css.map
+-rw-r--r--   0        0        0   233056 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0   588696 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0        0        0    88585 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/icons/bootstrap-icons.css
+-rw-r--r--   0        0        0    47188 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/icons/bootstrap-icons.json
+-rw-r--r--   0        0        0   211136 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/icons/bootstrap-icons.scss
+-rw-r--r--   0        0        0   972584 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/icons/bootstrap-icons.svg
+-rw-r--r--   0        0        0   207731 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   444287 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80664 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   331887 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   135747 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   305153 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    74155 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   222463 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145313 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/js/bootstrap.js
+-rw-r--r--   0        0        0   306321 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60578 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/js/bootstrap.min.js
+-rw-r--r--   0        0        0   220351 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/static/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0      303 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/table/__init__.py
+-rw-r--r--   0        0        0     5552 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/table/base.py
+-rw-r--r--   0        0        0     2862 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/table/columns.py
+-rw-r--r--   0        0        0       67 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/testing/__init__.py
+-rw-r--r--   0        0        0     4939 2024-05-21 04:09:54.000000 bootlace-0.2.3/src/bootlace/testing/html.py
+-rw-r--r--   0        0        0     1222 2024-05-21 04:09:54.000000 bootlace-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1096 2024-05-21 04:09:54.000000 bootlace-0.2.3/LICENSE.txt
+-rw-r--r--   0        0        0      478 2024-05-21 04:09:54.000000 bootlace-0.2.3/README.md
+-rw-r--r--   0        0        0     2687 2024-05-21 04:09:54.000000 bootlace-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1323 2024-05-21 04:09:54.000000 bootlace-0.2.3/PKG-INFO
```

### Comparing `bootlace-0.2.2/src/bootlace/breadcrumbs.py` & `bootlace-0.2.3/src/bootlace/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/endpoint.py` & `bootlace-0.2.3/src/bootlace/endpoint.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/extension.py` & `bootlace-0.2.3/src/bootlace/extension.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/icon.py` & `bootlace-0.2.3/src/bootlace/icon.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/links.py` & `bootlace-0.2.3/src/bootlace/links.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/resources.py` & `bootlace-0.2.3/src/bootlace/resources.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/size.py` & `bootlace-0.2.3/src/bootlace/size.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/style.py` & `bootlace-0.2.3/src/bootlace/style.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/util.py` & `bootlace-0.2.3/src/bootlace/util.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/forms/fields.py` & `bootlace-0.2.3/src/bootlace/forms/fields.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/forms/widgets.py` & `bootlace-0.2.3/src/bootlace/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/forms/templates/bootlace/_form.html` & `bootlace-0.2.3/src/bootlace/forms/templates/bootlace/_form.html`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/nav/bar.py` & `bootlace-0.2.3/src/bootlace/nav/bar.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/nav/core.py` & `bootlace-0.2.3/src/bootlace/nav/core.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/nav/nav.py` & `bootlace-0.2.3/src/bootlace/nav/nav.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.css` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.css.map` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.min.css` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.min.css.map` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.rtl.css` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.rtl.css.map` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.rtl.min.css` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.rtl.min.css.map` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.css` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.css.map` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.min.css` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.min.css.map` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.rtl.css` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.rtl.css.map` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.rtl.min.css` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.rtl.min.css.map` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.css` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.css.map` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.min.css` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.min.css.map` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.rtl.css` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.rtl.css.map` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.rtl.min.css` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.rtl.min.css.map` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap.css` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap.css.map` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap.min.css` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap.min.css.map` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap.rtl.css` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap.rtl.css.map` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap.rtl.min.css` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/css/bootstrap.rtl.min.css.map` & `bootlace-0.2.3/src/bootlace/static/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/icons/bootstrap-icons.css` & `bootlace-0.2.3/src/bootlace/static/icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/icons/bootstrap-icons.json` & `bootlace-0.2.3/src/bootlace/static/icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/icons/bootstrap-icons.scss` & `bootlace-0.2.3/src/bootlace/static/icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/icons/bootstrap-icons.svg` & `bootlace-0.2.3/src/bootlace/static/icons/bootstrap-icons.svg`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/js/bootstrap.bundle.js` & `bootlace-0.2.3/src/bootlace/static/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/js/bootstrap.bundle.js.map` & `bootlace-0.2.3/src/bootlace/static/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/js/bootstrap.bundle.min.js` & `bootlace-0.2.3/src/bootlace/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/js/bootstrap.bundle.min.js.map` & `bootlace-0.2.3/src/bootlace/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/js/bootstrap.esm.js` & `bootlace-0.2.3/src/bootlace/static/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/js/bootstrap.esm.js.map` & `bootlace-0.2.3/src/bootlace/static/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/js/bootstrap.esm.min.js` & `bootlace-0.2.3/src/bootlace/static/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/js/bootstrap.esm.min.js.map` & `bootlace-0.2.3/src/bootlace/static/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/js/bootstrap.js` & `bootlace-0.2.3/src/bootlace/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/js/bootstrap.js.map` & `bootlace-0.2.3/src/bootlace/static/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/js/bootstrap.min.js` & `bootlace-0.2.3/src/bootlace/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/static/js/bootstrap.min.js.map` & `bootlace-0.2.3/src/bootlace/static/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/table/base.py` & `bootlace-0.2.3/src/bootlace/table/base.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/table/columns.py` & `bootlace-0.2.3/src/bootlace/table/columns.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/src/bootlace/testing/html.py` & `bootlace-0.2.3/src/bootlace/testing/html.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/.gitignore` & `bootlace-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/LICENSE.txt` & `bootlace-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/pyproject.toml` & `bootlace-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.2/PKG-INFO` & `bootlace-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bootlace
-Version: 0.2.2
+Version: 0.2.3
 Summary: Pythonic Bootstrap Utilities
 Project-URL: Documentation, https://github.com/alexrudy/bootlace#readme
 Project-URL: Issues, https://github.com/alexrudy/bootlace/issues
 Project-URL: Source, https://github.com/alexrudy/bootlace
 Author-email: Alex Rudy <github@alexrudy.net>
 License-Expression: MIT
 License-File: LICENSE.txt
```

