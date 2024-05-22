# Comparing `tmp/xblock-poll-1.13.0.tar.gz` & `tmp/xblock-poll-1.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xblock-poll-1.13.0.tar", last modified: Tue Feb  7 20:51:29 2023, max compression
+gzip compressed data, was "xblock-poll-1.14.0.tar", last modified: Wed May 22 15:30:48 2024, max compression
```

## Comparing `xblock-poll-1.13.0.tar` & `xblock-poll-1.14.0.tar`

### file list

```diff
@@ -1,120 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.790897 xblock-poll-1.13.0/
--rw-r--r--   0 runner    (1001) docker     (122)    34500 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      491 2023-02-07 20:51:29.790897 xblock-poll-1.13.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17509 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.782897 xblock-poll-1.13.0/poll/
--rw-r--r--   0 runner    (1001) docker     (122)      978 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    56497 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/poll.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.782897 xblock-poll-1.13.0/poll/public/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/css/
--rw-r--r--   0 runner    (1001) docker     (122)     7429 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/css/poll.css
--rw-r--r--   0 runner    (1001) docker     (122)      896 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/css/poll_edit.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/css/themes/
--rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/css/themes/lms.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/handlebars/
--rw-r--r--   0 runner    (1001) docker     (122)     2149 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/handlebars/poll_results.handlebars
--rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/handlebars/poll_studio.handlebars
--rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/handlebars/survey_results.handlebars
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/html/
--rw-r--r--   0 runner    (1001) docker     (122)     2968 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/html/poll.html
--rw-r--r--   0 runner    (1001) docker     (122)     6811 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/html/poll_edit.html
--rw-r--r--   0 runner    (1001) docker     (122)     4679 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/html/survey.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/js/
--rw-r--r--   0 runner    (1001) docker     (122)    10818 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/poll.js
--rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/poll_common.js
--rw-r--r--   0 runner    (1001) docker     (122)    10863 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/poll_edit.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.782897 xblock-poll-1.13.0/poll/public/js/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/js/translations/ar/
--rw-r--r--   0 runner    (1001) docker     (122)     3685 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/translations/ar/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/js/translations/de_DE/
--rw-r--r--   0 runner    (1001) docker     (122)     4828 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/translations/de_DE/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/js/translations/en/
--rw-r--r--   0 runner    (1001) docker     (122)     3516 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/translations/en/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/js/translations/eo/
--rw-r--r--   0 runner    (1001) docker     (122)     8874 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/translations/eo/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/js/translations/es_419/
--rw-r--r--   0 runner    (1001) docker     (122)     4955 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/translations/es_419/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/js/translations/fr/
--rw-r--r--   0 runner    (1001) docker     (122)     5127 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/translations/fr/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/js/translations/fr_CA/
--rw-r--r--   0 runner    (1001) docker     (122)     5127 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/translations/fr_CA/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/js/translations/he/
--rw-r--r--   0 runner    (1001) docker     (122)     3685 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/translations/he/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/js/translations/hi/
--rw-r--r--   0 runner    (1001) docker     (122)     3667 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/translations/hi/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/js/translations/ja_JP/
--rw-r--r--   0 runner    (1001) docker     (122)     5724 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/translations/ja_JP/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/js/translations/ko_KR/
--rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/translations/ko_KR/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/js/translations/pl/
--rw-r--r--   0 runner    (1001) docker     (122)     3444 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/translations/pl/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/js/translations/pt_BR/
--rw-r--r--   0 runner    (1001) docker     (122)     4530 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/translations/pt_BR/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/js/translations/ru/
--rw-r--r--   0 runner    (1001) docker     (122)     3548 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/translations/ru/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/js/translations/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (122)     3664 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/translations/zh_CN/textjs.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/public/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (122)    89667 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/public/js/vendor/handlebars.js
--rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.782897 xblock-poll-1.13.0/poll/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     5489 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/ar/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11890 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/ar/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)      547 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.782897 xblock-poll-1.13.0/poll/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9527 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/de_DE/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    13153 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/de_DE/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     2907 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/de_DE/LC_MESSAGES/textjs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.782897 xblock-poll-1.13.0/poll/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/en/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9145 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/en/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     1756 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/en/LC_MESSAGES/textjs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.782897 xblock-poll-1.13.0/poll/translations/eo/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.786897 xblock-poll-1.13.0/poll/translations/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    16541 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/eo/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    20059 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/eo/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/eo/LC_MESSAGES/textjs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.782897 xblock-poll-1.13.0/poll/translations/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.790897 xblock-poll-1.13.0/poll/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9662 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    13430 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/es_419/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     2828 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/es_419/LC_MESSAGES/textjs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.782897 xblock-poll-1.13.0/poll/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.790897 xblock-poll-1.13.0/poll/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9798 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/fr/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    13455 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/fr/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     2938 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/fr/LC_MESSAGES/textjs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.782897 xblock-poll-1.13.0/poll/translations/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.790897 xblock-poll-1.13.0/poll/translations/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9899 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/fr_CA/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    13546 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/fr_CA/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/fr_CA/LC_MESSAGES/textjs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.782897 xblock-poll-1.13.0/poll/translations/he/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.790897 xblock-poll-1.13.0/poll/translations/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     5038 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/he/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11311 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/he/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.782897 xblock-poll-1.13.0/poll/translations/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.790897 xblock-poll-1.13.0/poll/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10325 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/ja_JP/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    13982 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/ja_JP/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     2870 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/ja_JP/LC_MESSAGES/textjs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.782897 xblock-poll-1.13.0/poll/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.790897 xblock-poll-1.13.0/poll/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4837 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/pt_BR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11273 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/pt_BR/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     2594 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/translations/pt_BR/LC_MESSAGES/textjs.po
--rw-r--r--   0 runner    (1001) docker     (122)      916 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/poll/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-07 20:51:29.790897 xblock-poll-1.13.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2227 2023-02-07 20:51:27.000000 xblock-poll-1.13.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 20:51:29.790897 xblock-poll-1.13.0/xblock_poll.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      491 2023-02-07 20:51:29.000000 xblock-poll-1.13.0/xblock_poll.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-02-07 20:51:29.000000 xblock-poll-1.13.0/xblock_poll.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-07 20:51:29.000000 xblock-poll-1.13.0/xblock_poll.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-02-07 20:51:29.000000 xblock-poll-1.13.0/xblock_poll.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-02-07 20:51:29.000000 xblock-poll-1.13.0/xblock_poll.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-02-07 20:51:29.000000 xblock-poll-1.13.0/xblock_poll.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.359191 xblock-poll-1.14.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34500 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18115 2024-05-22 15:30:48.359191 xblock-poll-1.14.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17509 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.347191 xblock-poll-1.14.0/poll/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56702 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/poll.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.339191 xblock-poll-1.14.0/poll/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.347191 xblock-poll-1.14.0/poll/public/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/css/poll.css
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/css/poll_edit.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.347191 xblock-poll-1.14.0/poll/public/css/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/css/themes/lms.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.347191 xblock-poll-1.14.0/poll/public/handlebars/
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/handlebars/poll_results.handlebars
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/handlebars/poll_studio.handlebars
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/handlebars/survey_results.handlebars
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.347191 xblock-poll-1.14.0/poll/public/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/html/poll.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/html/poll_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/html/survey.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/public/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/poll.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/poll_common.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/poll_edit.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.343191 xblock-poll-1.14.0/poll/public/js/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/public/js/translations/ar/
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/translations/ar/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/public/js/translations/de_DE/
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/translations/de_DE/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/public/js/translations/en/
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/translations/en/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/public/js/translations/eo/
+-rw-r--r--   0 runner    (1001) docker     (127)     8874 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/translations/eo/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/public/js/translations/es_419/
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/translations/es_419/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/public/js/translations/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/translations/fr/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/public/js/translations/fr_CA/
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/translations/fr_CA/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/public/js/translations/he/
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/translations/he/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/public/js/translations/hi/
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/translations/hi/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/public/js/translations/ja_JP/
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/translations/ja_JP/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/public/js/translations/ko_KR/
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/translations/ko_KR/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/public/js/translations/pl/
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/translations/pl/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/public/js/translations/pt_BR/
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/translations/pt_BR/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/public/js/translations/ru/
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/translations/ru/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/public/js/translations/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/translations/zh_CN/textjs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/public/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)    89667 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/public/js/vendor/handlebars.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.343191 xblock-poll-1.14.0/poll/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/ar/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/ar/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.343191 xblock-poll-1.14.0/poll/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.351191 xblock-poll-1.14.0/poll/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/de_DE/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13153 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/de_DE/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/de_DE/LC_MESSAGES/textjs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.343191 xblock-poll-1.14.0/poll/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.355191 xblock-poll-1.14.0/poll/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/en/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/en/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/en/LC_MESSAGES/textjs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.343191 xblock-poll-1.14.0/poll/translations/eo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.355191 xblock-poll-1.14.0/poll/translations/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16541 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/eo/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    20059 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/eo/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/eo/LC_MESSAGES/textjs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.343191 xblock-poll-1.14.0/poll/translations/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.355191 xblock-poll-1.14.0/poll/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/es_419/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13430 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/es_419/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/es_419/LC_MESSAGES/textjs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.343191 xblock-poll-1.14.0/poll/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.355191 xblock-poll-1.14.0/poll/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     9798 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/fr/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13455 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/fr/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/fr/LC_MESSAGES/textjs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.343191 xblock-poll-1.14.0/poll/translations/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.355191 xblock-poll-1.14.0/poll/translations/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/fr_CA/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13546 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/fr_CA/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/fr_CA/LC_MESSAGES/textjs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.343191 xblock-poll-1.14.0/poll/translations/he/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.355191 xblock-poll-1.14.0/poll/translations/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/he/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11311 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/he/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.343191 xblock-poll-1.14.0/poll/translations/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.355191 xblock-poll-1.14.0/poll/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10325 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/ja_JP/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13982 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/ja_JP/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/ja_JP/LC_MESSAGES/textjs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.343191 xblock-poll-1.14.0/poll/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.355191 xblock-poll-1.14.0/poll/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/pt_BR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11273 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/pt_BR/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/translations/pt_BR/LC_MESSAGES/textjs.po
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/poll/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.355191 xblock-poll-1.14.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:30:48.359191 xblock-poll-1.14.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-22 15:30:45.000000 xblock-poll-1.14.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:30:48.359191 xblock-poll-1.14.0/xblock_poll.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18115 2024-05-22 15:30:48.000000 xblock-poll-1.14.0/xblock_poll.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-22 15:30:48.000000 xblock-poll-1.14.0/xblock_poll.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:30:48.000000 xblock-poll-1.14.0/xblock_poll.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 15:30:48.000000 xblock-poll-1.14.0/xblock_poll.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 15:30:48.000000 xblock-poll-1.14.0/xblock_poll.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 15:30:48.000000 xblock-poll-1.14.0/xblock_poll.egg-info/top_level.txt
```

### Comparing `xblock-poll-1.13.0/LICENSE` & `xblock-poll-1.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/README.md` & `xblock-poll-1.14.0/README.md`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/__init__.py` & `xblock-poll-1.14.0/poll/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,7 +18,9 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program in a file in the toplevel directory called
 # "AGPLv3".  If not, see <http://www.gnu.org/licenses/>.
 #
 
 from .poll import PollBlock, SurveyBlock
+
+__version__ = "1.14.0"
```

### Comparing `xblock-poll-1.13.0/poll/poll.py` & `xblock-poll-1.14.0/poll/poll.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,33 +17,35 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Affero
 # General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program in a file in the toplevel directory called
 # "AGPLv3".  If not, see <http://www.gnu.org/licenses/>.
 #
-from __future__ import absolute_import
-
 import functools
 import json
 import time
 from collections import OrderedDict
 
 import pkg_resources
-import six
 from django import utils
 from markdown import markdown
+from web_fragments.fragment import Fragment
 from webob import Response
 from xblock.completable import XBlockCompletionMode
 from xblock.core import XBlock
 from xblock.fields import Boolean, Dict, Integer, List, Scope, String
-from web_fragments.fragment import Fragment
-from xblockutils.publish_event import PublishEventMixin
-from xblockutils.resources import ResourceLoader
-from xblockutils.settings import ThemableXBlockMixin, XBlockWithSettingsMixin
+try:
+    from xblock.utils.publish_event import PublishEventMixin
+    from xblock.utils.resources import ResourceLoader
+    from xblock.utils.settings import ThemableXBlockMixin, XBlockWithSettingsMixin
+except ModuleNotFoundError:  # For backward compatibility with releases older than Quince.
+    from xblockutils.publish_event import PublishEventMixin
+    from xblockutils.resources import ResourceLoader
+    from xblockutils.settings import ThemableXBlockMixin, XBlockWithSettingsMixin
 
 from .utils import DummyTranslationService, _, remove_markdown_and_html_tags
 
 try:
     # pylint: disable=import-error, bad-option-value, ungrouped-imports
     from django.conf import settings
     from api_manager.models import GroupProfile
@@ -132,16 +134,16 @@
         Asynchronously export given data as a CSV file.
         """
         # Launch task
         from .tasks import export_csv_data  # Import here since this is edX LMS specific
 
         # Make sure we nail down our state before sending off an asynchronous task.
         async_result = export_csv_data.delay(
-            six.text_type(getattr(self.scope_ids, 'usage_id', None)),
-            six.text_type(getattr(self.runtime, 'course_id', 'course_id')),
+            str(getattr(self.scope_ids, 'usage_id', None)),
+            str(getattr(self.runtime, 'course_id', 'course_id')),
         )
         if not async_result.ready():
             self.active_export_task_id = async_result.id
         else:
             self._store_export_result(async_result)
 
         return self._get_export_status()
@@ -200,15 +202,15 @@
         self.active_export_task_id = ''
         if task_result.successful():
             if isinstance(task_result.result, dict) and not task_result.result.get('error'):
                 self.last_export_result = task_result.result
             else:
                 self.last_export_result = {'error': u'Unexpected result: {}'.format(repr(task_result.result))}
         else:
-            self.last_export_result = {'error': six.text_type(task_result.result)}
+            self.last_export_result = {'error': str(task_result.result)}
 
     def prepare_data(self):
         """
         Return a two-dimensional list containing cells of data ready for CSV export.
         """
         raise NotImplementedError
 
@@ -269,15 +271,15 @@
         Works both in LMS/Studio and workbench runtimes:
         - In LMS/Studio, use the location.html_id method.
         - In the workbench, use the usage_id.
         """
         if hasattr(self, 'location'):
             return self.location.html_id()  # pylint: disable=no-member
 
-        return six.text_type(self.scope_ids.usage_id)
+        return str(self.scope_ids.usage_id)
 
     def img_alt_mandatory(self):
         """
         Determine whether alt attributes for images are configured to be mandatory.  Defaults to True.
         """
         settings_service = self.runtime.service(self, "settings")
         if not settings_service:
@@ -948,15 +950,15 @@
             'block_name': self.block_name,
             'can_vote': self.can_vote(),
             'submissions_count': self.submissions_count,
             'max_submissions': self.max_submissions,
             'can_view_private_results': self.can_view_private_results(),
             # a11y: Transfer block ID to enable creating unique ids for questions and answers in the template
             'block_id': self._get_block_id(),
-            'usage_id': six.text_type(self.scope_ids.usage_id),
+            'usage_id': str(self.scope_ids.usage_id),
         })
         return self.create_fragment(
             context,
             template="public/html/survey.html",
             css="public/css/poll.css",
             js="public/js/poll.js",
             js_init="SurveyBlock"
```

### Comparing `xblock-poll-1.13.0/poll/public/css/poll.css` & `xblock-poll-1.14.0/poll/public/css/poll.css`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/css/poll_edit.css` & `xblock-poll-1.14.0/poll/public/css/poll_edit.css`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/css/themes/lms.css` & `xblock-poll-1.14.0/poll/public/css/themes/lms.css`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/handlebars/poll_results.handlebars` & `xblock-poll-1.14.0/poll/public/handlebars/poll_results.handlebars`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,14 @@
                 </div>
                 <div class="poll-percent-container">
                     <span class="poll-percent-display{{#if leader}} poll-top-choice{{/if}}">{{percent}}%</span>
                 </div>
             </li>
         {{/each}}
         </ul>
-        <input class="input-main" type="button" name="poll-submit" value="{{gettext "Submit"}}" disabled>
         <div class="poll-footnote">
           {{interpolate (ngettext "Results gathered from {total} respondent." "Results gathered from {total} respondents." total) total=total}}
         </div>
         {{#if feedback}}
             <hr />
             <h3 class="poll-header">{{gettext "Feedback" }}</h3>
             <div class="poll-feedback">
```

### Comparing `xblock-poll-1.13.0/poll/public/handlebars/poll_studio.handlebars` & `xblock-poll-1.14.0/poll/public/handlebars/poll_studio.handlebars`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/handlebars/survey_results.handlebars` & `xblock-poll-1.14.0/poll/public/handlebars/survey_results.handlebars`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,14 @@
                             </span>
                             <span class="percentage">{{percent}}%</span>
                         </td>
                     {{/each}}
                 </tr>
             {{/each}}
         </table>
-        <input class="input-main" type="button" name="poll-submit" value="{{gettext "Submit"}}" disabled>
         <div class="poll-footnote">
             {{interpolate (ngettext "Results gathered from {total} respondent." "Results gathered from {total} respondents." total) total=total}}
         </div>
 
         {{#if feedback}}
             <hr />
             <h3 class="poll-header">{{gettext "Feedback" }}</h3>
```

### Comparing `xblock-poll-1.13.0/poll/public/html/poll.html` & `xblock-poll-1.14.0/poll/public/html/poll.html`

 * *Files 15% similar despite different names*

```diff
@@ -28,15 +28,17 @@
                 </div>
               {% endif %}
               <label class="poll-answer-text" for="poll-{{ block_id }}-answer-{{ key }}">{{ value.label|safe }}</label>
             </div>
           {% endfor %}
         </div>
       </fieldset>
-      <input class="input-main" type="button" name="poll-submit" value="{% trans 'Submit' %}" disabled/>
+      <button type="button" class="submit btn-brand" disabled>
+          <span class="submit-label">{% trans 'Submit' %}</span>
+      </button>
     </form>
 
     <div class="poll-voting-thanks
         {% if not choice or can_vote %}poll-hidden{% endif %}">
       <span>{% trans 'Thank you.' %}</span>
     </div>
 
@@ -57,22 +59,22 @@
       </div>
     {% endif %}
 
 
   </div>
       {% if can_view_private_results %}
       <div class="view-results-button-wrapper">
-        <button class="view-results-button">{% trans 'View results' %}</button>
+          <button type="button" class="view-results-button btn-link btn-small"><span class="show-label">{% trans 'View results' %}</span></button>
       </div>
     {% endif %}
 </div>
 {% if can_view_private_results %}
   {% if not studio_edit %}
     <div class="export-results-button-wrapper">
-      <button class="export-results-button">{% trans "Export results to CSV" %}</button>
-      <button disabled class="download-results-button">{% trans "Download CSV" %}</button>
+      <button class="export-results-button btn-brand">{% trans "Export results to CSV" %}</button>
+      <button disabled class="download-results-button btn-brand">{% trans "Download CSV" %}</button>
       <p class="error-message poll-hidden"></p>
     </div>
   {% else %}
     <p>{% trans "Student data and results CSV available for download in the LMS." %}</p>
   {% endif %}
 {% endif %}
```

### Comparing `xblock-poll-1.13.0/poll/public/html/poll_edit.html` & `xblock-poll-1.14.0/poll/public/html/poll_edit.html`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/html/survey.html` & `xblock-poll-1.14.0/poll/public/html/survey.html`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,17 @@
                             {% endfor %}
                         {% endwith %}
                     </td>
                 {% endfor %}
                 </tr>
             {% endfor %}
             </table>
-            <input class="input-main" type="button" name="poll-submit" value="{% trans 'Submit' %}" disabled />
+            <button type="button" class="submit btn-brand" disabled>
+                <span class="submit-label">{% trans 'Submit' %}</span>
+            </button>
         </form>
         <div class="poll-voting-thanks{% if not choices or can_vote %} poll-hidden{% endif %}"><span>{% trans 'Thank you.' %}</span></div>
         <div class="poll-submissions-count poll-hidden">
             {% blocktrans with submissions_count_s='<span class="poll-current-count">{{ submissions_count }}</span>' max_submissions_s='<span class="poll-max-submissions">{{ max_submissions }}</span>' %}
                 You have used {{ submissions_count_s }} out of {{ max_submissions_s }} submissions.
             {% endblocktrans %}
         </div>
@@ -66,23 +68,23 @@
                     {{feedback|safe}}
                 </div>
             </div>
         {% endif %}
 
         {% if can_view_private_results %}
             <div class="view-results-button-wrapper">
-                <button class="view-results-button">{% trans "View results" %}</button>
+                <button type="button" class="view-results-button btn-link btn-small"><span class="show-label">{% trans 'View results' %}</span></button>
             </div>
         {% endif %}
     </div>
 </div>
 {% if can_view_private_results %}
   {% if not studio_edit %}
     <div class="export-results-button-wrapper">
-      <button class="export-results-button">{% trans "Export results to CSV" %}</button>
-      <button disabled class="download-results-button">{% trans "Download CSV" %}</button>
+      <button class="export-results-button btn-brand">{% trans "Export results to CSV" %}</button>
+      <button disabled class="download-results-button btn-brand">{% trans "Download CSV" %}</button>
       <p class="error-message poll-hidden"></p>
     </div>
   {% else %}
     <p>{% trans "Student data and results CSV available for download in the LMS." %}</p>
   {% endif %}
 {% endif %}
```

#### html2text {}

```diff
@@ -6,25 +6,25 @@
 {{%% iiff qquueessttiioonn..iimmgg %%}}                forloop.counter == answer_count %}
 [[{{{{qquueessttiioonn..iimmgg__aalltt||ddeeffaauulltt__iiff__nnoonnee:: % if question.choice == answer %} checked
 ''''}}}}]]                                {% endif %} {% if question.img_alt %}
 {{%% eennddiiff %%}} {{{{qquueessttiioonn..llaabbeell||ssaaffee}}}}  aria-label="{{question.img_alt}} {
                                      {label}}" {% else %} aria-label="{
                                      {label|safe}}" {% endif %} /> {{label}}
                                      {% endif %} {% endfor %} {% endwith %}
-[Unknown INPUT type]
+{% trans 'Submit' %}
 {% trans 'Thank you.' %}
 {% blocktrans with submissions_count_s='{{ submissions_count }}'
 max_submissions_s='{{ max_submissions }}' %} You have used {
 { submissions_count_s }} out of {{ max_submissions_s }} submissions. {%
 endblocktrans %}
 {% if feedback %}
 ===============================================================================
 ******** {{%% ttrraannss ''FFeeeeddbbaacckk'' %%}} ********
 {{feedback|safe}}
 {% endif %} {% if can_view_private_results %}
-{% trans "View results" %}
+{% trans 'View results' %}
 {% endif %}
 {% if can_view_private_results %} {% if not studio_edit %}
 {% trans "Export results to CSV" %} {% trans "Download CSV" %}
 {% else %}
 {% trans "Student data and results CSV available for download in the LMS." %}
 {% endif %} {% endif %}
```

### Comparing `xblock-poll-1.13.0/poll/public/js/poll.js` & `xblock-poll-1.14.0/poll/public/js/poll.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
 
     this.init = function() {
         // Initialization function used for both Poll Types
         this.voteUrl = runtime.handlerUrl(element, 'vote');
         this.tallyURL = runtime.handlerUrl(element, 'get_results');
         this.csv_url = runtime.handlerUrl(element, 'csv_export');
         this.votedUrl = runtime.handlerUrl(element, 'student_voted');
-        this.submit = $('input[type=button]', element);
+        this.submit = $('button.submit', element);
         this.answers = $('input[type=radio]', element);
         this.errorMessage = $('.error-message', element);
 
         PollCommonUtil.init(Handlebars);
 
         this.resultsTemplate = Handlebars.compile($("." + pollType + "-results-template", element).html());
```

### Comparing `xblock-poll-1.13.0/poll/public/js/poll_common.js` & `xblock-poll-1.14.0/poll/public/js/poll_common.js`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/js/poll_edit.js` & `xblock-poll-1.14.0/poll/public/js/poll_edit.js`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/js/translations/ar/textjs.js` & `xblock-poll-1.14.0/poll/public/js/translations/ar/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/js/translations/de_DE/textjs.js` & `xblock-poll-1.14.0/poll/public/js/translations/de_DE/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/js/translations/en/textjs.js` & `xblock-poll-1.14.0/poll/public/js/translations/en/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/js/translations/eo/textjs.js` & `xblock-poll-1.14.0/poll/public/js/translations/eo/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/js/translations/es_419/textjs.js` & `xblock-poll-1.14.0/poll/public/js/translations/es_419/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/js/translations/fr/textjs.js` & `xblock-poll-1.14.0/poll/public/js/translations/fr/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/js/translations/fr_CA/textjs.js` & `xblock-poll-1.14.0/poll/public/js/translations/fr_CA/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/js/translations/he/textjs.js` & `xblock-poll-1.14.0/poll/public/js/translations/he/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/js/translations/hi/textjs.js` & `xblock-poll-1.14.0/poll/public/js/translations/hi/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/js/translations/ja_JP/textjs.js` & `xblock-poll-1.14.0/poll/public/js/translations/ja_JP/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/js/translations/ko_KR/textjs.js` & `xblock-poll-1.14.0/poll/public/js/translations/ko_KR/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/js/translations/pl/textjs.js` & `xblock-poll-1.14.0/poll/public/js/translations/pl/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/js/translations/pt_BR/textjs.js` & `xblock-poll-1.14.0/poll/public/js/translations/pt_BR/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/js/translations/ru/textjs.js` & `xblock-poll-1.14.0/poll/public/js/translations/ru/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/js/translations/zh_CN/textjs.js` & `xblock-poll-1.14.0/poll/public/js/translations/zh_CN/textjs.js`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/public/js/vendor/handlebars.js` & `xblock-poll-1.14.0/poll/public/js/vendor/handlebars.js`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/settings.py` & `xblock-poll-1.14.0/poll/settings.py`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/tasks.py` & `xblock-poll-1.14.0/poll/tasks.py`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/ar/LC_MESSAGES/text.mo` & `xblock-poll-1.14.0/poll/translations/ar/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/ar/LC_MESSAGES/text.po` & `xblock-poll-1.14.0/poll/translations/ar/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/config.yaml` & `xblock-poll-1.14.0/poll/translations/config.yaml`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/de_DE/LC_MESSAGES/text.mo` & `xblock-poll-1.14.0/poll/translations/de_DE/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/de_DE/LC_MESSAGES/text.po` & `xblock-poll-1.14.0/poll/translations/de_DE/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/de_DE/LC_MESSAGES/textjs.po` & `xblock-poll-1.14.0/poll/translations/de_DE/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/en/LC_MESSAGES/text.po` & `xblock-poll-1.14.0/poll/translations/en/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/en/LC_MESSAGES/textjs.po` & `xblock-poll-1.14.0/poll/translations/en/LC_MESSAGES/textjs.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
-#: poll/public/handlebars/survey_results.handlebars:4
 #: poll/public/handlebars/poll_results.handlebars:5
+#: poll/public/handlebars/survey_results.handlebars:4
 msgid "Results"
 msgstr ""
 
-#: poll/public/handlebars/survey_results.handlebars:39
-#: poll/public/handlebars/poll_results.handlebars:31
-msgid "Submit"
-msgstr ""
-
-#: poll/public/handlebars/survey_results.handlebars:41
-#: poll/public/handlebars/poll_results.handlebars:33
+#: poll/public/handlebars/poll_results.handlebars:32
+#: poll/public/handlebars/survey_results.handlebars:40
 msgid "Results gathered from {total} respondent."
 msgid_plural "Results gathered from {total} respondents."
 msgstr[0] ""
 msgstr[1] ""
 
-#: poll/public/handlebars/survey_results.handlebars:46
-#: poll/public/handlebars/poll_results.handlebars:37
+#: poll/public/handlebars/poll_results.handlebars:36
+#: poll/public/handlebars/survey_results.handlebars:45
 msgid "Feedback"
 msgstr ""
 
 #: poll/public/handlebars/poll_studio.handlebars:6
 msgid "move poll up"
 msgstr ""
 
@@ -59,8 +54,8 @@
 
 #: poll/public/handlebars/poll_studio.handlebars:27
 msgid ""
 "This must have an image URL or text, and can have both.  If you add an "
 "image, you must also provide an alternative text that describes the image "
 "in a way that would allow someone to answer the poll if the image did not "
 "load."
-msgstr ""
+msgstr ""
```

### Comparing `xblock-poll-1.13.0/poll/translations/eo/LC_MESSAGES/text.mo` & `xblock-poll-1.14.0/poll/translations/eo/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/eo/LC_MESSAGES/text.po` & `xblock-poll-1.14.0/poll/translations/eo/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/eo/LC_MESSAGES/textjs.po` & `xblock-poll-1.14.0/poll/translations/eo/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/es_419/LC_MESSAGES/text.mo` & `xblock-poll-1.14.0/poll/translations/es_419/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/es_419/LC_MESSAGES/text.po` & `xblock-poll-1.14.0/poll/translations/es_419/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/es_419/LC_MESSAGES/textjs.po` & `xblock-poll-1.14.0/poll/translations/es_419/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/fr/LC_MESSAGES/text.mo` & `xblock-poll-1.14.0/poll/translations/fr/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/fr/LC_MESSAGES/text.po` & `xblock-poll-1.14.0/poll/translations/fr/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/fr/LC_MESSAGES/textjs.po` & `xblock-poll-1.14.0/poll/translations/fr/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/fr_CA/LC_MESSAGES/text.mo` & `xblock-poll-1.14.0/poll/translations/fr_CA/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/fr_CA/LC_MESSAGES/text.po` & `xblock-poll-1.14.0/poll/translations/fr_CA/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/fr_CA/LC_MESSAGES/textjs.po` & `xblock-poll-1.14.0/poll/translations/fr_CA/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/he/LC_MESSAGES/text.mo` & `xblock-poll-1.14.0/poll/translations/he/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/he/LC_MESSAGES/text.po` & `xblock-poll-1.14.0/poll/translations/he/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/ja_JP/LC_MESSAGES/text.mo` & `xblock-poll-1.14.0/poll/translations/ja_JP/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/ja_JP/LC_MESSAGES/text.po` & `xblock-poll-1.14.0/poll/translations/ja_JP/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/ja_JP/LC_MESSAGES/textjs.po` & `xblock-poll-1.14.0/poll/translations/ja_JP/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/pt_BR/LC_MESSAGES/text.mo` & `xblock-poll-1.14.0/poll/translations/pt_BR/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/pt_BR/LC_MESSAGES/text.po` & `xblock-poll-1.14.0/poll/translations/pt_BR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/translations/pt_BR/LC_MESSAGES/textjs.po` & `xblock-poll-1.14.0/poll/translations/pt_BR/LC_MESSAGES/textjs.po`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/poll/utils.py` & `xblock-poll-1.14.0/poll/utils.py`

 * *Files identical despite different names*

### Comparing `xblock-poll-1.13.0/xblock_poll.egg-info/SOURCES.txt` & `xblock-poll-1.14.0/xblock_poll.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.py
 poll/__init__.py
 poll/poll.py
 poll/settings.py
 poll/tasks.py
 poll/utils.py
@@ -59,13 +60,15 @@
 poll/translations/he/LC_MESSAGES/text.po
 poll/translations/ja_JP/LC_MESSAGES/text.mo
 poll/translations/ja_JP/LC_MESSAGES/text.po
 poll/translations/ja_JP/LC_MESSAGES/textjs.po
 poll/translations/pt_BR/LC_MESSAGES/text.mo
 poll/translations/pt_BR/LC_MESSAGES/text.po
 poll/translations/pt_BR/LC_MESSAGES/textjs.po
+requirements/base.in
+requirements/constraints.txt
 xblock_poll.egg-info/PKG-INFO
 xblock_poll.egg-info/SOURCES.txt
 xblock_poll.egg-info/dependency_links.txt
 xblock_poll.egg-info/entry_points.txt
 xblock_poll.egg-info/requires.txt
 xblock_poll.egg-info/top_level.txt
```

