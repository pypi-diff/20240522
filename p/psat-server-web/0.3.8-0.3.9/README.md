# Comparing `tmp/psat-server-web-0.3.8.tar.gz` & `tmp/psat-server-web-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/psat-server-web-0.3.8.tar", last modified: Thu Mar  7 17:17:07 2024, max compression
+gzip compressed data, was "dist/psat-server-web-0.3.9.tar", last modified: Wed Apr 10 23:53:56 2024, max compression
```

## Comparing `psat-server-web-0.3.8.tar` & `psat-server-web-0.3.9.tar`

### file list

```diff
@@ -1,474 +1,476 @@
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.661786 psat-server-web-0.3.8/
--rw-r--r--   0 kws        (502) staff       (20)     1067 2021-03-09 12:47:41.000000 psat-server-web-0.3.8/LICENSE
--rw-r--r--   0 kws        (502) staff       (20)      228 2021-05-20 00:05:16.000000 psat-server-web-0.3.8/MANIFEST.in
--rw-r--r--   0 kws        (502) staff       (20)      839 2024-03-07 17:17:07.661367 psat-server-web-0.3.8/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      349 2021-07-23 12:29:29.000000 psat-server-web-0.3.8/README.md
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.126755 psat-server-web-0.3.8/psat_server_web/
--rw-r--r--   0 kws        (502) staff       (20)     6148 2022-08-23 15:10:48.000000 psat-server-web-0.3.8/psat_server_web/.DS_Store
--rw-r--r--   0 kws        (502) staff       (20)       38 2021-05-15 13:54:02.000000 psat-server-web-0.3.8/psat_server_web/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       22 2024-03-07 17:16:06.000000 psat-server-web-0.3.8/psat_server_web/__version__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.132820 psat-server-web-0.3.8/psat_server_web/atlas/
--rw-r--r--   0 kws        (502) staff       (20)     6148 2022-08-23 15:31:27.000000 psat-server-web-0.3.8/psat_server_web/atlas/.DS_Store
--rw-r--r--   0 kws        (502) staff       (20)        0 2021-05-15 12:47:24.000000 psat-server-web-0.3.8/psat_server_web/atlas/__init__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.154795 psat-server-web-0.3.8/psat_server_web/atlas/atlas/
--rw-r--r--   0 kws        (502) staff       (20)        0 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlas/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)     6930 2024-02-27 15:34:54.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlas/apiutils.py
--rw-r--r--   0 kws        (502) staff       (20)    47213 2024-03-07 14:45:13.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlas/commonqueries.py
--rw-r--r--   0 kws        (502) staff       (20)    20905 2024-03-07 17:15:40.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlas/dbviews.py
--rw-r--r--   0 kws        (502) staff       (20)      379 2021-03-09 14:56:31.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlas/document.sh
--rw-r--r--   0 kws        (502) staff       (20)     6163 2023-10-06 13:24:07.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlas/formchoices.py
--rw-r--r--   0 kws        (502) staff       (20)    16699 2023-06-22 11:09:10.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlas/helpers.py
--rw-r--r--   0 kws        (502) staff       (20)      381 2023-05-25 09:28:16.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlas/insert_gravity_event.sql
--rw-r--r--   0 kws        (502) staff       (20)    29140 2023-11-30 16:50:35.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlas/lightcurvequeries.py
--rw-r--r--   0 kws        (502) staff       (20)    51998 2024-02-22 10:15:43.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlas/models.py
--rw-r--r--   0 kws        (502) staff       (20)     5345 2024-03-07 10:25:59.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlas/settings.py
--rw-r--r--   0 kws        (502) staff       (20)     5390 2021-03-11 00:41:45.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlas/sqlpaginator.py
--rw-r--r--   0 kws        (502) staff       (20)     5037 2023-10-24 08:51:40.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlas/urls.py
--rw-r--r--   0 kws        (502) staff       (20)   181139 2024-03-05 11:24:55.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlas/views.py
--rw-r--r--   0 kws        (502) staff       (20)     1165 2021-03-10 22:48:56.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlas/wsgi.atlas.conf
--rw-r--r--   0 kws        (502) staff       (20)      329 2021-05-05 21:27:19.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlas/wsgi.py
--rw-r--r--   0 kws        (502) staff       (20)      945 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlas/wsgi_apache_example.conf
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.160563 psat-server-web-0.3.8/psat_server_web/atlas/atlasapi/
--rw-r--r--   0 kws        (502) staff       (20)       92 2023-08-21 13:40:07.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlasapi/apps.py
--rw-r--r--   0 kws        (502) staff       (20)      532 2022-07-14 11:44:45.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlasapi/query_auth.py
--rw-r--r--   0 kws        (502) staff       (20)     8277 2024-02-27 15:41:14.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlasapi/serializers.py
--rw-r--r--   0 kws        (502) staff       (20)      604 2024-02-22 10:19:21.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlasapi/urls.py
--rw-r--r--   0 kws        (502) staff       (20)     4669 2024-02-22 10:28:06.000000 psat-server-web-0.3.8/psat_server_web/atlas/atlasapi/views.py
--rwxr-xr-x   0 kws        (502) staff       (20)     2044 2023-01-02 18:14:38.000000 psat-server-web-0.3.8/psat_server_web/atlas/generate_mod_wsgi_apachectl.sh
--rwxr-xr-x   0 kws        (502) staff       (20)      248 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/manage.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.112607 psat-server-web-0.3.8/psat_server_web/atlas/media/
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.161917 psat-server-web-0.3.8/psat_server_web/atlas/media/images/
--rw-r--r--   0 kws        (502) staff       (20)       81 2021-05-15 10:03:26.000000 psat-server-web-0.3.8/psat_server_web/atlas/media/images/README.txt
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.115240 psat-server-web-0.3.8/psat_server_web/atlas/site_media/
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.169099 psat-server-web-0.3.8/psat_server_web/atlas/site_media/css/
--rw-r--r--   0 kws        (502) staff       (20)    15810 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/css/aladin.css
--rw-r--r--   0 kws        (502) staff       (20)     6501 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/css/celestial.css
--rw-r--r--   0 kws        (502) staff       (20)    73577 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/css/fontawesome.css
--rw-r--r--   0 kws        (502) staff       (20)    13978 2023-09-08 11:36:45.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/css/main.css
--rw-r--r--   0 kws        (502) staff       (20)     3657 2023-09-08 11:37:01.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/css/main_bootstrap.css
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.173196 psat-server-web-0.3.8/psat_server_web/atlas/site_media/images/
--rw-r--r--   0 kws        (502) staff       (20)   163712 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/images/atlas_logo.png
--rw-r--r--   0 kws        (502) staff       (20)    14986 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/images/image_not_available.jpeg
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.194752 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/
--rw-r--r--   0 kws        (502) staff       (20)   455854 2023-11-21 23:43:18.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/aladin.js
--rw-r--r--   0 kws        (502) staff       (20)     1620 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/bootstrap_utils.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.208377 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/
--rw-r--r--   0 kws        (502) staff       (20)   160860 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/celestial.js
--rw-r--r--   0 kws        (502) staff       (20)    90592 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/d3.geo.projection.js
--rw-r--r--   0 kws        (502) staff       (20)    46780 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/d3.geo.projection.min.js
--rw-r--r--   0 kws        (502) staff       (20)     8471 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/d3.geo.zoom.js
--rw-r--r--   0 kws        (502) staff       (20)   151732 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/d3.min.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.230219 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/data/
--rw-r--r--   0 kws        (502) staff       (20)        0 2021-05-14 23:13:00.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/data/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)    39824 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/data/constellations.bounds.json
--rw-r--r--   0 kws        (502) staff       (20)    19510 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/data/constellations.json
--rw-r--r--   0 kws        (502) staff       (20)    26254 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/data/constellations.lines.json
--rw-r--r--   0 kws        (502) staff       (20)     7398 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/data/dsos.bright.json
--rw-r--r--   0 kws        (502) staff       (20)    61574 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/data/lg.json
--rw-r--r--   0 kws        (502) staff       (20)   534254 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/data/mw.json
--rw-r--r--   0 kws        (502) staff       (20)     3884 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/data/planets.json
--rw-r--r--   0 kws        (502) staff       (20)   759360 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/data/stars.6.json
--rw-r--r--   0 kws        (502) staff       (20)     9941 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/colourplot.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.261714 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/
--rw-r--r--   0 kws        (502) staff       (20)    41784 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/excanvas.js
--rw-r--r--   0 kws        (502) staff       (20)   252881 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery-1.7.2.js
--rw-r--r--   0 kws        (502) staff       (20)    17407 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.axislabels.js
--rw-r--r--   0 kws        (502) staff       (20)     5191 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.crosshair.js
--rw-r--r--   0 kws        (502) staff       (20)    12389 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.errorbars.js
--rw-r--r--   0 kws        (502) staff       (20)     6771 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.fillbetween.js
--rw-r--r--   0 kws        (502) staff       (20)     7351 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.image.js
--rw-r--r--   0 kws        (502) staff       (20)   106797 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.js
--rw-r--r--   0 kws        (502) staff       (20)    13634 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.navigate.js
--rw-r--r--   0 kws        (502) staff       (20)    22589 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.pie.js
--rw-r--r--   0 kws        (502) staff       (20)     2458 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.resize.js
--rw-r--r--   0 kws        (502) staff       (20)    12018 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.selection.js
--rw-r--r--   0 kws        (502) staff       (20)     6968 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.stack.js
--rw-r--r--   0 kws        (502) staff       (20)     2441 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.symbol.js
--rw-r--r--   0 kws        (502) staff       (20)     3291 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.threshold.js
--rw-r--r--   0 kws        (502) staff       (20)     3074 2023-09-06 22:55:29.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/followup_selectall.js
--rw-r--r--   0 kws        (502) staff       (20)     5973 2022-09-06 22:01:34.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/heatmap.js
--rw-r--r--   0 kws        (502) staff       (20)    10907 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/lightcurve.js
--rw-r--r--   0 kws        (502) staff       (20)     8349 2021-03-09 13:34:59.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/lightcurveplotly.js
--rw-r--r--   0 kws        (502) staff       (20)     5637 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/mjdcalc.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.263199 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/plotly/
--rw-r--r--   0 kws        (502) staff       (20)  8718595 2022-05-05 10:53:12.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/plotly/plotly-latest.kws.js
--rw-r--r--   0 kws        (502) staff       (20)     7661 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/recurrenceplot.js
--rw-r--r--   0 kws        (502) staff       (20)     7430 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/recurrenceplotplotly.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.328714 psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/
--rw-r--r--   0 kws        (502) staff       (20)   134294 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-brands-400.eot
--rw-r--r--   0 kws        (502) staff       (20)   747927 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-brands-400.svg
--rw-r--r--   0 kws        (502) staff       (20)   133988 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-brands-400.ttf
--rw-r--r--   0 kws        (502) staff       (20)    89988 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-brands-400.woff
--rw-r--r--   0 kws        (502) staff       (20)    76736 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-brands-400.woff2
--rw-r--r--   0 kws        (502) staff       (20)    34034 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-regular-400.eot
--rw-r--r--   0 kws        (502) staff       (20)   144714 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-regular-400.svg
--rw-r--r--   0 kws        (502) staff       (20)    33736 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-regular-400.ttf
--rw-r--r--   0 kws        (502) staff       (20)    16276 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-regular-400.woff
--rw-r--r--   0 kws        (502) staff       (20)    13224 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-regular-400.woff2
--rw-r--r--   0 kws        (502) staff       (20)   203030 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-solid-900.eot
--rw-r--r--   0 kws        (502) staff       (20)   918991 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-solid-900.svg
--rw-r--r--   0 kws        (502) staff       (20)   202744 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-solid-900.ttf
--rw-r--r--   0 kws        (502) staff       (20)   101648 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-solid-900.woff
--rw-r--r--   0 kws        (502) staff       (20)    78268 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.330620 psat-server-web-0.3.8/psat_server_web/atlas/sql/
--rw-r--r--   0 kws        (502) staff       (20)    20150 2023-10-04 14:20:38.000000 psat-server-web-0.3.8/psat_server_web/atlas/sql/create_web_views.sql
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.352678 psat-server-web-0.3.8/psat_server_web/atlas/templates/
--rw-r--r--   0 kws        (502) staff       (20)     8196 2022-08-28 23:54:09.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/.DS_Store
--rw-r--r--   0 kws        (502) staff       (20)      448 2021-05-20 10:54:42.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/400.html
--rw-r--r--   0 kws        (502) staff       (20)      435 2021-05-20 10:37:36.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/403.html
--rw-r--r--   0 kws        (502) staff       (20)      446 2021-05-20 08:49:19.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/404.html
--rw-r--r--   0 kws        (502) staff       (20)      465 2021-05-20 10:56:58.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/500.html
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.411664 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/
--rw-r--r--   0 kws        (502) staff       (20)     4396 2022-08-18 15:21:36.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/atelfasttrackobject.txt
--rw-r--r--   0 kws        (502) staff       (20)     1276 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/atelsdiscovery.txt
--rw-r--r--   0 kws        (502) staff       (20)     5724 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/atelsfast.txt
--rw-r--r--   0 kws        (502) staff       (20)    40656 2023-10-06 12:33:53.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/candidate.html
--rw-r--r--   0 kws        (502) staff       (20)    39775 2023-11-21 23:26:39.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/candidate_plotly.html
--rw-r--r--   0 kws        (502) staff       (20)    36849 2023-06-14 09:36:00.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/candidate_plotly_test.html
--rw-r--r--   0 kws        (502) staff       (20)     3245 2023-10-06 12:35:37.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/crossmatch_external.html
--rw-r--r--   0 kws        (502) staff       (20)      462 2021-03-09 13:34:59.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/error.html
--rw-r--r--   0 kws        (502) staff       (20)     2079 2023-10-06 12:35:54.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/followup.html
--rw-r--r--   0 kws        (502) staff       (20)      761 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/followup.txt
--rw-r--r--   0 kws        (502) staff       (20)     2413 2023-10-06 12:37:05.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/followup2.html
--rw-r--r--   0 kws        (502) staff       (20)      657 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/followup_bs.html
--rw-r--r--   0 kws        (502) staff       (20)     3226 2023-10-06 12:37:25.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/followup_bypass_django_tables.html
--rw-r--r--   0 kws        (502) staff       (20)    13097 2023-10-06 12:52:11.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/followup_quickview.html
--rw-r--r--   0 kws        (502) staff       (20)     1015 2022-03-22 15:05:48.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/followup_quickview_bs.html
--rw-r--r--   0 kws        (502) staff       (20)      570 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/followup_subset.txt
--rw-r--r--   0 kws        (502) staff       (20)      664 2023-06-14 12:23:24.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/gcn.txt
--rw-r--r--   0 kws        (502) staff       (20)      697 2023-06-13 17:06:10.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/gcn_latex.txt
--rw-r--r--   0 kws        (502) staff       (20)     1524 2022-09-06 21:57:51.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/heatmap.html
--rw-r--r--   0 kws        (502) staff       (20)     1251 2022-05-12 22:47:04.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/heatmap_test.html
--rw-r--r--   0 kws        (502) staff       (20)     2764 2023-10-06 12:36:46.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/index.html
--rw-r--r--   0 kws        (502) staff       (20)     1527 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/index_bs.html
--rw-r--r--   0 kws        (502) staff       (20)     7168 2023-02-01 23:50:54.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/index_bs_celestial.html
--rw-r--r--   0 kws        (502) staff       (20)      169 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/iobserve.txt
--rw-r--r--   0 kws        (502) staff       (20)      557 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/lightcurve.txt
--rw-r--r--   0 kws        (502) staff       (20)      751 2021-08-06 00:13:33.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/lightcurveddc.txt
--rw-r--r--   0 kws        (502) staff       (20)      813 2024-02-05 12:21:36.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/lightcurveforced.txt
--rw-r--r--   0 kws        (502) staff       (20)      368 2023-06-21 21:49:03.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/lightcurvestackedforced.txt
--rw-r--r--   0 kws        (502) staff       (20)      445 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/pesstorecurrences.txt
--rw-r--r--   0 kws        (502) staff       (20)      294 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/pesstorecurrencesddc.txt
--rw-r--r--   0 kws        (502) staff       (20)      725 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/pesstosummary.txt
--rw-r--r--   0 kws        (502) staff       (20)     6941 2023-10-06 12:38:26.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/search_results.html
--rw-r--r--   0 kws        (502) staff       (20)    24428 2023-10-06 12:56:33.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/search_results_plotly.html
--rw-r--r--   0 kws        (502) staff       (20)       19 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/sne.json
--rw-r--r--   0 kws        (502) staff       (20)      626 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/summary.csv
--rw-r--r--   0 kws        (502) staff       (20)     2057 2023-10-06 12:35:15.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/userdefinedlists.html
--rw-r--r--   0 kws        (502) staff       (20)      538 2021-05-10 19:49:10.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/userdefinedlists_bs.html
--rw-r--r--   0 kws        (502) staff       (20)      176 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/visibility.txt
--rw-r--r--   0 kws        (502) staff       (20)     1006 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/base.html
--rw-r--r--   0 kws        (502) staff       (20)    10824 2023-10-06 14:18:26.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/base_bootstrap.html
--rw-r--r--   0 kws        (502) staff       (20)     2800 2023-02-23 22:40:49.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/base_bootstrap_login.html
--rw-r--r--   0 kws        (502) staff       (20)     6107 2021-05-14 16:01:35.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/bootstrap4_django_tables2_atlas.html
--rw-r--r--   0 kws        (502) staff       (20)      501 2021-05-19 21:12:44.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/invalid_login.html
--rw-r--r--   0 kws        (502) staff       (20)      355 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/loggedin.html
--rw-r--r--   0 kws        (502) staff       (20)      937 2021-05-19 21:36:39.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/login.html
--rw-r--r--   0 kws        (502) staff       (20)      428 2021-05-19 21:12:06.000000 psat-server-web-0.3.8/psat_server_web/atlas/templates/logout.html
--rw-r--r--   0 kws        (502) staff       (20)      514 2023-03-30 21:22:33.000000 psat-server-web-0.3.8/psat_server_web/atlas/test.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.412785 psat-server-web-0.3.8/psat_server_web/config/
--rw-r--r--   0 kws        (502) staff       (20)      770 2020-10-02 22:40:04.000000 psat-server-web-0.3.8/psat_server_web/config/wsgi.conf.template
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.417700 psat-server-web-0.3.8/psat_server_web/ps1/
--rw-r--r--   0 kws        (502) staff       (20)        0 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)     1890 2021-03-09 14:51:15.000000 psat-server-web-0.3.8/psat_server_web/ps1/createUsers.py
--rwxr-xr-x   0 kws        (502) staff       (20)     2123 2023-01-02 18:15:50.000000 psat-server-web-0.3.8/psat_server_web/ps1/generate_mod_wsgi_apachectl.sh
--rwxr-xr-x   0 kws        (502) staff       (20)      247 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/manage.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.117437 psat-server-web-0.3.8/psat_server_web/ps1/media/
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.419027 psat-server-web-0.3.8/psat_server_web/ps1/media/images/
--rw-r--r--   0 kws        (502) staff       (20)       81 2021-05-15 10:03:26.000000 psat-server-web-0.3.8/psat_server_web/ps1/media/images/README.txt
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.440543 psat-server-web-0.3.8/psat_server_web/ps1/psdb/
--rw-r--r--   0 kws        (502) staff       (20)        0 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/psdb/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)      697 2021-03-09 14:54:01.000000 psat-server-web-0.3.8/psat_server_web/ps1/psdb/admin.py.old
--rw-r--r--   0 kws        (502) staff       (20)     7589 2023-04-17 17:11:11.000000 psat-server-web-0.3.8/psat_server_web/ps1/psdb/catalogueviews.py
--rw-r--r--   0 kws        (502) staff       (20)    42656 2021-12-28 20:23:00.000000 psat-server-web-0.3.8/psat_server_web/ps1/psdb/commonqueries.py
--rw-r--r--   0 kws        (502) staff       (20)    30114 2021-07-28 15:09:31.000000 psat-server-web-0.3.8/psat_server_web/ps1/psdb/dbviews.py
--rw-r--r--   0 kws        (502) staff       (20)     6908 2022-10-12 11:14:48.000000 psat-server-web-0.3.8/psat_server_web/ps1/psdb/formchoices.py
--rw-r--r--   0 kws        (502) staff       (20)    16504 2023-06-22 14:43:52.000000 psat-server-web-0.3.8/psat_server_web/ps1/psdb/helpers.py
--rw-r--r--   0 kws        (502) staff       (20)    15791 2021-03-09 14:35:48.000000 psat-server-web-0.3.8/psat_server_web/ps1/psdb/img_scale.py
--rw-r--r--   0 kws        (502) staff       (20)    18778 2021-11-22 17:25:49.000000 psat-server-web-0.3.8/psat_server_web/ps1/psdb/lightcurvequeries.py
--rw-r--r--   0 kws        (502) staff       (20)    49437 2023-06-08 15:54:15.000000 psat-server-web-0.3.8/psat_server_web/ps1/psdb/models.py
--rw-r--r--   0 kws        (502) staff       (20)     5357 2024-01-13 00:04:10.000000 psat-server-web-0.3.8/psat_server_web/ps1/psdb/settings.py
--rw-r--r--   0 kws        (502) staff       (20)     4279 2023-06-13 17:18:38.000000 psat-server-web-0.3.8/psat_server_web/ps1/psdb/urls.py
--rw-r--r--   0 kws        (502) staff       (20)   116682 2024-01-13 00:00:30.000000 psat-server-web-0.3.8/psat_server_web/ps1/psdb/views.py
--rw-r--r--   0 kws        (502) staff       (20)      327 2021-07-24 16:19:59.000000 psat-server-web-0.3.8/psat_server_web/ps1/psdb/wsgi.py
--rw-r--r--   0 kws        (502) staff       (20)      893 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/psdb/wsgi_apache_example.conf
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.120533 psat-server-web-0.3.8/psat_server_web/ps1/site_media/
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.444389 psat-server-web-0.3.8/psat_server_web/ps1/site_media/css/
--rw-r--r--   0 kws        (502) staff       (20)    15810 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/css/aladin.css
--rw-r--r--   0 kws        (502) staff       (20)     6501 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/css/celestial.css
--rw-r--r--   0 kws        (502) staff       (20)    73577 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/css/fontawesome.css
--rw-r--r--   0 kws        (502) staff       (20)    13430 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/css/main.css
--rw-r--r--   0 kws        (502) staff       (20)     3479 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/css/main_bootstrap.css
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.499461 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/
--rw-r--r--   0 kws        (502) staff       (20)    35860 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/1-star-hover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    22130 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/1-star.jpg
--rw-r--r--   0 kws        (502) staff       (20)    36051 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/2-star-hover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    27068 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/2-star.jpg
--rw-r--r--   0 kws        (502) staff       (20)    36308 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/3-star-hover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    31801 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/3-star.jpg
--rw-r--r--   0 kws        (502) staff       (20)     2610 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/aladin.gif
--rw-r--r--   0 kws        (502) staff       (20)    58676 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/cfaIcon.jpg
--rw-r--r--   0 kws        (502) staff       (20)    61573 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/cfaIconHover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    21821 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/confirmed-sne-hover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    23630 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/confirmed-sne.jpg
--rw-r--r--   0 kws        (502) staff       (20)    57933 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/detection_example.jpg
--rwxr-xr-x   0 kws        (502) staff       (20)      465 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/down.jpeg
--rw-r--r--   0 kws        (502) staff       (20)     6659 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/down.jpg
--rw-r--r--   0 kws        (502) staff       (20)    14986 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/image_not_available.jpeg
--rw-r--r--   0 kws        (502) staff       (20)    36417 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/jhuIcon.jpg
--rw-r--r--   0 kws        (502) staff       (20)    38864 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/jhuIconHover.jpg
--rw-r--r--   0 kws        (502) staff       (20)     7928 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/minus.jpg
--rw-r--r--   0 kws        (502) staff       (20)    44343 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/ncuIcon.jpg
--rw-r--r--   0 kws        (502) staff       (20)    46130 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/ncuIconHover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    58496 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/non_detection_example.jpg
--rw-r--r--   0 kws        (502) staff       (20)     8506 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/others-hover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    11289 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/others.jpg
--rw-r--r--   0 kws        (502) staff       (20)    25306 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs-logo-hover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    21877 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs-logo.jpg
--rw-r--r--   0 kws        (502) staff       (20)    74999 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs1_logo.jpg
--rw-r--r--   0 kws        (502) staff       (20)    85348 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs1_o3_logo.jpg
--rw-r--r--   0 kws        (502) staff       (20)    76781 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs2_logo.jpg
--rw-r--r--   0 kws        (502) staff       (20)    86931 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs2_o3_logo.jpg
--rw-r--r--   0 kws        (502) staff       (20)    95536 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs_logo.jpg
--rw-r--r--   0 kws        (502) staff       (20)    95536 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs_logo_original.jpg
--rw-r--r--   0 kws        (502) staff       (20)    81716 2021-08-04 14:28:23.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs_logo_yse.jpg
--rw-r--r--   0 kws        (502) staff       (20)    83382 2021-08-04 14:35:48.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs_logo_yse_stack.jpg
--rw-r--r--   0 kws        (502) staff       (20)    48452 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/pittsIcon.jpg
--rw-r--r--   0 kws        (502) staff       (20)    50248 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/pittsIconHover.jpg
--rw-r--r--   0 kws        (502) staff       (20)     7740 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/plus.jpg
--rw-r--r--   0 kws        (502) staff       (20)    47509 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/ps1Icon.jpg
--rw-r--r--   0 kws        (502) staff       (20)    45155 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/ps1IconHover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    12609 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/ps1sc.gif
--rw-r--r--   0 kws        (502) staff       (20)    30826 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/qub-logo-hover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    26675 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/qub-logo.jpg
--rw-r--r--   0 kws        (502) staff       (20)    37401 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/qubIcon.jpg
--rw-r--r--   0 kws        (502) staff       (20)    38167 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/qubIconHover.jpg
--rw-r--r--   0 kws        (502) staff       (20)     1493 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/sdss.gif
--rw-r--r--   0 kws        (502) staff       (20)    15197 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/table-background.jpg
--rw-r--r--   0 kws        (502) staff       (20)     1524 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/table-bottom-left.jpg
--rw-r--r--   0 kws        (502) staff       (20)     1551 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/table-bottom-right.jpg
--rw-r--r--   0 kws        (502) staff       (20)     1272 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/table-row.jpg
--rw-r--r--   0 kws        (502) staff       (20)     1442 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/table-top-left.jpg
--rw-r--r--   0 kws        (502) staff       (20)     1549 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/table-top-right.jpg
--rw-r--r--   0 kws        (502) staff       (20)    41765 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/uhifaIcon.jpg
--rw-r--r--   0 kws        (502) staff       (20)    44162 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/uhifaIconHover.jpg
--rw-r--r--   0 kws        (502) staff       (20)      473 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/up.jpeg
--rw-r--r--   0 kws        (502) staff       (20)     6445 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/up.jpg
--rw-r--r--   0 kws        (502) staff       (20)    14173 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/variable-stars-hover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    16952 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/variable-stars.jpg
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.506355 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/
--rw-r--r--   0 kws        (502) staff       (20)   455854 2023-11-21 23:43:18.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/aladin.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.510057 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/
--rw-r--r--   0 kws        (502) staff       (20)   160860 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/celestial.js
--rw-r--r--   0 kws        (502) staff       (20)    90592 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/d3.geo.projection.js
--rw-r--r--   0 kws        (502) staff       (20)    46780 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/d3.geo.projection.min.js
--rw-r--r--   0 kws        (502) staff       (20)     8471 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/d3.geo.zoom.js
--rw-r--r--   0 kws        (502) staff       (20)   151732 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/d3.min.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.515279 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/data/
--rw-r--r--   0 kws        (502) staff       (20)        0 2021-05-14 23:13:00.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/data/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)    39824 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/data/constellations.bounds.json
--rw-r--r--   0 kws        (502) staff       (20)    19510 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/data/constellations.json
--rw-r--r--   0 kws        (502) staff       (20)    26254 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/data/constellations.lines.json
--rw-r--r--   0 kws        (502) staff       (20)     7398 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/data/dsos.bright.json
--rw-r--r--   0 kws        (502) staff       (20)    61574 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/data/lg.json
--rw-r--r--   0 kws        (502) staff       (20)   534254 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/data/mw.json
--rw-r--r--   0 kws        (502) staff       (20)     3884 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/data/planets.json
--rw-r--r--   0 kws        (502) staff       (20)   759360 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/data/stars.6.json
--rw-r--r--   0 kws        (502) staff       (20)     9941 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/colourplot.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.531082 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/
--rw-r--r--   0 kws        (502) staff       (20)    41784 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/excanvas.js
--rw-r--r--   0 kws        (502) staff       (20)   252881 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery-1.7.2.js
--rw-r--r--   0 kws        (502) staff       (20)    17407 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.axislabels.js
--rw-r--r--   0 kws        (502) staff       (20)     5191 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.crosshair.js
--rw-r--r--   0 kws        (502) staff       (20)    12389 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.errorbars.js
--rw-r--r--   0 kws        (502) staff       (20)     6771 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.fillbetween.js
--rw-r--r--   0 kws        (502) staff       (20)     7351 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.image.js
--rw-r--r--   0 kws        (502) staff       (20)   106797 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.js
--rw-r--r--   0 kws        (502) staff       (20)    13634 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.navigate.js
--rw-r--r--   0 kws        (502) staff       (20)    22589 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.pie.js
--rw-r--r--   0 kws        (502) staff       (20)     2458 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.resize.js
--rw-r--r--   0 kws        (502) staff       (20)    12018 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.selection.js
--rw-r--r--   0 kws        (502) staff       (20)     6968 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.stack.js
--rw-r--r--   0 kws        (502) staff       (20)     2441 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.symbol.js
--rw-r--r--   0 kws        (502) staff       (20)     3291 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.threshold.js
--rw-r--r--   0 kws        (502) staff       (20)     1260 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/followup_selectall.js
--rw-r--r--   0 kws        (502) staff       (20)    10724 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/lightcurve.js
--rw-r--r--   0 kws        (502) staff       (20)     8308 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/lightcurveplotly.js
--rw-r--r--   0 kws        (502) staff       (20)     5859 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/mjdcalc.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.531552 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/plotly/
--rw-r--r--   0 kws        (502) staff       (20)  8718595 2022-05-05 10:53:12.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/plotly/plotly-latest.kws.js
--rw-r--r--   0 kws        (502) staff       (20)     7661 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/recurrenceplot.js
--rw-r--r--   0 kws        (502) staff       (20)     7430 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/recurrenceplotplotly.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.557211 psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/
--rw-r--r--   0 kws        (502) staff       (20)   134294 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-brands-400.eot
--rw-r--r--   0 kws        (502) staff       (20)   747927 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-brands-400.svg
--rw-r--r--   0 kws        (502) staff       (20)   133988 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-brands-400.ttf
--rw-r--r--   0 kws        (502) staff       (20)    89988 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-brands-400.woff
--rw-r--r--   0 kws        (502) staff       (20)    76736 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-brands-400.woff2
--rw-r--r--   0 kws        (502) staff       (20)    34034 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-regular-400.eot
--rw-r--r--   0 kws        (502) staff       (20)   144714 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-regular-400.svg
--rw-r--r--   0 kws        (502) staff       (20)    33736 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-regular-400.ttf
--rw-r--r--   0 kws        (502) staff       (20)    16276 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-regular-400.woff
--rw-r--r--   0 kws        (502) staff       (20)    13224 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-regular-400.woff2
--rw-r--r--   0 kws        (502) staff       (20)   203030 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-solid-900.eot
--rw-r--r--   0 kws        (502) staff       (20)   918991 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-solid-900.svg
--rw-r--r--   0 kws        (502) staff       (20)   202744 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-solid-900.ttf
--rw-r--r--   0 kws        (502) staff       (20)   101648 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-solid-900.woff
--rw-r--r--   0 kws        (502) staff       (20)    78268 2021-08-04 16:25:46.000000 psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.560207 psat-server-web-0.3.8/psat_server_web/ps1/sql/
--rw-r--r--   0 kws        (502) staff       (20)      982 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/sql/create_web_cat_views.sql
--rw-r--r--   0 kws        (502) staff       (20)      812 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/sql/create_web_user_grants.sql
--rw-r--r--   0 kws        (502) staff       (20)    17989 2021-07-28 09:31:13.000000 psat-server-web-0.3.8/psat_server_web/ps1/sql/create_web_views.sql
--rw-r--r--   0 kws        (502) staff       (20)    13969 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/sql/create_web_views_fgss.sql
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.569268 psat-server-web-0.3.8/psat_server_web/ps1/templates/
--rw-r--r--   0 kws        (502) staff       (20)      448 2021-05-20 10:54:42.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/400.html
--rw-r--r--   0 kws        (502) staff       (20)      435 2021-05-20 10:37:36.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/403.html
--rw-r--r--   0 kws        (502) staff       (20)      446 2021-05-20 08:49:19.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/404.html
--rw-r--r--   0 kws        (502) staff       (20)      465 2021-05-20 10:56:58.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/500.html
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.570013 psat-server-web-0.3.8/psat_server_web/ps1/templates/admin/
--rw-r--r--   0 kws        (502) staff       (20)      333 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/admin/base_site.html
--rw-r--r--   0 kws        (502) staff       (20)    10344 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/base.html
--rw-r--r--   0 kws        (502) staff       (20)     9714 2021-11-06 14:16:39.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/base_bootstrap.html
--rw-r--r--   0 kws        (502) staff       (20)     2621 2021-11-06 11:26:25.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/base_bootstrap_login.html
--rw-r--r--   0 kws        (502) staff       (20)      956 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/base_new.html
--rw-r--r--   0 kws        (502) staff       (20)     6107 2021-05-14 16:01:35.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/bootstrap4_django_tables2_atlas.html
--rw-r--r--   0 kws        (502) staff       (20)      501 2021-05-19 21:12:44.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/invalid_login.html
--rw-r--r--   0 kws        (502) staff       (20)      359 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/loggedin.html
--rw-r--r--   0 kws        (502) staff       (20)      856 2021-07-31 15:08:21.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/login.html
--rw-r--r--   0 kws        (502) staff       (20)      428 2021-05-19 21:12:06.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/logout.html
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.595193 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/
--rw-r--r--   0 kws        (502) staff       (20)     1173 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/atelsdiscovery.txt
--rw-r--r--   0 kws        (502) staff       (20)    18257 2023-03-03 00:07:15.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/candidate.html
--rw-r--r--   0 kws        (502) staff       (20)    39797 2023-06-14 09:36:20.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/candidate_plotly.html
--rw-r--r--   0 kws        (502) staff       (20)    32802 2023-03-03 00:05:29.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/candidate_quickview.html
--rw-r--r--   0 kws        (502) staff       (20)    40828 2023-06-14 09:36:42.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/candidateflot.html
--rw-r--r--   0 kws        (502) staff       (20)     2215 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/candidates.html
--rw-r--r--   0 kws        (502) staff       (20)      756 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/colourdata.txt
--rw-r--r--   0 kws        (502) staff       (20)     3628 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/crossmatch_cfa_with_ipp.html
--rw-r--r--   0 kws        (502) staff       (20)     3328 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/crossmatch_external.html
--rw-r--r--   0 kws        (502) staff       (20)       17 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/dss2.html
--rw-r--r--   0 kws        (502) staff       (20)      462 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/error.html
--rw-r--r--   0 kws        (502) staff       (20)     3229 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/fasttrackastronote.txt
--rw-r--r--   0 kws        (502) staff       (20)     2095 2021-10-26 11:36:56.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/filter.html
--rw-r--r--   0 kws        (502) staff       (20)     3731 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/followup.html
--rw-r--r--   0 kws        (502) staff       (20)      864 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/followup.txt
--rw-r--r--   0 kws        (502) staff       (20)      657 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/followup_bs.html
--rw-r--r--   0 kws        (502) staff       (20)     2873 2021-03-09 13:30:11.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/followup_bs_old.html
--rw-r--r--   0 kws        (502) staff       (20)    12747 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/followup_quickview.html
--rw-r--r--   0 kws        (502) staff       (20)     1012 2021-05-14 12:15:07.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/followup_quickview_bs.html
--rw-r--r--   0 kws        (502) staff       (20)     9846 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/followup_quickview_bs_old.html
--rw-r--r--   0 kws        (502) staff       (20)      660 2023-06-14 12:25:27.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/gcn.txt
--rw-r--r--   0 kws        (502) staff       (20)      693 2023-06-13 17:19:55.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/gcn_latex.txt
--rw-r--r--   0 kws        (502) staff       (20)     4902 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/index.html
--rw-r--r--   0 kws        (502) staff       (20)    10229 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/index_bs_celestial.html
--rw-r--r--   0 kws        (502) staff       (20)    15063 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/index_public.html
--rw-r--r--   0 kws        (502) staff       (20)      277 2021-12-28 20:25:35.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/lightcurve.txt
--rw-r--r--   0 kws        (502) staff       (20)      419 2021-12-28 20:18:08.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/lightcurveforced.txt
--rw-r--r--   0 kws        (502) staff       (20)     5801 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/lightcurves.html
--rw-r--r--   0 kws        (502) staff       (20)      294 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/obscat.txt
--rw-r--r--   0 kws        (502) staff       (20)     1344 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/obsmediawiki.txt
--rw-r--r--   0 kws        (502) staff       (20)     3803 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/public.html
--rw-r--r--   0 kws        (502) staff       (20)      859 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/public_textonly.txt
--rw-r--r--   0 kws        (502) staff       (20)     9225 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/reports.html
--rw-r--r--   0 kws        (502) staff       (20)     3801 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/search_results.html
--rw-r--r--   0 kws        (502) staff       (20)    23233 2023-06-08 15:49:42.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/search_results_plotly.html
--rw-r--r--   0 kws        (502) staff       (20)       19 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/sne.json
--rw-r--r--   0 kws        (502) staff       (20)     2537 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/userdefinedlists.html
--rw-r--r--   0 kws        (502) staff       (20)      538 2021-05-10 19:49:10.000000 psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/userdefinedlists_bs.html
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.660029 psat-server-web-0.3.8/psat_server_web/schema/
--rw-r--r--   0 kws        (502) staff       (20)     2421 2023-04-17 10:11:00.000000 psat-server-web-0.3.8/psat_server_web/schema/atlas_detections.sql
--rw-r--r--   0 kws        (502) staff       (20)     1889 2023-04-17 09:49:01.000000 psat-server-web-0.3.8/psat_server_web/schema/atlas_detectionsddc.sql
--rw-r--r--   0 kws        (502) staff       (20)     2370 2023-04-17 09:47:53.000000 psat-server-web-0.3.8/psat_server_web/schema/atlas_diff_detections.sql
--rw-r--r--   0 kws        (502) staff       (20)      810 2023-04-17 09:53:48.000000 psat-server-web-0.3.8/psat_server_web/schema/atlas_diff_logs.sql
--rw-r--r--   0 kws        (502) staff       (20)     1251 2023-04-17 09:48:11.000000 psat-server-web-0.3.8/psat_server_web/schema/atlas_diff_moments.sql
--rw-r--r--   0 kws        (502) staff       (20)     3477 2023-04-17 09:47:20.000000 psat-server-web-0.3.8/psat_server_web/schema/atlas_diff_objects.sql
--rw-r--r--   0 kws        (502) staff       (20)      803 2023-04-17 09:52:38.000000 psat-server-web-0.3.8/psat_server_web/schema/atlas_diff_subcell_logs.sql
--rw-r--r--   0 kws        (502) staff       (20)      698 2023-04-17 09:52:25.000000 psat-server-web-0.3.8/psat_server_web/schema/atlas_diff_subcells.sql
--rw-r--r--   0 kws        (502) staff       (20)     1804 2023-04-17 09:52:04.000000 psat-server-web-0.3.8/psat_server_web/schema/atlas_forced_photometry.sql
--rw-r--r--   0 kws        (502) staff       (20)      553 2023-04-17 09:54:02.000000 psat-server-web-0.3.8/psat_server_web/schema/atlas_heatmaps.sql
--rw-r--r--   0 kws        (502) staff       (20)     3086 2023-04-17 09:48:44.000000 psat-server-web-0.3.8/psat_server_web/schema/atlas_metadata.sql
--rw-r--r--   0 kws        (502) staff       (20)     1558 2023-04-17 10:11:30.000000 psat-server-web-0.3.8/psat_server_web/schema/atlas_metadataddc.sql
--rw-r--r--   0 kws        (502) staff       (20)     1982 2023-04-17 10:12:20.000000 psat-server-web-0.3.8/psat_server_web/schema/atlas_objects.sql
--rw-r--r--   0 kws        (502) staff       (20)     1753 2023-04-17 09:53:07.000000 psat-server-web-0.3.8/psat_server_web/schema/atlas_stacked_forced_photometry.sql
--rw-r--r--   0 kws        (502) staff       (20)     2210 2022-10-07 11:16:51.000000 psat-server-web-0.3.8/psat_server_web/schema/convert_backend_storage_to_innodb.sql
--rw-r--r--   0 kws        (502) staff       (20)      970 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/create_atlas_flattened_view.sql
--rw-r--r--   0 kws        (502) staff       (20)     4055 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/create_photpipe_views.sql
--rw-r--r--   0 kws        (502) staff       (20)     2946 2024-02-22 10:16:30.000000 psat-server-web-0.3.8/psat_server_web/schema/create_schema.sql
--rw-r--r--   0 kws        (502) staff       (20)     3312 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/create_user_grants.sql
--rw-r--r--   0 kws        (502) staff       (20)     1332 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/create_user_grants_generic.sql
--rw-r--r--   0 kws        (502) staff       (20)      232 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/create_user_grants_root.sql
--rw-r--r--   0 kws        (502) staff       (20)     1190 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/delete_transients.sql
--rw-r--r--   0 kws        (502) staff       (20)    60402 2021-03-10 12:07:36.000000 psat-server-web-0.3.8/psat_server_web/schema/generateATLASSchemaAndCPPClasses.py
--rw-r--r--   0 kws        (502) staff       (20)     2489 2021-03-10 12:03:01.000000 psat-server-web-0.3.8/psat_server_web/schema/get_table_columns_for_avro.py
--rw-r--r--   0 kws        (502) staff       (20)      182 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/get_table_columns_for_avro.sql
--rw-r--r--   0 kws        (502) staff       (20)      117 2023-04-18 09:51:15.000000 psat-server-web-0.3.8/psat_server_web/schema/mjdnow.sql
--rw-r--r--   0 kws        (502) staff       (20)      977 2021-03-10 12:32:10.000000 psat-server-web-0.3.8/psat_server_web/schema/refresh_django_views.py
--rw-r--r--   0 kws        (502) staff       (20)     4853 2021-03-10 22:44:14.000000 psat-server-web-0.3.8/psat_server_web/schema/setup_database.py
--rw-r--r--   0 kws        (502) staff       (20)    13195 2021-03-10 22:48:16.000000 psat-server-web-0.3.8/psat_server_web/schema/setup_database_utils.py
--rw-r--r--   0 kws        (502) staff       (20)      714 2021-03-09 13:30:11.000000 psat-server-web-0.3.8/psat_server_web/schema/sherlock_classifications.sql
--rw-r--r--   0 kws        (502) staff       (20)     3104 2021-03-09 13:30:11.000000 psat-server-web-0.3.8/psat_server_web/schema/sherlock_crossmatches.sql
--rw-r--r--   0 kws        (502) staff       (20)     2038 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_cat_gaia_dr1.sql
--rw-r--r--   0 kws        (502) staff       (20)     2927 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_cat_gaia_dr2.sql
--rw-r--r--   0 kws        (502) staff       (20)     2421 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_cat_gaia_dr2_cassandra.cql
--rw-r--r--   0 kws        (502) staff       (20)     1378 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_cat_kepler_k2.sql
--rw-r--r--   0 kws        (502) staff       (20)      699 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_cat_kepler_k2_pixels.sql
--rw-r--r--   0 kws        (502) staff       (20)     6105 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_cat_ps1_medium_deep_ref.sql
--rw-r--r--   0 kws        (502) staff       (20)      713 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_cat_ps1_ubercal_stars.sql
--rw-r--r--   0 kws        (502) staff       (20)      570 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_cat_satellites.sql
--rw-r--r--   0 kws        (502) staff       (20)     4756 2023-04-17 09:11:12.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_catalogue_tables.sql
--rw-r--r--   0 kws        (502) staff       (20)     1659 2023-04-17 09:43:29.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_cfa_detections.sql
--rw-r--r--   0 kws        (502) staff       (20)      576 2023-04-17 09:44:10.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_cfa_to_ipp_lookup.sql
--rw-r--r--   0 kws        (502) staff       (20)     1074 2023-04-17 09:11:49.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_classification_flags.sql
--rw-r--r--   0 kws        (502) staff       (20)      547 2023-04-17 09:12:36.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_classification_history.sql
--rw-r--r--   0 kws        (502) staff       (20)     5743 2023-04-17 09:09:37.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_cmf_metadata.sql
--rw-r--r--   0 kws        (502) staff       (20)     2015 2023-04-17 09:10:34.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_cross_matches.sql
--rw-r--r--   0 kws        (502) staff       (20)      974 2023-04-17 09:46:54.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_cross_matches_external.sql
--rw-r--r--   0 kws        (502) staff       (20)      776 2023-04-17 09:22:29.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_detection_lists.sql
--rw-r--r--   0 kws        (502) staff       (20)      763 2023-04-17 10:12:43.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_detection_lists_atlas.sql
--rw-r--r--   0 kws        (502) staff       (20)      730 2023-04-17 09:45:16.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_followup_photometry.sql
--rw-r--r--   0 kws        (502) staff       (20)     1078 2023-04-17 09:46:10.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_followup_telescope_instruments.sql
--rw-r--r--   0 kws        (502) staff       (20)      837 2023-04-17 09:46:26.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_followup_telescopes.sql
--rw-r--r--   0 kws        (502) staff       (20)     2096 2023-04-17 09:23:20.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_forced_photometry.sql
--rw-r--r--   0 kws        (502) staff       (20)     1020 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_function_lunation.sql
--rw-r--r--   0 kws        (502) staff       (20)      898 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_function_mjdlunation.sql
--rw-r--r--   0 kws        (502) staff       (20)     1327 2023-06-15 15:50:56.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_gravity_alerts.sql
--rw-r--r--   0 kws        (502) staff       (20)     1426 2023-06-02 14:29:20.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_gravity_event_annotations.sql
--rw-r--r--   0 kws        (502) staff       (20)      609 2023-04-17 09:50:41.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_gravity_events.sql
--rw-r--r--   0 kws        (502) staff       (20)     1501 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_guide_star_cat.sql
--rw-r--r--   0 kws        (502) staff       (20)      875 2023-04-17 09:20:30.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_image_groups.sql
--rw-r--r--   0 kws        (502) staff       (20)      921 2023-04-17 09:12:16.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_images.sql
--rw-r--r--   0 kws        (502) staff       (20)      576 2023-04-17 09:43:46.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_ipp_to_cfa_lookup.sql
--rw-r--r--   0 kws        (502) staff       (20)     2677 2023-04-17 09:24:31.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_latest_object_stats.sql
--rw-r--r--   0 kws        (502) staff       (20)      919 2023-04-17 09:49:53.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_object_comments.sql
--rw-r--r--   0 kws        (502) staff       (20)     2622 2023-04-17 09:25:25.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_object_group_definitions.sql
--rw-r--r--   0 kws        (502) staff       (20)     1904 2023-04-17 10:10:30.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_object_group_definitions_atlas.sql
--rw-r--r--   0 kws        (502) staff       (20)      623 2023-04-17 09:24:56.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_object_groups.sql
--rw-r--r--   0 kws        (502) staff       (20)     2929 2023-04-17 09:19:54.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_parameter_definitions.sql
--rw-r--r--   0 kws        (502) staff       (20)     1347 2023-04-17 10:13:23.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_photpipe_detections.sql
--rw-r--r--   0 kws        (502) staff       (20)     1100 2023-04-17 09:20:57.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_postage_stamp_images.sql
--rw-r--r--   0 kws        (502) staff       (20)      715 2023-04-17 09:21:25.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_postage_stamp_requests.sql
--rw-r--r--   0 kws        (502) staff       (20)     1091 2023-04-17 09:22:07.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_postage_stamp_status_codes.sql
--rw-r--r--   0 kws        (502) staff       (20)     1037 2023-04-17 09:44:43.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_processing_status.sql
--rw-r--r--   0 kws        (502) staff       (20)      830 2023-04-17 09:13:08.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_search_parameters.sql
--rw-r--r--   0 kws        (502) staff       (20)      680 2023-04-17 09:50:14.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_tns_requests.sql
--rw-r--r--   0 kws        (502) staff       (20)     1298 2023-04-17 10:13:40.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_tphot_detections.sql
--rw-r--r--   0 kws        (502) staff       (20)     7956 2023-04-17 09:07:52.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_transient_objects.sql
--rw-r--r--   0 kws        (502) staff       (20)     4644 2023-04-17 09:08:54.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_transient_reobservations.sql
--rw-r--r--   0 kws        (502) staff       (20)      586 2024-02-22 10:16:13.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_vra_scores.sql
--rw-r--r--   0 kws        (502) staff       (20)      829 2023-04-17 09:24:11.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_zoo_requests.sql
--rw-r--r--   0 kws        (502) staff       (20)      703 2023-04-17 09:53:30.000000 psat-server-web-0.3.8/psat_server_web/schema/tcs_zooniverse_scores.sql
--rw-r--r--   0 kws        (502) staff       (20)      537 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/types_gaia_dr2_cassandra.txt
--rw-r--r--   0 kws        (502) staff       (20)     4346 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/update_database_types_to_tns_types_atlas.sql
--rw-r--r--   0 kws        (502) staff       (20)     4521 2021-03-09 13:29:22.000000 psat-server-web-0.3.8/psat_server_web/schema/update_database_types_to_tns_types_panstarrs.sql
--rw-r--r--   0 kws        (502) staff       (20)       96 2023-06-15 16:08:21.000000 psat-server-web-0.3.8/psat_server_web/schema/update_tcs_gravity_alerts_001.sql
--rw-r--r--   0 kws        (502) staff       (20)      808 2023-06-02 14:32:50.000000 psat-server-web-0.3.8/psat_server_web/schema/update_tcs_gravity_event_annotations_001.sql
--rw-r--r--   0 kws        (502) staff       (20)     1497 2021-11-23 00:25:03.000000 psat-server-web-0.3.8/psat_server_web/schema/update_tcs_latest_object_stats_001.sql
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-03-07 17:17:07.129794 psat-server-web-0.3.8/psat_server_web.egg-info/
--rw-r--r--   0 kws        (502) staff       (20)      839 2024-03-07 17:17:04.000000 psat-server-web-0.3.8/psat_server_web.egg-info/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)    22535 2024-03-07 17:17:06.000000 psat-server-web-0.3.8/psat_server_web.egg-info/SOURCES.txt
--rw-r--r--   0 kws        (502) staff       (20)        1 2024-03-07 17:17:04.000000 psat-server-web-0.3.8/psat_server_web.egg-info/dependency_links.txt
--rw-r--r--   0 kws        (502) staff       (20)        1 2023-04-17 21:29:34.000000 psat-server-web-0.3.8/psat_server_web.egg-info/not-zip-safe
--rw-r--r--   0 kws        (502) staff       (20)      138 2024-03-07 17:17:04.000000 psat-server-web-0.3.8/psat_server_web.egg-info/requires.txt
--rw-r--r--   0 kws        (502) staff       (20)       16 2024-03-07 17:17:04.000000 psat-server-web-0.3.8/psat_server_web.egg-info/top_level.txt
--rw-r--r--   0 kws        (502) staff       (20)       38 2024-03-07 17:17:07.662050 psat-server-web-0.3.8/setup.cfg
--rwxr-xr-x   0 kws        (502) staff       (20)     1318 2024-03-06 14:13:15.000000 psat-server-web-0.3.8/setup.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.836369 psat-server-web-0.3.9/
+-rw-r--r--   0 kws        (502) staff       (20)     1067 2021-03-09 12:47:41.000000 psat-server-web-0.3.9/LICENSE
+-rw-r--r--   0 kws        (502) staff       (20)      228 2021-05-20 00:05:16.000000 psat-server-web-0.3.9/MANIFEST.in
+-rw-r--r--   0 kws        (502) staff       (20)      839 2024-04-10 23:53:56.836092 psat-server-web-0.3.9/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      349 2021-07-23 12:29:29.000000 psat-server-web-0.3.9/README.md
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.349052 psat-server-web-0.3.9/psat_server_web/
+-rw-r--r--   0 kws        (502) staff       (20)     6148 2022-08-23 15:10:48.000000 psat-server-web-0.3.9/psat_server_web/.DS_Store
+-rw-r--r--   0 kws        (502) staff       (20)       38 2021-05-15 13:54:02.000000 psat-server-web-0.3.9/psat_server_web/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       22 2024-04-10 23:42:15.000000 psat-server-web-0.3.9/psat_server_web/__version__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.354272 psat-server-web-0.3.9/psat_server_web/atlas/
+-rw-r--r--   0 kws        (502) staff       (20)     6148 2022-08-23 15:31:27.000000 psat-server-web-0.3.9/psat_server_web/atlas/.DS_Store
+-rw-r--r--   0 kws        (502) staff       (20)        0 2021-05-15 12:47:24.000000 psat-server-web-0.3.9/psat_server_web/atlas/__init__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.371863 psat-server-web-0.3.9/psat_server_web/atlas/atlas/
+-rw-r--r--   0 kws        (502) staff       (20)        0 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlas/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)     6930 2024-02-27 15:34:54.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlas/apiutils.py
+-rw-r--r--   0 kws        (502) staff       (20)    47213 2024-03-07 14:45:13.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlas/commonqueries.py
+-rw-r--r--   0 kws        (502) staff       (20)    20905 2024-03-07 17:15:40.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlas/dbviews.py
+-rw-r--r--   0 kws        (502) staff       (20)      379 2021-03-09 14:56:31.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlas/document.sh
+-rw-r--r--   0 kws        (502) staff       (20)     6163 2023-10-06 13:24:07.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlas/formchoices.py
+-rw-r--r--   0 kws        (502) staff       (20)    16701 2024-04-10 23:23:49.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlas/helpers.py
+-rw-r--r--   0 kws        (502) staff       (20)      381 2023-05-25 09:28:16.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlas/insert_gravity_event.sql
+-rw-r--r--   0 kws        (502) staff       (20)    29140 2023-11-30 16:50:35.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlas/lightcurvequeries.py
+-rw-r--r--   0 kws        (502) staff       (20)    51998 2024-02-22 10:15:43.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlas/models.py
+-rw-r--r--   0 kws        (502) staff       (20)     5345 2024-03-07 10:25:59.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlas/settings.py
+-rw-r--r--   0 kws        (502) staff       (20)     5390 2021-03-11 00:41:45.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlas/sqlpaginator.py
+-rw-r--r--   0 kws        (502) staff       (20)     5037 2023-10-24 08:51:40.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlas/urls.py
+-rw-r--r--   0 kws        (502) staff       (20)   181139 2024-03-05 11:24:55.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlas/views.py
+-rw-r--r--   0 kws        (502) staff       (20)     1165 2021-03-10 22:48:56.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlas/wsgi.atlas.conf
+-rw-r--r--   0 kws        (502) staff       (20)      329 2021-05-05 21:27:19.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlas/wsgi.py
+-rw-r--r--   0 kws        (502) staff       (20)      945 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlas/wsgi_apache_example.conf
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.376982 psat-server-web-0.3.9/psat_server_web/atlas/atlasapi/
+-rw-r--r--   0 kws        (502) staff       (20)       92 2023-08-21 13:40:07.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlasapi/apps.py
+-rw-r--r--   0 kws        (502) staff       (20)      532 2022-07-14 11:44:45.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlasapi/query_auth.py
+-rw-r--r--   0 kws        (502) staff       (20)     8277 2024-02-27 15:41:14.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlasapi/serializers.py
+-rw-r--r--   0 kws        (502) staff       (20)      604 2024-02-22 10:19:21.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlasapi/urls.py
+-rw-r--r--   0 kws        (502) staff       (20)     4669 2024-02-22 10:28:06.000000 psat-server-web-0.3.9/psat_server_web/atlas/atlasapi/views.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     2044 2023-01-02 18:14:38.000000 psat-server-web-0.3.9/psat_server_web/atlas/generate_mod_wsgi_apachectl.sh
+-rwxr-xr-x   0 kws        (502) staff       (20)      248 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/manage.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.336433 psat-server-web-0.3.9/psat_server_web/atlas/media/
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.377916 psat-server-web-0.3.9/psat_server_web/atlas/media/images/
+-rw-r--r--   0 kws        (502) staff       (20)       81 2021-05-15 10:03:26.000000 psat-server-web-0.3.9/psat_server_web/atlas/media/images/README.txt
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.338947 psat-server-web-0.3.9/psat_server_web/atlas/site_media/
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.385935 psat-server-web-0.3.9/psat_server_web/atlas/site_media/css/
+-rw-r--r--   0 kws        (502) staff       (20)    15810 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/css/aladin.css
+-rw-r--r--   0 kws        (502) staff       (20)     6501 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/css/celestial.css
+-rw-r--r--   0 kws        (502) staff       (20)    73577 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/css/fontawesome.css
+-rw-r--r--   0 kws        (502) staff       (20)    13978 2023-09-08 11:36:45.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/css/main.css
+-rw-r--r--   0 kws        (502) staff       (20)     3657 2023-09-08 11:37:01.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/css/main_bootstrap.css
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.389165 psat-server-web-0.3.9/psat_server_web/atlas/site_media/images/
+-rw-r--r--   0 kws        (502) staff       (20)   163712 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/images/atlas_logo.png
+-rw-r--r--   0 kws        (502) staff       (20)    14986 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/images/image_not_available.jpeg
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.408861 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/
+-rw-r--r--   0 kws        (502) staff       (20)   455854 2023-11-21 23:43:18.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/aladin.js
+-rw-r--r--   0 kws        (502) staff       (20)     1620 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/bootstrap_utils.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.421110 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/
+-rw-r--r--   0 kws        (502) staff       (20)   160860 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/celestial.js
+-rw-r--r--   0 kws        (502) staff       (20)    90592 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/d3.geo.projection.js
+-rw-r--r--   0 kws        (502) staff       (20)    46780 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/d3.geo.projection.min.js
+-rw-r--r--   0 kws        (502) staff       (20)     8471 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/d3.geo.zoom.js
+-rw-r--r--   0 kws        (502) staff       (20)   151732 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/d3.min.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.441608 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/data/
+-rw-r--r--   0 kws        (502) staff       (20)        0 2021-05-14 23:13:00.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/data/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)    39824 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/data/constellations.bounds.json
+-rw-r--r--   0 kws        (502) staff       (20)    19510 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/data/constellations.json
+-rw-r--r--   0 kws        (502) staff       (20)    26254 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/data/constellations.lines.json
+-rw-r--r--   0 kws        (502) staff       (20)     7398 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/data/dsos.bright.json
+-rw-r--r--   0 kws        (502) staff       (20)    61574 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/data/lg.json
+-rw-r--r--   0 kws        (502) staff       (20)   534254 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/data/mw.json
+-rw-r--r--   0 kws        (502) staff       (20)     3884 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/data/planets.json
+-rw-r--r--   0 kws        (502) staff       (20)   759360 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/data/stars.6.json
+-rw-r--r--   0 kws        (502) staff       (20)     9941 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/colourplot.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.472582 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/
+-rw-r--r--   0 kws        (502) staff       (20)    41784 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/excanvas.js
+-rw-r--r--   0 kws        (502) staff       (20)   252881 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery-1.7.2.js
+-rw-r--r--   0 kws        (502) staff       (20)    17407 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.axislabels.js
+-rw-r--r--   0 kws        (502) staff       (20)     5191 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.crosshair.js
+-rw-r--r--   0 kws        (502) staff       (20)    12389 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.errorbars.js
+-rw-r--r--   0 kws        (502) staff       (20)     6771 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.fillbetween.js
+-rw-r--r--   0 kws        (502) staff       (20)     7351 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.image.js
+-rw-r--r--   0 kws        (502) staff       (20)   106797 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.js
+-rw-r--r--   0 kws        (502) staff       (20)    13634 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.navigate.js
+-rw-r--r--   0 kws        (502) staff       (20)    22589 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.pie.js
+-rw-r--r--   0 kws        (502) staff       (20)     2458 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.resize.js
+-rw-r--r--   0 kws        (502) staff       (20)    12018 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.selection.js
+-rw-r--r--   0 kws        (502) staff       (20)     6968 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.stack.js
+-rw-r--r--   0 kws        (502) staff       (20)     2441 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.symbol.js
+-rw-r--r--   0 kws        (502) staff       (20)     3291 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.threshold.js
+-rw-r--r--   0 kws        (502) staff       (20)     3074 2023-09-06 22:55:29.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/followup_selectall.js
+-rw-r--r--   0 kws        (502) staff       (20)     5973 2022-09-06 22:01:34.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/heatmap.js
+-rw-r--r--   0 kws        (502) staff       (20)    10907 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/lightcurve.js
+-rw-r--r--   0 kws        (502) staff       (20)     8349 2021-03-09 13:34:59.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/lightcurveplotly.js
+-rw-r--r--   0 kws        (502) staff       (20)     5637 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/mjdcalc.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.473815 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/plotly/
+-rw-r--r--   0 kws        (502) staff       (20)  8718595 2022-05-05 10:53:12.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/plotly/plotly-latest.kws.js
+-rw-r--r--   0 kws        (502) staff       (20)     7661 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/recurrenceplot.js
+-rw-r--r--   0 kws        (502) staff       (20)     7430 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/recurrenceplotplotly.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.554376 psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/
+-rw-r--r--   0 kws        (502) staff       (20)   134294 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-brands-400.eot
+-rw-r--r--   0 kws        (502) staff       (20)   747927 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-brands-400.svg
+-rw-r--r--   0 kws        (502) staff       (20)   133988 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 kws        (502) staff       (20)    89988 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-brands-400.woff
+-rw-r--r--   0 kws        (502) staff       (20)    76736 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 kws        (502) staff       (20)    34034 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-regular-400.eot
+-rw-r--r--   0 kws        (502) staff       (20)   144714 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-regular-400.svg
+-rw-r--r--   0 kws        (502) staff       (20)    33736 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 kws        (502) staff       (20)    16276 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-regular-400.woff
+-rw-r--r--   0 kws        (502) staff       (20)    13224 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 kws        (502) staff       (20)   203030 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-solid-900.eot
+-rw-r--r--   0 kws        (502) staff       (20)   918991 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-solid-900.svg
+-rw-r--r--   0 kws        (502) staff       (20)   202744 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 kws        (502) staff       (20)   101648 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-solid-900.woff
+-rw-r--r--   0 kws        (502) staff       (20)    78268 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.555930 psat-server-web-0.3.9/psat_server_web/atlas/sql/
+-rw-r--r--   0 kws        (502) staff       (20)    20150 2023-10-04 14:20:38.000000 psat-server-web-0.3.9/psat_server_web/atlas/sql/create_web_views.sql
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.574988 psat-server-web-0.3.9/psat_server_web/atlas/templates/
+-rw-r--r--   0 kws        (502) staff       (20)     8196 2022-08-28 23:54:09.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/.DS_Store
+-rw-r--r--   0 kws        (502) staff       (20)      448 2021-05-20 10:54:42.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/400.html
+-rw-r--r--   0 kws        (502) staff       (20)      435 2021-05-20 10:37:36.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/403.html
+-rw-r--r--   0 kws        (502) staff       (20)      446 2021-05-20 08:49:19.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/404.html
+-rw-r--r--   0 kws        (502) staff       (20)      465 2021-05-20 10:56:58.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/500.html
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.628252 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/
+-rw-r--r--   0 kws        (502) staff       (20)     4396 2022-08-18 15:21:36.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/atelfasttrackobject.txt
+-rw-r--r--   0 kws        (502) staff       (20)     1276 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/atelsdiscovery.txt
+-rw-r--r--   0 kws        (502) staff       (20)     5724 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/atelsfast.txt
+-rw-r--r--   0 kws        (502) staff       (20)    40656 2023-10-06 12:33:53.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/candidate.html
+-rw-r--r--   0 kws        (502) staff       (20)    39775 2023-11-21 23:26:39.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/candidate_plotly.html
+-rw-r--r--   0 kws        (502) staff       (20)    36849 2023-06-14 09:36:00.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/candidate_plotly_test.html
+-rw-r--r--   0 kws        (502) staff       (20)     3245 2023-10-06 12:35:37.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/crossmatch_external.html
+-rw-r--r--   0 kws        (502) staff       (20)      462 2021-03-09 13:34:59.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/error.html
+-rw-r--r--   0 kws        (502) staff       (20)     2079 2023-10-06 12:35:54.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/followup.html
+-rw-r--r--   0 kws        (502) staff       (20)      761 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/followup.txt
+-rw-r--r--   0 kws        (502) staff       (20)     2413 2023-10-06 12:37:05.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/followup2.html
+-rw-r--r--   0 kws        (502) staff       (20)      657 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/followup_bs.html
+-rw-r--r--   0 kws        (502) staff       (20)     3226 2023-10-06 12:37:25.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/followup_bypass_django_tables.html
+-rw-r--r--   0 kws        (502) staff       (20)    13097 2023-10-06 12:52:11.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/followup_quickview.html
+-rw-r--r--   0 kws        (502) staff       (20)     1015 2022-03-22 15:05:48.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/followup_quickview_bs.html
+-rw-r--r--   0 kws        (502) staff       (20)      570 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/followup_subset.txt
+-rw-r--r--   0 kws        (502) staff       (20)      664 2023-06-14 12:23:24.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/gcn.txt
+-rw-r--r--   0 kws        (502) staff       (20)      697 2023-06-13 17:06:10.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/gcn_latex.txt
+-rw-r--r--   0 kws        (502) staff       (20)     1524 2022-09-06 21:57:51.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/heatmap.html
+-rw-r--r--   0 kws        (502) staff       (20)     1251 2022-05-12 22:47:04.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/heatmap_test.html
+-rw-r--r--   0 kws        (502) staff       (20)     2764 2023-10-06 12:36:46.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/index.html
+-rw-r--r--   0 kws        (502) staff       (20)     1527 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/index_bs.html
+-rw-r--r--   0 kws        (502) staff       (20)     7168 2023-02-01 23:50:54.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/index_bs_celestial.html
+-rw-r--r--   0 kws        (502) staff       (20)      169 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/iobserve.txt
+-rw-r--r--   0 kws        (502) staff       (20)      557 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/lightcurve.txt
+-rw-r--r--   0 kws        (502) staff       (20)      751 2021-08-06 00:13:33.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/lightcurveddc.txt
+-rw-r--r--   0 kws        (502) staff       (20)      813 2024-02-05 12:21:36.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/lightcurveforced.txt
+-rw-r--r--   0 kws        (502) staff       (20)      368 2023-06-21 21:49:03.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/lightcurvestackedforced.txt
+-rw-r--r--   0 kws        (502) staff       (20)      445 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/pesstorecurrences.txt
+-rw-r--r--   0 kws        (502) staff       (20)      294 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/pesstorecurrencesddc.txt
+-rw-r--r--   0 kws        (502) staff       (20)      725 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/pesstosummary.txt
+-rw-r--r--   0 kws        (502) staff       (20)     6941 2023-10-06 12:38:26.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/search_results.html
+-rw-r--r--   0 kws        (502) staff       (20)    24428 2023-10-06 12:56:33.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/search_results_plotly.html
+-rw-r--r--   0 kws        (502) staff       (20)       19 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/sne.json
+-rw-r--r--   0 kws        (502) staff       (20)      626 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/summary.csv
+-rw-r--r--   0 kws        (502) staff       (20)     2057 2023-10-06 12:35:15.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/userdefinedlists.html
+-rw-r--r--   0 kws        (502) staff       (20)      538 2021-05-10 19:49:10.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/userdefinedlists_bs.html
+-rw-r--r--   0 kws        (502) staff       (20)      176 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/visibility.txt
+-rw-r--r--   0 kws        (502) staff       (20)     1006 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/base.html
+-rw-r--r--   0 kws        (502) staff       (20)    10824 2023-10-06 14:18:26.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/base_bootstrap.html
+-rw-r--r--   0 kws        (502) staff       (20)     2800 2023-02-23 22:40:49.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/base_bootstrap_login.html
+-rw-r--r--   0 kws        (502) staff       (20)     6107 2021-05-14 16:01:35.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/bootstrap4_django_tables2_atlas.html
+-rw-r--r--   0 kws        (502) staff       (20)      501 2021-05-19 21:12:44.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/invalid_login.html
+-rw-r--r--   0 kws        (502) staff       (20)      355 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/loggedin.html
+-rw-r--r--   0 kws        (502) staff       (20)      937 2021-05-19 21:36:39.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/login.html
+-rw-r--r--   0 kws        (502) staff       (20)      428 2021-05-19 21:12:06.000000 psat-server-web-0.3.9/psat_server_web/atlas/templates/logout.html
+-rw-r--r--   0 kws        (502) staff       (20)      514 2023-03-30 21:22:33.000000 psat-server-web-0.3.9/psat_server_web/atlas/test.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.629023 psat-server-web-0.3.9/psat_server_web/config/
+-rw-r--r--   0 kws        (502) staff       (20)      770 2020-10-02 22:40:04.000000 psat-server-web-0.3.9/psat_server_web/config/wsgi.conf.template
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.631871 psat-server-web-0.3.9/psat_server_web/ps1/
+-rw-r--r--   0 kws        (502) staff       (20)        0 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)     1890 2021-03-09 14:51:15.000000 psat-server-web-0.3.9/psat_server_web/ps1/createUsers.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     2123 2023-01-02 18:15:50.000000 psat-server-web-0.3.9/psat_server_web/ps1/generate_mod_wsgi_apachectl.sh
+-rwxr-xr-x   0 kws        (502) staff       (20)      247 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/manage.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.340866 psat-server-web-0.3.9/psat_server_web/ps1/media/
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.633026 psat-server-web-0.3.9/psat_server_web/ps1/media/images/
+-rw-r--r--   0 kws        (502) staff       (20)       81 2021-05-15 10:03:26.000000 psat-server-web-0.3.9/psat_server_web/ps1/media/images/README.txt
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.647980 psat-server-web-0.3.9/psat_server_web/ps1/psdb/
+-rw-r--r--   0 kws        (502) staff       (20)        0 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/psdb/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)      697 2021-03-09 14:54:01.000000 psat-server-web-0.3.9/psat_server_web/ps1/psdb/admin.py.old
+-rw-r--r--   0 kws        (502) staff       (20)     7589 2023-04-17 17:11:11.000000 psat-server-web-0.3.9/psat_server_web/ps1/psdb/catalogueviews.py
+-rw-r--r--   0 kws        (502) staff       (20)    42656 2021-12-28 20:23:00.000000 psat-server-web-0.3.9/psat_server_web/ps1/psdb/commonqueries.py
+-rw-r--r--   0 kws        (502) staff       (20)    30114 2021-07-28 15:09:31.000000 psat-server-web-0.3.9/psat_server_web/ps1/psdb/dbviews.py
+-rw-r--r--   0 kws        (502) staff       (20)     6908 2022-10-12 11:14:48.000000 psat-server-web-0.3.9/psat_server_web/ps1/psdb/formchoices.py
+-rw-r--r--   0 kws        (502) staff       (20)    16504 2023-06-22 14:43:52.000000 psat-server-web-0.3.9/psat_server_web/ps1/psdb/helpers.py
+-rw-r--r--   0 kws        (502) staff       (20)    15791 2021-03-09 14:35:48.000000 psat-server-web-0.3.9/psat_server_web/ps1/psdb/img_scale.py
+-rw-r--r--   0 kws        (502) staff       (20)    18778 2021-11-22 17:25:49.000000 psat-server-web-0.3.9/psat_server_web/ps1/psdb/lightcurvequeries.py
+-rw-r--r--   0 kws        (502) staff       (20)    49437 2023-06-08 15:54:15.000000 psat-server-web-0.3.9/psat_server_web/ps1/psdb/models.py
+-rw-r--r--   0 kws        (502) staff       (20)     5357 2024-01-13 00:04:10.000000 psat-server-web-0.3.9/psat_server_web/ps1/psdb/settings.py
+-rw-r--r--   0 kws        (502) staff       (20)     4279 2023-06-13 17:18:38.000000 psat-server-web-0.3.9/psat_server_web/ps1/psdb/urls.py
+-rw-r--r--   0 kws        (502) staff       (20)   116682 2024-01-13 00:00:30.000000 psat-server-web-0.3.9/psat_server_web/ps1/psdb/views.py
+-rw-r--r--   0 kws        (502) staff       (20)      327 2021-07-24 16:19:59.000000 psat-server-web-0.3.9/psat_server_web/ps1/psdb/wsgi.py
+-rw-r--r--   0 kws        (502) staff       (20)      893 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/psdb/wsgi_apache_example.conf
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.343160 psat-server-web-0.3.9/psat_server_web/ps1/site_media/
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.652203 psat-server-web-0.3.9/psat_server_web/ps1/site_media/css/
+-rw-r--r--   0 kws        (502) staff       (20)    15810 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/css/aladin.css
+-rw-r--r--   0 kws        (502) staff       (20)     6501 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/css/celestial.css
+-rw-r--r--   0 kws        (502) staff       (20)    73577 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/css/fontawesome.css
+-rw-r--r--   0 kws        (502) staff       (20)    13430 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/css/main.css
+-rw-r--r--   0 kws        (502) staff       (20)     3479 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/css/main_bootstrap.css
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.698701 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/
+-rw-r--r--   0 kws        (502) staff       (20)    35860 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/1-star-hover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    22130 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/1-star.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    36051 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/2-star-hover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    27068 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/2-star.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    36308 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/3-star-hover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    31801 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/3-star.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     2610 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/aladin.gif
+-rw-r--r--   0 kws        (502) staff       (20)    58676 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/cfaIcon.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    61573 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/cfaIconHover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    21821 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/confirmed-sne-hover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    23630 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/confirmed-sne.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    57933 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/detection_example.jpg
+-rwxr-xr-x   0 kws        (502) staff       (20)      465 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/down.jpeg
+-rw-r--r--   0 kws        (502) staff       (20)     6659 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/down.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    14986 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/image_not_available.jpeg
+-rw-r--r--   0 kws        (502) staff       (20)    36417 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/jhuIcon.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    38864 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/jhuIconHover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     7928 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/minus.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    44343 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/ncuIcon.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    46130 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/ncuIconHover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    58496 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/non_detection_example.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     8506 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/others-hover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    11289 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/others.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    25306 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs-logo-hover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    21877 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs-logo.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    74999 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs1_logo.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    85348 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs1_o3_logo.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    76781 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs2_logo.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    86931 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs2_o3_logo.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    95536 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs_logo.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    95536 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs_logo_original.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    81716 2021-08-04 14:28:23.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs_logo_yse.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    83382 2021-08-04 14:35:48.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs_logo_yse_stack.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    48452 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/pittsIcon.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    50248 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/pittsIconHover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     7740 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/plus.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    47509 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/ps1Icon.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    45155 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/ps1IconHover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    12609 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/ps1sc.gif
+-rw-r--r--   0 kws        (502) staff       (20)    30826 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/qub-logo-hover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    26675 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/qub-logo.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    37401 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/qubIcon.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    38167 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/qubIconHover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     1493 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/sdss.gif
+-rw-r--r--   0 kws        (502) staff       (20)    15197 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/table-background.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     1524 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/table-bottom-left.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     1551 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/table-bottom-right.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     1272 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/table-row.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     1442 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/table-top-left.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     1549 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/table-top-right.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    41765 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/uhifaIcon.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    44162 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/uhifaIconHover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)      473 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/up.jpeg
+-rw-r--r--   0 kws        (502) staff       (20)     6445 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/up.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    14173 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/variable-stars-hover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    16952 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/variable-stars.jpg
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.703887 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/
+-rw-r--r--   0 kws        (502) staff       (20)   455854 2023-11-21 23:43:18.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/aladin.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.706513 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/
+-rw-r--r--   0 kws        (502) staff       (20)   160860 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/celestial.js
+-rw-r--r--   0 kws        (502) staff       (20)    90592 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/d3.geo.projection.js
+-rw-r--r--   0 kws        (502) staff       (20)    46780 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/d3.geo.projection.min.js
+-rw-r--r--   0 kws        (502) staff       (20)     8471 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/d3.geo.zoom.js
+-rw-r--r--   0 kws        (502) staff       (20)   151732 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/d3.min.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.711226 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/data/
+-rw-r--r--   0 kws        (502) staff       (20)        0 2021-05-14 23:13:00.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/data/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)    39824 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/data/constellations.bounds.json
+-rw-r--r--   0 kws        (502) staff       (20)    19510 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/data/constellations.json
+-rw-r--r--   0 kws        (502) staff       (20)    26254 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/data/constellations.lines.json
+-rw-r--r--   0 kws        (502) staff       (20)     7398 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/data/dsos.bright.json
+-rw-r--r--   0 kws        (502) staff       (20)    61574 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/data/lg.json
+-rw-r--r--   0 kws        (502) staff       (20)   534254 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/data/mw.json
+-rw-r--r--   0 kws        (502) staff       (20)     3884 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/data/planets.json
+-rw-r--r--   0 kws        (502) staff       (20)   759360 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/data/stars.6.json
+-rw-r--r--   0 kws        (502) staff       (20)     9941 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/colourplot.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.724174 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/
+-rw-r--r--   0 kws        (502) staff       (20)    41784 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/excanvas.js
+-rw-r--r--   0 kws        (502) staff       (20)   252881 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery-1.7.2.js
+-rw-r--r--   0 kws        (502) staff       (20)    17407 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.axislabels.js
+-rw-r--r--   0 kws        (502) staff       (20)     5191 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.crosshair.js
+-rw-r--r--   0 kws        (502) staff       (20)    12389 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.errorbars.js
+-rw-r--r--   0 kws        (502) staff       (20)     6771 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.fillbetween.js
+-rw-r--r--   0 kws        (502) staff       (20)     7351 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.image.js
+-rw-r--r--   0 kws        (502) staff       (20)   106797 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.js
+-rw-r--r--   0 kws        (502) staff       (20)    13634 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.navigate.js
+-rw-r--r--   0 kws        (502) staff       (20)    22589 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.pie.js
+-rw-r--r--   0 kws        (502) staff       (20)     2458 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.resize.js
+-rw-r--r--   0 kws        (502) staff       (20)    12018 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.selection.js
+-rw-r--r--   0 kws        (502) staff       (20)     6968 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.stack.js
+-rw-r--r--   0 kws        (502) staff       (20)     2441 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.symbol.js
+-rw-r--r--   0 kws        (502) staff       (20)     3291 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.threshold.js
+-rw-r--r--   0 kws        (502) staff       (20)     1260 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/followup_selectall.js
+-rw-r--r--   0 kws        (502) staff       (20)    10724 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/lightcurve.js
+-rw-r--r--   0 kws        (502) staff       (20)     8308 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/lightcurveplotly.js
+-rw-r--r--   0 kws        (502) staff       (20)     5859 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/mjdcalc.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.724604 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/plotly/
+-rw-r--r--   0 kws        (502) staff       (20)  8718595 2022-05-05 10:53:12.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/plotly/plotly-latest.kws.js
+-rw-r--r--   0 kws        (502) staff       (20)     7661 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/recurrenceplot.js
+-rw-r--r--   0 kws        (502) staff       (20)     7430 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/recurrenceplotplotly.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.746983 psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/
+-rw-r--r--   0 kws        (502) staff       (20)   134294 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-brands-400.eot
+-rw-r--r--   0 kws        (502) staff       (20)   747927 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-brands-400.svg
+-rw-r--r--   0 kws        (502) staff       (20)   133988 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 kws        (502) staff       (20)    89988 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-brands-400.woff
+-rw-r--r--   0 kws        (502) staff       (20)    76736 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 kws        (502) staff       (20)    34034 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-regular-400.eot
+-rw-r--r--   0 kws        (502) staff       (20)   144714 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-regular-400.svg
+-rw-r--r--   0 kws        (502) staff       (20)    33736 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 kws        (502) staff       (20)    16276 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-regular-400.woff
+-rw-r--r--   0 kws        (502) staff       (20)    13224 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 kws        (502) staff       (20)   203030 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-solid-900.eot
+-rw-r--r--   0 kws        (502) staff       (20)   918991 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-solid-900.svg
+-rw-r--r--   0 kws        (502) staff       (20)   202744 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 kws        (502) staff       (20)   101648 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-solid-900.woff
+-rw-r--r--   0 kws        (502) staff       (20)    78268 2021-08-04 16:25:46.000000 psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.749581 psat-server-web-0.3.9/psat_server_web/ps1/sql/
+-rw-r--r--   0 kws        (502) staff       (20)      982 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/sql/create_web_cat_views.sql
+-rw-r--r--   0 kws        (502) staff       (20)      812 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/sql/create_web_user_grants.sql
+-rw-r--r--   0 kws        (502) staff       (20)    17989 2021-07-28 09:31:13.000000 psat-server-web-0.3.9/psat_server_web/ps1/sql/create_web_views.sql
+-rw-r--r--   0 kws        (502) staff       (20)    13969 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/sql/create_web_views_fgss.sql
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.758310 psat-server-web-0.3.9/psat_server_web/ps1/templates/
+-rw-r--r--   0 kws        (502) staff       (20)      448 2021-05-20 10:54:42.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/400.html
+-rw-r--r--   0 kws        (502) staff       (20)      435 2021-05-20 10:37:36.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/403.html
+-rw-r--r--   0 kws        (502) staff       (20)      446 2021-05-20 08:49:19.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/404.html
+-rw-r--r--   0 kws        (502) staff       (20)      465 2021-05-20 10:56:58.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/500.html
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.758943 psat-server-web-0.3.9/psat_server_web/ps1/templates/admin/
+-rw-r--r--   0 kws        (502) staff       (20)      333 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/admin/base_site.html
+-rw-r--r--   0 kws        (502) staff       (20)    10344 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/base.html
+-rw-r--r--   0 kws        (502) staff       (20)     9714 2021-11-06 14:16:39.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/base_bootstrap.html
+-rw-r--r--   0 kws        (502) staff       (20)     2621 2021-11-06 11:26:25.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/base_bootstrap_login.html
+-rw-r--r--   0 kws        (502) staff       (20)      956 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/base_new.html
+-rw-r--r--   0 kws        (502) staff       (20)     6107 2021-05-14 16:01:35.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/bootstrap4_django_tables2_atlas.html
+-rw-r--r--   0 kws        (502) staff       (20)      501 2021-05-19 21:12:44.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/invalid_login.html
+-rw-r--r--   0 kws        (502) staff       (20)      359 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/loggedin.html
+-rw-r--r--   0 kws        (502) staff       (20)      856 2021-07-31 15:08:21.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/login.html
+-rw-r--r--   0 kws        (502) staff       (20)      428 2021-05-19 21:12:06.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/logout.html
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.782553 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/
+-rw-r--r--   0 kws        (502) staff       (20)     1173 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/atelsdiscovery.txt
+-rw-r--r--   0 kws        (502) staff       (20)    18257 2023-03-03 00:07:15.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/candidate.html
+-rw-r--r--   0 kws        (502) staff       (20)    39797 2023-06-14 09:36:20.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/candidate_plotly.html
+-rw-r--r--   0 kws        (502) staff       (20)    32802 2023-03-03 00:05:29.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/candidate_quickview.html
+-rw-r--r--   0 kws        (502) staff       (20)    40828 2023-06-14 09:36:42.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/candidateflot.html
+-rw-r--r--   0 kws        (502) staff       (20)     2215 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/candidates.html
+-rw-r--r--   0 kws        (502) staff       (20)      756 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/colourdata.txt
+-rw-r--r--   0 kws        (502) staff       (20)     3628 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/crossmatch_cfa_with_ipp.html
+-rw-r--r--   0 kws        (502) staff       (20)     3328 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/crossmatch_external.html
+-rw-r--r--   0 kws        (502) staff       (20)       17 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/dss2.html
+-rw-r--r--   0 kws        (502) staff       (20)      462 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/error.html
+-rw-r--r--   0 kws        (502) staff       (20)     3229 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/fasttrackastronote.txt
+-rw-r--r--   0 kws        (502) staff       (20)     2095 2021-10-26 11:36:56.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/filter.html
+-rw-r--r--   0 kws        (502) staff       (20)     3731 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/followup.html
+-rw-r--r--   0 kws        (502) staff       (20)      864 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/followup.txt
+-rw-r--r--   0 kws        (502) staff       (20)      657 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/followup_bs.html
+-rw-r--r--   0 kws        (502) staff       (20)     2873 2021-03-09 13:30:11.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/followup_bs_old.html
+-rw-r--r--   0 kws        (502) staff       (20)    12747 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/followup_quickview.html
+-rw-r--r--   0 kws        (502) staff       (20)     1012 2021-05-14 12:15:07.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/followup_quickview_bs.html
+-rw-r--r--   0 kws        (502) staff       (20)     9846 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/followup_quickview_bs_old.html
+-rw-r--r--   0 kws        (502) staff       (20)      660 2023-06-14 12:25:27.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/gcn.txt
+-rw-r--r--   0 kws        (502) staff       (20)      693 2023-06-13 17:19:55.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/gcn_latex.txt
+-rw-r--r--   0 kws        (502) staff       (20)     4902 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/index.html
+-rw-r--r--   0 kws        (502) staff       (20)    10229 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/index_bs_celestial.html
+-rw-r--r--   0 kws        (502) staff       (20)    15063 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/index_public.html
+-rw-r--r--   0 kws        (502) staff       (20)      277 2021-12-28 20:25:35.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/lightcurve.txt
+-rw-r--r--   0 kws        (502) staff       (20)      419 2021-12-28 20:18:08.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/lightcurveforced.txt
+-rw-r--r--   0 kws        (502) staff       (20)     5801 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/lightcurves.html
+-rw-r--r--   0 kws        (502) staff       (20)      294 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/obscat.txt
+-rw-r--r--   0 kws        (502) staff       (20)     1344 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/obsmediawiki.txt
+-rw-r--r--   0 kws        (502) staff       (20)     3803 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/public.html
+-rw-r--r--   0 kws        (502) staff       (20)      859 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/public_textonly.txt
+-rw-r--r--   0 kws        (502) staff       (20)     9225 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/reports.html
+-rw-r--r--   0 kws        (502) staff       (20)     3801 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/search_results.html
+-rw-r--r--   0 kws        (502) staff       (20)    23233 2023-06-08 15:49:42.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/search_results_plotly.html
+-rw-r--r--   0 kws        (502) staff       (20)       19 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/sne.json
+-rw-r--r--   0 kws        (502) staff       (20)     2537 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/userdefinedlists.html
+-rw-r--r--   0 kws        (502) staff       (20)      538 2021-05-10 19:49:10.000000 psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/userdefinedlists_bs.html
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.835381 psat-server-web-0.3.9/psat_server_web/schema/
+-rw-r--r--   0 kws        (502) staff       (20)     2421 2023-04-17 10:11:00.000000 psat-server-web-0.3.9/psat_server_web/schema/atlas_detections.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1889 2023-04-17 09:49:01.000000 psat-server-web-0.3.9/psat_server_web/schema/atlas_detectionsddc.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2370 2023-04-17 09:47:53.000000 psat-server-web-0.3.9/psat_server_web/schema/atlas_diff_detections.sql
+-rw-r--r--   0 kws        (502) staff       (20)      810 2023-04-17 09:53:48.000000 psat-server-web-0.3.9/psat_server_web/schema/atlas_diff_logs.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1251 2023-04-17 09:48:11.000000 psat-server-web-0.3.9/psat_server_web/schema/atlas_diff_moments.sql
+-rw-r--r--   0 kws        (502) staff       (20)     3477 2023-04-17 09:47:20.000000 psat-server-web-0.3.9/psat_server_web/schema/atlas_diff_objects.sql
+-rw-r--r--   0 kws        (502) staff       (20)      803 2023-04-17 09:52:38.000000 psat-server-web-0.3.9/psat_server_web/schema/atlas_diff_subcell_logs.sql
+-rw-r--r--   0 kws        (502) staff       (20)      698 2023-04-17 09:52:25.000000 psat-server-web-0.3.9/psat_server_web/schema/atlas_diff_subcells.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1804 2023-04-17 09:52:04.000000 psat-server-web-0.3.9/psat_server_web/schema/atlas_forced_photometry.sql
+-rw-r--r--   0 kws        (502) staff       (20)      553 2023-04-17 09:54:02.000000 psat-server-web-0.3.9/psat_server_web/schema/atlas_heatmaps.sql
+-rw-r--r--   0 kws        (502) staff       (20)     3086 2023-04-17 09:48:44.000000 psat-server-web-0.3.9/psat_server_web/schema/atlas_metadata.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1558 2023-04-17 10:11:30.000000 psat-server-web-0.3.9/psat_server_web/schema/atlas_metadataddc.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1982 2023-04-17 10:12:20.000000 psat-server-web-0.3.9/psat_server_web/schema/atlas_objects.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1753 2023-04-17 09:53:07.000000 psat-server-web-0.3.9/psat_server_web/schema/atlas_stacked_forced_photometry.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2210 2022-10-07 11:16:51.000000 psat-server-web-0.3.9/psat_server_web/schema/convert_backend_storage_to_innodb.sql
+-rw-r--r--   0 kws        (502) staff       (20)      970 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/create_atlas_flattened_view.sql
+-rw-r--r--   0 kws        (502) staff       (20)     4055 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/create_photpipe_views.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2946 2024-02-22 10:16:30.000000 psat-server-web-0.3.9/psat_server_web/schema/create_schema.sql
+-rw-r--r--   0 kws        (502) staff       (20)     3312 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/create_user_grants.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1332 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/create_user_grants_generic.sql
+-rw-r--r--   0 kws        (502) staff       (20)      232 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/create_user_grants_root.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1190 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/delete_transients.sql
+-rw-r--r--   0 kws        (502) staff       (20)    60402 2021-03-10 12:07:36.000000 psat-server-web-0.3.9/psat_server_web/schema/generateATLASSchemaAndCPPClasses.py
+-rw-r--r--   0 kws        (502) staff       (20)     2489 2021-03-10 12:03:01.000000 psat-server-web-0.3.9/psat_server_web/schema/get_table_columns_for_avro.py
+-rw-r--r--   0 kws        (502) staff       (20)      182 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/get_table_columns_for_avro.sql
+-rw-r--r--   0 kws        (502) staff       (20)      117 2023-04-18 09:51:15.000000 psat-server-web-0.3.9/psat_server_web/schema/mjdnow.sql
+-rw-r--r--   0 kws        (502) staff       (20)      977 2021-03-10 12:32:10.000000 psat-server-web-0.3.9/psat_server_web/schema/refresh_django_views.py
+-rw-r--r--   0 kws        (502) staff       (20)     4853 2021-03-10 22:44:14.000000 psat-server-web-0.3.9/psat_server_web/schema/setup_database.py
+-rw-r--r--   0 kws        (502) staff       (20)    13195 2021-03-10 22:48:16.000000 psat-server-web-0.3.9/psat_server_web/schema/setup_database_utils.py
+-rw-r--r--   0 kws        (502) staff       (20)      714 2021-03-09 13:30:11.000000 psat-server-web-0.3.9/psat_server_web/schema/sherlock_classifications.sql
+-rw-r--r--   0 kws        (502) staff       (20)     3104 2021-03-09 13:30:11.000000 psat-server-web-0.3.9/psat_server_web/schema/sherlock_crossmatches.sql
+-rw-r--r--   0 kws        (502) staff       (20)      646 2024-03-13 18:06:44.000000 psat-server-web-0.3.9/psat_server_web/schema/sherlock_triggers_atlas.sql
+-rw-r--r--   0 kws        (502) staff       (20)      649 2024-03-13 18:08:10.000000 psat-server-web-0.3.9/psat_server_web/schema/sherlock_triggers_ps1.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2038 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_cat_gaia_dr1.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2927 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_cat_gaia_dr2.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2421 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_cat_gaia_dr2_cassandra.cql
+-rw-r--r--   0 kws        (502) staff       (20)     1378 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_cat_kepler_k2.sql
+-rw-r--r--   0 kws        (502) staff       (20)      699 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_cat_kepler_k2_pixels.sql
+-rw-r--r--   0 kws        (502) staff       (20)     6105 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_cat_ps1_medium_deep_ref.sql
+-rw-r--r--   0 kws        (502) staff       (20)      713 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_cat_ps1_ubercal_stars.sql
+-rw-r--r--   0 kws        (502) staff       (20)      570 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_cat_satellites.sql
+-rw-r--r--   0 kws        (502) staff       (20)     4756 2023-04-17 09:11:12.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_catalogue_tables.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1659 2023-04-17 09:43:29.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_cfa_detections.sql
+-rw-r--r--   0 kws        (502) staff       (20)      576 2023-04-17 09:44:10.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_cfa_to_ipp_lookup.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1074 2023-04-17 09:11:49.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_classification_flags.sql
+-rw-r--r--   0 kws        (502) staff       (20)      547 2023-04-17 09:12:36.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_classification_history.sql
+-rw-r--r--   0 kws        (502) staff       (20)     5743 2023-04-17 09:09:37.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_cmf_metadata.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2015 2023-04-17 09:10:34.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_cross_matches.sql
+-rw-r--r--   0 kws        (502) staff       (20)      974 2023-04-17 09:46:54.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_cross_matches_external.sql
+-rw-r--r--   0 kws        (502) staff       (20)      776 2023-04-17 09:22:29.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_detection_lists.sql
+-rw-r--r--   0 kws        (502) staff       (20)      763 2023-04-17 10:12:43.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_detection_lists_atlas.sql
+-rw-r--r--   0 kws        (502) staff       (20)      730 2023-04-17 09:45:16.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_followup_photometry.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1078 2023-04-17 09:46:10.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_followup_telescope_instruments.sql
+-rw-r--r--   0 kws        (502) staff       (20)      837 2023-04-17 09:46:26.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_followup_telescopes.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2096 2023-04-17 09:23:20.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_forced_photometry.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1020 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_function_lunation.sql
+-rw-r--r--   0 kws        (502) staff       (20)      898 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_function_mjdlunation.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1327 2023-06-15 15:50:56.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_gravity_alerts.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1426 2023-06-02 14:29:20.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_gravity_event_annotations.sql
+-rw-r--r--   0 kws        (502) staff       (20)      609 2023-04-17 09:50:41.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_gravity_events.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1501 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_guide_star_cat.sql
+-rw-r--r--   0 kws        (502) staff       (20)      875 2023-04-17 09:20:30.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_image_groups.sql
+-rw-r--r--   0 kws        (502) staff       (20)      921 2023-04-17 09:12:16.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_images.sql
+-rw-r--r--   0 kws        (502) staff       (20)      576 2023-04-17 09:43:46.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_ipp_to_cfa_lookup.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2677 2023-04-17 09:24:31.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_latest_object_stats.sql
+-rw-r--r--   0 kws        (502) staff       (20)      919 2023-04-17 09:49:53.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_object_comments.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2622 2023-04-17 09:25:25.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_object_group_definitions.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1904 2023-04-17 10:10:30.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_object_group_definitions_atlas.sql
+-rw-r--r--   0 kws        (502) staff       (20)      623 2023-04-17 09:24:56.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_object_groups.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2929 2023-04-17 09:19:54.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_parameter_definitions.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1347 2023-04-17 10:13:23.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_photpipe_detections.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1100 2023-04-17 09:20:57.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_postage_stamp_images.sql
+-rw-r--r--   0 kws        (502) staff       (20)      715 2023-04-17 09:21:25.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_postage_stamp_requests.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1091 2023-04-17 09:22:07.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_postage_stamp_status_codes.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1037 2023-04-17 09:44:43.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_processing_status.sql
+-rw-r--r--   0 kws        (502) staff       (20)      830 2023-04-17 09:13:08.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_search_parameters.sql
+-rw-r--r--   0 kws        (502) staff       (20)      680 2023-04-17 09:50:14.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_tns_requests.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1298 2023-04-17 10:13:40.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_tphot_detections.sql
+-rw-r--r--   0 kws        (502) staff       (20)     7956 2023-04-17 09:07:52.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_transient_objects.sql
+-rw-r--r--   0 kws        (502) staff       (20)     4644 2023-04-17 09:08:54.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_transient_reobservations.sql
+-rw-r--r--   0 kws        (502) staff       (20)      586 2024-02-22 10:16:13.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_vra_scores.sql
+-rw-r--r--   0 kws        (502) staff       (20)      829 2023-04-17 09:24:11.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_zoo_requests.sql
+-rw-r--r--   0 kws        (502) staff       (20)      703 2023-04-17 09:53:30.000000 psat-server-web-0.3.9/psat_server_web/schema/tcs_zooniverse_scores.sql
+-rw-r--r--   0 kws        (502) staff       (20)      537 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/types_gaia_dr2_cassandra.txt
+-rw-r--r--   0 kws        (502) staff       (20)     4346 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/update_database_types_to_tns_types_atlas.sql
+-rw-r--r--   0 kws        (502) staff       (20)     4521 2021-03-09 13:29:22.000000 psat-server-web-0.3.9/psat_server_web/schema/update_database_types_to_tns_types_panstarrs.sql
+-rw-r--r--   0 kws        (502) staff       (20)       96 2023-06-15 16:08:21.000000 psat-server-web-0.3.9/psat_server_web/schema/update_tcs_gravity_alerts_001.sql
+-rw-r--r--   0 kws        (502) staff       (20)      808 2023-06-02 14:32:50.000000 psat-server-web-0.3.9/psat_server_web/schema/update_tcs_gravity_event_annotations_001.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1497 2021-11-23 00:25:03.000000 psat-server-web-0.3.9/psat_server_web/schema/update_tcs_latest_object_stats_001.sql
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2024-04-10 23:53:56.351635 psat-server-web-0.3.9/psat_server_web.egg-info/
+-rw-r--r--   0 kws        (502) staff       (20)      839 2024-04-10 23:53:52.000000 psat-server-web-0.3.9/psat_server_web.egg-info/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)    22635 2024-04-10 23:53:56.000000 psat-server-web-0.3.9/psat_server_web.egg-info/SOURCES.txt
+-rw-r--r--   0 kws        (502) staff       (20)        1 2024-04-10 23:53:52.000000 psat-server-web-0.3.9/psat_server_web.egg-info/dependency_links.txt
+-rw-r--r--   0 kws        (502) staff       (20)        1 2023-04-17 21:29:34.000000 psat-server-web-0.3.9/psat_server_web.egg-info/not-zip-safe
+-rw-r--r--   0 kws        (502) staff       (20)      138 2024-04-10 23:53:52.000000 psat-server-web-0.3.9/psat_server_web.egg-info/requires.txt
+-rw-r--r--   0 kws        (502) staff       (20)       16 2024-04-10 23:53:52.000000 psat-server-web-0.3.9/psat_server_web.egg-info/top_level.txt
+-rw-r--r--   0 kws        (502) staff       (20)       38 2024-04-10 23:53:56.836490 psat-server-web-0.3.9/setup.cfg
+-rwxr-xr-x   0 kws        (502) staff       (20)     1318 2024-04-10 23:50:46.000000 psat-server-web-0.3.9/setup.py
```

### Comparing `psat-server-web-0.3.8/LICENSE` & `psat-server-web-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/PKG-INFO` & `psat-server-web-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psat-server-web
-Version: 0.3.8
+Version: 0.3.9
 Summary: Pan-STARRS and ATLAS web interface.
 Home-page: https://github.com/genghisken/psat-server-web
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `psat-server-web-0.3.8/psat_server_web/.DS_Store` & `psat-server-web-0.3.9/psat_server_web/.DS_Store`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/.DS_Store` & `psat-server-web-0.3.9/psat_server_web/atlas/.DS_Store`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/atlas/apiutils.py` & `psat-server-web-0.3.9/psat_server_web/atlas/atlas/apiutils.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/atlas/commonqueries.py` & `psat-server-web-0.3.9/psat_server_web/atlas/atlas/commonqueries.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/atlas/dbviews.py` & `psat-server-web-0.3.9/psat_server_web/atlas/atlas/dbviews.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/atlas/formchoices.py` & `psat-server-web-0.3.9/psat_server_web/atlas/atlas/formchoices.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/atlas/helpers.py` & `psat-server-web-0.3.9/psat_server_web/atlas/atlas/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,16 +63,16 @@
     else:
          # It must be a coordinate or a match failure
          coords = getCoordsAndSearchRadius(searchText)
          if coords:
              searchRadius = 4.0
              if coords['radius']:
                  searchRadius = float(coords['radius'])
-                 if searchRadius > 99.0:
-                      searchRadius = 99.0
+                 if searchRadius > 300.0:
+                      searchRadius = 300.0
          
              message, xmObjects = coneSearchHTM(coords['ra'], coords['dec'], searchRadius, 'atlas_diff_objects', queryType = FULL, conn = connection, django = True)
              for xm in xmObjects:
                  dictRow = xm[1]
                  dictRow.update({'xmseparation': xm[0]})
                  # Add sexagesimal RA and Dec
                  dictRow.update({'ra_sex': ra_to_sex(dictRow['ra'])})
```

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/atlas/lightcurvequeries.py` & `psat-server-web-0.3.9/psat_server_web/atlas/atlas/lightcurvequeries.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/atlas/models.py` & `psat-server-web-0.3.9/psat_server_web/atlas/atlas/models.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/atlas/settings.py` & `psat-server-web-0.3.9/psat_server_web/atlas/atlas/settings.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/atlas/sqlpaginator.py` & `psat-server-web-0.3.9/psat_server_web/atlas/atlas/sqlpaginator.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/atlas/urls.py` & `psat-server-web-0.3.9/psat_server_web/atlas/atlas/urls.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/atlas/views.py` & `psat-server-web-0.3.9/psat_server_web/atlas/atlas/views.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/atlas/wsgi.atlas.conf` & `psat-server-web-0.3.9/psat_server_web/atlas/atlas/wsgi.atlas.conf`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/atlas/wsgi_apache_example.conf` & `psat-server-web-0.3.9/psat_server_web/atlas/atlas/wsgi_apache_example.conf`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/atlasapi/query_auth.py` & `psat-server-web-0.3.9/psat_server_web/atlas/atlasapi/query_auth.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/atlasapi/serializers.py` & `psat-server-web-0.3.9/psat_server_web/atlas/atlasapi/serializers.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/atlasapi/urls.py` & `psat-server-web-0.3.9/psat_server_web/atlas/atlasapi/urls.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/atlasapi/views.py` & `psat-server-web-0.3.9/psat_server_web/atlas/atlasapi/views.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/generate_mod_wsgi_apachectl.sh` & `psat-server-web-0.3.9/psat_server_web/atlas/generate_mod_wsgi_apachectl.sh`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/css/aladin.css` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/css/aladin.css`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/css/celestial.css` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/css/celestial.css`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/css/fontawesome.css` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/css/main.css` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/css/main.css`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/css/main_bootstrap.css` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/css/main_bootstrap.css`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/images/atlas_logo.png` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/images/atlas_logo.png`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/images/image_not_available.jpeg` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/images/image_not_available.jpeg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/aladin.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/aladin.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/bootstrap_utils.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/bootstrap_utils.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/celestial.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/celestial.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/d3.geo.projection.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/d3.geo.projection.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/d3.geo.projection.min.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/d3.geo.projection.min.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/d3.geo.zoom.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/d3.geo.zoom.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/d3.min.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/d3.min.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/data/constellations.bounds.json` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/data/constellations.bounds.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/data/constellations.json` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/data/constellations.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/data/constellations.lines.json` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/data/constellations.lines.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/data/dsos.bright.json` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/data/dsos.bright.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/data/lg.json` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/data/lg.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/data/mw.json` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/data/mw.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/data/planets.json` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/data/planets.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/celestial/data/stars.6.json` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/celestial/data/stars.6.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/colourplot.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/colourplot.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/excanvas.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/excanvas.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery-1.7.2.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery-1.7.2.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.axislabels.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.axislabels.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.crosshair.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.crosshair.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.errorbars.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.errorbars.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.fillbetween.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.fillbetween.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.image.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.image.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.navigate.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.navigate.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.pie.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.pie.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.resize.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.resize.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.selection.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.selection.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.stack.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.stack.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.symbol.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.symbol.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.threshold.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.threshold.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/followup_selectall.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/followup_selectall.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/heatmap.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/heatmap.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/lightcurve.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/lightcurve.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/lightcurveplotly.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/lightcurveplotly.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/mjdcalc.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/mjdcalc.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/plotly/plotly-latest.kws.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/plotly/plotly-latest.kws.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/recurrenceplot.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/recurrenceplot.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/js/recurrenceplotplotly.js` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/js/recurrenceplotplotly.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-brands-400.eot` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-brands-400.svg` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-brands-400.ttf` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-brands-400.woff` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-brands-400.woff2` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-regular-400.eot` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-regular-400.svg` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-regular-400.ttf` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-regular-400.woff` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-regular-400.woff2` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-solid-900.eot` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-solid-900.svg` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-solid-900.ttf` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-solid-900.woff` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/site_media/webfonts/fa-solid-900.woff2` & `psat-server-web-0.3.9/psat_server_web/atlas/site_media/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/sql/create_web_views.sql` & `psat-server-web-0.3.9/psat_server_web/atlas/sql/create_web_views.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/.DS_Store` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/atelfasttrackobject.txt` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/atelfasttrackobject.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/atelsdiscovery.txt` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/atelsdiscovery.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/atelsfast.txt` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/atelsfast.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/candidate.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/candidate.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/candidate_plotly.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/candidate_plotly.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/candidate_plotly_test.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/candidate_plotly_test.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/crossmatch_external.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/crossmatch_external.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/followup.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/followup.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/followup.txt` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/followup.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/followup2.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/followup2.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/followup_bs.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/followup_bs.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/followup_bypass_django_tables.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/followup_bypass_django_tables.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/followup_quickview.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/followup_quickview.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/followup_quickview_bs.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/followup_quickview_bs.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/followup_subset.txt` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/followup_subset.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/gcn.txt` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/gcn.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/gcn_latex.txt` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/gcn_latex.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/heatmap.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/heatmap.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/heatmap_test.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/heatmap_test.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/index.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/index.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/index_bs.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/index_bs.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/index_bs_celestial.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/index_bs_celestial.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/lightcurve.txt` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/lightcurve.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/lightcurveddc.txt` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/lightcurveddc.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/lightcurveforced.txt` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/lightcurveforced.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/pesstosummary.txt` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/pesstosummary.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/search_results.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/search_results.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/search_results_plotly.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/search_results_plotly.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/summary.csv` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/summary.csv`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/userdefinedlists.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/userdefinedlists.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/atlas/userdefinedlists_bs.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/atlas/userdefinedlists_bs.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/base.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/base.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/base_bootstrap.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/base_bootstrap.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/base_bootstrap_login.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/base_bootstrap_login.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/bootstrap4_django_tables2_atlas.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/bootstrap4_django_tables2_atlas.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/templates/login.html` & `psat-server-web-0.3.9/psat_server_web/atlas/templates/login.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/atlas/test.py` & `psat-server-web-0.3.9/psat_server_web/atlas/test.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/config/wsgi.conf.template` & `psat-server-web-0.3.9/psat_server_web/config/wsgi.conf.template`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/createUsers.py` & `psat-server-web-0.3.9/psat_server_web/ps1/createUsers.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/generate_mod_wsgi_apachectl.sh` & `psat-server-web-0.3.9/psat_server_web/ps1/generate_mod_wsgi_apachectl.sh`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/psdb/admin.py.old` & `psat-server-web-0.3.9/psat_server_web/ps1/psdb/admin.py.old`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/psdb/catalogueviews.py` & `psat-server-web-0.3.9/psat_server_web/ps1/psdb/catalogueviews.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/psdb/commonqueries.py` & `psat-server-web-0.3.9/psat_server_web/ps1/psdb/commonqueries.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/psdb/dbviews.py` & `psat-server-web-0.3.9/psat_server_web/ps1/psdb/dbviews.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/psdb/formchoices.py` & `psat-server-web-0.3.9/psat_server_web/ps1/psdb/formchoices.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/psdb/helpers.py` & `psat-server-web-0.3.9/psat_server_web/ps1/psdb/helpers.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/psdb/img_scale.py` & `psat-server-web-0.3.9/psat_server_web/ps1/psdb/img_scale.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/psdb/lightcurvequeries.py` & `psat-server-web-0.3.9/psat_server_web/ps1/psdb/lightcurvequeries.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/psdb/models.py` & `psat-server-web-0.3.9/psat_server_web/ps1/psdb/models.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/psdb/settings.py` & `psat-server-web-0.3.9/psat_server_web/ps1/psdb/settings.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/psdb/urls.py` & `psat-server-web-0.3.9/psat_server_web/ps1/psdb/urls.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/psdb/views.py` & `psat-server-web-0.3.9/psat_server_web/ps1/psdb/views.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/psdb/wsgi_apache_example.conf` & `psat-server-web-0.3.9/psat_server_web/ps1/psdb/wsgi_apache_example.conf`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/css/aladin.css` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/css/aladin.css`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/css/celestial.css` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/css/celestial.css`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/css/fontawesome.css` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/css/main.css` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/css/main.css`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/css/main_bootstrap.css` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/css/main_bootstrap.css`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/1-star-hover.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/1-star-hover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/1-star.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/1-star.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/2-star-hover.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/2-star-hover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/2-star.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/2-star.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/3-star-hover.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/3-star-hover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/3-star.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/3-star.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/aladin.gif` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/aladin.gif`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/cfaIcon.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/cfaIcon.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/cfaIconHover.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/cfaIconHover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/confirmed-sne-hover.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/confirmed-sne-hover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/confirmed-sne.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/confirmed-sne.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/detection_example.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/detection_example.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/down.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/down.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/image_not_available.jpeg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/image_not_available.jpeg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/jhuIcon.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/jhuIcon.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/jhuIconHover.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/jhuIconHover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/minus.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/minus.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/ncuIcon.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/ncuIcon.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/ncuIconHover.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/ncuIconHover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/non_detection_example.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/non_detection_example.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/others-hover.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/others-hover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/others.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/others.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs-logo-hover.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs-logo-hover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs-logo.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs-logo.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs1_logo.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs1_logo.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs1_o3_logo.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs1_o3_logo.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs2_logo.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs2_logo.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs2_o3_logo.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs2_o3_logo.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs_logo.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs_logo.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs_logo_original.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs_logo_original.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs_logo_yse.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs_logo_yse.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/panstarrs_logo_yse_stack.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/panstarrs_logo_yse_stack.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/pittsIcon.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/pittsIcon.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/pittsIconHover.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/pittsIconHover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/plus.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/plus.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/ps1Icon.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/ps1Icon.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/ps1IconHover.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/ps1IconHover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/ps1sc.gif` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/ps1sc.gif`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/qub-logo-hover.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/qub-logo-hover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/qub-logo.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/qub-logo.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/qubIcon.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/qubIcon.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/qubIconHover.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/qubIconHover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/sdss.gif` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/sdss.gif`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/table-background.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/table-background.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/table-bottom-left.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/table-bottom-left.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/table-bottom-right.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/table-bottom-right.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/table-row.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/table-row.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/table-top-left.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/table-top-left.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/table-top-right.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/table-top-right.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/uhifaIcon.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/uhifaIcon.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/uhifaIconHover.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/uhifaIconHover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/up.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/up.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/variable-stars-hover.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/variable-stars-hover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/images/variable-stars.jpg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/images/variable-stars.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/aladin.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/aladin.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/celestial.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/celestial.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/d3.geo.projection.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/d3.geo.projection.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/d3.geo.projection.min.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/d3.geo.projection.min.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/d3.geo.zoom.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/d3.geo.zoom.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/d3.min.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/d3.min.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/data/constellations.bounds.json` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/data/constellations.bounds.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/data/constellations.json` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/data/constellations.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/data/constellations.lines.json` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/data/constellations.lines.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/data/dsos.bright.json` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/data/dsos.bright.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/data/lg.json` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/data/lg.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/data/mw.json` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/data/mw.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/data/planets.json` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/data/planets.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/celestial/data/stars.6.json` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/celestial/data/stars.6.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/colourplot.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/colourplot.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/excanvas.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/excanvas.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery-1.7.2.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery-1.7.2.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.axislabels.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.axislabels.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.crosshair.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.crosshair.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.errorbars.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.errorbars.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.fillbetween.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.fillbetween.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.image.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.image.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.navigate.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.navigate.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.pie.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.pie.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.resize.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.resize.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.selection.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.selection.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.stack.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.stack.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.symbol.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.symbol.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.threshold.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.threshold.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/followup_selectall.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/followup_selectall.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/lightcurve.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/lightcurve.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/lightcurveplotly.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/lightcurveplotly.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/mjdcalc.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/mjdcalc.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/plotly/plotly-latest.kws.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/plotly/plotly-latest.kws.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/recurrenceplot.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/recurrenceplot.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/js/recurrenceplotplotly.js` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/js/recurrenceplotplotly.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-brands-400.eot` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-brands-400.svg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-brands-400.ttf` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-brands-400.woff` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-brands-400.woff2` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-regular-400.eot` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-regular-400.svg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-regular-400.ttf` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-regular-400.woff` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-regular-400.woff2` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-solid-900.eot` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-solid-900.svg` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-solid-900.ttf` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-solid-900.woff` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/site_media/webfonts/fa-solid-900.woff2` & `psat-server-web-0.3.9/psat_server_web/ps1/site_media/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/sql/create_web_cat_views.sql` & `psat-server-web-0.3.9/psat_server_web/ps1/sql/create_web_cat_views.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/sql/create_web_user_grants.sql` & `psat-server-web-0.3.9/psat_server_web/ps1/sql/create_web_user_grants.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/sql/create_web_views.sql` & `psat-server-web-0.3.9/psat_server_web/ps1/sql/create_web_views.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/sql/create_web_views_fgss.sql` & `psat-server-web-0.3.9/psat_server_web/ps1/sql/create_web_views_fgss.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/base.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/base.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/base_bootstrap.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/base_bootstrap.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/base_bootstrap_login.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/base_bootstrap_login.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/base_new.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/base_new.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/bootstrap4_django_tables2_atlas.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/bootstrap4_django_tables2_atlas.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/login.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/login.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/atelsdiscovery.txt` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/atelsdiscovery.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/candidate.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/candidate.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/candidate_plotly.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/candidate_plotly.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/candidate_quickview.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/candidate_quickview.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/candidateflot.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/candidateflot.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/candidates.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/candidates.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/colourdata.txt` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/colourdata.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/crossmatch_cfa_with_ipp.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/crossmatch_cfa_with_ipp.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/crossmatch_external.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/crossmatch_external.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/fasttrackastronote.txt` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/fasttrackastronote.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/filter.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/filter.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/followup.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/followup.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/followup.txt` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/followup.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/followup_bs.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/followup_bs.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/followup_bs_old.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/followup_bs_old.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/followup_quickview.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/followup_quickview.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/followup_quickview_bs.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/followup_quickview_bs.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/followup_quickview_bs_old.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/followup_quickview_bs_old.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/gcn.txt` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/gcn.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/gcn_latex.txt` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/gcn_latex.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/index.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/index.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/index_bs_celestial.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/index_bs_celestial.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/index_public.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/index_public.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/lightcurves.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/lightcurves.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/obsmediawiki.txt` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/obsmediawiki.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/public.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/public.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/public_textonly.txt` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/public_textonly.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/reports.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/reports.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/search_results.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/search_results.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/search_results_plotly.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/search_results_plotly.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/userdefinedlists.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/userdefinedlists.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/ps1/templates/psdb/userdefinedlists_bs.html` & `psat-server-web-0.3.9/psat_server_web/ps1/templates/psdb/userdefinedlists_bs.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/atlas_detections.sql` & `psat-server-web-0.3.9/psat_server_web/schema/atlas_detections.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/atlas_detectionsddc.sql` & `psat-server-web-0.3.9/psat_server_web/schema/atlas_detectionsddc.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/atlas_diff_detections.sql` & `psat-server-web-0.3.9/psat_server_web/schema/atlas_diff_detections.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/atlas_diff_logs.sql` & `psat-server-web-0.3.9/psat_server_web/schema/atlas_diff_logs.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/atlas_diff_moments.sql` & `psat-server-web-0.3.9/psat_server_web/schema/atlas_diff_moments.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/atlas_diff_objects.sql` & `psat-server-web-0.3.9/psat_server_web/schema/atlas_diff_objects.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/atlas_diff_subcell_logs.sql` & `psat-server-web-0.3.9/psat_server_web/schema/atlas_diff_subcell_logs.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/atlas_diff_subcells.sql` & `psat-server-web-0.3.9/psat_server_web/schema/atlas_diff_subcells.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/atlas_forced_photometry.sql` & `psat-server-web-0.3.9/psat_server_web/schema/atlas_forced_photometry.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/atlas_heatmaps.sql` & `psat-server-web-0.3.9/psat_server_web/schema/atlas_heatmaps.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/atlas_metadata.sql` & `psat-server-web-0.3.9/psat_server_web/schema/atlas_metadata.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/atlas_metadataddc.sql` & `psat-server-web-0.3.9/psat_server_web/schema/atlas_metadataddc.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/atlas_objects.sql` & `psat-server-web-0.3.9/psat_server_web/schema/atlas_objects.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/atlas_stacked_forced_photometry.sql` & `psat-server-web-0.3.9/psat_server_web/schema/atlas_stacked_forced_photometry.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/convert_backend_storage_to_innodb.sql` & `psat-server-web-0.3.9/psat_server_web/schema/convert_backend_storage_to_innodb.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/create_atlas_flattened_view.sql` & `psat-server-web-0.3.9/psat_server_web/schema/create_atlas_flattened_view.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/create_photpipe_views.sql` & `psat-server-web-0.3.9/psat_server_web/schema/create_photpipe_views.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/create_schema.sql` & `psat-server-web-0.3.9/psat_server_web/schema/create_schema.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/create_user_grants.sql` & `psat-server-web-0.3.9/psat_server_web/schema/create_user_grants.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/create_user_grants_generic.sql` & `psat-server-web-0.3.9/psat_server_web/schema/create_user_grants_generic.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/delete_transients.sql` & `psat-server-web-0.3.9/psat_server_web/schema/delete_transients.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/generateATLASSchemaAndCPPClasses.py` & `psat-server-web-0.3.9/psat_server_web/schema/generateATLASSchemaAndCPPClasses.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/get_table_columns_for_avro.py` & `psat-server-web-0.3.9/psat_server_web/schema/get_table_columns_for_avro.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/refresh_django_views.py` & `psat-server-web-0.3.9/psat_server_web/schema/refresh_django_views.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/setup_database.py` & `psat-server-web-0.3.9/psat_server_web/schema/setup_database.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/setup_database_utils.py` & `psat-server-web-0.3.9/psat_server_web/schema/setup_database_utils.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/sherlock_classifications.sql` & `psat-server-web-0.3.9/psat_server_web/schema/sherlock_classifications.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/sherlock_crossmatches.sql` & `psat-server-web-0.3.9/psat_server_web/schema/sherlock_crossmatches.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_cat_gaia_dr1.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_cat_gaia_dr1.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_cat_gaia_dr2.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_cat_gaia_dr2.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_cat_gaia_dr2_cassandra.cql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_cat_gaia_dr2_cassandra.cql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_cat_kepler_k2.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_cat_kepler_k2.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_cat_kepler_k2_pixels.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_cat_kepler_k2_pixels.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_cat_ps1_medium_deep_ref.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_cat_ps1_medium_deep_ref.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_cat_ps1_ubercal_stars.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_cat_ps1_ubercal_stars.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_cat_satellites.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_cat_satellites.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_catalogue_tables.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_catalogue_tables.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_cfa_detections.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_cfa_detections.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_cfa_to_ipp_lookup.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_cfa_to_ipp_lookup.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_classification_flags.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_classification_flags.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_classification_history.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_classification_history.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_cmf_metadata.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_cmf_metadata.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_cross_matches.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_cross_matches.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_cross_matches_external.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_cross_matches_external.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_detection_lists.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_detection_lists.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_detection_lists_atlas.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_detection_lists_atlas.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_followup_photometry.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_followup_photometry.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_followup_telescope_instruments.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_followup_telescope_instruments.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_followup_telescopes.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_followup_telescopes.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_forced_photometry.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_forced_photometry.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_function_lunation.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_function_lunation.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_function_mjdlunation.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_function_mjdlunation.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_gravity_alerts.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_gravity_alerts.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_gravity_event_annotations.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_gravity_event_annotations.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_gravity_events.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_gravity_events.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_guide_star_cat.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_guide_star_cat.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_image_groups.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_image_groups.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_images.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_images.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_ipp_to_cfa_lookup.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_ipp_to_cfa_lookup.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_latest_object_stats.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_latest_object_stats.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_object_comments.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_object_comments.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_object_group_definitions.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_object_group_definitions.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_object_group_definitions_atlas.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_object_group_definitions_atlas.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_object_groups.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_object_groups.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_parameter_definitions.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_parameter_definitions.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_photpipe_detections.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_photpipe_detections.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_postage_stamp_images.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_postage_stamp_images.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_postage_stamp_requests.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_postage_stamp_requests.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_postage_stamp_status_codes.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_postage_stamp_status_codes.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_processing_status.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_processing_status.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_search_parameters.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_search_parameters.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_tns_requests.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_tns_requests.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_tphot_detections.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_tphot_detections.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_transient_objects.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_transient_objects.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_transient_reobservations.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_transient_reobservations.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_vra_scores.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_vra_scores.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_zoo_requests.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_zoo_requests.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/tcs_zooniverse_scores.sql` & `psat-server-web-0.3.9/psat_server_web/schema/tcs_zooniverse_scores.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/types_gaia_dr2_cassandra.txt` & `psat-server-web-0.3.9/psat_server_web/schema/types_gaia_dr2_cassandra.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/update_database_types_to_tns_types_atlas.sql` & `psat-server-web-0.3.9/psat_server_web/schema/update_database_types_to_tns_types_atlas.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/update_database_types_to_tns_types_panstarrs.sql` & `psat-server-web-0.3.9/psat_server_web/schema/update_database_types_to_tns_types_panstarrs.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/update_tcs_gravity_event_annotations_001.sql` & `psat-server-web-0.3.9/psat_server_web/schema/update_tcs_gravity_event_annotations_001.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web/schema/update_tcs_latest_object_stats_001.sql` & `psat-server-web-0.3.9/psat_server_web/schema/update_tcs_latest_object_stats_001.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.3.8/psat_server_web.egg-info/PKG-INFO` & `psat-server-web-0.3.9/psat_server_web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psat-server-web
-Version: 0.3.8
+Version: 0.3.9
 Summary: Pan-STARRS and ATLAS web interface.
 Home-page: https://github.com/genghisken/psat-server-web
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `psat-server-web-0.3.8/psat_server_web.egg-info/SOURCES.txt` & `psat-server-web-0.3.9/psat_server_web.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -371,14 +371,16 @@
 psat_server_web/schema/get_table_columns_for_avro.sql
 psat_server_web/schema/mjdnow.sql
 psat_server_web/schema/refresh_django_views.py
 psat_server_web/schema/setup_database.py
 psat_server_web/schema/setup_database_utils.py
 psat_server_web/schema/sherlock_classifications.sql
 psat_server_web/schema/sherlock_crossmatches.sql
+psat_server_web/schema/sherlock_triggers_atlas.sql
+psat_server_web/schema/sherlock_triggers_ps1.sql
 psat_server_web/schema/tcs_cat_gaia_dr1.sql
 psat_server_web/schema/tcs_cat_gaia_dr2.sql
 psat_server_web/schema/tcs_cat_gaia_dr2_cassandra.cql
 psat_server_web/schema/tcs_cat_kepler_k2.sql
 psat_server_web/schema/tcs_cat_kepler_k2_pixels.sql
 psat_server_web/schema/tcs_cat_ps1_medium_deep_ref.sql
 psat_server_web/schema/tcs_cat_ps1_ubercal_stars.sql
```

### Comparing `psat-server-web-0.3.8/setup.py` & `psat-server-web-0.3.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,15 @@
           'django<4.2',
           'django_tables2',
           'djangorestframework',
           'pyyaml',
           'docopt',
           'python-dotenv',
           'gkhtm',
-          'gkutils>=0.3.0',
+          'gkutils>=0.3.2',
           'requests',
           'lasair',
           'dustmaps',
       ],
     python_requires='>=3.6',
     include_package_data=True,
     zip_safe=False
```

