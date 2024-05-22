# Comparing `tmp/django-reportbroD-3.0.tar.gz` & `tmp/django-reportbroD-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-reportbroD-3.0.tar", last modified: Mon May  6 16:19:14 2024, max compression
+gzip compressed data, was "django-reportbroD-4.0.tar", last modified: Wed May 22 15:14:56 2024, max compression
```

## Comparing `django-reportbroD-3.0.tar` & `django-reportbroD-4.0.tar`

### file list

```diff
@@ -1,173 +1,185 @@
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.829754 django-reportbroD-3.0/
--rw-r--r--   0 rider     (1000) rider     (1000)      131 2024-05-06 16:14:06.000000 django-reportbroD-3.0/MANIFEST.in
--rw-r--r--   0 rider     (1000) rider     (1000)     3580 2024-05-06 16:19:14.833087 django-reportbroD-3.0/PKG-INFO
--rw-r--r--   0 rider     (1000) rider     (1000)     2522 2024-05-06 15:46:26.000000 django-reportbroD-3.0/README.md
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.713086 django-reportbroD-3.0/django_reportbroD/
--rw-r--r--   0 rider     (1000) rider     (1000)        0 2024-02-16 20:55:14.000000 django-reportbroD-3.0/django_reportbroD/__init__.py
--rw-r--r--   0 rider     (1000) rider     (1000)      164 2024-02-18 03:27:34.000000 django-reportbroD-3.0/django_reportbroD/admin.py
--rw-r--r--   0 rider     (1000) rider     (1000)      191 2024-05-06 13:12:04.000000 django-reportbroD-3.0/django_reportbroD/apps.py
--rw-r--r--   0 rider     (1000) rider     (1000)      803 2024-05-01 16:21:02.000000 django-reportbroD-3.0/django_reportbroD/base.py
--rw-r--r--   0 rider     (1000) rider     (1000)      832 2024-04-14 18:53:48.000000 django-reportbroD-3.0/django_reportbroD/forms.py
--rw-r--r--   0 rider     (1000) rider     (1000)      984 2024-05-05 01:43:48.000000 django-reportbroD-3.0/django_reportbroD/menus.py
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.713086 django-reportbroD-3.0/django_reportbroD/migrations/
--rw-r--r--   0 rider     (1000) rider     (1000)        0 2024-02-16 20:55:14.000000 django-reportbroD-3.0/django_reportbroD/migrations/__init__.py
--rw-r--r--   0 rider     (1000) rider     (1000)     1864 2024-04-14 17:00:30.000000 django-reportbroD-3.0/django_reportbroD/models.py
--rw-r--r--   0 rider     (1000) rider     (1000)    13363 2024-05-01 16:25:14.000000 django-reportbroD-3.0/django_reportbroD/reportcore.py
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.709752 django-reportbroD-3.0/django_reportbroD/static/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.709752 django-reportbroD-3.0/django_reportbroD/static/assets/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.716419 django-reportbroD-3.0/django_reportbroD/static/assets/css/
--rw-r--r--   0 rider     (1000) rider     (1000)     1772 2019-03-30 20:18:02.000000 django-reportbroD-3.0/django_reportbroD/static/assets/css/mCSB_buttons.html
--rw-r--r--   0 rider     (1000) rider     (1000)     1772 2019-03-30 20:18:02.000000 django-reportbroD-3.0/django_reportbroD/static/assets/css/owl.video.play.html
--rw-r--r--   0 rider     (1000) rider     (1000)   509223 2019-03-30 20:18:10.000000 django-reportbroD-3.0/django_reportbroD/static/assets/css/style.css
--rw-r--r--   0 rider     (1000) rider     (1000)   236692 2024-05-05 16:55:58.000000 django-reportbroD-3.0/django_reportbroD/static/assets/css/vendors.css
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.766420 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/
--rw-r--r--   0 rider     (1000) rider     (1000)    62984 2019-03-30 20:18:20.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    24288 2019-03-30 20:18:20.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.html
--rw-r--r--   0 rider     (1000) rider     (1000)   351196 2019-03-30 20:18:20.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    62768 2019-03-30 20:18:20.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    31064 2019-03-30 20:18:20.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    62984 2019-03-30 20:18:20.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-iconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    41808 2019-03-30 20:18:22.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    16604 2019-03-30 20:18:22.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.html
--rw-r--r--   0 rider     (1000) rider     (1000)   163862 2019-03-30 20:18:22.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    41636 2019-03-30 20:18:22.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    20528 2019-03-30 20:18:22.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    41808 2019-03-30 20:18:22.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashiconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    40522 2019-03-30 20:18:22.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripicons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    99368 2019-03-30 20:18:22.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripicons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    40348 2019-03-30 20:18:22.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripicons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    26004 2019-03-30 20:18:24.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripicons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    40522 2019-03-30 20:18:24.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripiconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    62084 2019-03-30 20:18:24.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/feather.eot
--rw-r--r--   0 rider     (1000) rider     (1000)   213926 2019-03-30 20:18:26.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/feather.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    61920 2019-03-30 20:18:24.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/feather.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    29500 2019-03-30 20:18:24.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/feather.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    62084 2019-03-30 20:18:24.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/featherd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)   165742 2019-03-30 20:18:26.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    77159 2019-03-30 20:18:26.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.html
--rw-r--r--   0 rider     (1000) rider     (1000)   444379 2019-03-30 20:18:28.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.svg
--rw-r--r--   0 rider     (1000) rider     (1000)   165548 2019-03-30 20:18:28.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    98024 2019-03-30 20:18:26.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.woff
--rw-r--r--   0 rider     (1000) rider     (1000)   165742 2019-03-30 20:18:28.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesomed41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)   144114 2019-03-30 20:18:28.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    61020 2019-03-30 20:18:28.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.html
--rw-r--r--   0 rider     (1000) rider     (1000)   400219 2019-03-30 20:18:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)   143936 2019-03-30 20:18:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    80356 2019-03-30 20:18:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)   144114 2019-03-30 20:18:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ioniconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    21514 2019-03-30 20:18:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weather.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    48132 2019-03-30 20:18:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weather.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    21308 2019-03-30 20:18:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weather.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)     7936 2019-03-30 20:18:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weather.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    21514 2019-03-30 20:18:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weatherd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    42495 2019-03-30 20:18:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    38383 2019-03-30 20:18:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.html
--rw-r--r--   0 rider     (1000) rider     (1000)   238287 2019-03-30 20:18:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    99212 2019-03-30 20:18:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    50312 2019-03-30 20:18:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    42495 2019-03-30 20:18:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-iconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    16746 2019-03-30 20:18:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/summernotec360.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    16560 2019-03-30 20:18:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/summernotec360.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    10324 2019-03-30 20:18:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/summernotec360.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    78748 2019-03-30 20:18:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-icons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)   234269 2019-03-30 20:18:36.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-icons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    78584 2019-03-30 20:18:36.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-icons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    56108 2019-03-30 20:18:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-icons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    78748 2019-03-30 20:18:36.000000 django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-iconsd41d.eot
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.769753 django-reportbroD-3.0/django_reportbroD/static/assets/img/
--rw-r--r--   0 rider     (1000) rider     (1000)    39361 2019-03-30 21:07:44.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/02.jpg
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.769753 django-reportbroD-3.0/django_reportbroD/static/assets/img/export/
--rw-r--r--   0 rider     (1000) rider     (1000)     1876 2019-03-30 21:07:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/export/csv.svg
--rw-r--r--   0 rider     (1000) rider     (1000)     1348 2019-03-30 21:07:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/export/txt.svg
--rw-r--r--   0 rider     (1000) rider     (1000)     2060 2019-03-30 21:07:30.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/export/xlsx.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    48878 2024-02-21 14:09:26.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/favicon.ico
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.776420 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/
--rw-r--r--   0 rider     (1000) rider     (1000)     1182 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/ai.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1380 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/css.png
--rw-r--r--   0 rider     (1000) rider     (1000)      948 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/dbf.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1383 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/doc.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1215 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/dwg.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1269 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/exe.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1006 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/html.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1364 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/jpg.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1399 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/pdf.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1397 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/png.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1430 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/psd.png
--rw-r--r--   0 rider     (1000) rider     (1000)     6359 2024-04-14 18:02:54.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/reporte.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1005 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/rtf.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1421 2019-03-30 21:07:32.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/svg.png
--rw-r--r--   0 rider     (1000) rider     (1000)      974 2019-03-30 21:07:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/xls.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1332 2019-03-30 21:07:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/xml.png
--rw-r--r--   0 rider     (1000) rider     (1000)      997 2019-03-30 21:07:34.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/zip.png
--rw-r--r--   0 rider     (1000) rider     (1000)     7446 2024-03-09 16:12:06.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/lista.png
--rw-r--r--   0 rider     (1000) rider     (1000)     4814 2024-02-21 13:55:04.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/logo-icon.png
--rw-r--r--   0 rider     (1000) rider     (1000)     2422 2019-03-30 20:18:36.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/logo-light.png
--rw-r--r--   0 rider     (1000) rider     (1000)    13606 2024-02-21 13:43:58.000000 django-reportbroD-3.0/django_reportbroD/static/assets/img/logo.png
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.779753 django-reportbroD-3.0/django_reportbroD/static/assets/js/
--rw-r--r--   0 rider     (1000) rider     (1000)   576312 2019-03-30 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/assets/js/app.js
--rw-r--r--   0 rider     (1000) rider     (1000)  8320860 2019-03-30 20:19:02.000000 django-reportbroD-3.0/django_reportbroD/static/assets/js/vendors.js
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.813087 django-reportbroD-3.0/django_reportbroD/static/reportlib/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.813087 django-reportbroD-3.0/django_reportbroD/static/reportlib/css/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.813087 django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.816420 django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/
--rw-r--r--   0 rider     (1000) rider     (1000)     1633 2024-02-14 15:51:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.svg
--rw-r--r--   0 rider     (1000) rider     (1000)     1384 2024-02-14 15:51:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)     1460 2024-02-14 15:51:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff
--rw-r--r--   0 rider     (1000) rider     (1000)      684 2024-02-14 15:51:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)      855 2024-02-14 15:51:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/style.css
--rw-r--r--   0 rider     (1000) rider     (1000)     4509 2024-02-21 21:05:40.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/css/styles.css
--rw-r--r--   0 rider     (1000) rider     (1000)     2238 2024-02-14 15:51:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/favicon.ico
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.819754 django-reportbroD-3.0/django_reportbroD/static/reportlib/js/
--rw-r--r--   0 rider     (1000) rider     (1000)   288580 2024-02-14 15:51:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.js
--rw-r--r--   0 rider     (1000) rider     (1000)    89501 2024-02-14 15:51:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.min.js
--rw-r--r--   0 rider     (1000) rider     (1000)     3121 2024-02-14 15:51:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/js/jquery.cookie.js
--rw-r--r--   0 rider     (1000) rider     (1000)    55398 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.css
--rw-r--r--   0 rider     (1000) rider     (1000)    77644 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.css.map
--rw-r--r--   0 rider     (1000) rider     (1000)   733475 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.js
--rw-r--r--   0 rider     (1000) rider     (1000)      665 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.js.LICENSE.txt
--rw-r--r--   0 rider     (1000) rider     (1000)  2440768 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.js.map
--rw-r--r--   0 rider     (1000) rider     (1000)   722287 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.min.js
--rw-r--r--   0 rider     (1000) rider     (1000)   803864 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.min.js.map
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.823087 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/
--rw-r--r--   0 rider     (1000) rider     (1000)    24374 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/ajaxload.gif
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.826420 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/
--rw-r--r--   0 rider     (1000) rider     (1000)    20756 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    16748 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)    20672 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    16756 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)    20664 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    16696 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)    20712 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    16740 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff2
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.826420 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/iconfonts/
--rw-r--r--   0 rider     (1000) rider     (1000)    37788 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    12676 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    12752 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff
--rw-r--r--   0 rider     (1000) rider     (1000)     4460 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)    12924 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/rb_logo_dark.png
--rw-r--r--   0 rider     (1000) rider     (1000)    13606 2024-02-21 20:18:44.000000 django-reportbroD-3.0/django_reportbroD/static/reportlib/src/rb_logo_white.png
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.829754 django-reportbroD-3.0/django_reportbroD/templates/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.829754 django-reportbroD-3.0/django_reportbroD/templates/bases/
--rw-r--r--   0 rider     (1000) rider     (1000)     1926 2024-05-05 18:22:34.000000 django-reportbroD-3.0/django_reportbroD/templates/bases/base.html
--rw-r--r--   0 rider     (1000) rider     (1000)      352 2024-04-15 00:52:16.000000 django-reportbroD-3.0/django_reportbroD/templates/bases/footer.html
--rw-r--r--   0 rider     (1000) rider     (1000)     2825 2024-05-05 18:10:40.000000 django-reportbroD-3.0/django_reportbroD/templates/bases/header.html
--rw-r--r--   0 rider     (1000) rider     (1000)      654 2024-05-05 01:48:02.000000 django-reportbroD-3.0/django_reportbroD/templates/bases/navigator.html
--rw-r--r--   0 rider     (1000) rider     (1000)     1890 2024-02-21 13:51:56.000000 django-reportbroD-3.0/django_reportbroD/templates/create.html
--rw-r--r--   0 rider     (1000) rider     (1000)    20738 2024-05-05 02:23:36.000000 django-reportbroD-3.0/django_reportbroD/templates/document.html
--rw-r--r--   0 rider     (1000) rider     (1000)     2122 2024-04-30 23:35:42.000000 django-reportbroD-3.0/django_reportbroD/templates/edit.html
--rw-r--r--   0 rider     (1000) rider     (1000)    22882 2024-05-05 16:43:04.000000 django-reportbroD-3.0/django_reportbroD/templates/especif.html
--rw-r--r--   0 rider     (1000) rider     (1000)     1128 2024-02-20 03:51:56.000000 django-reportbroD-3.0/django_reportbroD/templates/formulario.html
--rw-r--r--   0 rider     (1000) rider     (1000)     3066 2024-04-15 00:38:30.000000 django-reportbroD-3.0/django_reportbroD/templates/import.html
--rw-r--r--   0 rider     (1000) rider     (1000)    10082 2024-05-05 02:25:04.000000 django-reportbroD-3.0/django_reportbroD/templates/index.html
--rw-r--r--   0 rider     (1000) rider     (1000)     3065 2024-04-14 18:52:08.000000 django-reportbroD-3.0/django_reportbroD/templates/report.html
--rw-r--r--   0 rider     (1000) rider     (1000)      743 2024-04-14 18:59:30.000000 django-reportbroD-3.0/django_reportbroD/urls.py
--rw-r--r--   0 rider     (1000) rider     (1000)     3568 2024-05-01 16:21:34.000000 django-reportbroD-3.0/django_reportbroD/utils.py
--rw-r--r--   0 rider     (1000) rider     (1000)     3281 2024-04-15 01:49:12.000000 django-reportbroD-3.0/django_reportbroD/views.py
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-06 16:19:14.713086 django-reportbroD-3.0/django_reportbroD.egg-info/
--rw-r--r--   0 rider     (1000) rider     (1000)     3580 2024-05-06 16:19:14.000000 django-reportbroD-3.0/django_reportbroD.egg-info/PKG-INFO
--rw-r--r--   0 rider     (1000) rider     (1000)     7696 2024-05-06 16:19:14.000000 django-reportbroD-3.0/django_reportbroD.egg-info/SOURCES.txt
--rw-r--r--   0 rider     (1000) rider     (1000)        1 2024-05-06 16:19:14.000000 django-reportbroD-3.0/django_reportbroD.egg-info/dependency_links.txt
--rw-r--r--   0 rider     (1000) rider     (1000)       33 2024-05-06 16:19:14.000000 django-reportbroD-3.0/django_reportbroD.egg-info/requires.txt
--rw-r--r--   0 rider     (1000) rider     (1000)       18 2024-05-06 16:19:14.000000 django-reportbroD-3.0/django_reportbroD.egg-info/top_level.txt
--rw-r--r--   0 rider     (1000) rider     (1000)     1177 2024-05-06 16:19:14.833087 django-reportbroD-3.0/setup.cfg
--rw-r--r--   0 rider     (1000) rider     (1000)       37 2024-02-21 17:28:39.000000 django-reportbroD-3.0/setup.py
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.977805 django-reportbroD-4.0/
+-rw-r--r--   0 rider     (1000) rider     (1000)      176 2024-05-22 11:02:56.000000 django-reportbroD-4.0/MANIFEST.in
+-rw-r--r--   0 rider     (1000) rider     (1000)     5861 2024-05-22 15:14:56.977805 django-reportbroD-4.0/PKG-INFO
+-rw-r--r--   0 rider     (1000) rider     (1000)     4803 2024-05-22 15:12:16.000000 django-reportbroD-4.0/README.md
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.894470 django-reportbroD-4.0/django_reportbroD/
+-rw-r--r--   0 rider     (1000) rider     (1000)        0 2024-02-16 20:55:14.000000 django-reportbroD-4.0/django_reportbroD/__init__.py
+-rw-r--r--   0 rider     (1000) rider     (1000)      164 2024-02-18 03:27:34.000000 django-reportbroD-4.0/django_reportbroD/admin.py
+-rw-r--r--   0 rider     (1000) rider     (1000)      189 2024-05-20 13:44:27.000000 django-reportbroD-4.0/django_reportbroD/apps.py
+-rw-r--r--   0 rider     (1000) rider     (1000)      803 2024-05-01 16:21:02.000000 django-reportbroD-4.0/django_reportbroD/base.py
+-rw-r--r--   0 rider     (1000) rider     (1000)      865 2024-05-17 14:51:48.000000 django-reportbroD-4.0/django_reportbroD/forms.py
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.887803 django-reportbroD-4.0/django_reportbroD/locale/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.887803 django-reportbroD-4.0/django_reportbroD/locale/en/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.894470 django-reportbroD-4.0/django_reportbroD/locale/en/LC_MESSAGES/
+-rw-r--r--   0 rider     (1000) rider     (1000)     9709 2024-05-22 11:17:28.000000 django-reportbroD-4.0/django_reportbroD/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 rider     (1000) rider     (1000)     9997 2024-05-22 11:17:28.000000 django-reportbroD-4.0/django_reportbroD/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.887803 django-reportbroD-4.0/django_reportbroD/locale/es/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.894470 django-reportbroD-4.0/django_reportbroD/locale/es/LC_MESSAGES/
+-rw-r--r--   0 rider     (1000) rider     (1000)    10561 2024-05-20 12:40:39.000000 django-reportbroD-4.0/django_reportbroD/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 rider     (1000) rider     (1000)    10852 2024-05-19 00:43:40.000000 django-reportbroD-4.0/django_reportbroD/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0 rider     (1000) rider     (1000)     1123 2024-05-19 02:27:08.000000 django-reportbroD-4.0/django_reportbroD/menus.py
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.897803 django-reportbroD-4.0/django_reportbroD/migrations/
+-rw-r--r--   0 rider     (1000) rider     (1000)     1737 2024-05-15 13:06:40.000000 django-reportbroD-4.0/django_reportbroD/migrations/0001_initial.py
+-rw-r--r--   0 rider     (1000) rider     (1000)        0 2024-02-16 20:55:14.000000 django-reportbroD-4.0/django_reportbroD/migrations/__init__.py
+-rw-r--r--   0 rider     (1000) rider     (1000)     1883 2024-05-13 14:18:14.000000 django-reportbroD-4.0/django_reportbroD/models.py
+-rw-r--r--   0 rider     (1000) rider     (1000)    13459 2024-05-09 20:40:36.000000 django-reportbroD-4.0/django_reportbroD/reportcore.py
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.887803 django-reportbroD-4.0/django_reportbroD/static/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.887803 django-reportbroD-4.0/django_reportbroD/static/assets/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.897803 django-reportbroD-4.0/django_reportbroD/static/assets/css/
+-rw-r--r--   0 rider     (1000) rider     (1000)     1772 2019-03-30 20:18:02.000000 django-reportbroD-4.0/django_reportbroD/static/assets/css/mCSB_buttons.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     1772 2019-03-30 20:18:02.000000 django-reportbroD-4.0/django_reportbroD/static/assets/css/owl.video.play.html
+-rw-r--r--   0 rider     (1000) rider     (1000)   509223 2019-03-30 20:18:10.000000 django-reportbroD-4.0/django_reportbroD/static/assets/css/style.css
+-rw-r--r--   0 rider     (1000) rider     (1000)   236692 2024-05-05 16:55:58.000000 django-reportbroD-4.0/django_reportbroD/static/assets/css/vendors.css
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.931137 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/
+-rw-r--r--   0 rider     (1000) rider     (1000)    62984 2019-03-30 20:18:20.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    24288 2019-03-30 20:18:20.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.html
+-rw-r--r--   0 rider     (1000) rider     (1000)   351196 2019-03-30 20:18:20.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    62768 2019-03-30 20:18:20.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    31064 2019-03-30 20:18:20.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    62984 2019-03-30 20:18:20.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-iconsd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    41808 2019-03-30 20:18:22.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    16604 2019-03-30 20:18:22.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.html
+-rw-r--r--   0 rider     (1000) rider     (1000)   163862 2019-03-30 20:18:22.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    41636 2019-03-30 20:18:22.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    20528 2019-03-30 20:18:22.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    41808 2019-03-30 20:18:22.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashiconsd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    40522 2019-03-30 20:18:22.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripicons.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    99368 2019-03-30 20:18:22.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripicons.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    40348 2019-03-30 20:18:22.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripicons.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    26004 2019-03-30 20:18:24.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripicons.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    40522 2019-03-30 20:18:24.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripiconsd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    62084 2019-03-30 20:18:24.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/feather.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)   213926 2019-03-30 20:18:26.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/feather.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    61920 2019-03-30 20:18:24.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/feather.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    29500 2019-03-30 20:18:24.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/feather.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    62084 2019-03-30 20:18:24.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/featherd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)   165742 2019-03-30 20:18:26.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    77159 2019-03-30 20:18:26.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.html
+-rw-r--r--   0 rider     (1000) rider     (1000)   444379 2019-03-30 20:18:28.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)   165548 2019-03-30 20:18:28.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    98024 2019-03-30 20:18:26.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)   165742 2019-03-30 20:18:28.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesomed41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)   144114 2019-03-30 20:18:28.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    61020 2019-03-30 20:18:28.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.html
+-rw-r--r--   0 rider     (1000) rider     (1000)   400219 2019-03-30 20:18:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)   143936 2019-03-30 20:18:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    80356 2019-03-30 20:18:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)   144114 2019-03-30 20:18:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ioniconsd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    21514 2019-03-30 20:18:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weather.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    48132 2019-03-30 20:18:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weather.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    21308 2019-03-30 20:18:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weather.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)     7936 2019-03-30 20:18:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weather.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    21514 2019-03-30 20:18:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weatherd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    42495 2019-03-30 20:18:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    38383 2019-03-30 20:18:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.html
+-rw-r--r--   0 rider     (1000) rider     (1000)   238287 2019-03-30 20:18:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    99212 2019-03-30 20:18:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    50312 2019-03-30 20:18:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    42495 2019-03-30 20:18:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-iconsd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    16746 2019-03-30 20:18:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/summernotec360.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    16560 2019-03-30 20:18:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/summernotec360.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    10324 2019-03-30 20:18:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/summernotec360.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    78748 2019-03-30 20:18:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-icons.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)   234269 2019-03-30 20:18:36.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-icons.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    78584 2019-03-30 20:18:36.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-icons.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    56108 2019-03-30 20:18:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-icons.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    78748 2019-03-30 20:18:36.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-iconsd41d.eot
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.931137 django-reportbroD-4.0/django_reportbroD/static/assets/img/
+-rw-r--r--   0 rider     (1000) rider     (1000)    39361 2019-03-30 21:07:44.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/02.jpg
+-rw-r--r--   0 rider     (1000) rider     (1000)    29789 2024-05-13 15:49:44.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/eeuu.png
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.934471 django-reportbroD-4.0/django_reportbroD/static/assets/img/export/
+-rw-r--r--   0 rider     (1000) rider     (1000)     1876 2019-03-30 21:07:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/export/csv.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)     1348 2019-03-30 21:07:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/export/txt.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)     2060 2019-03-30 21:07:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/export/xlsx.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    48878 2024-02-21 14:09:26.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/favicon.ico
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.937804 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/
+-rw-r--r--   0 rider     (1000) rider     (1000)     1182 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/ai.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1380 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/css.png
+-rw-r--r--   0 rider     (1000) rider     (1000)      948 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/dbf.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1383 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/doc.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1215 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/dwg.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1269 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/exe.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1006 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/html.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1364 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/jpg.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1399 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/pdf.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1397 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/png.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1430 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/psd.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     6359 2024-04-14 18:02:54.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/reporte.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1005 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/rtf.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1421 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/svg.png
+-rw-r--r--   0 rider     (1000) rider     (1000)      974 2019-03-30 21:07:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/xls.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1332 2019-03-30 21:07:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/xml.png
+-rw-r--r--   0 rider     (1000) rider     (1000)      997 2019-03-30 21:07:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/zip.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     7446 2024-03-09 16:12:06.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/lista.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     4814 2024-02-21 13:55:04.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/logo-icon.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     2422 2019-03-30 20:18:36.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/logo-light.png
+-rw-r--r--   0 rider     (1000) rider     (1000)    13606 2024-02-21 13:43:58.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/logo.png
+-rw-r--r--   0 rider     (1000) rider     (1000)    28535 2024-05-13 15:49:44.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/spain.png
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.937804 django-reportbroD-4.0/django_reportbroD/static/assets/js/
+-rw-r--r--   0 rider     (1000) rider     (1000)   576312 2019-03-30 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/assets/js/app.js
+-rw-r--r--   0 rider     (1000) rider     (1000)  8320860 2019-03-30 20:19:02.000000 django-reportbroD-4.0/django_reportbroD/static/assets/js/vendors.js
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.961138 django-reportbroD-4.0/django_reportbroD/static/reportlib/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.964471 django-reportbroD-4.0/django_reportbroD/static/reportlib/css/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.964471 django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.964471 django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/
+-rw-r--r--   0 rider     (1000) rider     (1000)     1633 2024-02-14 15:51:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)     1384 2024-02-14 15:51:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)     1460 2024-02-14 15:51:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)      684 2024-02-14 15:51:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff2
+-rw-r--r--   0 rider     (1000) rider     (1000)      855 2024-02-14 15:51:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/style.css
+-rw-r--r--   0 rider     (1000) rider     (1000)     4509 2024-02-21 21:05:40.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/css/styles.css
+-rw-r--r--   0 rider     (1000) rider     (1000)     2238 2024-02-14 15:51:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/favicon.ico
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.964471 django-reportbroD-4.0/django_reportbroD/static/reportlib/js/
+-rw-r--r--   0 rider     (1000) rider     (1000)   288580 2024-02-14 15:51:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.js
+-rw-r--r--   0 rider     (1000) rider     (1000)    89501 2024-02-14 15:51:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.min.js
+-rw-r--r--   0 rider     (1000) rider     (1000)     3121 2024-02-14 15:51:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/js/jquery.cookie.js
+-rw-r--r--   0 rider     (1000) rider     (1000)    55398 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.css
+-rw-r--r--   0 rider     (1000) rider     (1000)    77644 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.css.map
+-rw-r--r--   0 rider     (1000) rider     (1000)   733475 2024-05-18 23:36:56.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.js
+-rw-r--r--   0 rider     (1000) rider     (1000)      665 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.js.LICENSE.txt
+-rw-r--r--   0 rider     (1000) rider     (1000)  2440768 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.js.map
+-rw-r--r--   0 rider     (1000) rider     (1000)   722287 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.min.js
+-rw-r--r--   0 rider     (1000) rider     (1000)   803864 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.min.js.map
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.967804 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/
+-rw-r--r--   0 rider     (1000) rider     (1000)    24374 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/ajaxload.gif
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.971138 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/
+-rw-r--r--   0 rider     (1000) rider     (1000)    20756 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    16748 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff2
+-rw-r--r--   0 rider     (1000) rider     (1000)    20672 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    16756 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff2
+-rw-r--r--   0 rider     (1000) rider     (1000)    20664 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    16696 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff2
+-rw-r--r--   0 rider     (1000) rider     (1000)    20712 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    16740 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff2
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.971138 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/iconfonts/
+-rw-r--r--   0 rider     (1000) rider     (1000)    37788 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    12676 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    12752 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)     4460 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff2
+-rw-r--r--   0 rider     (1000) rider     (1000)    12924 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/rb_logo_dark.png
+-rw-r--r--   0 rider     (1000) rider     (1000)    13606 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/rb_logo_white.png
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.974471 django-reportbroD-4.0/django_reportbroD/templates/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.977805 django-reportbroD-4.0/django_reportbroD/templates/bases/
+-rw-r--r--   0 rider     (1000) rider     (1000)     1942 2024-05-16 14:15:12.000000 django-reportbroD-4.0/django_reportbroD/templates/bases/base.html
+-rw-r--r--   0 rider     (1000) rider     (1000)      352 2024-04-15 00:52:16.000000 django-reportbroD-4.0/django_reportbroD/templates/bases/footer.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     3916 2024-05-19 02:26:34.000000 django-reportbroD-4.0/django_reportbroD/templates/bases/header.html
+-rw-r--r--   0 rider     (1000) rider     (1000)      677 2024-05-19 00:25:08.000000 django-reportbroD-4.0/django_reportbroD/templates/bases/navigator.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     1926 2024-05-17 14:02:34.000000 django-reportbroD-4.0/django_reportbroD/templates/create.html
+-rw-r--r--   0 rider     (1000) rider     (1000)    16761 2024-05-16 15:46:40.000000 django-reportbroD-4.0/django_reportbroD/templates/document.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     2157 2024-05-17 14:00:38.000000 django-reportbroD-4.0/django_reportbroD/templates/edit.html
+-rw-r--r--   0 rider     (1000) rider     (1000)    21051 2024-05-17 13:57:14.000000 django-reportbroD-4.0/django_reportbroD/templates/especif.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     1192 2024-05-17 14:18:06.000000 django-reportbroD-4.0/django_reportbroD/templates/formulario.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     3102 2024-05-17 14:04:22.000000 django-reportbroD-4.0/django_reportbroD/templates/import.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     8884 2024-05-13 14:01:34.000000 django-reportbroD-4.0/django_reportbroD/templates/index.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     6199 2024-05-20 13:21:45.000000 django-reportbroD-4.0/django_reportbroD/templates/report.html
+-rw-r--r--   0 rider     (1000) rider     (1000)      756 2024-05-20 12:15:37.000000 django-reportbroD-4.0/django_reportbroD/urls.py
+-rw-r--r--   0 rider     (1000) rider     (1000)     4621 2024-05-12 18:19:58.000000 django-reportbroD-4.0/django_reportbroD/utils.py
+-rw-r--r--   0 rider     (1000) rider     (1000)     3258 2024-05-16 12:47:16.000000 django-reportbroD-4.0/django_reportbroD/views.py
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.894470 django-reportbroD-4.0/django_reportbroD.egg-info/
+-rw-r--r--   0 rider     (1000) rider     (1000)     5861 2024-05-22 15:14:56.000000 django-reportbroD-4.0/django_reportbroD.egg-info/PKG-INFO
+-rw-r--r--   0 rider     (1000) rider     (1000)     8032 2024-05-22 15:14:56.000000 django-reportbroD-4.0/django_reportbroD.egg-info/SOURCES.txt
+-rw-r--r--   0 rider     (1000) rider     (1000)        1 2024-05-22 15:14:56.000000 django-reportbroD-4.0/django_reportbroD.egg-info/dependency_links.txt
+-rw-r--r--   0 rider     (1000) rider     (1000)       33 2024-05-22 15:14:56.000000 django-reportbroD-4.0/django_reportbroD.egg-info/requires.txt
+-rw-r--r--   0 rider     (1000) rider     (1000)       18 2024-05-22 15:14:56.000000 django-reportbroD-4.0/django_reportbroD.egg-info/top_level.txt
+-rw-r--r--   0 rider     (1000) rider     (1000)     1177 2024-05-22 15:14:56.977805 django-reportbroD-4.0/setup.cfg
+-rw-r--r--   0 rider     (1000) rider     (1000)       37 2024-02-21 17:28:39.000000 django-reportbroD-4.0/setup.py
```

### Comparing `django-reportbroD-3.0/PKG-INFO` & `django-reportbroD-4.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,67 @@
-Metadata-Version: 2.1
-Name: django-reportbroD
-Version: 3.0
-Summary: A Django app to create and use ReportBro reports with a sample admin. This allows you to generate yours reports using three options: by its code or name from database or JSON template.
-Author: Rider Raul Espinosa Perez
-Author-email: riderraule@gmail.com
-License: MIT
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 5.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # django-reportbroD
-A Django app to create and use ReportBro reports with a sample admin.
+A Django app to create, use and export ReportBro reports (free version) with a admin. 
+
+![Django](https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white) ![lib](https://badgen.net/badge/Export/PDF-XLSX/red?) ![JS](https://badgen.net/badge/Js/Reportbro_Designer/blue?icon=doc)  ![lib](https://badgen.net/badge/Package/Reportbro-lib/red?icon=doc)
 
 Quick start
 -----------
 
-1. Add "reportbroD" to your INSTALLED_APPS setting like this:
+1. Add "django_reportbroD" to your INSTALLED_APPS setting like this:
 ```
     INSTALLED_APPS = [
    
                 ... ,
    'django_reportbroD.apps.ReportbrodConfig',
 
    ]
 
 ```
-2. Add 'django_reportbroD.menus.get_menu_items' to your OPTIONS.context_processors in your TEMPLATES settings. This enables the use of menu for the installed report app. 
+2. Add LocaleMiddleware to your MIDDLEWARE list in your settings. This allows the reporting app to have translation in Spanish and English. 
+ ```
+        MIDDLEWARE = [
+    'django.middleware.locale.LocaleMiddleware',
+    ...
+            ],
+            
+        
+```
+
+3. Add 'django_reportbroD.menus.get_menu_items' to your OPTIONS.context_processors in your TEMPLATES settings. This enables the use of menu for the installed report app. 
  ```
         'OPTIONS': {
    
             'context_processors': [...,
 'django_reportbroD.menus.get_menu_items'
    
             ],
             
         }
 ```
 
-3. Include the reportbroD URLconf in your project urls.py like this:
+4. Include the reportbroD URLconf in your project urls.py and the i18n urls like this:
+
+```
+   path("reportbroD/", include("django_reportbroD.urls" namespace="reportbroD")),  
+   path('i18n/', include('django.conf.urls.i18n')),
+```
 
-   path("reportbroD/", include("django_reportbroD.urls", namespace="reportbroD")),
 
-4. Run ``python manage.py migrate reportbroD`` to create the models and to migrating to data base.
+5.  Run ``python manage.py migrate`` to create the models and to migrating to data base.
 
-5. Start the development server.
+6. Start the development server.
 
-6. Visit the ``/reportbroD/`` URL to create/update/edit/duplicate/remove reports.
+7. Visit the ``/reportbroD/`` URL to create/update/edit/duplicate/remove reports.
 
 
 Using report
 -----------
 
 1. Create a app to using the view file or other file .py for defining the view function to show/export selected report
- ```
+ ```   
   from django_reportbroD.utils import convert_to_base64, convert_list_to_dict, to_dict, export_report_by_code, export_report_by_name, export_report_from_JSON
   
    def generar_pdf(request):
    
      products=Product.objects.all()
    
      #converting in a dictionary
@@ -119,7 +111,70 @@
     }
    
 
      return export_report_from_JSON(path_json="reporte.json", data=data, extension="xlsx")
  
    ```
 
+
+2. Include a report into Django Admin through a action function.
+
+```
+
+# admin.py 
+from .views import reporte
+...
+
+def reportbro(modeladmin, request, queryset):
+    w=queryset.first()
+    if w:
+        return reporte(request, w.code)
+
+reportbro.short_description="Working Report"
+
+@admin.register(Working)
+class WorkAdmin(admin.ModelAdmin):
+    list_display = ("worker","date", "hours","payhorary", "descount", "pay_extra", "pay" )
+    list_filter=["date", "worker"]
+    list_display_links = ("worker","date" )
+    actions=[reportbro]
+```
+
+> **Parameter >>** **download = True**
+>
+>In this case,  download parameter from export_report_by_code, export_report_by_name and export_report_from_JSON functions must be "True" to avoid any errors when the report format is "pdf".
+
+```
+#views.py 
+from django_reportbroD.utils import convert_to_base64, convert_list_to_dict, to_dict, export_report_by_code, export_report_by_name, export_report_from_JSON
+  ...
+
+def reporte(request, code):
+
+    worker=Worker.objects.filter(code=code).first()
+    workings=Working.objects.filter(worker=worker)
+    
+    asistencia= [
+{
+    "date": w.date.date,
+    "payhorary" : w.payhorary,
+    "descount" : w.descount,
+    "pay_extra" : w.pay_extra,
+    "pay" : w.pay,
+    
+    }
+for w in workings
+    ]
+
+    trabajador=to_dict(worker)
+    trabajador["horary"]=worker.horary.horario()
+    trabajador["area"]=worker.area.Area()
+
+
+    data={
+        "worker":trabajador,
+        "working": asistencia,
+        "date":datetime.datetime.now()
+    }
+
+    return export_report_by_code(template_code=7, data=data, file="nuevo", download=True)
+```
```

### Comparing `django-reportbroD-3.0/django_reportbroD/base.py` & `django-reportbroD-4.0/django_reportbroD/base.py`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/menus.py` & `django-reportbroD-4.0/django_reportbroD/menus.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 from django.urls import reverse
 
+from django.utils.translation import gettext as _
+
 
 def get_menu_items(request):
     """Returns application menu items with special class for active menu item."""
     return {
       "active_page":"reportlist",
       "menu": ( {'url': reverse('reportbroD:list'), 'label': "ReportBro Admin",
         'icon': "nav-icon ti ti-pencil-alt",  'id':'reportlist' },
         
-        {'url': reverse('reportbroD:docs'), 'label': "Documentación de ReportBro Admin ",
+        {'url': reverse('reportbroD:docs'), 'label': _("opt1"),
         'icon': "nav-icon ti ti-comment-alt",  'id':  'reportdocs' },
         
-         {'url': 'https://www.reportbro.com/doc/tutorial', 'label': "Tutorial de ReportBro Designer",
+         {'url': 'https://www.reportbro.com/doc/tutorial', 'label': _("opt2"),
         'icon': "nav-icon fa fa-book",  'id': 'reportbro' },
         
-         {'url': reverse('admin:index'), 'label': "Administración del Sitio",
+         {'url': reverse('admin:index'), 'label': _("opt3"),
         'icon': "nav-icon fa fa-users",  'id': 'admin' },
         
-         {'url': '/', 'label': "Inicio",
+         {'url': '/', 'label': _("opt4"),
         'icon': "nav-icon ti ti-rocket",  'id': 'home'}
-         )
+         ),
+         
+        "reportbro_langs": (  
+    {"code":"es", "name_local":"Español"},
+     {"code":"en", "name_local":"English"} 
+              )
+
          }
```

### Comparing `django-reportbroD-3.0/django_reportbroD/models.py` & `django-reportbroD-4.0/django_reportbroD/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django.db import models
 from datetime import datetime
 import json
+from django.utils.translation import gettext as _
 
 
 
 
 # store report requests for testing, used by ReportBro Designer
 # for preview of pdf and xlsx
 class ReportRequest(models.Model):
@@ -27,15 +28,15 @@
     report_definition = models.TextField(default=json.dumps(""))
     name = models.CharField(max_length=200, unique=True, verbose_name="Nombre")
     remark = models.TextField(null=True, blank=True, verbose_name="Descripción")
     last_modified_at = models.DateTimeField(default=datetime.now())
 
     def unique_error_message(self, model_class, unique_check):
         if model_class == type(self) and unique_check == ("name",):
-            return 'Ya existe un reporte con el mismo nombre.'
+            return _("unique")
         else:
             return super(ReportDefinition, self).unique_error_message(model_class, unique_check)
 
     class Meta:
         db_table = 'report_definition'
         verbose_name='Reporte'
         verbose_name_plural='Reportes'
```

### Comparing `django-reportbroD-3.0/django_reportbroD/reportcore.py` & `django-reportbroD-4.0/django_reportbroD/reportcore.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,61 +218,60 @@
             report_definition=report_definition, 
             last_modified_at=now)
     return HttpResponse('ok')
 
 
 
 
-def reportPDF(report_definition, data, file="reporte"):
+def reportPDF(report_definition, data, file="reporte", download=False):
     """Prints a pdf file with the available data. 
 
     """
     # if ReportDefinition.objects.filter(pk=code)== None:
     #     create_base_report_template(code)
     
-
-    
+#attachment
+    view_mode="attachment" if download else "inline"
     try:
         report_inst = Report(json.loads(report_definition), data)
         
         if report_inst.errors:
             # report definition should never contain any errors,
             # unless you saved an invalid report and didn't test in ReportBro Designer
             raise ReportBroError(report_inst.errors[0])
         
         pdf_report = report_inst.generate_pdf()
 
         response = HttpResponse(bytes(pdf_report), content_type='application/pdf')
-        response['Content-Disposition'] = 'inline; filename="{filename}"'.format(filename=f"{file}.pdf")
+        response['Content-Disposition'] = '{view_mode}; filename="{filename}"'.format(filename=f"{file}.pdf", view_mode=view_mode)
         
         return response
     except ReportBroError as ex:
         return HttpResponseServerError('report error: ' + str(ex.error))
     except Exception as ex:
         return HttpResponseServerError('report exception: ' + str(ex))
     
 
 
-def reportXLSX(report_definition, data, file="reporte" ):
+def reportXLSX(report_definition, data, file="reporte"):
     """Prints a xlsx file with the available data. 
 
     """
     # if ReportDefinition.objects.filter(pk=code)== None:
     #     create_base_report_template(code)
-    
     try:
         report_inst = Report(json.loads(report_definition), data)
         
         if report_inst.errors:
             # report definition should never contain any errors,
             # unless you saved an invalid report and didn't test in ReportBro Designer
             raise ReportBroError(report_inst.errors[0])
         
         pdf_report = report_inst.generate_xlsx()
         
         response = HttpResponse(bytes(pdf_report), content_type='application/xlsx')
-        response['Content-Disposition'] = 'inline; filename="{filename}"'.format(filename=f"{file}.xlsx")
+        response['Content-Disposition'] = 'inline ; filename="{filename}"'.format(filename=f"{file}.xlsx")
         return response
     except ReportBroError as ex:
         return HttpResponseServerError('report error: ' + str(ex.error))
     except Exception as ex:
         return HttpResponseServerError('report exception: ' + str(ex))
```

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/css/mCSB_buttons.html` & `django-reportbroD-4.0/django_reportbroD/static/assets/css/mCSB_buttons.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/css/owl.video.play.html` & `django-reportbroD-4.0/django_reportbroD/static/assets/css/owl.video.play.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/css/style.css` & `django-reportbroD-4.0/django_reportbroD/static/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/css/vendors.css` & `django-reportbroD-4.0/django_reportbroD/static/assets/css/vendors.css`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.html` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.svg` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.ttf` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.woff` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/cryptocurrency-iconsd41d.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-iconsd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.html` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.svg` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.ttf` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashicons.woff` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dashiconsd41d.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashiconsd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripicons.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripicons.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripicons.svg` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripicons.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripicons.ttf` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripicons.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripicons.woff` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripicons.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/dripiconsd41d.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripiconsd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/feather.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/feather.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/feather.svg` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/feather.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/feather.ttf` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/feather.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/feather.woff` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/feather.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/featherd41d.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/featherd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.html` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.svg` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.ttf` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesome.woff` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/font-awesomed41d.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesomed41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.html` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.svg` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.ttf` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ionicons.woff` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/ioniconsd41d.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ioniconsd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weather.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weather.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weather.svg` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weather.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weather.ttf` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weather.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weather.woff` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weather.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/linea-weatherd41d.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weatherd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.html` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.svg` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.ttf` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-icons.woff` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/material-iconsd41d.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-iconsd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/summernotec360.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/summernotec360.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/summernotec360.ttf` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/summernotec360.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/summernotec360.woff` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/summernotec360.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-icons.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-icons.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-icons.svg` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-icons.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-icons.ttf` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-icons.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-icons.woff` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-icons.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/fonts/themify-iconsd41d.eot` & `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-iconsd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/02.jpg` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/02.jpg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/export/csv.svg` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/export/csv.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/export/txt.svg` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/export/txt.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/export/xlsx.svg` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/export/xlsx.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/favicon.ico` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/ai.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/ai.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/css.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/css.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/dbf.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/dbf.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/doc.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/doc.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/dwg.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/dwg.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/exe.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/exe.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/html.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/html.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/jpg.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/jpg.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/pdf.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/pdf.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/png.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/png.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/psd.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/psd.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/reporte.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/reporte.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/rtf.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/rtf.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/svg.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/svg.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/xls.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/xls.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/xml.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/xml.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/file-icon/zip.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/zip.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/lista.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/lista.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/logo-icon.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/logo-icon.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/logo-light.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/logo-light.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/img/logo.png` & `django-reportbroD-4.0/django_reportbroD/static/assets/img/logo.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/js/app.js` & `django-reportbroD-4.0/django_reportbroD/static/assets/js/app.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/assets/js/vendors.js` & `django-reportbroD-4.0/django_reportbroD/static/assets/js/vendors.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.svg` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.ttf` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff2` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff2`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/css/iconfonts/style.css` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/style.css`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/css/styles.css` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/css/styles.css`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/favicon.ico` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.js` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.min.js` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/js/jquery.cookie.js` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/js/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.css` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.css`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.css.map` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.css.map`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.js` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.js.LICENSE.txt` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.js.map` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.js.map`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.min.js` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.min.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/reportbro.min.js.map` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.min.js.map`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/ajaxload.gif` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/ajaxload.gif`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff2` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff2` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff2`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff2` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff2`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff2` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.svg` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.ttf` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff2` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff2`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/rb_logo_dark.png` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/rb_logo_dark.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/static/reportlib/src/rb_logo_white.png` & `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/rb_logo_white.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-3.0/django_reportbroD/templates/bases/base.html` & `django-reportbroD-4.0/django_reportbroD/templates/bases/base.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 {% load static %}
+{% load i18n %} 
 <!DOCTYPE html>
 <html lang="en">
 
 
 <head>
 	<title>
 		{% block title %}
-		Listado de Reportes
+		{% trans "app" %}
 		{% endblock %}
 
 	</title>
 	<meta charset="utf-8" />
 	<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1" />
 	<meta name="description" content="Admin template that can be used to build dashboards for CRM, CMS, etc." />
 	<meta name="author" content="Potenza Global Solutions" />
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
-{% load static %}
+{% load static %} {% load i18n %}
 {% block config%}
 {% endblock %} {% block configr%} {% endblock %}
 {% block header %} {% include 'bases/header.html' %} {% endblock %}
 {% block navigator %} {% include 'bases/navigator.html' %} {% endblock %} {%
 block content %} Contenido {% endblock %}
 {% block footer %} {% include 'bases/footer.html' %} {% endblock %}
```

### Comparing `django-reportbroD-3.0/django_reportbroD/templates/bases/navigator.html` & `django-reportbroD-4.0/django_reportbroD/templates/bases/navigator.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+{% load i18n %} 
+
 <aside class="app-navbar">
     <!-- begin sidebar-nav -->
     <div class="sidebar-nav scrollbar scroll_light">
         <ul class="metismenu " id="sidebarNav">
-            <li class="nav-static-title">Opciones principales</li>
+            <li class="nav-static-title">{% trans "options" %}</li>
 
  {% for elem in menu %}
  <li 
     {% if active_page == elem.id %}
     class="active"
   
     {% endif %}
@@ -24,10 +26,11 @@
        
         {% endfor %}
           
 
 
 
         </ul>
+
     </div>
     <!-- end sidebar-nav -->
 </aside>
```

### Comparing `django-reportbroD-3.0/django_reportbroD/templates/create.html` & `django-reportbroD-4.0/django_reportbroD/templates/create.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 {% extends 'bases/base.html'%}
 {% load static %}
+{% load i18n %} 
 
 {% block title %}
-		Creando Reporte
+		{% trans "title_add1" %}
 		{% endblock %}
 
 {% block content %}
 <div class="app-main" id="main">
     <!-- begin container-fluid -->
     <div class="container-fluid">
         <!-- begin row -->
         <div class="row">
             <div class="col-md-12 m-b-30">
                 <!-- begin page title -->
                 <div class="d-block d-sm-flex flex-nowrap align-items-center">
                     <div class="page-title mb-2 mb-sm-0">
-                        <h1>Registro de nuevo Reporte</h1>
+                        <h1>{% trans "title_add" %}</h1>
                     </div>
                     <div class="ml-auto d-flex align-items-center">
                         <nav>
                             <ol class="breadcrumb p-0 m-b-0">
                                 <li class="breadcrumb-item">
                                     <a href="/"><i class="ti ti-home"></i></a>
                                 </li>
                                 <li class="breadcrumb-item">
-                                    <a href="{% url 'reportbroD:list' %}">Administración de Reportes</a> 
+                                    <a href="{% url 'reportbroD:list' %}">{% trans "app" %}</a> 
                                 </li>
-                                <li class="breadcrumb-item active text-primary" aria-current="page">Nuevo</li>
+                                <li class="breadcrumb-item active text-primary" aria-current="page">{% trans 'subtitle_add' %}</li>
                             </ol>
                         </nav>
                     </div>
                 </div>
                 <!-- end page title -->
             </div>
         </div>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
-{% extends 'bases/base.html'%} {% load static %} {% block title %} Creando
-Reporte {% endblock %} {% block content %}
-************ RReeggiissttrroo ddee nnuueevvoo RReeppoorrttee ************
-   1. _A_d_m_i_n_i_s_t_r_a_c_i_Ã_³_n_ _d_e_ _R_e_p_o_r_t_e_s
-   2. Nuevo
+{% extends 'bases/base.html'%} {% load static %} {% load i18n %} {% block title
+%} {% trans "title_add1" %} {% endblock %} {% block content %}
+************ {{%% ttrraannss ""ttiittllee__aadddd"" %%}} ************
+   1. _{_%_ _t_r_a_n_s_ _"_a_p_p_"_ _%_}
+   2. {% trans 'subtitle_add' %}
 {% include 'formulario.html' %}
 {% endblock %}
```

### Comparing `django-reportbroD-3.0/django_reportbroD/templates/edit.html` & `django-reportbroD-4.0/django_reportbroD/templates/edit.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 {% extends 'bases/base.html'%}
 {% load static %}
+{% load i18n %} 
 
 {% block title %}
-		Editando Reporte
+		{% trans "title_edit" %}
 		{% endblock %}
 {% block content %}
 <div class="app-main" id="main">
     <!-- begin container-fluid -->
     <div class="container-fluid">
         <!-- begin row -->
         <div class="row">
             <div class="col-md-12 m-b-30">
                 <!-- begin page title -->
                 <div class="d-block d-sm-flex flex-nowrap align-items-center">
                     <div class="page-title mb-2 mb-sm-0">
-                        <h1>Editando Reporte</h1>
+                        <h1>{% trans "title_edit" %}</h1>
                     </div>
                     <div class="ml-auto d-flex align-items-center">
                         <nav>
                             <ol class="breadcrumb p-0 m-b-0">
                                 <li class="breadcrumb-item">
                                     <a href="/"><i class="ti ti-home"></i></a>
                                 </li>
                                 <li class="breadcrumb-item">
-                                    <a href="{% url 'reportbroD:list' %}">Administración de Reportes</a> 
+                                    <a href="{% url 'reportbroD:list' %}">{% trans "app" %}</a> 
                                 </li>
                                 <li class="breadcrumb-item active text-primary" aria-current="page">{{object.name}}</li>
                             </ol>
                         </nav>
                     </div>
                 </div>
                 <!-- end page title -->
@@ -36,15 +37,15 @@
         <!-- end row -->
         <!-- begin row -->
         <div class="row">
             <div class="col-xl-12">
                 <div class="card card-statistics">
                     <div class="card-header">
                         
-                        <a href="{% url 'reportbroD:template' reporte.id %}" class="btn btn-success" ><i class="zmdi zmdi-file-text"></i> Editar plantilla
+                        <a href="{% url 'reportbroD:template' reporte.id %}" class="btn btn-success" ><i class="zmdi zmdi-file-text"></i> {% trans "template_edit" %}
                         </a>     
                     </div>
      {% include 'formulario.html' %}
 
     </div>
 </div>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends 'bases/base.html'%} {% load static %} {% block title %} Editando
-Reporte {% endblock %} {% block content %}
-************ EEddiittaannddoo RReeppoorrttee ************
-   1. _A_d_m_i_n_i_s_t_r_a_c_i_Ã_³_n_ _d_e_ _R_e_p_o_r_t_e_s
+{% extends 'bases/base.html'%} {% load static %} {% load i18n %} {% block title
+%} {% trans "title_edit" %} {% endblock %} {% block content %}
+************ {{%% ttrraannss ""ttiittllee__eeddiitt"" %%}} ************
+   1. _{_%_ _t_r_a_n_s_ _"_a_p_p_"_ _%_}
    2. {{object.name}}
-_E_d_i_t_a_r_ _p_l_a_n_t_i_l_l_a
+_{_%_ _t_r_a_n_s_ _"_t_e_m_p_l_a_t_e___e_d_i_t_"_ _%_}
 {% include 'formulario.html' %}
 {% endblock %}
```

### Comparing `django-reportbroD-3.0/django_reportbroD/templates/formulario.html` & `django-reportbroD-4.0/django_reportbroD/templates/formulario.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 
+{% load i18n %} 
+            
             <div class="card-body">
                 <form method="post">
                     {% csrf_token %}
                     <div class="form-group">
-                        <label for="nombre">Nombre</label>
+                        <label for="nombre">{% trans "nameC" %}</label>
 
                         {{form.name}}
 
 
                         {% for error in form.name.errors %}
 
                         <div class="alert alert-danger alert-dismissible fade show" role="alert">
@@ -15,18 +17,18 @@
                             <button type="button" class="close" data-dismiss="alert" aria-label="Close">
                                 <i class="ti ti-close"></i>
                             </button>
                         </div>
                         {% endfor %}
                     </div>
                     <div class="form-group">
-                        <label for="desc">Descripción</label>
+                        <label for="desc">{% trans "descc" %}</label>
 
                         {{form.remark}}
 
                     </div>
 
-                    <button type="submit" class="btn btn-primary">Aceptar</button>
+                    <button type="submit" class="btn btn-primary">{% trans "btnok" %}</button>
                 </form>
                 
             </div>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-reportbroD-3.0/django_reportbroD/templates/import.html` & `django-reportbroD-4.0/django_reportbroD/templates/import.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 {% extends 'bases/base.html'%}
 {% load static %}
-
+{% load i18n %}
 {% block title %}
-		Importando Reporte
+	{% trans "title_import" %}
 		{% endblock %}
 
 {% block content %}
 <div class="app-main" id="main">
     <!-- begin container-fluid -->
     <div class="container-fluid">
         <!-- begin row -->
         <div class="row">
             <div class="col-md-12 m-b-30">
                 <!-- begin page title -->
                 <div class="d-block d-sm-flex flex-nowrap align-items-center">
                     <div class="page-title mb-2 mb-sm-0">
-                        <h1>Importando Reporte</h1>
+                        <h1>{% trans "title_edit" %}</h1>
                     </div>
                     <div class="ml-auto d-flex align-items-center">
                         <nav>
                             <ol class="breadcrumb p-0 m-b-0">
                                 <li class="breadcrumb-item">
                                     <a href="/"><i class="ti ti-home"></i></a>
                                 </li>
                                 <li class="breadcrumb-item">
-                                    <a href="{% url 'reportbroD:list' %}">Administración de Reportes</a> 
+                                    <a href="{% url 'reportbroD:list' %}">{% trans "app" %}</a> 
                                 </li>
-                                <li class="breadcrumb-item active text-primary" aria-current="page">Importar</li>
+                                <li class="breadcrumb-item active text-primary" aria-current="page">{% trans "title_import1" %}</li>
                             </ol>
                         </nav>
                     </div>
                 </div>
                 <!-- end page title -->
             </div>
         </div>
@@ -42,15 +42,15 @@
                     <div class="card-header">
         
                     </div>
                     <div class="card-body">
                         <form method="post" enctype="multipart/form-data">
                             {% csrf_token %}
                             <div class="form-group">
-                                <label for="nombre">{{form.template.label}} (Formato en JSON)</label>
+                                <label for="nombre">{% trans "especif" %}</label>
         
                                 {{form.template}}
         
         
                               
 
                             {% if error %}
@@ -62,15 +62,15 @@
                             </div>
 
                             {% endif %}
 
                             </div>
                            
         
-                            <button type="submit" class="btn btn-primary">Subir</button>
+                            <button type="submit" class="btn btn-primary">{% trans "btn_upload" %}</button>
                         </form>
                         
                     </div>
                
 
     </div>
 </div>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-{% extends 'bases/base.html'%} {% load static %} {% block title %} Importando
-Reporte {% endblock %} {% block content %}
-************ IImmppoorrttaannddoo RReeppoorrttee ************
-   1. _A_d_m_i_n_i_s_t_r_a_c_i_Ã_³_n_ _d_e_ _R_e_p_o_r_t_e_s
-   2. Importar
+{% extends 'bases/base.html'%} {% load static %} {% load i18n %} {% block title
+%} {% trans "title_import" %} {% endblock %} {% block content %}
+************ {{%% ttrraannss ""ttiittllee__eeddiitt"" %%}} ************
+   1. _{_%_ _t_r_a_n_s_ _"_a_p_p_"_ _%_}
+   2. {% trans "title_import1" %}
 {% csrf_token %}
-{{form.template.label}} (Formato en JSON) {{form.template}} {% if error %}
+{% trans "especif" %} {{form.template}} {% if error %}
 {{{{eerrrroorr}}}}
 {% endif %}
-Subir
+{% trans "btn_upload" %}
 {% endblock %}
```

### Comparing `django-reportbroD-3.0/django_reportbroD/urls.py` & `django-reportbroD-4.0/django_reportbroD/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from django.urls import path
+from django.urls import path, include
 from .views import *
 from  .reportcore import *
 
 app_name="reportbroD"
 urlpatterns = [
+ 
     path("", ReportList.as_view(), name="list"),
     path("create/", CreateReport.as_view(), name="create"),
      path("import/", importreport, name="import"),
  path("edit/<int:pk>", EditReport.as_view(), name="edit"),
     path("delete/<int:id>", deletereport, name="delete"),
      path("duplicate/<int:id>", duplicatereport, name="duplicate"),
      path("export/<int:id>", exportreport, name="exportation"),
     path("docs/", docs_view, name="docs"),
     path("template/<int:pk>/", edit, name="template"),
     path("run/", run, name="report_run"),
     path("save/<int:pk>/", save, name="report_save"),
 
 
-]
+]
```

### Comparing `django-reportbroD-3.0/django_reportbroD/utils.py` & `django-reportbroD-4.0/django_reportbroD/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 import json
 from .models import ReportDefinition
 from django.db import models
 from itertools import chain
 from django.http import HttpResponseServerError
 from .reportcore import reportPDF, reportXLSX
+from PIL import Image, ImageDraw, ImageOps
 
 
 
 
 def to_dict(instance):
     """Esta función permite convertir un objeto de tipo Model a un diccionario
     para que su información pueda ser pasada como parámetro a ReportBro"""
@@ -24,15 +25,14 @@
             if f.value_from_object(instance) is not None:
                 formato= f.value_from_object(instance).url.split(".")[-1]
                 data[f.name] = convert_to_base64(f.value_from_object(instance).url, formato)
             else:
                 data[f.name] = None
         else:
             data[f.name] = f.value_from_object(instance)
-   
     return data
 
 
 def convert_list_to_dict(listado):
     """Convierte una query o lista de elementos de la clase Model en un 
     diccionario entendible para ReportBro"""
 
@@ -43,63 +43,75 @@
 def convert_to_base64(path, format_image):
     """
     Nota: path se refiere a la ruta de la imagen y  format_image se refiere al fomato de la imagen (jpg, png, jpeg, etc)
     Este método permite convertir una imagen jpg o png a una imagen en base 64 
       para que ReportBro pueda renderizarla como parte de sus parámetros  """
     import base64
     from django.conf import settings
-    print(str(settings.BASE_DIR)+path)
     
     with open(str(settings.BASE_DIR)+path, "rb") as image_file:
         return f"data:image/{format_image};base64,{base64.b64encode(image_file.read()).decode('utf-8')}"
     
 
 
-def export_report_by_code(template_code, data, extension="pdf", file="reporte"):
-    """ Export a report using its code"""
+def export_report_by_code(template_code, data, extension="pdf", file="reporte", download=False):
+    """ Export a report using its code
+    view_mode: Its the way in the report pdf is going to download through the navegator. Two options:
+    1. download =False, (inline) >the pdf report is showed in the navegator and the user can download it handly or making print, etc.
+    2. download =True (attachment) >the pdf report is downloaded directly into pc
+    
+    """
     
     report = ReportDefinition.objects.filter(pk=template_code).first()
     
     if not report:
         return HttpResponseServerError('Este reporte no se encuentra disponible')
     
 
     if extension.lower() =="xlsx":
         return reportXLSX( report.report_definition, data, file)
     
-    return reportPDF( report.report_definition, data, file)
+    return reportPDF( report.report_definition, data, file, download)
 
 
 
-def export_report_by_name(template_name, data, extension="pdf", file="reporte"):
-    """ Export a report using its name"""
+def export_report_by_name(template_name, data, extension="pdf", file="reporte", download=False):
+    """ Export a report using its name
+    view_mode: Its the way in the report pdf is going to download through the navegator. Two options:
+    1. download =False, (inline) >the pdf report is showed in the navegator and the user can download it handly or making print, etc.
+    2. download =True (attachment) >the pdf report is downloaded directly into pc
+    """
 
     report = ReportDefinition.objects.filter(name=template_name).first()
     
     if not report:
         return HttpResponseServerError('Este reporte no se encuentra disponible')
 
 
     if extension.lower() =="xlsx":
         return reportXLSX(report.report_definition, data, file)
     
-    return reportPDF(report.report_definition, data, file)
+    return reportPDF(report.report_definition, data, file, download)
 
 
 
-def export_report_from_JSON(path_json, data, extension="pdf", file="reporte"):
-    """ Export a report using a JSON template report."""
+def export_report_from_JSON(path_json, data, extension="pdf", file="reporte", download=False):
+    """ Export a report using a JSON template report.
+    view_mode: Its the way in the report pdf is going to download through the navegator. Two options:
+    1. download =False, (inline) >the pdf report is showed in the navegator and the user can download it handly or making print, etc.
+    2. download =True (attachment) >the pdf report is downloaded directly into pc
+    """
     
     try:
         with open(path_json) as json_file:
             report = json.load(json_file)
     except FileNotFoundError :
         return HttpResponseServerError('La ruta especificada no contiene la plantilla.')
     except json.JSONDecodeError:
         return HttpResponseServerError('El fichero no tiene un formato adecuado.')
         
 
     if extension.lower() =="xlsx":
-        return reportXLSX(report["report_definition"], data, file)
+        return reportXLSX(report["report_definition"], data, file )
     
-    return reportPDF(report["report_definition"], data, file)
+    return reportPDF(report["report_definition"], data, file, download)
```

### Comparing `django-reportbroD-3.0/django_reportbroD/views.py` & `django-reportbroD-4.0/django_reportbroD/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Any
 from django.shortcuts import render, get_object_or_404, redirect
 from .models import ReportDefinition
 from django.views.generic import ListView, CreateView, UpdateView
 from .forms import ReportForm, ReportImpForm
 from django.urls import reverse_lazy
 from datetime import datetime
-from django.core.serializers import serialize
 from django.http import HttpResponse
 import json
+from django.utils.translation import gettext as _
 
 
 
 # Create your views here.
 
 def indexreport(request):
     return render (request, 'index.html')
@@ -92,15 +92,15 @@
                 namereport= file["name"] if ReportDefinition.objects.filter(name=file["name"]).first() is None else file["name"]+" "+actual.isoformat()
                 ReportDefinition.objects.create(
                  name=namereport,
                  report_definition=file["report_definition"],
                  remark=file ["remark"],  
                  last_modified_at=actual )
             except :
-                return render(request,"import.html",{"form":ReportImpForm(), "error":"El archivo no posee el formato adecuado."} )
+                return render(request,"import.html",{"form":ReportImpForm(), "error":_("not_format")} )
 
 
             return redirect("reportbroD:list")
         
     
     return render(request,"import.html",{"form":ReportImpForm()} )
```

### Comparing `django-reportbroD-3.0/django_reportbroD.egg-info/SOURCES.txt` & `django-reportbroD-4.0/django_reportbroD.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,19 @@
 django_reportbroD/utils.py
 django_reportbroD/views.py
 django_reportbroD.egg-info/PKG-INFO
 django_reportbroD.egg-info/SOURCES.txt
 django_reportbroD.egg-info/dependency_links.txt
 django_reportbroD.egg-info/requires.txt
 django_reportbroD.egg-info/top_level.txt
+django_reportbroD/locale/en/LC_MESSAGES/django.mo
+django_reportbroD/locale/en/LC_MESSAGES/django.po
+django_reportbroD/locale/es/LC_MESSAGES/django.mo
+django_reportbroD/locale/es/LC_MESSAGES/django.po
+django_reportbroD/migrations/0001_initial.py
 django_reportbroD/migrations/__init__.py
 django_reportbroD/static/assets/css/mCSB_buttons.html
 django_reportbroD/static/assets/css/owl.video.play.html
 django_reportbroD/static/assets/css/style.css
 django_reportbroD/static/assets/css/vendors.css
 django_reportbroD/static/assets/fonts/cryptocurrency-icons.eot
 django_reportbroD/static/assets/fonts/cryptocurrency-icons.html
@@ -73,19 +78,21 @@
 django_reportbroD/static/assets/fonts/summernotec360.woff
 django_reportbroD/static/assets/fonts/themify-icons.eot
 django_reportbroD/static/assets/fonts/themify-icons.svg
 django_reportbroD/static/assets/fonts/themify-icons.ttf
 django_reportbroD/static/assets/fonts/themify-icons.woff
 django_reportbroD/static/assets/fonts/themify-iconsd41d.eot
 django_reportbroD/static/assets/img/02.jpg
+django_reportbroD/static/assets/img/eeuu.png
 django_reportbroD/static/assets/img/favicon.ico
 django_reportbroD/static/assets/img/lista.png
 django_reportbroD/static/assets/img/logo-icon.png
 django_reportbroD/static/assets/img/logo-light.png
 django_reportbroD/static/assets/img/logo.png
+django_reportbroD/static/assets/img/spain.png
 django_reportbroD/static/assets/img/export/csv.svg
 django_reportbroD/static/assets/img/export/txt.svg
 django_reportbroD/static/assets/img/export/xlsx.svg
 django_reportbroD/static/assets/img/file-icon/ai.png
 django_reportbroD/static/assets/img/file-icon/css.png
 django_reportbroD/static/assets/img/file-icon/dbf.png
 django_reportbroD/static/assets/img/file-icon/doc.png
```

### Comparing `django-reportbroD-3.0/setup.cfg` & `django-reportbroD-4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-reportbroD
-version = 3.0
+version = 4.0
 description = A Django app to create and use ReportBro reports with a sample admin. This allows you to generate yours reports using three options: by its code or name from database or JSON template.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Rider Raul Espinosa Perez
 author_email = riderraule@gmail.com
 license = MIT
 classifiers =
```

