# Comparing `tmp/appier_extras-0.9.8.tar.gz` & `tmp/appier_extras-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/appier_extras-0.9.8.tar", last modified: Wed Apr 12 17:53:37 2017, max compression
+gzip compressed data, was "dist/appier_extras-0.9.9.tar", last modified: Wed Apr 12 18:31:40 2017, max compression
```

## Comparing `appier_extras-0.9.8.tar` & `appier_extras-0.9.9.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/models/
--rw-r--r--   0 travis    (1000) travis    (1000)     1617 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/models/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)    22588 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/models/account.py
--rw-r--r--   0 travis    (1000) travis    (1000)    16626 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/models/base.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2517 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/models/config.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4864 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/models/event.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3440 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/models/role.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4038 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/models/search.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5821 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/models/settings.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3047 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/models/snapshot.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/social/
--rw-r--r--   0 travis    (1000) travis    (1000)     1490 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/social/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3837 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/social/facebook_s.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3821 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/social/github_s.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4049 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/social/google_s.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3773 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/social/live_s.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4493 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/social/twitter_s.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/static/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/static/css/
--rw-r--r--   0 travis    (1000) travis    (1000)     3242 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/static/css/layout.css
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/static/images/
--rw-r--r--   0 travis    (1000) travis    (1000)      392 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/static/images/avatar_64.png
--rw-r--r--   0 travis    (1000) travis    (1000)      558 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/static/images/avatar_96.png
--rw-r--r--   0 travis    (1000) travis    (1000)     1150 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/static/images/favicon.ico
--rw-r--r--   0 travis    (1000) travis    (1000)      885 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/static/images/logo_96.png
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/static/js/
--rw-r--r--   0 travis    (1000) travis    (1000)     1049 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/static/js/main.js
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/email/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/email/account/
--rw-r--r--   0 travis    (1000) travis    (1000)      771 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/email/account/confirm.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     1888 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/email/account/new.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     1019 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/email/account/recover.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)      202 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/email/base.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     2332 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/email/layout.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     2482 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/email/macros.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     2129 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/email/test.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     2168 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/admin.fluid.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)      137 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/admin.simple.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)      266 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/admin.static.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     1626 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/bar.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)       71 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/content_type.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)       35 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/doctype.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)        9 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/end_doctype.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)      512 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/extras.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)      327 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/footer.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)       38 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/header.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     2174 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/includes.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)      414 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/layout.base.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     1966 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/layout.fluid.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     1190 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/layout.simple.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     1264 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/layout.static.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)    15586 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/macros.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)      204 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/message.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)      166 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/meta.html.tpl
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/account/
--rw-r--r--   0 travis    (1000) travis    (1000)     1828 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/account/new.html.tpl
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/database/
--rw-r--r--   0 travis    (1000) travis    (1000)     1251 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/database/import.html.tpl
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/entities/
--rw-r--r--   0 travis    (1000) travis    (1000)     1482 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/entities/edit.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     1180 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/entities/new.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     5255 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/entities/show.html.tpl
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/models/
--rw-r--r--   0 travis    (1000) travis    (1000)     1400 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/models/list.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     7686 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/models/show.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)      852 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/configs.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)      873 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/counters.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     1081 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/database.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)      391 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/done.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)      823 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/error.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)      858 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/libraries.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     1805 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/operations.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     1933 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/options.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)      845 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/parts.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     1070 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/recover.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     1216 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/reset.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     1323 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/routes.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     1210 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/session.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     1924 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/sessions.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     2003 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/signin.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     4683 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/social.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     5305 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/status.html.tpl
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/static/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/static/models/
--rw-r--r--   0 travis    (1000) travis    (1000)      368 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/static/models/list.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)      823 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/static/error.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     2003 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/templates/static/signin.html.tpl
--rw-r--r--   0 travis    (1000) travis    (1000)     1356 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)    52168 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/admin/part.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/static/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/static/fonts/
--rw-r--r--   0 travis    (1000) travis    (1000)    95380 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/static/fonts/aaaiight.ttf
--rw-r--r--   0 travis    (1000) travis    (1000)    46108 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/static/fonts/abscissa.ttf
--rw-r--r--   0 travis    (1000) travis    (1000)    53704 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/static/fonts/adler.ttf
--rw-r--r--   0 travis    (1000) travis    (1000)   774476 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/static/fonts/arial.ttf
--rw-r--r--   0 travis    (1000) travis    (1000)    20640 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/static/fonts/kbasalu.ttf
--rw-r--r--   0 travis    (1000) travis    (1000)    60748 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/static/fonts/knights_quest.ttf
--rw-r--r--   0 travis    (1000) travis    (1000)    21396 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/static/fonts/sevenbrg.ttf
--rw-r--r--   0 travis    (1000) travis    (1000)    16200 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/static/fonts/treasure_island.ttf
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/static/patterns/
--rw-r--r--   0 travis    (1000) travis    (1000)     1000 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/static/patterns/pattern_1.jpg
--rw-r--r--   0 travis    (1000) travis    (1000)     1103 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/static/patterns/pattern_2.jpg
--rw-r--r--   0 travis    (1000) travis    (1000)     1457 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/static/patterns/pattern_3.jpg
--rw-r--r--   0 travis    (1000) travis    (1000)     1024 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/static/patterns/pattern_4.jpg
--rw-r--r--   0 travis    (1000) travis    (1000)      935 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/static/patterns/pattern_5.jpg
--rw-r--r--   0 travis    (1000) travis    (1000)      959 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/static/patterns/pattern_6.jpg
--rw-r--r--   0 travis    (1000) travis    (1000)     1371 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/static/patterns/pattern_7.jpg
--rw-r--r--   0 travis    (1000) travis    (1000)     1268 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     7240 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/captcha/part.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/csfr/
--rw-r--r--   0 travis    (1000) travis    (1000)     1330 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/csfr/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2716 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/csfr/part.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2041 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/csfr/util.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/opbeat/
--rw-r--r--   0 travis    (1000) travis    (1000)     1267 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/opbeat/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4205 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/opbeat/part.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/parts/sematext/
--rw-r--r--   0 travis    (1000) travis    (1000)     1330 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/sematext/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4580 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/sematext/handler.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2844 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/sematext/part.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1531 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/parts/__init__.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/test/
--rw-r--r--   0 travis    (1000) travis    (1000)     1213 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/test/__init__.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras/utils/
--rw-r--r--   0 travis    (1000) travis    (1000)     1312 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/utils/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)    17025 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/utils/markdown.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1356 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1596 2017-04-12 17:53:11.000000 appier_extras-0.9.8/src/appier_extras/base.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)      997 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)     6359 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       63 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras.egg-info/entry_points.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-04-12 17:53:32.000000 appier_extras-0.9.8/src/appier_extras.egg-info/not-zip-safe
--rw-r--r--   0 travis    (1000) travis    (1000)        7 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       14 2017-04-12 17:53:37.000000 appier_extras-0.9.8/src/appier_extras.egg-info/top_level.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      665 2017-04-12 17:53:11.000000 appier_extras-0.9.8/MANIFEST.in
--rw-r--r--   0 travis    (1000) travis    (1000)     3698 2017-04-12 17:53:11.000000 appier_extras-0.9.8/setup.py
--rw-r--r--   0 travis    (1000) travis    (1000)      997 2017-04-12 17:53:37.000000 appier_extras-0.9.8/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)       88 2017-04-12 17:53:37.000000 appier_extras-0.9.8/setup.cfg
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/models/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1617 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/models/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    22588 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/models/account.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    16626 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/models/base.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2517 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/models/config.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4864 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/models/event.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3440 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/models/role.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4038 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/models/search.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5821 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/models/settings.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3047 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/models/snapshot.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/social/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1490 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/social/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3837 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/social/facebook_s.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3821 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/social/github_s.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4049 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/social/google_s.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3773 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/social/live_s.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4493 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/social/twitter_s.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/static/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/static/css/
+-rw-r--r--   0 travis    (1000) travis    (1000)     3242 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/static/css/layout.css
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/static/images/
+-rw-r--r--   0 travis    (1000) travis    (1000)      392 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/static/images/avatar_64.png
+-rw-r--r--   0 travis    (1000) travis    (1000)      558 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/static/images/avatar_96.png
+-rw-r--r--   0 travis    (1000) travis    (1000)     1150 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/static/images/favicon.ico
+-rw-r--r--   0 travis    (1000) travis    (1000)      885 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/static/images/logo_96.png
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/static/js/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1049 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/static/js/main.js
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/email/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/email/account/
+-rw-r--r--   0 travis    (1000) travis    (1000)      771 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/email/account/confirm.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     1888 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/email/account/new.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     1019 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/email/account/recover.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)      202 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/email/base.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     2332 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/email/layout.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     2482 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/email/macros.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     2129 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/email/test.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     2168 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/admin.fluid.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)      137 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/admin.simple.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)      266 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/admin.static.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     1626 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/bar.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)       71 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/content_type.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)       35 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/doctype.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)        9 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/end_doctype.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)      512 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/extras.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)      327 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/footer.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)       38 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/header.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     2174 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/includes.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)      414 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/layout.base.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     1966 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/layout.fluid.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     1190 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/layout.simple.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     1264 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/layout.static.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)    15586 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/macros.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)      204 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/message.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)      166 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/meta.html.tpl
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/account/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1828 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/account/new.html.tpl
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/database/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1251 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/database/import.html.tpl
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/entities/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1482 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/entities/edit.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     1180 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/entities/new.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     5255 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/entities/show.html.tpl
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/models/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1400 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/models/list.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     7686 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/models/show.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)      852 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/configs.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)      873 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/counters.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     1081 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/database.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)      391 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/done.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)      823 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/error.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)      858 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/libraries.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     1805 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/operations.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     1933 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/options.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)      845 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/parts.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     1070 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/recover.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     1216 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/reset.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     1323 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/routes.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     1210 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/session.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     1924 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/sessions.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     2003 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/signin.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     4683 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/social.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     5305 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/status.html.tpl
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/static/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/static/models/
+-rw-r--r--   0 travis    (1000) travis    (1000)      368 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/static/models/list.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)      823 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/static/error.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     2003 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/templates/static/signin.html.tpl
+-rw-r--r--   0 travis    (1000) travis    (1000)     1356 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    52383 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/admin/part.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/static/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/static/fonts/
+-rw-r--r--   0 travis    (1000) travis    (1000)    95380 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/static/fonts/aaaiight.ttf
+-rw-r--r--   0 travis    (1000) travis    (1000)    46108 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/static/fonts/abscissa.ttf
+-rw-r--r--   0 travis    (1000) travis    (1000)    53704 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/static/fonts/adler.ttf
+-rw-r--r--   0 travis    (1000) travis    (1000)   774476 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/static/fonts/arial.ttf
+-rw-r--r--   0 travis    (1000) travis    (1000)    20640 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/static/fonts/kbasalu.ttf
+-rw-r--r--   0 travis    (1000) travis    (1000)    60748 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/static/fonts/knights_quest.ttf
+-rw-r--r--   0 travis    (1000) travis    (1000)    21396 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/static/fonts/sevenbrg.ttf
+-rw-r--r--   0 travis    (1000) travis    (1000)    16200 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/static/fonts/treasure_island.ttf
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/static/patterns/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1000 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/static/patterns/pattern_1.jpg
+-rw-r--r--   0 travis    (1000) travis    (1000)     1103 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/static/patterns/pattern_2.jpg
+-rw-r--r--   0 travis    (1000) travis    (1000)     1457 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/static/patterns/pattern_3.jpg
+-rw-r--r--   0 travis    (1000) travis    (1000)     1024 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/static/patterns/pattern_4.jpg
+-rw-r--r--   0 travis    (1000) travis    (1000)      935 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/static/patterns/pattern_5.jpg
+-rw-r--r--   0 travis    (1000) travis    (1000)      959 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/static/patterns/pattern_6.jpg
+-rw-r--r--   0 travis    (1000) travis    (1000)     1371 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/static/patterns/pattern_7.jpg
+-rw-r--r--   0 travis    (1000) travis    (1000)     1268 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     7240 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/captcha/part.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/csfr/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1330 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/csfr/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2716 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/csfr/part.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2041 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/csfr/util.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/opbeat/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1267 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/opbeat/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4205 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/opbeat/part.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/parts/sematext/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1330 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/sematext/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4580 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/sematext/handler.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2844 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/sematext/part.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1531 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/parts/__init__.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/test/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1213 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/test/__init__.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras/utils/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1312 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/utils/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    17025 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/utils/markdown.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1356 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1596 2017-04-12 18:31:16.000000 appier_extras-0.9.9/src/appier_extras/base.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras.egg-info/
+-rw-r--r--   0 travis    (1000) travis    (1000)      997 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)     6359 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       63 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras.egg-info/entry_points.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-04-12 18:31:35.000000 appier_extras-0.9.9/src/appier_extras.egg-info/not-zip-safe
+-rw-r--r--   0 travis    (1000) travis    (1000)        7 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras.egg-info/requires.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       14 2017-04-12 18:31:40.000000 appier_extras-0.9.9/src/appier_extras.egg-info/top_level.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)      665 2017-04-12 18:31:16.000000 appier_extras-0.9.9/MANIFEST.in
+-rw-r--r--   0 travis    (1000) travis    (1000)     3698 2017-04-12 18:31:16.000000 appier_extras-0.9.9/setup.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      997 2017-04-12 18:31:40.000000 appier_extras-0.9.9/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)       88 2017-04-12 18:31:40.000000 appier_extras-0.9.9/setup.cfg
```

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/models/__init__.py` & `appier_extras-0.9.9/src/appier_extras/parts/admin/models/__init__.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/models/account.py` & `appier_extras-0.9.9/src/appier_extras/parts/admin/models/account.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/models/base.py` & `appier_extras-0.9.9/src/appier_extras/parts/admin/models/base.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/models/config.py` & `appier_extras-0.9.9/src/appier_extras/parts/admin/models/config.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/models/event.py` & `appier_extras-0.9.9/src/appier_extras/parts/admin/models/event.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/models/role.py` & `appier_extras-0.9.9/src/appier_extras/parts/admin/models/role.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/models/search.py` & `appier_extras-0.9.9/src/appier_extras/parts/admin/models/search.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/models/settings.py` & `appier_extras-0.9.9/src/appier_extras/parts/admin/models/settings.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/models/snapshot.py` & `appier_extras-0.9.9/src/appier_extras/parts/admin/models/snapshot.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/social/__init__.py` & `appier_extras-0.9.9/src/appier_extras/parts/admin/social/__init__.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/social/facebook_s.py` & `appier_extras-0.9.9/src/appier_extras/parts/admin/social/facebook_s.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/social/github_s.py` & `appier_extras-0.9.9/src/appier_extras/parts/admin/social/github_s.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/social/google_s.py` & `appier_extras-0.9.9/src/appier_extras/parts/admin/social/google_s.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/social/live_s.py` & `appier_extras-0.9.9/src/appier_extras/parts/admin/social/live_s.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/social/twitter_s.py` & `appier_extras-0.9.9/src/appier_extras/parts/admin/social/twitter_s.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/static/css/layout.css` & `appier_extras-0.9.9/src/appier_extras/parts/admin/static/css/layout.css`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/static/images/avatar_96.png` & `appier_extras-0.9.9/src/appier_extras/parts/admin/static/images/avatar_96.png`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/static/images/favicon.ico` & `appier_extras-0.9.9/src/appier_extras/parts/admin/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/static/images/logo_96.png` & `appier_extras-0.9.9/src/appier_extras/parts/admin/static/images/logo_96.png`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/static/js/main.js` & `appier_extras-0.9.9/src/appier_extras/parts/admin/static/js/main.js`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/email/account/confirm.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/email/account/confirm.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/email/account/new.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/email/account/new.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/email/account/recover.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/email/account/recover.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/email/layout.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/email/layout.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/email/macros.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/email/macros.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/email/test.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/email/test.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/admin.fluid.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/admin.fluid.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/bar.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/bar.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/extras.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/extras.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/includes.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/includes.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/layout.fluid.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/layout.fluid.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/layout.simple.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/layout.simple.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/layout.static.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/layout.static.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/admin/macros.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/admin/macros.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/account/new.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/account/new.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/database/import.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/database/import.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/entities/edit.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/entities/edit.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/entities/new.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/entities/new.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/entities/show.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/entities/show.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/models/list.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/models/list.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/models/show.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/models/show.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/configs.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/configs.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/counters.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/counters.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/database.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/database.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/error.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/error.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/libraries.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/libraries.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/operations.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/operations.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/options.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/options.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/parts.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/parts.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/recover.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/recover.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/reset.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/reset.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/routes.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/routes.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/session.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/session.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/sessions.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/sessions.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/signin.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/signin.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/social.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/social.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/fluid/status.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/fluid/status.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/static/error.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/static/error.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/templates/static/signin.html.tpl` & `appier_extras-0.9.9/src/appier_extras/parts/admin/templates/static/signin.html.tpl`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/__init__.py` & `appier_extras-0.9.9/src/appier_extras/parts/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/admin/part.py` & `appier_extras-0.9.9/src/appier_extras/parts/admin/part.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,14 +109,15 @@
         self.owner.login_route = "admin.login"
         self.owner.login_route_admin = "admin.login"
         self.owner.login_redirect = "admin.index"
         self.owner.admin_account = self.account_c
         self.owner.admin_open = True
         self.owner.admin_login_route = "admin.login"
         self.owner.admin_login_redirect = "admin.index"
+        self.owner.admin_logout_redirect = "admin.login"
         self.owner.admin_facebook_scope = ("email",)
         self.owner.admin_github_scope = ("user:email",)
         self.owner.admin_google_scope = ("email",)
         self.owner.admin_live_scope = ("wl.basic", "wl.emails")
 
         self.owner.lib_loaders["appier_extras"] = self._appier_extras_loader
         self.owner.lib_loaders["netius"] = self._netius_loader
@@ -248,18 +249,20 @@
         )
 
     def index(self):
         return self.list_models()
 
     def signin(self):
         next = self.field("next")
+        error = self.field("error")
         socials = self.socials()
         return self.template(
             "signin.html.tpl",
             next = next,
+            error = error,
             socials = socials
         )
 
     def login(self):
         # retrieves the various fields that are going to be
         # used for the validation of the user under the current
         # authentication/authorization process
@@ -304,15 +307,15 @@
         # attributes and in case they exist removes them from session as
         # the user is currently logging out from session
         self.account_c._unset_session()
 
         # runs the proper redirect operation, taking into account if the
         # next value has been provided or not
         return self.redirect(
-            next or self.url_for(self.owner.admin_login_redirect)
+            next or self.url_for(self.owner.admin_logout_redirect)
         )
 
     def recover(self):
         return self.template("recover.html.tpl")
 
     def recover_do(self):
         identifier = self.field("identifier")
@@ -783,14 +786,16 @@
         return self.template(
             "models/list.html.tpl",
             section = "admin"
         )
 
     @appier.ensure(token = "admin")
     def show_model(self, model):
+        token = "admin.models." + model
+        appier.ensure_login(self, token = token)
         model = self.get_model(model)
         model.assert_is_concrete_g()
         object = appier.get_object(
             alias = True,
             page = True,
             find = True
         )
```

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/captcha/static/fonts/aaaiight.ttf` & `appier_extras-0.9.9/src/appier_extras/parts/captcha/static/fonts/aaaiight.ttf`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/captcha/static/fonts/abscissa.ttf` & `appier_extras-0.9.9/src/appier_extras/parts/captcha/static/fonts/abscissa.ttf`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/captcha/static/fonts/adler.ttf` & `appier_extras-0.9.9/src/appier_extras/parts/captcha/static/fonts/adler.ttf`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/captcha/static/fonts/arial.ttf` & `appier_extras-0.9.9/src/appier_extras/parts/captcha/static/fonts/arial.ttf`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/captcha/static/fonts/kbasalu.ttf` & `appier_extras-0.9.9/src/appier_extras/parts/captcha/static/fonts/kbasalu.ttf`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/captcha/static/fonts/knights_quest.ttf` & `appier_extras-0.9.9/src/appier_extras/parts/captcha/static/fonts/knights_quest.ttf`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/captcha/static/fonts/sevenbrg.ttf` & `appier_extras-0.9.9/src/appier_extras/parts/captcha/static/fonts/sevenbrg.ttf`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/captcha/static/fonts/treasure_island.ttf` & `appier_extras-0.9.9/src/appier_extras/parts/captcha/static/fonts/treasure_island.ttf`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/captcha/static/patterns/pattern_1.jpg` & `appier_extras-0.9.9/src/appier_extras/parts/captcha/static/patterns/pattern_1.jpg`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/captcha/static/patterns/pattern_2.jpg` & `appier_extras-0.9.9/src/appier_extras/parts/captcha/static/patterns/pattern_2.jpg`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/captcha/static/patterns/pattern_3.jpg` & `appier_extras-0.9.9/src/appier_extras/parts/captcha/static/patterns/pattern_3.jpg`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/captcha/static/patterns/pattern_4.jpg` & `appier_extras-0.9.9/src/appier_extras/parts/captcha/static/patterns/pattern_4.jpg`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/captcha/static/patterns/pattern_5.jpg` & `appier_extras-0.9.9/src/appier_extras/parts/captcha/static/patterns/pattern_5.jpg`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/captcha/static/patterns/pattern_6.jpg` & `appier_extras-0.9.9/src/appier_extras/parts/captcha/static/patterns/pattern_6.jpg`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/captcha/static/patterns/pattern_7.jpg` & `appier_extras-0.9.9/src/appier_extras/parts/captcha/static/patterns/pattern_7.jpg`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/captcha/__init__.py` & `appier_extras-0.9.9/src/appier_extras/parts/captcha/__init__.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/captcha/part.py` & `appier_extras-0.9.9/src/appier_extras/parts/captcha/part.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/csfr/__init__.py` & `appier_extras-0.9.9/src/appier_extras/parts/csfr/__init__.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/csfr/part.py` & `appier_extras-0.9.9/src/appier_extras/parts/csfr/part.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/csfr/util.py` & `appier_extras-0.9.9/src/appier_extras/parts/csfr/util.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/opbeat/__init__.py` & `appier_extras-0.9.9/src/appier_extras/parts/opbeat/__init__.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/opbeat/part.py` & `appier_extras-0.9.9/src/appier_extras/parts/opbeat/part.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/sematext/__init__.py` & `appier_extras-0.9.9/src/appier_extras/parts/sematext/__init__.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/sematext/handler.py` & `appier_extras-0.9.9/src/appier_extras/parts/sematext/handler.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/sematext/part.py` & `appier_extras-0.9.9/src/appier_extras/parts/sematext/part.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/parts/__init__.py` & `appier_extras-0.9.9/src/appier_extras/parts/__init__.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/test/__init__.py` & `appier_extras-0.9.9/src/appier_extras/test/__init__.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/utils/__init__.py` & `appier_extras-0.9.9/src/appier_extras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/utils/markdown.py` & `appier_extras-0.9.9/src/appier_extras/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/__init__.py` & `appier_extras-0.9.9/src/appier_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/src/appier_extras/base.py` & `appier_extras-0.9.9/src/appier_extras/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,10 +37,10 @@
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 NAME = "appier_extras"
 """ The name to be used to describe the library while working
 on its own environment, this is just a descriptive value """
 
-VERSION = "0.9.8"
+VERSION = "0.9.9"
 """ The version of the library that is currently installed
 this value may be used for debugging/diagnostic purposes """
```

### Comparing `appier_extras-0.9.8/src/appier_extras.egg-info/PKG-INFO` & `appier_extras-0.9.9/src/appier_extras.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: appier-extras
-Version: 0.9.8
+Version: 0.9.9
 Summary: Appier Framework Extra Elements
 Home-page: http://appier_extras.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Keywords: appier extras framework web json
```

### Comparing `appier_extras-0.9.8/src/appier_extras.egg-info/SOURCES.txt` & `appier_extras-0.9.9/src/appier_extras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/MANIFEST.in` & `appier_extras-0.9.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `appier_extras-0.9.8/setup.py` & `appier_extras-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 """ The license for the module """
 
 import os
 import setuptools
 
 setuptools.setup(
     name = "appier_extras",
-    version = "0.9.8",
+    version = "0.9.9",
     author = "Hive Solutions Lda.",
     author_email = "development@hive.pt",
     description = "Appier Framework Extra Elements",
     license = "Apache License, Version 2.0",
     keywords = "appier extras framework web json",
     url = "http://appier_extras.hive.pt",
     zip_safe = False,
```

### Comparing `appier_extras-0.9.8/PKG-INFO` & `appier_extras-0.9.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: appier_extras
-Version: 0.9.8
+Version: 0.9.9
 Summary: Appier Framework Extra Elements
 Home-page: http://appier_extras.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Keywords: appier extras framework web json
```

