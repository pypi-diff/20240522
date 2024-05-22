# Comparing `tmp/invenio_theme_tuw-2024.1.2.tar.gz` & `tmp/invenio_theme_tuw-2024.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio_theme_tuw-2024.1.2.tar", last modified: Fri May 17 18:38:16 2024, max compression
+gzip compressed data, was "invenio_theme_tuw-2024.1.3.tar", last modified: Wed May 22 15:58:38 2024, max compression
```

## Comparing `invenio_theme_tuw-2024.1.2.tar` & `invenio_theme_tuw-2024.1.3.tar`

### file list

```diff
@@ -1,266 +1,266 @@
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.125448 invenio_theme_tuw-2024.1.2/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.2/.dockerignore
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      617 2022-11-23 16:27:37.000000 invenio_theme_tuw-2024.1.2/.editorconfig
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2022-11-23 16:27:37.000000 invenio_theme_tuw-2024.1.2/.git-blame-ignore-revs
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.097447 invenio_theme_tuw-2024.1.2/.tx/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1042 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.2/.tx/config
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      287 2021-07-15 12:29:34.000000 invenio_theme_tuw-2024.1.2/AUTHORS.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7113 2024-05-17 14:55:56.000000 invenio_theme_tuw-2024.1.2/CHANGES.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3370 2021-07-15 12:29:34.000000 invenio_theme_tuw-2024.1.2/CONTRIBUTING.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      202 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.2/INSTALL.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.2/LICENSE
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1746 2024-03-14 10:32:25.000000 invenio_theme_tuw-2024.1.2/MANIFEST.in
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     9427 2024-05-17 18:38:16.125448 invenio_theme_tuw-2024.1.2/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1040 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.2/README.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      535 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.2/babel.ini
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.097447 invenio_theme_tuw-2024.1.2/docs/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7453 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.2/docs/Makefile
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      233 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.2/docs/authors.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      233 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.2/docs/changes.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10182 2024-02-29 16:56:49.000000 invenio_theme_tuw-2024.1.2/docs/conf.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      238 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.2/docs/contributing.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      441 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.2/docs/index.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.2/docs/license.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7003 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.2/docs/make.bat
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.2/docs/requirements.txt
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.097447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      372 2024-05-17 14:55:56.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/__init__.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.101447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/build_project/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       78 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/build_project/.babelrc
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       11 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/build_project/.eslintignore
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      849 2023-04-24 15:50:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/build_project/.eslintrc.js
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.101447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/build_project/build/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7181 2023-04-24 15:50:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/build_project/build/webpack.config.js
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2385 2023-08-25 12:49:04.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/build_project/package.json
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.101447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/build_project/patches/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      560 2023-04-24 15:50:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/build_project/patches/watchpack+1.7.5.patch
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4376 2023-12-13 15:21:45.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/config.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2617 2023-08-25 08:52:24.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/ext.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      763 2022-10-17 09:59:49.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/search.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.093447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.093447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.093447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.093447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/js/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.093447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.101447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/mobilemenu/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      576 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/mobilemenu/index.js
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.101447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/snowfall/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      517 2023-12-13 15:21:45.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/snowfall/index.js
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.101447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/tracking/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      966 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/tracking/index.js
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.093447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.101447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.101447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.101447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      213 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/breadcrumb.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       70 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/breadcrumb.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      984 2022-09-07 12:08:20.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/form.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/form.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/grid.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/grid.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7166 2023-09-11 19:50:33.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1040 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       69 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/message.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      210 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/message.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/table.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/table.variables
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.101447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      479 2022-09-08 10:53:10.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/contact.less
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      665 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/file-list.less
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1312 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/flip-card.less
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3045 2022-11-25 16:08:24.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/fonts.less
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.105447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      503 2022-09-02 11:49:31.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/button.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      725 2022-09-02 11:49:31.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/button.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      599 2022-09-02 13:37:47.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/container.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       68 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/container.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/divider.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/divider.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/flag.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/flag.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/header.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/header.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      331 2022-10-27 14:52:31.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/icon.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/icon.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/image.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/image.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/input.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/input.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/label.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/label.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/list.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/list.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/loader.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/loader.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/rail.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/rail.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/reveal.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/reveal.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/segment.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/segment.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/step.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/step.variables
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.109447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   287936 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Bold.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   209784 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-BoldItalic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   270524 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Italic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   278168 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Regular.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168060 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Black.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   174108 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BlackItalic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   167336 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Bold.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   171508 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BoldItalic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   170504 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Italic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   167000 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Light.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   173172 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-LightItalic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168644 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Medium.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   173416 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-MediumItalic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168260 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Regular.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168488 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Thin.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   172860 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-ThinItalic.ttf
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.113448 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      291 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/reset.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/reset.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4302 2023-04-24 11:32:11.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1150 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.variables
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.113448 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    36366 2022-10-10 09:44:16.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-background.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    22946 2022-10-10 09:44:16.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-contact.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    43552 2022-10-10 09:44:16.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-policies.webp
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.117447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/accordion.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/accordion.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/chatroom.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/chatroom.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2569 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/checkbox.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/checkbox.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dimmer.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dimmer.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      154 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dropdown.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      161 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dropdown.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/embed.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/embed.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/modal.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/modal.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       59 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/nag.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       59 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/nag.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/popup.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/popup.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/progress.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/progress.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/rating.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/rating.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/search.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/search.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/shape.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/shape.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      369 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sidebar.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      338 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sidebar.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sticky.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sticky.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/tab.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/tab.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/transition.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/transition.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2326 2023-05-03 16:49:56.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/theme.less
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.117447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       56 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/ad.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       56 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/ad.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/card.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/card.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/comment.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/comment.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/feed.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/feed.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       60 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/item.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/item.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/statistic.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/statistic.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2022-09-05 14:21:18.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/tuwstone.less
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1106 2024-05-17 14:55:56.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/user_infos.less
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.093447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.117447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      794 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/favicon-16x16.png
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1101 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/favicon-32x32.png
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.117447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/features/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    12850 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/features/faq.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    27714 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/features/magnifying-glass.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    13548 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/features/online-chat.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    21722 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/features/upload-file.webp
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.121448 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/footer-logos/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   201844 2023-09-11 19:50:33.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/footer-logos/fairsharing-logo.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    29306 2023-09-11 19:50:33.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/footer-logos/inveniordm-logo.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4636 2022-11-30 11:55:52.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.png
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2512 2022-11-30 11:55:52.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     9811 2022-11-30 11:55:52.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.png
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3926 2022-11-30 11:55:52.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    13674 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/pdf.webp
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.121448 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/planned-features/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    19926 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/planned-features/analytics.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    36394 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/planned-features/connection.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8098 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/planned-features/git.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    37302 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/planned-features/group.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    34924 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/planned-features/online-community.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    22964 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/planned-features/team.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    29404 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/planned-features/user.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    31176 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/planned-features/version.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10686 2023-10-04 10:01:08.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/tu-wien-logo-hd.png
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2626 2023-10-04 10:01:08.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/tu-wien-logo.png
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.121448 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/tuwstones/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    70038 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/tuwstones/fwoerister.png
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.093447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.093447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.093447 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.121448 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    16065 2023-04-24 14:08:12.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/detail.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      955 2023-04-24 14:08:12.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/search.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.121448 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1719 2022-10-03 16:21:50.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      679 2023-08-30 13:44:57.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_mail_html.jinja
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      591 2023-08-25 12:49:04.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_mail_text.jinja
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3294 2023-08-25 08:52:24.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_uploader.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.121448 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7653 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/details.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2836 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/side_bar.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      981 2023-08-30 13:44:57.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/uploaders.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.121448 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1710 2023-02-20 18:21:08.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/community.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1649 2023-04-05 13:35:38.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/deposit.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.121448 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/macros/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      974 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/macros/detail.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.125448 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2458 2023-09-11 19:50:33.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/footer.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8340 2023-10-18 13:58:40.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/frontpage.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5012 2023-02-20 18:21:08.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/header.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      657 2023-12-13 15:21:45.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/javascript.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1501 2023-04-24 14:08:12.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/login_user.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8550 2023-04-24 14:08:12.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      758 2023-04-24 14:08:12.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page_error.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2101 2023-04-24 14:08:12.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/signup.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2676 2023-02-20 18:21:08.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/policies.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      668 2022-10-03 16:21:50.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/search_bar.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.125448 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/settings/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2045 2023-12-22 13:32:07.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/settings/curation.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1463 2022-11-30 11:55:52.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/terms_of_use.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.125448 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/tuwstones/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1278 2022-09-05 14:21:18.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/tuwstones/florian_woerister.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2148 2024-05-17 14:55:56.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/users_infos.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    14745 2024-05-17 14:55:56.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/views.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3338 2024-05-17 14:55:56.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw/webpack.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.125448 invenio_theme_tuw-2024.1.2/invenio_theme_tuw.egg-info/
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     9427 2024-05-17 18:38:16.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    16664 2024-05-17 18:38:16.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-05-17 18:38:16.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      228 2024-05-17 18:38:16.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-05-17 18:38:08.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw.egg-info/not-zip-safe
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      215 2024-05-17 18:38:16.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       18 2024-05-17 18:38:16.000000 invenio_theme_tuw-2024.1.2/invenio_theme_tuw.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2022-11-23 16:27:37.000000 invenio_theme_tuw-2024.1.2/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      491 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.2/requirements-devel.txt
--rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      712 2024-02-29 16:56:49.000000 invenio_theme_tuw-2024.1.2/run-tests.sh
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2403 2024-05-17 18:38:16.129448 invenio_theme_tuw-2024.1.2/setup.cfg
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      294 2022-11-23 16:27:37.000000 invenio_theme_tuw-2024.1.2/setup.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-17 18:38:16.125448 invenio_theme_tuw-2024.1.2/tests/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8379 2024-02-29 16:56:49.000000 invenio_theme_tuw-2024.1.2/tests/conftest.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3849 2024-02-29 17:31:49.000000 invenio_theme_tuw-2024.1.2/tests/test_functions.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1935 2024-02-29 16:56:49.000000 invenio_theme_tuw-2024.1.2/tests/test_invenio_theme_tuw.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1263 2024-02-29 16:56:49.000000 invenio_theme_tuw-2024.1.2/tests/test_routes.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.453795 invenio_theme_tuw-2024.1.3/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.3/.dockerignore
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      617 2022-11-23 16:27:37.000000 invenio_theme_tuw-2024.1.3/.editorconfig
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2022-11-23 16:27:37.000000 invenio_theme_tuw-2024.1.3/.git-blame-ignore-revs
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.421794 invenio_theme_tuw-2024.1.3/.tx/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1042 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.3/.tx/config
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      287 2021-07-15 12:29:34.000000 invenio_theme_tuw-2024.1.3/AUTHORS.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7182 2024-05-22 15:48:42.000000 invenio_theme_tuw-2024.1.3/CHANGES.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3370 2021-07-15 12:29:34.000000 invenio_theme_tuw-2024.1.3/CONTRIBUTING.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      202 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.3/INSTALL.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.3/LICENSE
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1746 2024-03-14 10:32:25.000000 invenio_theme_tuw-2024.1.3/MANIFEST.in
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     9496 2024-05-22 15:58:38.453795 invenio_theme_tuw-2024.1.3/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1040 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.3/README.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      535 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.3/babel.ini
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.421794 invenio_theme_tuw-2024.1.3/docs/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7453 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.3/docs/Makefile
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      233 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.3/docs/authors.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      233 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.3/docs/changes.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10182 2024-02-29 16:56:49.000000 invenio_theme_tuw-2024.1.3/docs/conf.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      238 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.3/docs/contributing.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      441 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.3/docs/index.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.3/docs/license.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7003 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.3/docs/make.bat
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.3/docs/requirements.txt
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.425794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      372 2024-05-22 15:48:42.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/__init__.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.425794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/build_project/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       78 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/build_project/.babelrc
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       11 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/build_project/.eslintignore
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      849 2023-04-24 15:50:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/build_project/.eslintrc.js
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.425794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/build_project/build/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7181 2023-04-24 15:50:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/build_project/build/webpack.config.js
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2385 2023-08-25 12:49:04.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/build_project/package.json
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.425794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/build_project/patches/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      560 2023-04-24 15:50:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/build_project/patches/watchpack+1.7.5.patch
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4376 2023-12-13 15:21:45.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2617 2023-08-25 08:52:24.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/ext.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      763 2022-10-17 09:59:49.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/search.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.417794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.417794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.417794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.417794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/js/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.417794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.425794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/mobilemenu/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      576 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/mobilemenu/index.js
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.425794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/snowfall/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      517 2023-12-13 15:21:45.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/snowfall/index.js
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.425794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/tracking/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      966 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/tracking/index.js
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.417794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.425794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.425794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.429794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      213 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/breadcrumb.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       70 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/breadcrumb.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      984 2022-09-07 12:08:20.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/form.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/form.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/grid.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/grid.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7166 2023-09-11 19:50:33.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1040 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       69 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/message.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      210 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/message.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/table.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/table.variables
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.429794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      479 2022-09-08 10:53:10.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/contact.less
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      665 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/file-list.less
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1312 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/flip-card.less
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3045 2022-11-25 16:08:24.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/fonts.less
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.433794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      503 2022-09-02 11:49:31.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/button.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      725 2022-09-02 11:49:31.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/button.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      599 2022-09-02 13:37:47.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/container.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       68 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/container.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/divider.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/divider.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/flag.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/flag.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/header.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/header.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      331 2022-10-27 14:52:31.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/icon.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/icon.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/image.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/image.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/input.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/input.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/label.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/label.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/list.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/list.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/loader.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/loader.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/rail.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/rail.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/reveal.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/reveal.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/segment.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/segment.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/step.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/step.variables
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.437795 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   287936 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Bold.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   209784 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-BoldItalic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   270524 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Italic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   278168 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Regular.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168060 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Black.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   174108 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BlackItalic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   167336 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Bold.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   171508 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BoldItalic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   170504 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Italic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   167000 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Light.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   173172 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-LightItalic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168644 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Medium.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   173416 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-MediumItalic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168260 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Regular.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168488 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Thin.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   172860 2022-09-19 15:50:46.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-ThinItalic.ttf
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.437795 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      291 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/reset.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/reset.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4302 2023-04-24 11:32:11.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1150 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.variables
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.441794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    36366 2022-10-10 09:44:16.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-background.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    22946 2022-10-10 09:44:16.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-contact.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    43552 2022-10-10 09:44:16.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-policies.webp
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.445795 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/accordion.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/accordion.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/chatroom.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/chatroom.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2569 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/checkbox.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/checkbox.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dimmer.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dimmer.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      154 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dropdown.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      161 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dropdown.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/embed.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/embed.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/modal.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/modal.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       59 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/nag.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       59 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/nag.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/popup.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/popup.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/progress.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/progress.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/rating.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/rating.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/search.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/search.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/shape.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/shape.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      369 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sidebar.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      338 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sidebar.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sticky.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sticky.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/tab.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/tab.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/transition.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/transition.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2326 2023-05-03 16:49:56.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/theme.less
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.445795 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       56 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/ad.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       56 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/ad.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/card.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/card.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/comment.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/comment.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/feed.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/feed.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       60 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/item.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/item.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/statistic.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/statistic.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2022-09-05 14:21:18.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/tuwstone.less
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1106 2024-05-17 14:55:56.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/user_infos.less
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.417794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.445795 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      794 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/favicon-16x16.png
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1101 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/favicon-32x32.png
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.445795 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/features/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    12850 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/features/faq.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    27714 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/features/magnifying-glass.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    13548 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/features/online-chat.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    21722 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/features/upload-file.webp
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.449795 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/footer-logos/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   201844 2023-09-11 19:50:33.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/footer-logos/fairsharing-logo.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    29306 2023-09-11 19:50:33.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/footer-logos/inveniordm-logo.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4636 2022-11-30 11:55:52.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.png
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2512 2022-11-30 11:55:52.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     9811 2022-11-30 11:55:52.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.png
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3926 2022-11-30 11:55:52.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    13674 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/pdf.webp
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.449795 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/planned-features/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    19926 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/planned-features/analytics.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    36394 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/planned-features/connection.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8098 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/planned-features/git.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    37302 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/planned-features/group.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    34924 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/planned-features/online-community.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    22964 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/planned-features/team.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    29404 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/planned-features/user.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    31176 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/planned-features/version.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10686 2023-10-04 10:01:08.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/tu-wien-logo-hd.png
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2626 2023-10-04 10:01:08.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/tu-wien-logo.png
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.449795 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/tuwstones/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    70038 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/tuwstones/fwoerister.png
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.417794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.417794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.417794 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.449795 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    16065 2023-04-24 14:08:12.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/detail.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      955 2023-04-24 14:08:12.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/search.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.449795 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1719 2022-10-03 16:21:50.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      679 2023-08-30 13:44:57.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_mail_html.jinja
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      591 2023-08-25 12:49:04.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_mail_text.jinja
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3294 2023-08-25 08:52:24.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_uploader.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.449795 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7653 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/details.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2836 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/side_bar.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      981 2023-08-30 13:44:57.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/uploaders.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.449795 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1710 2023-02-20 18:21:08.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/community.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1649 2023-04-05 13:35:38.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/deposit.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.449795 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/macros/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      974 2022-07-14 09:43:44.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/macros/detail.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.453795 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2458 2023-09-11 19:50:33.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/footer.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8340 2023-10-18 13:58:40.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/frontpage.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5012 2023-02-20 18:21:08.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/header.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      657 2023-12-13 15:21:45.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/javascript.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1501 2023-04-24 14:08:12.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/login_user.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8550 2023-04-24 14:08:12.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      758 2023-04-24 14:08:12.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page_error.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2101 2023-04-24 14:08:12.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/signup.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2676 2023-02-20 18:21:08.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/policies.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      668 2022-10-03 16:21:50.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/search_bar.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.453795 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/settings/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2045 2023-12-22 13:32:07.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/settings/curation.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1463 2022-11-30 11:55:52.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/terms_of_use.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.453795 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/tuwstones/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1278 2022-09-05 14:21:18.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/tuwstones/florian_woerister.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2148 2024-05-17 14:55:56.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/users_infos.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    14123 2024-05-22 15:48:42.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/views.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3338 2024-05-17 14:55:56.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw/webpack.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.453795 invenio_theme_tuw-2024.1.3/invenio_theme_tuw.egg-info/
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     9496 2024-05-22 15:58:38.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    16664 2024-05-22 15:58:38.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-05-22 15:58:38.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      228 2024-05-22 15:58:38.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-05-22 15:58:31.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw.egg-info/not-zip-safe
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      215 2024-05-22 15:58:38.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       18 2024-05-22 15:58:38.000000 invenio_theme_tuw-2024.1.3/invenio_theme_tuw.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2022-11-23 16:27:37.000000 invenio_theme_tuw-2024.1.3/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      491 2021-07-05 13:11:26.000000 invenio_theme_tuw-2024.1.3/requirements-devel.txt
+-rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      712 2024-02-29 16:56:49.000000 invenio_theme_tuw-2024.1.3/run-tests.sh
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2403 2024-05-22 15:58:38.457795 invenio_theme_tuw-2024.1.3/setup.cfg
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      294 2022-11-23 16:27:37.000000 invenio_theme_tuw-2024.1.3/setup.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-22 15:58:38.453795 invenio_theme_tuw-2024.1.3/tests/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8379 2024-02-29 16:56:49.000000 invenio_theme_tuw-2024.1.3/tests/conftest.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3849 2024-02-29 17:31:49.000000 invenio_theme_tuw-2024.1.3/tests/test_functions.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1935 2024-02-29 16:56:49.000000 invenio_theme_tuw-2024.1.3/tests/test_invenio_theme_tuw.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1263 2024-02-29 16:56:49.000000 invenio_theme_tuw-2024.1.3/tests/test_routes.py
```

### Comparing `invenio_theme_tuw-2024.1.2/.editorconfig` & `invenio_theme_tuw-2024.1.3/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/.tx/config` & `invenio_theme_tuw-2024.1.3/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/CHANGES.rst` & `invenio_theme_tuw-2024.1.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,20 @@
     Invenio-Theme-TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2024.1 (released 2024-03-01, updated 2024-05-17)
+Version 2024.1 (released 2024-03-01, updated 2024-05-22)
 
 - Views: add status code in guards' response
 - Add automated tests
 - Add TUW-specific user administration page
+- Fetch TISS ID from user profile rather than from old access tokens
 
 
 Version 2023.2 (released 2023-04-24, updated 2023-12-22)
 
 - v11 compat: Update templates and frontend build project
 - Remove PDF preview override, as it has been merged upstream
 - Rework "contact uploader" feature to a dedicated contact form
```

### Comparing `invenio_theme_tuw-2024.1.2/CONTRIBUTING.rst` & `invenio_theme_tuw-2024.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/LICENSE` & `invenio_theme_tuw-2024.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/MANIFEST.in` & `invenio_theme_tuw-2024.1.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/PKG-INFO` & `invenio_theme_tuw-2024.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-theme-tuw
-Version: 2024.1.2
+Version: 2024.1.3
 Summary: "TU Wien theme for Invenio (RDM)."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-theme-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio theme tuw
 Platform: any
@@ -74,19 +74,20 @@
     Invenio-Theme-TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2024.1 (released 2024-03-01, updated 2024-05-17)
+Version 2024.1 (released 2024-03-01, updated 2024-05-22)
 
 - Views: add status code in guards' response
 - Add automated tests
 - Add TUW-specific user administration page
+- Fetch TISS ID from user profile rather than from old access tokens
 
 
 Version 2023.2 (released 2023-04-24, updated 2023-12-22)
 
 - v11 compat: Update templates and frontend build project
 - Remove PDF preview override, as it has been merged upstream
 - Rework "contact uploader" feature to a dedicated contact form
```

### Comparing `invenio_theme_tuw-2024.1.2/README.rst` & `invenio_theme_tuw-2024.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/babel.ini` & `invenio_theme_tuw-2024.1.3/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/docs/Makefile` & `invenio_theme_tuw-2024.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/docs/conf.py` & `invenio_theme_tuw-2024.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/docs/make.bat` & `invenio_theme_tuw-2024.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/build_project/.eslintrc.js` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/build_project/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/build_project/build/webpack.config.js` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/build_project/build/webpack.config.js`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/build_project/package.json` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/build_project/package.json`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/build_project/patches/watchpack+1.7.5.patch` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/build_project/patches/watchpack+1.7.5.patch`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/config.py` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/config.py`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/ext.py` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/ext.py`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/search.py` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/search.py`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/mobilemenu/index.js` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/mobilemenu/index.js`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/snowfall/index.js` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/snowfall/index.js`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/tracking/index.js` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/tracking/index.js`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/form.overrides` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/form.overrides`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.overrides` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.overrides`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.variables` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.variables`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/file-list.less` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/file-list.less`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/flip-card.less` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/flip-card.less`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/fonts.less` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/fonts.less`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/button.variables` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/button.variables`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/container.overrides` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/container.overrides`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Bold.ttf` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-BoldItalic.ttf` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Italic.ttf` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Regular.ttf` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Black.ttf` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BlackItalic.ttf` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Bold.ttf` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BoldItalic.ttf` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Italic.ttf` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Light.ttf` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-LightItalic.ttf` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Medium.ttf` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-MediumItalic.ttf` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Regular.ttf` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Thin.ttf` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-ThinItalic.ttf` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.overrides` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.overrides`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.variables` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.variables`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-background.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-background.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-contact.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-contact.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-policies.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-policies.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/checkbox.overrides` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/checkbox.overrides`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/theme.less` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/theme.less`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/tuwstone.less` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/tuwstone.less`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/user_infos.less` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/user_infos.less`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/favicon-16x16.png` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/favicon-32x32.png` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/features/faq.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/features/faq.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/features/magnifying-glass.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/features/magnifying-glass.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/features/online-chat.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/features/online-chat.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/features/upload-file.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/features/upload-file.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/footer-logos/fairsharing-logo.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/footer-logos/fairsharing-logo.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/footer-logos/inveniordm-logo.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/footer-logos/inveniordm-logo.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.png` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.png`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.png` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.png`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/pdf.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/pdf.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/planned-features/analytics.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/planned-features/analytics.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/planned-features/connection.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/planned-features/connection.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/planned-features/git.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/planned-features/git.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/planned-features/group.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/planned-features/group.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/planned-features/online-community.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/planned-features/online-community.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/planned-features/team.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/planned-features/team.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/planned-features/user.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/planned-features/user.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/planned-features/version.webp` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/planned-features/version.webp`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/tu-wien-logo-hd.png` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/tu-wien-logo-hd.png`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/tu-wien-logo.png` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/tu-wien-logo.png`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/static/images/tuwstones/fwoerister.png` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/static/images/tuwstones/fwoerister.png`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/detail.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/detail.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/search.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/search.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_mail_html.jinja` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_mail_html.jinja`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_mail_text.jinja` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_mail_text.jinja`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_uploader.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_uploader.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/details.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/details.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/side_bar.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/side_bar.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/uploaders.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/uploaders.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/community.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/community.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/deposit.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/deposit.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/macros/detail.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/macros/detail.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/footer.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/footer.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/frontpage.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/frontpage.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/header.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/header.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/javascript.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/javascript.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/login_user.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page_error.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page_error.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/signup.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/signup.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/policies.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/policies.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/search_bar.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/search_bar.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/settings/curation.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/settings/curation.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/terms_of_use.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/terms_of_use.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/tuwstones/florian_woerister.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/tuwstones/florian_woerister.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/users_infos.html` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/users_infos.html`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/views.py` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -129,45 +129,27 @@
 
 def _fetch_user_infos():
     """Fetch information about each user for our hacky user info list."""
     user_infos = []
     trusted_user_role = current_datastore.find_role("trusted-user")
 
     for user in db.session.query(User).order_by(User.id).all():
-
-        # get the TISS ID for the user, if available
-        tiss_id = None
-        for remote_account in user.remote_accounts:
-            for remote_token in remote_account.remote_tokens:
-                token = jwt.decode(
-                    remote_token.access_token, options={"verify_signature": False}
-                )
-
-                # for TUW people, the UID is the TISS ID
-                if any(
-                    [
-                        aff.endswith("@tuwien.ac.at")
-                        for aff in token.get("affiliation", [])
-                    ]
-                ):
-                    tiss_id = tiss_id or token.get("saml_uid", None)
-
         # check if the user has given us consent for record curation
         curation_consent = False
         if user.preferences:
             curation_consent = user.preferences.get("curation", {}).get(
                 "consent", False
             )
 
         # check if the user can upload datasets
         trusted = user.has_role(trusted_user_role)
 
         info = {
             "user": user,
-            "tiss_id": tiss_id,
+            "tiss_id": (user.user_profile or {}).get("tiss_id", None),
             "curation_consent": curation_consent,
             "trusted": trusted,
         }
 
         user_infos.append(info)
 
     return user_infos
```

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw/webpack.py` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw.egg-info/PKG-INFO` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-theme-tuw
-Version: 2024.1.2
+Version: 2024.1.3
 Summary: "TU Wien theme for Invenio (RDM)."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-theme-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio theme tuw
 Platform: any
@@ -74,19 +74,20 @@
     Invenio-Theme-TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2024.1 (released 2024-03-01, updated 2024-05-17)
+Version 2024.1 (released 2024-03-01, updated 2024-05-22)
 
 - Views: add status code in guards' response
 - Add automated tests
 - Add TUW-specific user administration page
+- Fetch TISS ID from user profile rather than from old access tokens
 
 
 Version 2023.2 (released 2023-04-24, updated 2023-12-22)
 
 - v11 compat: Update templates and frontend build project
 - Remove PDF preview override, as it has been merged upstream
 - Rework "contact uploader" feature to a dedicated contact form
```

### Comparing `invenio_theme_tuw-2024.1.2/invenio_theme_tuw.egg-info/SOURCES.txt` & `invenio_theme_tuw-2024.1.3/invenio_theme_tuw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/run-tests.sh` & `invenio_theme_tuw-2024.1.3/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/setup.cfg` & `invenio_theme_tuw-2024.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/tests/conftest.py` & `invenio_theme_tuw-2024.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/tests/test_functions.py` & `invenio_theme_tuw-2024.1.3/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/tests/test_invenio_theme_tuw.py` & `invenio_theme_tuw-2024.1.3/tests/test_invenio_theme_tuw.py`

 * *Files identical despite different names*

### Comparing `invenio_theme_tuw-2024.1.2/tests/test_routes.py` & `invenio_theme_tuw-2024.1.3/tests/test_routes.py`

 * *Files identical despite different names*

