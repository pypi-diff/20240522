# Comparing `tmp/conf_ini_g-2024.1.tar.gz` & `tmp/conf_ini_g-2024.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf_ini_g-2024.1.tar", last modified: Mon Apr 15 11:17:02 2024, max compression
+gzip compressed data, was "conf_ini_g-2024.2.tar", last modified: Wed May 22 17:16:46 2024, max compression
```

## Comparing `conf_ini_g-2024.1.tar` & `conf_ini_g-2024.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.423001 conf_ini_g-2024.1/
--rwx------   0 eric      (1000) users      (984)      114 2023-03-01 07:58:57.000000 conf_ini_g-2024.1/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4554 2024-04-15 11:17:02.423001 conf_ini_g-2024.1/PKG-INFO
--rwx------   0 eric      (1000) users      (984)      636 2023-03-01 08:10:10.000000 conf_ini_g-2024.1/README-COPYRIGHT-utf8.txt
--rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 conf_ini_g-2024.1/README-LICENCE-utf8.txt
--rwx------   0 eric      (1000) users      (984)     3536 2023-03-01 09:58:27.000000 conf_ini_g-2024.1/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.416334 conf_ini_g-2024.1/conf_ini_g/
--rwx------   0 eric      (1000) users      (984)     1597 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.413001 conf_ini_g-2024.1/conf_ini_g/catalog/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.413001 conf_ini_g-2024.1/conf_ini_g/catalog/interface/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.413001 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.416334 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/
--rwx------   0 eric      (1000) users      (984)     3643 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/boolean.py
--rwx------   0 eric      (1000) users      (984)     5727 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/callable.py
--rwx------   0 eric      (1000) users      (984)     3833 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/choices.py
--rwx------   0 eric      (1000) users      (984)    10756 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/collection.py
--rwx------   0 eric      (1000) users      (984)     4036 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/directory.py
--rwx------   0 eric      (1000) users      (984)     3616 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/multitype.py
--rwx------   0 eric      (1000) users      (984)     2212 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/none.py
--rwx------   0 eric      (1000) users      (984)     6879 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/path.py
--rwx------   0 eric      (1000) users      (984)     2521 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/text_line.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.413001 conf_ini_g-2024.1/conf_ini_g/catalog/specification/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.416334 conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/
--rwx------   0 eric      (1000) users      (984)     2701 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/boolean.py
--rwx------   0 eric      (1000) users      (984)     3007 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/callable.py
--rwx------   0 eric      (1000) users      (984)     3162 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/choices.py
--rwx------   0 eric      (1000) users      (984)     4991 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/collection.py
--rwx------   0 eric      (1000) users      (984)     4823 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/number.py
--rwx------   0 eric      (1000) users      (984)     3250 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/path.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.416334 conf_ini_g-2024.1/conf_ini_g/extension/
--rwx------   0 eric      (1000) users      (984)     3082 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/extension/path.py
--rwx------   0 eric      (1000) users      (984)     3731 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/extension/python.py
--rwx------   0 eric      (1000) users      (984)     2436 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/extension/string.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.416334 conf_ini_g-2024.1/conf_ini_g/interface/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/interface/console/
--rwx------   0 eric      (1000) users      (984)     7001 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/console/config.py
--rwx------   0 eric      (1000) users      (984)     1783 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/constant.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/interface/storage/
--rwx------   0 eric      (1000) users      (984)     7519 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/storage/config.py
--rwx------   0 eric      (1000) users      (984)     1634 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/storage/parameter.py
--rwx------   0 eric      (1000) users      (984)     1598 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/storage/section.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/interface/window/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/interface/window/config/
--rwx------   0 eric      (1000) users      (984)     3293 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/config/action.py
--rwx------   0 eric      (1000) users      (984)     2471 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/config/advanced.py
--rwx------   0 eric      (1000) users      (984)    16998 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/config/main.py
--rwx------   0 eric      (1000) users      (984)     4113 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/config/title.py
--rwx------   0 eric      (1000) users      (984)     1862 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/generic.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/interface/window/parameter/
--rwx------   0 eric      (1000) users      (984)     5386 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/parameter/main.py
--rwx------   0 eric      (1000) users      (984)     2235 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/parameter/type.py
--rwx------   0 eric      (1000) users      (984)     2958 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/parameter/value.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/interface/window/section/
--rwx------   0 eric      (1000) users      (984)     4039 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/section/collection.py
--rwx------   0 eric      (1000) users      (984)     8783 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/section/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/light/
--rwx------   0 eric      (1000) users      (984)     4259 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/light/config.py
--rwx------   0 eric      (1000) users      (984)     3763 2024-04-15 11:06:57.000000 conf_ini_g-2024.1/conf_ini_g/light/conversion.py
--rwx------   0 eric      (1000) users      (984)     2607 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/light/ini.py
--rwx------   0 eric      (1000) users      (984)     2102 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/light/xlsx.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.413001 conf_ini_g-2024.1/conf_ini_g/phase/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/phase/generic/
--rwx------   0 eric      (1000) users      (984)     4025 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/generic/config.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/phase/specification/
--rwx------   0 eric      (1000) users      (984)     3294 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/base.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/phase/specification/config/
--rwx------   0 eric      (1000) users      (984)    13255 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/config/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/phase/specification/parameter/
--rwx------   0 eric      (1000) users      (984)     4284 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/parameter/main.py
--rwx------   0 eric      (1000) users      (984)     3569 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/parameter/type.py
--rwx------   0 eric      (1000) users      (984)     2445 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/parameter/unit.py
--rwx------   0 eric      (1000) users      (984)     1853 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/parameter/value.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/phase/specification/section/
--rwx------   0 eric      (1000) users      (984)     2390 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/section/controller.py
--rwx------   0 eric      (1000) users      (984)     6306 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/section/generic.py
--rwx------   0 eric      (1000) users      (984)     6543 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/section/specific.py
--rwx------   0 eric      (1000) users      (984)     1845 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/section/unit.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.413001 conf_ini_g-2024.1/conf_ini_g/phase/typed/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/phase/typed/config/
--rwx------   0 eric      (1000) users      (984)     7985 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/typed/config/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/phase/typed/parameter/
--rwx------   0 eric      (1000) users      (984)     1936 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/typed/parameter/invalid.py
--rwx------   0 eric      (1000) users      (984)     2833 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/typed/parameter/main.py
--rwx------   0 eric      (1000) users      (984)     2572 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/typed/parameter/unit.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/phase/typed/section/
--rwx------   0 eric      (1000) users      (984)     2705 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/typed/section/units.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/phase/untyped/
--rwx------   0 eric      (1000) users      (984)     1628 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/untyped/config.py
--rwx------   0 eric      (1000) users      (984)     2637 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/untyped/parameter.py
--rwx------   0 eric      (1000) users      (984)     2588 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/untyped/section.py
--rwx------   0 eric      (1000) users      (984)     1616 2024-04-15 11:15:25.000000 conf_ini_g-2024.1/conf_ini_g/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4554 2024-04-15 11:17:02.000000 conf_ini_g-2024.1/conf_ini_g.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     2870 2024-04-15 11:17:02.000000 conf_ini_g-2024.1/conf_ini_g.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-15 11:17:02.000000 conf_ini_g-2024.1/conf_ini_g.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       51 2024-04-15 11:17:02.000000 conf_ini_g-2024.1/conf_ini_g.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)       11 2024-04-15 11:17:02.000000 conf_ini_g-2024.1/conf_ini_g.egg-info/top_level.txt
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.413001 conf_ini_g-2024.1/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/documentation/wiki/
--rwx------   0 eric      (1000) users      (984)     1982 2023-03-01 10:23:59.000000 conf_ini_g-2024.1/documentation/wiki/description.asciidoc
--rwx------   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 conf_ini_g-2024.1/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-15 11:17:02.423001 conf_ini_g-2024.1/setup.cfg
--rwx------   0 eric      (1000) users      (984)     6607 2023-11-09 15:02:40.000000 conf_ini_g-2024.1/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.509441 conf_ini_g-2024.2/
+-rwx------   0 eric      (1000) users      (984)      114 2023-03-01 07:58:57.000000 conf_ini_g-2024.2/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4554 2024-05-22 17:16:46.509441 conf_ini_g-2024.2/PKG-INFO
+-rwx------   0 eric      (1000) users      (984)      636 2023-03-01 08:10:10.000000 conf_ini_g-2024.2/README-COPYRIGHT-utf8.txt
+-rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 conf_ini_g-2024.2/README-LICENCE-utf8.txt
+-rwx------   0 eric      (1000) users      (984)     3536 2023-03-01 09:58:27.000000 conf_ini_g-2024.2/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.489441 conf_ini_g-2024.2/conf_ini_g/
+-rwx------   0 eric      (1000) users      (984)     1597 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.486108 conf_ini_g-2024.2/conf_ini_g/catalog/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.482774 conf_ini_g-2024.2/conf_ini_g/catalog/interface/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.486108 conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.492774 conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/
+-rwx------   0 eric      (1000) users      (984)     3643 2024-05-22 17:11:01.000000 conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/boolean.py
+-rwx------   0 eric      (1000) users      (984)     5727 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/callable.py
+-rwx------   0 eric      (1000) users      (984)     3833 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/choices.py
+-rwx------   0 eric      (1000) users      (984)    10756 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/collection.py
+-rwx------   0 eric      (1000) users      (984)     4036 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/directory.py
+-rwx------   0 eric      (1000) users      (984)     3616 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/multitype.py
+-rwx------   0 eric      (1000) users      (984)     2212 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/none.py
+-rwx------   0 eric      (1000) users      (984)     6879 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/path.py
+-rwx------   0 eric      (1000) users      (984)     2521 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/text_line.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.486108 conf_ini_g-2024.2/conf_ini_g/catalog/specification/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.492774 conf_ini_g-2024.2/conf_ini_g/catalog/specification/annotation/
+-rwx------   0 eric      (1000) users      (984)     2701 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/catalog/specification/annotation/boolean.py
+-rwx------   0 eric      (1000) users      (984)     3007 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/catalog/specification/annotation/callable.py
+-rwx------   0 eric      (1000) users      (984)     3162 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/catalog/specification/annotation/choices.py
+-rwx------   0 eric      (1000) users      (984)     4991 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/catalog/specification/annotation/collection.py
+-rwx------   0 eric      (1000) users      (984)     4823 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/catalog/specification/annotation/number.py
+-rwx------   0 eric      (1000) users      (984)     3250 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/catalog/specification/annotation/path.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.496108 conf_ini_g-2024.2/conf_ini_g/extension/
+-rwx------   0 eric      (1000) users      (984)     3082 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/extension/path.py
+-rwx------   0 eric      (1000) users      (984)     3731 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/extension/python.py
+-rwx------   0 eric      (1000) users      (984)     2436 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/extension/string.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.496108 conf_ini_g-2024.2/conf_ini_g/interface/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.496108 conf_ini_g-2024.2/conf_ini_g/interface/console/
+-rwx------   0 eric      (1000) users      (984)     7001 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/interface/console/config.py
+-rwx------   0 eric      (1000) users      (984)     1783 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/interface/constant.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.496108 conf_ini_g-2024.2/conf_ini_g/interface/storage/
+-rwx------   0 eric      (1000) users      (984)     7519 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/interface/storage/config.py
+-rwx------   0 eric      (1000) users      (984)     1634 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/interface/storage/parameter.py
+-rwx------   0 eric      (1000) users      (984)     1598 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/interface/storage/section.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.496108 conf_ini_g-2024.2/conf_ini_g/interface/window/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.499441 conf_ini_g-2024.2/conf_ini_g/interface/window/config/
+-rwx------   0 eric      (1000) users      (984)     3293 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/interface/window/config/action.py
+-rwx------   0 eric      (1000) users      (984)     2471 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/interface/window/config/advanced.py
+-rwx------   0 eric      (1000) users      (984)    16998 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/interface/window/config/main.py
+-rwx------   0 eric      (1000) users      (984)     4113 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/interface/window/config/title.py
+-rwx------   0 eric      (1000) users      (984)     1862 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/interface/window/generic.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.499441 conf_ini_g-2024.2/conf_ini_g/interface/window/parameter/
+-rwx------   0 eric      (1000) users      (984)     5386 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/interface/window/parameter/main.py
+-rwx------   0 eric      (1000) users      (984)     2235 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/interface/window/parameter/type.py
+-rwx------   0 eric      (1000) users      (984)     2958 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/interface/window/parameter/value.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.499441 conf_ini_g-2024.2/conf_ini_g/interface/window/section/
+-rwx------   0 eric      (1000) users      (984)     4039 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/interface/window/section/collection.py
+-rwx------   0 eric      (1000) users      (984)     8783 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/interface/window/section/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.499441 conf_ini_g-2024.2/conf_ini_g/light/
+-rwx------   0 eric      (1000) users      (984)     4259 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/light/config.py
+-rwx------   0 eric      (1000) users      (984)     3763 2024-04-15 11:06:57.000000 conf_ini_g-2024.2/conf_ini_g/light/conversion.py
+-rwx------   0 eric      (1000) users      (984)     2607 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/light/ini.py
+-rwx------   0 eric      (1000) users      (984)     2102 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/light/xlsx.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.486108 conf_ini_g-2024.2/conf_ini_g/phase/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.499441 conf_ini_g-2024.2/conf_ini_g/phase/generic/
+-rwx------   0 eric      (1000) users      (984)     4025 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/generic/config.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.502774 conf_ini_g-2024.2/conf_ini_g/phase/specification/
+-rwx------   0 eric      (1000) users      (984)     3294 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/specification/base.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.502774 conf_ini_g-2024.2/conf_ini_g/phase/specification/config/
+-rwx------   0 eric      (1000) users      (984)    13255 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/specification/config/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.502774 conf_ini_g-2024.2/conf_ini_g/phase/specification/parameter/
+-rwx------   0 eric      (1000) users      (984)     4284 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/specification/parameter/main.py
+-rwx------   0 eric      (1000) users      (984)     3569 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/specification/parameter/type.py
+-rwx------   0 eric      (1000) users      (984)     2445 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/specification/parameter/unit.py
+-rwx------   0 eric      (1000) users      (984)     1853 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/specification/parameter/value.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.506108 conf_ini_g-2024.2/conf_ini_g/phase/specification/section/
+-rwx------   0 eric      (1000) users      (984)     2390 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/specification/section/controller.py
+-rwx------   0 eric      (1000) users      (984)     6306 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/specification/section/generic.py
+-rwx------   0 eric      (1000) users      (984)     6543 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/specification/section/specific.py
+-rwx------   0 eric      (1000) users      (984)     1845 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/specification/section/unit.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.486108 conf_ini_g-2024.2/conf_ini_g/phase/typed/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.506108 conf_ini_g-2024.2/conf_ini_g/phase/typed/config/
+-rwx------   0 eric      (1000) users      (984)     7985 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/typed/config/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.506108 conf_ini_g-2024.2/conf_ini_g/phase/typed/parameter/
+-rwx------   0 eric      (1000) users      (984)     1936 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/typed/parameter/invalid.py
+-rwx------   0 eric      (1000) users      (984)     2833 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/typed/parameter/main.py
+-rwx------   0 eric      (1000) users      (984)     2572 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/typed/parameter/unit.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.506108 conf_ini_g-2024.2/conf_ini_g/phase/typed/section/
+-rwx------   0 eric      (1000) users      (984)     2705 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/typed/section/units.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.506108 conf_ini_g-2024.2/conf_ini_g/phase/untyped/
+-rwx------   0 eric      (1000) users      (984)     1628 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/untyped/config.py
+-rwx------   0 eric      (1000) users      (984)     2637 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/untyped/parameter.py
+-rwx------   0 eric      (1000) users      (984)     2588 2024-04-15 11:10:03.000000 conf_ini_g-2024.2/conf_ini_g/phase/untyped/section.py
+-rwx------   0 eric      (1000) users      (984)     1616 2024-05-22 17:16:00.000000 conf_ini_g-2024.2/conf_ini_g/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.509441 conf_ini_g-2024.2/conf_ini_g.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4554 2024-05-22 17:16:46.000000 conf_ini_g-2024.2/conf_ini_g.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     2870 2024-05-22 17:16:46.000000 conf_ini_g-2024.2/conf_ini_g.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2024-05-22 17:16:46.000000 conf_ini_g-2024.2/conf_ini_g.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       51 2024-05-22 17:16:46.000000 conf_ini_g-2024.2/conf_ini_g.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)       11 2024-05-22 17:16:46.000000 conf_ini_g-2024.2/conf_ini_g.egg-info/top_level.txt
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.486108 conf_ini_g-2024.2/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 17:16:46.506108 conf_ini_g-2024.2/documentation/wiki/
+-rwx------   0 eric      (1000) users      (984)     1982 2023-03-01 10:23:59.000000 conf_ini_g-2024.2/documentation/wiki/description.asciidoc
+-rwx------   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 conf_ini_g-2024.2/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2024-05-22 17:16:46.509441 conf_ini_g-2024.2/setup.cfg
+-rwx------   0 eric      (1000) users      (984)     6607 2023-11-09 15:02:40.000000 conf_ini_g-2024.2/setup.py
```

### Comparing `conf_ini_g-2024.1/PKG-INFO` & `conf_ini_g-2024.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conf-ini-g
-Version: 2024.1
+Version: 2024.2
 Summary: App Configuration in INI format with Automatic Command-Line Parser and Graphical Interface Generation
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
```

### Comparing `conf_ini_g-2024.1/README-COPYRIGHT-utf8.txt` & `conf_ini_g-2024.2/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/README-LICENCE-utf8.txt` & `conf_ini_g-2024.2/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/README.rst` & `conf_ini_g-2024.2/README.rst`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/__init__.py` & `conf_ini_g-2024.2/conf_ini_g/__init__.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/boolean.py` & `conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/boolean.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -54,16 +54,14 @@
         stripe: type_t | boolean_t | None,
         backend: backend_t,
         /,
     ) -> boolean_wgt_t:
         """"""
         output = cls(library_wgt=backend.base_t())
 
-        output.SetupValueChangedMessaging(output.true_btn, "released", backend)
-
         if stripe is None:
             annotation = None
         elif isinstance(stripe, type_t):
             annotation = stripe.FirstAnnotationWithType(boolean_t)
         else:
             annotation = stripe
         if annotation is None:
@@ -73,14 +71,16 @@
 
         true_btn = backend.radio_choice_t(labels[0], parent=output.library_wgt)
         false_btn = backend.radio_choice_t(labels[1], parent=output.library_wgt)
 
         output.true_btn = true_btn
         output.false_btn = false_btn
 
+        output.SetupValueChangedMessaging(output.true_btn, "released", backend)
+
         layout = backend.hbox_lyt_t()
         layout.setContentsMargins(0, 0, 0, 0)
         layout.addWidget(true_btn)
         layout.addWidget(false_btn)
         output.library_wgt.setLayout(layout)
 
         return output
```

### Comparing `conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/callable.py` & `conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/callable.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/choices.py` & `conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/choices.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/collection.py` & `conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/collection.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/directory.py` & `conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/directory.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/multitype.py` & `conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/multitype.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/none.py` & `conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/none.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/path.py` & `conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/path.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/text_line.py` & `conf_ini_g-2024.2/conf_ini_g/catalog/interface/window/parameter/text_line.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/boolean.py` & `conf_ini_g-2024.2/conf_ini_g/catalog/specification/annotation/boolean.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/callable.py` & `conf_ini_g-2024.2/conf_ini_g/catalog/specification/annotation/callable.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/choices.py` & `conf_ini_g-2024.2/conf_ini_g/catalog/specification/annotation/choices.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/collection.py` & `conf_ini_g-2024.2/conf_ini_g/catalog/specification/annotation/collection.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/number.py` & `conf_ini_g-2024.2/conf_ini_g/catalog/specification/annotation/number.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/path.py` & `conf_ini_g-2024.2/conf_ini_g/catalog/specification/annotation/path.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/extension/path.py` & `conf_ini_g-2024.2/conf_ini_g/extension/path.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/extension/python.py` & `conf_ini_g-2024.2/conf_ini_g/extension/python.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/extension/string.py` & `conf_ini_g-2024.2/conf_ini_g/extension/string.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/interface/console/config.py` & `conf_ini_g-2024.2/conf_ini_g/interface/console/config.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/interface/constant.py` & `conf_ini_g-2024.2/conf_ini_g/interface/constant.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/interface/storage/config.py` & `conf_ini_g-2024.2/conf_ini_g/interface/storage/config.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/interface/storage/parameter.py` & `conf_ini_g-2024.2/conf_ini_g/interface/storage/parameter.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/interface/storage/section.py` & `conf_ini_g-2024.2/conf_ini_g/interface/storage/section.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/interface/window/config/action.py` & `conf_ini_g-2024.2/conf_ini_g/interface/window/config/action.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/interface/window/config/advanced.py` & `conf_ini_g-2024.2/conf_ini_g/interface/window/config/advanced.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/interface/window/config/main.py` & `conf_ini_g-2024.2/conf_ini_g/interface/window/config/main.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/interface/window/config/title.py` & `conf_ini_g-2024.2/conf_ini_g/interface/window/config/title.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/interface/window/generic.py` & `conf_ini_g-2024.2/conf_ini_g/interface/window/generic.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/interface/window/parameter/main.py` & `conf_ini_g-2024.2/conf_ini_g/interface/window/parameter/main.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/interface/window/parameter/type.py` & `conf_ini_g-2024.2/conf_ini_g/interface/window/parameter/type.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/interface/window/parameter/value.py` & `conf_ini_g-2024.2/conf_ini_g/interface/window/parameter/value.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/interface/window/section/collection.py` & `conf_ini_g-2024.2/conf_ini_g/interface/window/section/collection.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/interface/window/section/main.py` & `conf_ini_g-2024.2/conf_ini_g/interface/window/section/main.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/light/config.py` & `conf_ini_g-2024.2/conf_ini_g/light/config.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/light/conversion.py` & `conf_ini_g-2024.2/conf_ini_g/light/conversion.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/light/ini.py` & `conf_ini_g-2024.2/conf_ini_g/light/ini.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/light/xlsx.py` & `conf_ini_g-2024.2/conf_ini_g/light/xlsx.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/generic/config.py` & `conf_ini_g-2024.2/conf_ini_g/phase/generic/config.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/specification/base.py` & `conf_ini_g-2024.2/conf_ini_g/phase/specification/base.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/specification/config/main.py` & `conf_ini_g-2024.2/conf_ini_g/phase/specification/config/main.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/specification/parameter/main.py` & `conf_ini_g-2024.2/conf_ini_g/phase/specification/parameter/main.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/specification/parameter/type.py` & `conf_ini_g-2024.2/conf_ini_g/phase/specification/parameter/type.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/specification/parameter/unit.py` & `conf_ini_g-2024.2/conf_ini_g/phase/specification/parameter/unit.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/specification/parameter/value.py` & `conf_ini_g-2024.2/conf_ini_g/phase/specification/parameter/value.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/specification/section/controller.py` & `conf_ini_g-2024.2/conf_ini_g/phase/specification/section/controller.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/specification/section/generic.py` & `conf_ini_g-2024.2/conf_ini_g/phase/specification/section/generic.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/specification/section/specific.py` & `conf_ini_g-2024.2/conf_ini_g/phase/specification/section/specific.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/specification/section/unit.py` & `conf_ini_g-2024.2/conf_ini_g/phase/specification/section/unit.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/typed/config/main.py` & `conf_ini_g-2024.2/conf_ini_g/phase/typed/config/main.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/typed/parameter/invalid.py` & `conf_ini_g-2024.2/conf_ini_g/phase/typed/parameter/invalid.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/typed/parameter/main.py` & `conf_ini_g-2024.2/conf_ini_g/phase/typed/parameter/main.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/typed/parameter/unit.py` & `conf_ini_g-2024.2/conf_ini_g/phase/typed/parameter/unit.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/typed/section/units.py` & `conf_ini_g-2024.2/conf_ini_g/phase/typed/section/units.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/untyped/config.py` & `conf_ini_g-2024.2/conf_ini_g/phase/untyped/config.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/untyped/parameter.py` & `conf_ini_g-2024.2/conf_ini_g/phase/untyped/parameter.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/phase/untyped/section.py` & `conf_ini_g-2024.2/conf_ini_g/phase/untyped/section.py`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/conf_ini_g/version.py` & `conf_ini_g-2024.2/conf_ini_g/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,10 +25,10 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2024.1"
+__version__ = "2024.2"
 
 # TODO: Callable parameter still a WIP.
```

### Comparing `conf_ini_g-2024.1/conf_ini_g.egg-info/PKG-INFO` & `conf_ini_g-2024.2/conf_ini_g.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conf-ini-g
-Version: 2024.1
+Version: 2024.2
 Summary: App Configuration in INI format with Automatic Command-Line Parser and Graphical Interface Generation
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
```

### Comparing `conf_ini_g-2024.1/conf_ini_g.egg-info/SOURCES.txt` & `conf_ini_g-2024.2/conf_ini_g.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/documentation/wiki/description.asciidoc` & `conf_ini_g-2024.2/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `conf_ini_g-2024.1/setup.py` & `conf_ini_g-2024.2/setup.py`

 * *Files identical despite different names*

