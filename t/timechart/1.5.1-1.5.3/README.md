# Comparing `tmp/timechart-1.5.1.tar.gz` & `tmp/timechart-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timechart-1.5.1.tar", last modified: Thu Sep  1 19:36:58 2022, max compression
+gzip compressed data, was "timechart-1.5.3.tar", last modified: Tue May 21 22:17:47 2024, max compression
```

## Comparing `timechart-1.5.1.tar` & `timechart-1.5.3.tar`

### file list

```diff
@@ -1,48 +1,97 @@
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-09-01 19:36:58.956053 timechart-1.5.1/
--rw-r--r--   0 klauer   (1318172782) 1704612529     2449 2022-06-03 18:48:27.000000 timechart-1.5.1/LICENSE.md
--rw-r--r--   0 klauer   (1318172782) 1704612529      136 2022-06-03 18:48:27.000000 timechart-1.5.1/MANIFEST.in
--rw-r--r--   0 klauer   (1318172782) 1704612529      495 2022-09-01 19:36:58.956198 timechart-1.5.1/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529     1270 2022-06-03 18:48:27.000000 timechart-1.5.1/README.md
--rw-r--r--   0 klauer   (1318172782) 1704612529       53 2022-06-03 18:48:27.000000 timechart-1.5.1/requirements.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529      177 2022-09-01 19:36:58.956670 timechart-1.5.1/setup.cfg
--rw-r--r--   0 klauer   (1318172782) 1704612529     1341 2022-06-03 18:48:27.000000 timechart-1.5.1/setup.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-09-01 19:36:58.957056 timechart-1.5.1/timechart/
--rw-r--r--   0 klauer   (1318172782) 1704612529       92 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      497 2022-09-01 19:36:58.957174 timechart-1.5.1/timechart/_version.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-09-01 19:36:58.950147 timechart-1.5.1/timechart/data_io/
--rw-r--r--   0 klauer   (1318172782) 1704612529        1 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart/data_io/__init__.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-09-01 19:36:58.951014 timechart-1.5.1/timechart/data_io/importers/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart/data_io/importers/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     9072 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart/data_io/importers/striptool_config_importer.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     7559 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart/data_io/importers/timechart_config_importer.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     4873 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart/data_io/settings_exporter.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3184 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart/data_io/settings_importer.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-09-01 19:36:58.952793 timechart-1.5.1/timechart/displays/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart/displays/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     9072 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart/displays/axis_settings_display.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    10611 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart/displays/chart_data_export_display.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     9654 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart/displays/curve_settings_display.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      664 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart/displays/defaults.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    51741 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart/displays/main_display.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3158 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart/tool.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-09-01 19:36:58.953437 timechart-1.5.1/timechart/utilities/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart/utilities/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3443 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart/utilities/utils.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-09-01 19:36:58.949226 timechart-1.5.1/timechart.egg-info/
--rw-r--r--   0 klauer   (1318172782) 1704612529      495 2022-09-01 19:36:58.000000 timechart-1.5.1/timechart.egg-info/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529     1195 2022-09-01 19:36:58.000000 timechart-1.5.1/timechart.egg-info/SOURCES.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        1 2022-09-01 19:36:58.000000 timechart-1.5.1/timechart.egg-info/dependency_links.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529      114 2022-09-01 19:36:58.000000 timechart-1.5.1/timechart.egg-info/entry_points.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       53 2022-09-01 19:36:58.000000 timechart-1.5.1/timechart.egg-info/requires.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       29 2022-09-01 19:36:58.000000 timechart-1.5.1/timechart.egg-info/top_level.txt
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-09-01 19:36:58.954009 timechart-1.5.1/timechart_launcher/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart_launcher/__init__.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-09-01 19:36:58.955814 timechart-1.5.1/timechart_launcher/icons/
--rw-r--r--   0 klauer   (1318172782) 1704612529     4609 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart_launcher/icons/charts_128.png
--rw-r--r--   0 klauer   (1318172782) 1704612529      665 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart_launcher/icons/charts_16.png
--rw-r--r--   0 klauer   (1318172782) 1704612529      988 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart_launcher/icons/charts_24.png
--rw-r--r--   0 klauer   (1318172782) 1704612529     8255 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart_launcher/icons/charts_256.png
--rw-r--r--   0 klauer   (1318172782) 1704612529     1313 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart_launcher/icons/charts_32.png
--rw-r--r--   0 klauer   (1318172782) 1704612529     2685 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart_launcher/icons/charts_64.png
--rw-r--r--   0 klauer   (1318172782) 1704612529     3260 2022-06-03 18:48:27.000000 timechart-1.5.1/timechart_launcher/main.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    68611 2022-06-03 18:48:27.000000 timechart-1.5.1/versioneer.py
+drwxrwxr-x   0 roberttk (1215380206) 1704612529        0 2024-05-21 22:17:47.186040 timechart-1.5.3/
+-rw-rw-r--   0 roberttk (1215380206) 1704612529      130 2024-05-21 20:24:59.000000 timechart-1.5.3/.coveragerc
+-rw-rw-r--   0 roberttk (1215380206) 1704612529      125 2024-05-21 20:24:59.000000 timechart-1.5.3/.git_archival.txt
+-rw-rw-r--   0 roberttk (1215380206) 1704612529       32 2024-05-21 20:24:59.000000 timechart-1.5.3/.gitattributes
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     1296 2024-05-21 20:24:59.000000 timechart-1.5.3/.gitignore
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     3624 2024-05-21 20:24:59.000000 timechart-1.5.3/.travis.yml
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     2468 2024-05-21 20:24:59.000000 timechart-1.5.3/LICENSE.md
+-rw-rw-r--   0 roberttk (1215380206) 1704612529      136 2024-05-21 20:24:59.000000 timechart-1.5.3/MANIFEST.in
+-rw-r--r--   0 roberttk (1215380206) 1704612529     5040 2024-05-21 22:17:47.185717 timechart-1.5.3/PKG-INFO
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     1273 2024-05-21 22:17:12.000000 timechart-1.5.3/README.md
+drwxrwxr-x   0 roberttk (1215380206) 1704612529        0 2024-05-21 22:17:47.164436 timechart-1.5.3/conda-recipe/
+-rw-rw-r--   0 roberttk (1215380206) 1704612529       84 2024-05-21 20:24:59.000000 timechart-1.5.3/conda-recipe/bld.bat
+-rw-rw-r--   0 roberttk (1215380206) 1704612529      103 2024-05-21 20:24:59.000000 timechart-1.5.3/conda-recipe/build.sh
+-rw-rw-r--   0 roberttk (1215380206) 1704612529      651 2024-05-21 20:24:59.000000 timechart-1.5.3/conda-recipe/meta.yaml
+-rw-rw-r--   0 roberttk (1215380206) 1704612529       36 2024-05-21 20:24:59.000000 timechart-1.5.3/dev-requirements.txt
+drwxrwxr-x   0 roberttk (1215380206) 1704612529        0 2024-05-21 22:17:47.164765 timechart-1.5.3/docs/
+-rw-rw-r--   0 roberttk (1215380206) 1704612529      584 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/Makefile
+-rw-rw-r--   0 roberttk (1215380206) 1704612529      791 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/make.bat
+drwxrwxr-x   0 roberttk (1215380206) 1704612529        0 2024-05-21 22:17:47.166607 timechart-1.5.3/docs/source/
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     5656 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/source/conf.py
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     9691 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/source/control_panel.rst
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     1860 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/source/exporting_importing_settings.rst
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     1675 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/source/graphing.rst
+drwxrwxr-x   0 roberttk (1215380206) 1704612529        0 2024-05-21 22:17:47.171426 timechart-1.5.3/docs/source/images/
+-rw-rw-r--   0 roberttk (1215380206) 1704612529    71326 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/source/images/curves.png
+-rw-rw-r--   0 roberttk (1215380206) 1704612529   298889 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/source/images/data.png
+-rw-rw-r--   0 roberttk (1215380206) 1704612529    22883 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/source/images/export.png
+-rw-rw-r--   0 roberttk (1215380206) 1704612529   287572 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/source/images/graph.png
+-rw-rw-r--   0 roberttk (1215380206) 1704612529   224540 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/source/images/graphing.png
+-rw-rw-r--   0 roberttk (1215380206) 1704612529   269764 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/source/images/intro.png
+-rw-rw-r--   0 roberttk (1215380206) 1704612529   272470 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/source/images/right_click.png
+-rw-rw-r--   0 roberttk (1215380206) 1704612529   127571 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/source/images/ui_layout.png
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     1104 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/source/index.rst
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     6105 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/source/installing.rst
+-rw-rw-r--   0 roberttk (1215380206) 1704612529      502 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/source/introduction.rst
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     2462 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/source/running.rst
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     3281 2024-05-21 20:24:59.000000 timechart-1.5.3/docs/source/ui_layout.rst
+-rw-rw-r--   0 roberttk (1215380206) 1704612529       54 2024-05-21 20:24:59.000000 timechart-1.5.3/docs-requirements.txt
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     4452 2024-05-21 20:24:59.000000 timechart-1.5.3/github_deploy_key_slaclab_timechart.enc
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     1302 2024-05-21 20:24:59.000000 timechart-1.5.3/pyproject.toml
+-rw-rw-r--   0 roberttk (1215380206) 1704612529       53 2024-05-21 20:24:59.000000 timechart-1.5.3/requirements.txt
+-rw-rw-r--   0 roberttk (1215380206) 1704612529      542 2024-05-21 20:24:59.000000 timechart-1.5.3/run_tests.py
+-rw-rw-r--   0 roberttk (1215380206) 1704612529       38 2024-05-21 22:17:47.186100 timechart-1.5.3/setup.cfg
+drwxrwxr-x   0 roberttk (1215380206) 1704612529        0 2024-05-21 22:17:47.172723 timechart-1.5.3/timechart/
+-rw-rw-r--   0 roberttk (1215380206) 1704612529       47 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/__init__.py
+-rw-rw-r--   0 roberttk (1215380206) 1704612529      411 2024-05-21 22:17:47.000000 timechart-1.5.3/timechart/_version.py
+drwxrwxr-x   0 roberttk (1215380206) 1704612529        0 2024-05-21 22:17:47.174188 timechart-1.5.3/timechart/data_io/
+-rw-rw-r--   0 roberttk (1215380206) 1704612529        1 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/data_io/__init__.py
+drwxrwxr-x   0 roberttk (1215380206) 1704612529        0 2024-05-21 22:17:47.174780 timechart-1.5.3/timechart/data_io/importers/
+-rw-rw-r--   0 roberttk (1215380206) 1704612529        0 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/data_io/importers/__init__.py
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     9077 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/data_io/importers/striptool_config_importer.py
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     7559 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/data_io/importers/timechart_config_importer.py
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     4878 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/data_io/settings_exporter.py
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     3184 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/data_io/settings_importer.py
+drwxrwxr-x   0 roberttk (1215380206) 1704612529        0 2024-05-21 22:17:47.176410 timechart-1.5.3/timechart/displays/
+-rw-rw-r--   0 roberttk (1215380206) 1704612529        0 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/displays/__init__.py
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     9072 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/displays/axis_settings_display.py
+-rw-rw-r--   0 roberttk (1215380206) 1704612529    10611 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/displays/chart_data_export_display.py
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     9654 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/displays/curve_settings_display.py
+-rw-rw-r--   0 roberttk (1215380206) 1704612529      664 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/displays/defaults.py
+-rw-rw-r--   0 roberttk (1215380206) 1704612529    51741 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/displays/main_display.py
+drwxrwxr-x   0 roberttk (1215380206) 1704612529        0 2024-05-21 22:17:47.160432 timechart-1.5.3/timechart/tests/
+drwxrwxr-x   0 roberttk (1215380206) 1704612529        0 2024-05-21 22:17:47.177069 timechart-1.5.3/timechart/tests/striptool_config_import/
+-rw-rw-r--   0 roberttk (1215380206) 1704612529        0 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/tests/striptool_config_import/__init__.py
+drwxrwxr-x   0 roberttk (1215380206) 1704612529        0 2024-05-21 22:17:47.177583 timechart-1.5.3/timechart/tests/striptool_config_import/data/
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     1420 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/tests/striptool_config_import/data/strip.stp
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     1552 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/tests/striptool_config_import/data/twocurves.stp
+drwxrwxr-x   0 roberttk (1215380206) 1704612529        0 2024-05-21 22:17:47.177979 timechart-1.5.3/timechart/tests/striptool_config_import/expected_output/
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     1132 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/tests/striptool_config_import/expected_output/strip.stp.json
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     1421 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/tests/striptool_config_import/expected_output/twocurves.stp.json
+drwxrwxr-x   0 roberttk (1215380206) 1704612529        0 2024-05-21 22:17:47.178367 timechart-1.5.3/timechart/tests/striptool_config_import/output/
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     1213 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/tests/striptool_config_import/output/strip.stp.json
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     1513 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/tests/striptool_config_import/output/twocurves.stp.json
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     5672 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/tests/striptool_config_import/test_striptool_config_import.py
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     3158 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/tool.py
+drwxrwxr-x   0 roberttk (1215380206) 1704612529        0 2024-05-21 22:17:47.178735 timechart-1.5.3/timechart/utilities/
+-rw-rw-r--   0 roberttk (1215380206) 1704612529        0 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/utilities/__init__.py
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     3443 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/utilities/utils.py
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     1898 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart/version.py
+-rwxrwxr-x   0 roberttk (1215380206) 1704612529      145 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart.bash
+drwxrwxr-x   0 roberttk (1215380206) 1704612529        0 2024-05-21 22:17:47.184628 timechart-1.5.3/timechart.egg-info/
+-rw-r--r--   0 roberttk (1215380206) 1704612529     5040 2024-05-21 22:17:47.000000 timechart-1.5.3/timechart.egg-info/PKG-INFO
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     2477 2024-05-21 22:17:47.000000 timechart-1.5.3/timechart.egg-info/SOURCES.txt
+-rw-rw-r--   0 roberttk (1215380206) 1704612529        1 2024-05-21 22:17:47.000000 timechart-1.5.3/timechart.egg-info/dependency_links.txt
+-rw-rw-r--   0 roberttk (1215380206) 1704612529      113 2024-05-21 22:17:47.000000 timechart-1.5.3/timechart.egg-info/entry_points.txt
+-rw-rw-r--   0 roberttk (1215380206) 1704612529      157 2024-05-21 22:17:47.000000 timechart-1.5.3/timechart.egg-info/requires.txt
+-rw-rw-r--   0 roberttk (1215380206) 1704612529       29 2024-05-21 22:17:47.000000 timechart-1.5.3/timechart.egg-info/top_level.txt
+drwxrwxr-x   0 roberttk (1215380206) 1704612529        0 2024-05-21 22:17:47.179117 timechart-1.5.3/timechart_launcher/
+-rw-rw-r--   0 roberttk (1215380206) 1704612529        0 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart_launcher/__init__.py
+drwxrwxr-x   0 roberttk (1215380206) 1704612529        0 2024-05-21 22:17:47.184204 timechart-1.5.3/timechart_launcher/icons/
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     4609 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart_launcher/icons/charts_128.png
+-rw-rw-r--   0 roberttk (1215380206) 1704612529      665 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart_launcher/icons/charts_16.png
+-rw-rw-r--   0 roberttk (1215380206) 1704612529      988 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart_launcher/icons/charts_24.png
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     8255 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart_launcher/icons/charts_256.png
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     1313 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart_launcher/icons/charts_32.png
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     2685 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart_launcher/icons/charts_64.png
+-rw-rw-r--   0 roberttk (1215380206) 1704612529     3260 2024-05-21 20:24:59.000000 timechart-1.5.3/timechart_launcher/main.py
```

### Comparing `timechart-1.5.1/LICENSE.md` & `timechart-1.5.3/LICENSE.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,39 @@
-Copyright (c) 2017-2018, The Board of Trustees of the Leland Stanford Junior University, through SLAC National Accelerator Laboratory (subject to receipt of any required approvals from the U.S. Dept. of Energy). All rights reserved. Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
+University, through SLAC National Accelerator Laboratory (subject to receipt
+of any required approvals from the U.S. Dept. of Energy). All rights reserved.
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
 
-(1) Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+(1) Redistributions of source code must retain the above copyright notice,
+    this list of conditions and the following disclaimer.
 
-(2) Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+(2) Redistributions in binary form must reproduce the above copyright notice,
+    this list of conditions and the following disclaimer in the documentation
+    and/or other materials provided with the distribution.
 
-(3) Neither the name of the Leland Stanford Junior University, SLAC National Accelerator Laboratory, U.S. Dept. of Energy nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+(3) Neither the name of the Leland Stanford Junior University, SLAC National
+    Accelerator Laboratory, U.S. Dept. of Energy nor the names of its
+    contributors may be used to endorse or promote products derived from this
+    software without specific prior written permission.
 
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER, THE UNITED STATES GOVERNMENT, OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER, THE UNITED STATES GOVERNMENT,
+OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
+EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT
+OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
+IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY
+OF SUCH DAMAGE.
 
-You are under no obligation whatsoever to provide any bug fixes, patches, or upgrades to the features, functionality or performance of the source code ("Enhancements") to anyone; however, if you choose to make your Enhancements available either publicly, or directly to SLAC National Accelerator Laboratory, without imposing a separate written license agreement for such Enhancements, then you hereby grant the following license: a non-exclusive, royalty-free perpetual license to install, use, modify, prepare derivative works, incorporate into other computer software, distribute, and sublicense such Enhancements or derivative works thereof, in binary and source code form.
+You are under no obligation whatsoever to provide any bug fixes, patches, or
+upgrades to the features, functionality or performance of the source code
+("Enhancements") to anyone; however, if you choose to make your Enhancements
+available either publicly, or directly to SLAC National Accelerator Laboratory,
+without imposing a separate written license agreement for such Enhancements,
+then you hereby grant the following license: a non-exclusive, royalty-free
+perpetual license to install, use, modify, prepare derivative works, incorporate
+into other computer software, distribute, and sublicense such Enhancements or
+derivative works thereof, in binary and source code form.
```

### Comparing `timechart-1.5.1/README.md` & `timechart-1.5.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-<img src="timechart_launcher/icons/charts_128.png" width="128" height="128" align="right"/>
-  <h1>TimeChart</h1>
-  <h3>A Charting Tool based on PyDM</h3>
-</p>
+# TimeChart
+## A Charting Tool based on PyDM
+![TimeChart logo](https://raw.githubusercontent.com/slaclab/timechart/master/timechart_launcher/icons/charts_128.png)
 
 TimeChart is a Python Qt-based graphing application for control systems.
 It is intended to be the modern, feature-by-feature matching alternative
 to the Motif [EPICS Strip Tool](https://epics.anl.gov/extensions/StripTool/ "EPICS Strip Tool") application.
 
 Comparing with Strip Tool, TimeChart possesses the inherent cross-platform,
 responsive, and regularly maintained and supported advantages offered by
 [Python Display Manager (PyDM)](https://github.com/slaclab/pydm "PyDM").
 As a Python Qt-based framework, PyDM is also created and maintained by SLAC.
 Its charting capability is built upon [pyqtgraph](http://pyqtgraph.org/ "PyQtGraph"),
 and the PyDM's TimePlot is the central widget in TimeChart.
 
 # Installing and Running TimeChart
 
-Refer to [TimeChart Documentation] (https://slaclab.github.io/timechart/ "TimeChart Documentation") for detailed
+Refer to [TimeChart Documentation](https://slaclab.github.io/timechart/ "TimeChart Documentation") for detailed
 instructions on how to install and run TimeChart.
 
 # Acknowledgements
 
 Icons made by [monkik](https://www.flaticon.com/authors/monkik) from [www.flaticon.com](https://www.flaticon.com/) is
 licensed by [CC 3.0 BY](http://creativecommons.org/licenses/by/3.0/).
```

### Comparing `timechart-1.5.1/timechart/data_io/importers/striptool_config_importer.py` & `timechart-1.5.3/timechart/data_io/importers/striptool_config_importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 
         Returns
         -------
             The equivalent TimeChart settings.
 
         """
         timechart_settings = OrderedDict()
-        timechart_settings["__version__"] = ver
+        timechart_settings["__version__"] = str(ver)
 
         timechart_settings["pvs"] = OrderedDict()
 
         timechart_settings["chart_settings"] = OrderedDict()
         timechart_settings["chart_settings"]["title"] = DEFAULT_CHART_TITLE
         timechart_settings["chart_settings"]["x_axis_label"] = None
         timechart_settings["chart_settings"]["x_axis_unit"] = None
```

### Comparing `timechart-1.5.1/timechart/data_io/importers/timechart_config_importer.py` & `timechart-1.5.3/timechart/data_io/importers/timechart_config_importer.py`

 * *Files identical despite different names*

### Comparing `timechart-1.5.1/timechart/data_io/settings_exporter.py` & `timechart-1.5.3/timechart/data_io/settings_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
         Parameters
         ----------
         filename : str
             The filename to export the configuration data to.
         """
         settings = OrderedDict()
-        settings["__version__"] = ver
+        settings["__version__"] = str(ver)
         settings["pvs"] = OrderedDict()
         settings["chart_settings"] = OrderedDict()
         chart = self.main_display.chart
 
         if self.include_pvs:
             pv_list = list()
             for k, v in self.main_display.channel_map.items():
```

### Comparing `timechart-1.5.1/timechart/data_io/settings_importer.py` & `timechart-1.5.3/timechart/data_io/settings_importer.py`

 * *Files identical despite different names*

### Comparing `timechart-1.5.1/timechart/displays/axis_settings_display.py` & `timechart-1.5.3/timechart/displays/axis_settings_display.py`

 * *Files identical despite different names*

### Comparing `timechart-1.5.1/timechart/displays/chart_data_export_display.py` & `timechart-1.5.3/timechart/displays/chart_data_export_display.py`

 * *Files identical despite different names*

### Comparing `timechart-1.5.1/timechart/displays/curve_settings_display.py` & `timechart-1.5.3/timechart/displays/curve_settings_display.py`

 * *Files identical despite different names*

### Comparing `timechart-1.5.1/timechart/displays/defaults.py` & `timechart-1.5.3/timechart/displays/defaults.py`

 * *Files identical despite different names*

### Comparing `timechart-1.5.1/timechart/displays/main_display.py` & `timechart-1.5.3/timechart/displays/main_display.py`

 * *Files identical despite different names*

### Comparing `timechart-1.5.1/timechart/tool.py` & `timechart-1.5.3/timechart/tool.py`

 * *Files identical despite different names*

### Comparing `timechart-1.5.1/timechart/utilities/utils.py` & `timechart-1.5.3/timechart/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `timechart-1.5.1/timechart_launcher/icons/charts_128.png` & `timechart-1.5.3/timechart_launcher/icons/charts_128.png`

 * *Files identical despite different names*

### Comparing `timechart-1.5.1/timechart_launcher/icons/charts_16.png` & `timechart-1.5.3/timechart_launcher/icons/charts_16.png`

 * *Files identical despite different names*

### Comparing `timechart-1.5.1/timechart_launcher/icons/charts_24.png` & `timechart-1.5.3/timechart_launcher/icons/charts_24.png`

 * *Files identical despite different names*

### Comparing `timechart-1.5.1/timechart_launcher/icons/charts_256.png` & `timechart-1.5.3/timechart_launcher/icons/charts_256.png`

 * *Files identical despite different names*

### Comparing `timechart-1.5.1/timechart_launcher/icons/charts_32.png` & `timechart-1.5.3/timechart_launcher/icons/charts_32.png`

 * *Files identical despite different names*

### Comparing `timechart-1.5.1/timechart_launcher/icons/charts_64.png` & `timechart-1.5.3/timechart_launcher/icons/charts_64.png`

 * *Files identical despite different names*

### Comparing `timechart-1.5.1/timechart_launcher/main.py` & `timechart-1.5.3/timechart_launcher/main.py`

 * *Files identical despite different names*

