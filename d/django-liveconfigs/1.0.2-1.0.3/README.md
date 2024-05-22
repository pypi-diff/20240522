# Comparing `tmp/django_liveconfigs-1.0.2.tar.gz` & `tmp/django_liveconfigs-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_liveconfigs-1.0.2.tar", last modified: Tue May 21 19:24:01 2024, max compression
+gzip compressed data, was "django_liveconfigs-1.0.3.tar", last modified: Wed May 22 11:53:38 2024, max compression
```

## Comparing `django_liveconfigs-1.0.2.tar` & `django_liveconfigs-1.0.3.tar`

### file list

```diff
@@ -1,40 +1,44 @@
-drwxrwxr-x   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2024-05-21 19:24:01.350261 django_liveconfigs-1.0.2/
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     1488 2024-05-21 19:13:23.000000 django_liveconfigs-1.0.2/LICENSE
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)       58 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.2/MANIFEST.in
--rw-r--r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)    14368 2024-05-21 19:24:01.350261 django_liveconfigs-1.0.2/PKG-INFO
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)    10616 2024-05-21 19:13:30.000000 django_liveconfigs-1.0.2/README.md
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     2219 2024-05-21 19:13:30.000000 django_liveconfigs-1.0.2/pyproject.toml
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)       38 2024-05-21 19:24:01.350261 django_liveconfigs-1.0.2/setup.cfg
-drwxrwxr-x   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2024-05-21 19:24:01.342261 django_liveconfigs-1.0.2/src/
-drwxrwxr-x   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2024-05-21 19:24:01.350261 django_liveconfigs-1.0.2/src/django_liveconfigs.egg-info/
--rw-r--r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)    14368 2024-05-21 19:24:01.000000 django_liveconfigs-1.0.2/src/django_liveconfigs.egg-info/PKG-INFO
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      976 2024-05-21 19:24:01.000000 django_liveconfigs-1.0.2/src/django_liveconfigs.egg-info/SOURCES.txt
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        1 2024-05-21 19:24:01.000000 django_liveconfigs-1.0.2/src/django_liveconfigs.egg-info/dependency_links.txt
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      112 2024-05-21 19:24:01.000000 django_liveconfigs-1.0.2/src/django_liveconfigs.egg-info/requires.txt
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)       12 2024-05-21 19:24:01.000000 django_liveconfigs-1.0.2/src/django_liveconfigs.egg-info/top_level.txt
-drwxrwxr-x   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2024-05-21 19:24:01.350261 django_liveconfigs-1.0.2/src/liveconfigs/
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.2/src/liveconfigs/__init__.py
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     2671 2024-05-21 19:13:30.000000 django_liveconfigs-1.0.2/src/liveconfigs/admin.py
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)       97 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.2/src/liveconfigs/apps.py
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     3447 2024-05-21 19:13:30.000000 django_liveconfigs-1.0.2/src/liveconfigs/filters.py
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     1874 2024-05-21 19:13:30.000000 django_liveconfigs-1.0.2/src/liveconfigs/forms.py
-drwxrwxr-x   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2024-05-21 19:24:01.350261 django_liveconfigs-1.0.2/src/liveconfigs/management/
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.2/src/liveconfigs/management/__init__.py
-drwxrwxr-x   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2024-05-21 19:24:01.350261 django_liveconfigs-1.0.2/src/liveconfigs/management/commands/
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.2/src/liveconfigs/management/commands/__init__.py
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     1015 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.2/src/liveconfigs/management/commands/delete_unused_configs.py
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     2226 2024-05-21 19:13:23.000000 django_liveconfigs-1.0.2/src/liveconfigs/management/commands/load_config.py
-drwxrwxr-x   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2024-05-21 19:24:01.350261 django_liveconfigs-1.0.2/src/liveconfigs/migrations/
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     1101 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.2/src/liveconfigs/migrations/0001_initial.py
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.2/src/liveconfigs/migrations/__init__.py
-drwxrwxr-x   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2024-05-21 19:24:01.350261 django_liveconfigs-1.0.2/src/liveconfigs/models/
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      323 2024-05-21 19:13:23.000000 django_liveconfigs-1.0.2/src/liveconfigs/models/__init__.py
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     4991 2024-05-21 19:13:23.000000 django_liveconfigs-1.0.2/src/liveconfigs/models/descriptors.py
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     2070 2024-05-21 19:13:30.000000 django_liveconfigs-1.0.2/src/liveconfigs/models/models.py
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      446 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.2/src/liveconfigs/serializers.py
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)       72 2024-02-20 13:46:32.000000 django_liveconfigs-1.0.2/src/liveconfigs/signals.py
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      414 2024-02-20 13:46:32.000000 django_liveconfigs-1.0.2/src/liveconfigs/tasks.py
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      233 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.2/src/liveconfigs/urls.py
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      901 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.2/src/liveconfigs/utils.py
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     1323 2024-02-20 13:46:32.000000 django_liveconfigs-1.0.2/src/liveconfigs/validators.py
--rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      774 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.2/src/liveconfigs/views.py
+drwxrwxr-x   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2024-05-22 11:53:38.106963 django_liveconfigs-1.0.3/
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     1488 2024-05-21 19:13:23.000000 django_liveconfigs-1.0.3/LICENSE
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)       58 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.3/MANIFEST.in
+-rw-r--r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)    14694 2024-05-22 11:53:38.106963 django_liveconfigs-1.0.3/PKG-INFO
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)    10940 2024-05-22 11:52:33.000000 django_liveconfigs-1.0.3/README.md
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     2221 2024-05-22 11:52:33.000000 django_liveconfigs-1.0.3/pyproject.toml
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)       38 2024-05-22 11:53:38.106963 django_liveconfigs-1.0.3/setup.cfg
+drwxrwxr-x   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2024-05-22 11:53:38.102963 django_liveconfigs-1.0.3/src/
+drwxrwxr-x   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2024-05-22 11:53:38.106963 django_liveconfigs-1.0.3/src/django_liveconfigs.egg-info/
+-rw-r--r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)    14694 2024-05-22 11:53:38.000000 django_liveconfigs-1.0.3/src/django_liveconfigs.egg-info/PKG-INFO
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     1190 2024-05-22 11:53:38.000000 django_liveconfigs-1.0.3/src/django_liveconfigs.egg-info/SOURCES.txt
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        1 2024-05-22 11:53:38.000000 django_liveconfigs-1.0.3/src/django_liveconfigs.egg-info/dependency_links.txt
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      114 2024-05-22 11:53:38.000000 django_liveconfigs-1.0.3/src/django_liveconfigs.egg-info/requires.txt
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)       12 2024-05-22 11:53:38.000000 django_liveconfigs-1.0.3/src/django_liveconfigs.egg-info/top_level.txt
+drwxrwxr-x   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2024-05-22 11:53:38.106963 django_liveconfigs-1.0.3/src/liveconfigs/
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.3/src/liveconfigs/__init__.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     2766 2024-05-22 11:52:33.000000 django_liveconfigs-1.0.3/src/liveconfigs/admin.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)       97 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.3/src/liveconfigs/apps.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     3450 2024-05-22 11:52:33.000000 django_liveconfigs-1.0.3/src/liveconfigs/filters.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     1718 2024-05-22 11:52:33.000000 django_liveconfigs-1.0.3/src/liveconfigs/forms.py
+drwxrwxr-x   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2024-05-22 11:53:38.106963 django_liveconfigs-1.0.3/src/liveconfigs/management/
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.3/src/liveconfigs/management/__init__.py
+drwxrwxr-x   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2024-05-22 11:53:38.106963 django_liveconfigs-1.0.3/src/liveconfigs/management/commands/
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.3/src/liveconfigs/management/commands/__init__.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     1015 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.3/src/liveconfigs/management/commands/delete_unused_configs.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     2294 2024-05-22 11:52:33.000000 django_liveconfigs-1.0.3/src/liveconfigs/management/commands/load_config.py
+drwxrwxr-x   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2024-05-22 11:53:38.106963 django_liveconfigs-1.0.3/src/liveconfigs/migrations/
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     1101 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.3/src/liveconfigs/migrations/0001_initial.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      940 2024-05-22 11:52:33.000000 django_liveconfigs-1.0.3/src/liveconfigs/migrations/0002_historyevent.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      400 2024-05-22 11:52:33.000000 django_liveconfigs-1.0.3/src/liveconfigs/migrations/0003_configrow_default_value.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      338 2024-05-22 11:52:33.000000 django_liveconfigs-1.0.3/src/liveconfigs/migrations/0004_remove_configrow_tags.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      400 2024-05-22 11:52:33.000000 django_liveconfigs-1.0.3/src/liveconfigs/migrations/0005_configrow_tags.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.3/src/liveconfigs/migrations/__init__.py
+drwxrwxr-x   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)        0 2024-05-22 11:53:38.106963 django_liveconfigs-1.0.3/src/liveconfigs/models/
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      353 2024-05-22 11:52:33.000000 django_liveconfigs-1.0.3/src/liveconfigs/models/__init__.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     5104 2024-05-22 11:52:33.000000 django_liveconfigs-1.0.3/src/liveconfigs/models/descriptors.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     2346 2024-05-22 11:52:33.000000 django_liveconfigs-1.0.3/src/liveconfigs/models/models.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      446 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.3/src/liveconfigs/serializers.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)       72 2024-02-20 13:46:32.000000 django_liveconfigs-1.0.3/src/liveconfigs/signals.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      414 2024-02-20 13:46:32.000000 django_liveconfigs-1.0.3/src/liveconfigs/tasks.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      233 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.3/src/liveconfigs/urls.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      901 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.3/src/liveconfigs/utils.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)     1323 2024-02-20 13:46:32.000000 django_liveconfigs-1.0.3/src/liveconfigs/validators.py
+-rw-rw-r--   0 evgeniykatsevman  (1001) evgeniykatsevman  (1001)      774 2023-11-23 13:07:51.000000 django_liveconfigs-1.0.3/src/liveconfigs/views.py
```

### Comparing `django_liveconfigs-1.0.2/LICENSE` & `django_liveconfigs-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_liveconfigs-1.0.2/PKG-INFO` & `django_liveconfigs-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-liveconfigs
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple powerful and convenient configs for Django
 Author-email: Evgenii Katsevman <eugene.katsevman@gmail.com>, Mihail Mayorov <mihail1-m1@yandex.ru>, Alexander Ignatov <goodwinsis@yandex.ru>, Alexander Mironov <mironov.miet@gmail.com>, Timur Timerkhanov <timurgrunge@gmail.com>, Ivan Shevyakov <iashevyakov@mail.ru>, Vladilav Nechaev <vladislavtv1@gmail.com>, Denis Dudnik <Denis.Dudnik@gmail.com>
 Maintainer-email: Denis Dudnik <Denis.Dudnik@gmail.com>
 License: Copyright (c) 2019-2024 F5Devs <https://f5devs.ru>
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
@@ -52,15 +52,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=3.2
-Requires-Dist: Django<=5
+Requires-Dist: Django<=5.1
 Requires-Dist: djangorestframework>=3.13.1
 Requires-Dist: typeguard>=3.0.0
 Requires-Dist: typeguard<=4.1.5
 Requires-Dist: django-import-export>=2.8.0
 
 # LiveConfigs
 
@@ -82,15 +82,15 @@
 ```python
 if MyConfig.IS_FEATURE_ENABLED:
    print('feature is enabled and feature value is', MyConfig.NEW_FEATURE_VALUE)
 ```
 
 Меняем через админку!
 
-![Экран редактирования конфига](/images/change_config.jpg)
+![Экран редактирования конфига](https://github.com/factory5group/django-liveconfigs/blob/main/images/change_config.jpg?raw=true)
 
 
 ## Термины
 + __настройка__, __конфиг__ - одно типизированное именованное значение
 + __класс конфига__, __группа настроек__ - настройки, объединенные в один класс python
 + __топик__ - общая "тема" для группы настроек, по которой можно производить поиск настроек в админке.
 У разных групп настроек в принципе может быть один и тот же топик
@@ -111,15 +111,15 @@
 + __теги__ и __топики__ для группировки и поиска
 + документацию
 + автоматическую загрузку новых конфигов в бд
 + валидацию при изменении (типы и значения)
 + сохранение даты последних изменений и чтений конфигов
 + импорт и экспорт (удобно для тестирования системы)
 
-![Экран поиска и фильтрации конфигов](/images/filter_config.jpg)
+![Экран поиска и фильтрации конфигов](https://github.com/factory5group/django-liveconfigs/blob/main/images/filter_config.jpg?raw=true)
 
 ## Как начать пользоваться
 
 1. Добавьте "liveconfigs" в INSTALLED_APPS в settings:
 ```
     INSTALLED_APPS = [
         ...,
@@ -131,14 +131,15 @@
 ```
     # liveconfigs settings
     # Максимальная длина текста в значении конфига при которой отображать поле редактирования конфига как textinput
     # При длине текста в значении конфига большей этого значения - отображать поле редактирования конфига как textarea
     LC_MAX_STR_LENGTH_DISPLAYED_AS_TEXTINPUT = 50
     LC_ENABLE_PRETTY_INPUT = True
     LIVECONFIGS_SYNCWRITE = True    # sync write mode
+    LC_CACHE_TTL = 1    # cache TTL in seconds (default = 1)
 ```
 
 3. Заведите себе файл собственно с конфигами, например `config/config.py`
 ```python
 from liveconfigs import models
 from liveconfigs.validators import greater_than
 from enum import Enum
@@ -262,10 +263,12 @@
  ```
 
  3. Если используете не Celery, то адаптируйте этот код под ваш случай
 
 ## Остались вопросы?
 + Посмотрите примеры использования конфигов: https://github.com/factory5group/django-liveconfigs-example/
 
-+ Примеры валидаторов : `validators.py` в https://github.com/factory5group/django-liveconfigs-example/
++ Примеры использования валидаторов : https://github.com/factory5group/django-liveconfigs-example/
+
++ Примеры валидаторов : `validators.py` в https://github.com/factory5group/django-liveconfigs/
 
 + Напишите нам!
```

### Comparing `django_liveconfigs-1.0.2/README.md` & `django_liveconfigs-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ```python
 if MyConfig.IS_FEATURE_ENABLED:
    print('feature is enabled and feature value is', MyConfig.NEW_FEATURE_VALUE)
 ```
 
 Меняем через админку!
 
-![Экран редактирования конфига](/images/change_config.jpg)
+![Экран редактирования конфига](https://github.com/factory5group/django-liveconfigs/blob/main/images/change_config.jpg?raw=true)
 
 
 ## Термины
 + __настройка__, __конфиг__ - одно типизированное именованное значение
 + __класс конфига__, __группа настроек__ - настройки, объединенные в один класс python
 + __топик__ - общая "тема" для группы настроек, по которой можно производить поиск настроек в админке.
 У разных групп настроек в принципе может быть один и тот же топик
@@ -47,15 +47,15 @@
 + __теги__ и __топики__ для группировки и поиска
 + документацию
 + автоматическую загрузку новых конфигов в бд
 + валидацию при изменении (типы и значения)
 + сохранение даты последних изменений и чтений конфигов
 + импорт и экспорт (удобно для тестирования системы)
 
-![Экран поиска и фильтрации конфигов](/images/filter_config.jpg)
+![Экран поиска и фильтрации конфигов](https://github.com/factory5group/django-liveconfigs/blob/main/images/filter_config.jpg?raw=true)
 
 ## Как начать пользоваться
 
 1. Добавьте "liveconfigs" в INSTALLED_APPS в settings:
 ```
     INSTALLED_APPS = [
         ...,
@@ -67,14 +67,15 @@
 ```
     # liveconfigs settings
     # Максимальная длина текста в значении конфига при которой отображать поле редактирования конфига как textinput
     # При длине текста в значении конфига большей этого значения - отображать поле редактирования конфига как textarea
     LC_MAX_STR_LENGTH_DISPLAYED_AS_TEXTINPUT = 50
     LC_ENABLE_PRETTY_INPUT = True
     LIVECONFIGS_SYNCWRITE = True    # sync write mode
+    LC_CACHE_TTL = 1    # cache TTL in seconds (default = 1)
 ```
 
 3. Заведите себе файл собственно с конфигами, например `config/config.py`
 ```python
 from liveconfigs import models
 from liveconfigs.validators import greater_than
 from enum import Enum
@@ -198,10 +199,12 @@
  ```
 
  3. Если используете не Celery, то адаптируйте этот код под ваш случай
 
 ## Остались вопросы?
 + Посмотрите примеры использования конфигов: https://github.com/factory5group/django-liveconfigs-example/
 
-+ Примеры валидаторов : `validators.py` в https://github.com/factory5group/django-liveconfigs-example/
++ Примеры использования валидаторов : https://github.com/factory5group/django-liveconfigs-example/
+
++ Примеры валидаторов : `validators.py` в https://github.com/factory5group/django-liveconfigs/
 
 + Напишите нам!
```

### Comparing `django_liveconfigs-1.0.2/pyproject.toml` & `django_liveconfigs-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-liveconfigs"
-version = "1.0.2"
+version = "1.0.3"
 description = "Simple powerful and convenient configs for Django"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
   {name = "Evgenii Katsevman", email = "eugene.katsevman@gmail.com"},
   {name = "Mihail Mayorov", email = "mihail1-m1@yandex.ru"},
@@ -39,15 +39,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
   "Django>=3.2",
-  "Django<=5",
+  "Django<=5.1",
   "djangorestframework>=3.13.1",
   "typeguard>=3.0.0",
   "typeguard<=4.1.5",
   "django-import-export>=2.8.0",
 ]
 
 [project.urls]
```

### Comparing `django_liveconfigs-1.0.2/src/django_liveconfigs.egg-info/PKG-INFO` & `django_liveconfigs-1.0.3/src/django_liveconfigs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-liveconfigs
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple powerful and convenient configs for Django
 Author-email: Evgenii Katsevman <eugene.katsevman@gmail.com>, Mihail Mayorov <mihail1-m1@yandex.ru>, Alexander Ignatov <goodwinsis@yandex.ru>, Alexander Mironov <mironov.miet@gmail.com>, Timur Timerkhanov <timurgrunge@gmail.com>, Ivan Shevyakov <iashevyakov@mail.ru>, Vladilav Nechaev <vladislavtv1@gmail.com>, Denis Dudnik <Denis.Dudnik@gmail.com>
 Maintainer-email: Denis Dudnik <Denis.Dudnik@gmail.com>
 License: Copyright (c) 2019-2024 F5Devs <https://f5devs.ru>
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
@@ -52,15 +52,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=3.2
-Requires-Dist: Django<=5
+Requires-Dist: Django<=5.1
 Requires-Dist: djangorestframework>=3.13.1
 Requires-Dist: typeguard>=3.0.0
 Requires-Dist: typeguard<=4.1.5
 Requires-Dist: django-import-export>=2.8.0
 
 # LiveConfigs
 
@@ -82,15 +82,15 @@
 ```python
 if MyConfig.IS_FEATURE_ENABLED:
    print('feature is enabled and feature value is', MyConfig.NEW_FEATURE_VALUE)
 ```
 
 Меняем через админку!
 
-![Экран редактирования конфига](/images/change_config.jpg)
+![Экран редактирования конфига](https://github.com/factory5group/django-liveconfigs/blob/main/images/change_config.jpg?raw=true)
 
 
 ## Термины
 + __настройка__, __конфиг__ - одно типизированное именованное значение
 + __класс конфига__, __группа настроек__ - настройки, объединенные в один класс python
 + __топик__ - общая "тема" для группы настроек, по которой можно производить поиск настроек в админке.
 У разных групп настроек в принципе может быть один и тот же топик
@@ -111,15 +111,15 @@
 + __теги__ и __топики__ для группировки и поиска
 + документацию
 + автоматическую загрузку новых конфигов в бд
 + валидацию при изменении (типы и значения)
 + сохранение даты последних изменений и чтений конфигов
 + импорт и экспорт (удобно для тестирования системы)
 
-![Экран поиска и фильтрации конфигов](/images/filter_config.jpg)
+![Экран поиска и фильтрации конфигов](https://github.com/factory5group/django-liveconfigs/blob/main/images/filter_config.jpg?raw=true)
 
 ## Как начать пользоваться
 
 1. Добавьте "liveconfigs" в INSTALLED_APPS в settings:
 ```
     INSTALLED_APPS = [
         ...,
@@ -131,14 +131,15 @@
 ```
     # liveconfigs settings
     # Максимальная длина текста в значении конфига при которой отображать поле редактирования конфига как textinput
     # При длине текста в значении конфига большей этого значения - отображать поле редактирования конфига как textarea
     LC_MAX_STR_LENGTH_DISPLAYED_AS_TEXTINPUT = 50
     LC_ENABLE_PRETTY_INPUT = True
     LIVECONFIGS_SYNCWRITE = True    # sync write mode
+    LC_CACHE_TTL = 1    # cache TTL in seconds (default = 1)
 ```
 
 3. Заведите себе файл собственно с конфигами, например `config/config.py`
 ```python
 from liveconfigs import models
 from liveconfigs.validators import greater_than
 from enum import Enum
@@ -262,10 +263,12 @@
  ```
 
  3. Если используете не Celery, то адаптируйте этот код под ваш случай
 
 ## Остались вопросы?
 + Посмотрите примеры использования конфигов: https://github.com/factory5group/django-liveconfigs-example/
 
-+ Примеры валидаторов : `validators.py` в https://github.com/factory5group/django-liveconfigs-example/
++ Примеры использования валидаторов : https://github.com/factory5group/django-liveconfigs-example/
+
++ Примеры валидаторов : `validators.py` в https://github.com/factory5group/django-liveconfigs/
 
 + Напишите нам!
```

### Comparing `django_liveconfigs-1.0.2/src/django_liveconfigs.egg-info/SOURCES.txt` & `django_liveconfigs-1.0.3/src/django_liveconfigs.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -20,11 +20,15 @@
 src/liveconfigs/validators.py
 src/liveconfigs/views.py
 src/liveconfigs/management/__init__.py
 src/liveconfigs/management/commands/__init__.py
 src/liveconfigs/management/commands/delete_unused_configs.py
 src/liveconfigs/management/commands/load_config.py
 src/liveconfigs/migrations/0001_initial.py
+src/liveconfigs/migrations/0002_historyevent.py
+src/liveconfigs/migrations/0003_configrow_default_value.py
+src/liveconfigs/migrations/0004_remove_configrow_tags.py
+src/liveconfigs/migrations/0005_configrow_tags.py
 src/liveconfigs/migrations/__init__.py
 src/liveconfigs/models/__init__.py
 src/liveconfigs/models/descriptors.py
 src/liveconfigs/models/models.py
```

### Comparing `django_liveconfigs-1.0.2/src/liveconfigs/admin.py` & `django_liveconfigs-1.0.3/src/liveconfigs/admin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import datetime as dt
 import json
 
 from django.contrib import admin
+from django.utils import timezone
 from import_export import formats, resources
 from import_export.admin import ImportExportModelAdmin
 from import_export.fields import Field
 from tablib import Dataset
 
 from .filters import TagsListFilter
 from .forms import ConfigRowForm
-from .models import ConfigRow
+from .models import ConfigRow, HistoryEvent
 from .utils import get_excluded_rows
 
 
 class ConfigRowResource(resources.ModelResource):
     value_ = Field(column_name='value')
 
     class Meta:
@@ -44,28 +44,27 @@
         )
 
 
 class ConfigRowAdmin(ImportExportModelAdmin):
     form = ConfigRowForm
     formats = [formats.base_formats.JSON]
     resource_class = ConfigRowResource
-    list_display = ('name', 'value', 'description', 'topic',
-                    'tags', 'last_read', 'last_set')
+    list_display = ('name', 'value', 'default_value', 'description', 'topic', 'tags', 'last_read', 'last_set')
     list_filter = ("topic", TagsListFilter,)
-    readonly_fields = ('name', 'description', 'topic',
-                       'tags', 'last_read', 'last_set')
+    readonly_fields = ('name', 'description', 'topic', 'tags', 'last_read', 'last_set', 'default_value')
     search_fields = ('name', 'description', 'topic', 'tags')
 
-    def get_export_queryset(self, request):
-        qs = ConfigRow.objects.all()
-        excluded_config_rows = get_excluded_rows()
-        return qs.exclude(name__in=excluded_config_rows)
-
     def save_model(self, request, obj, form, change):
-        """
-        Given a model instance save it to the database.
-        """
-        obj.last_set = dt.datetime.now(tz=dt.timezone.utc)
-        obj.save()
+        user = request.user
+        super().save_model(request, obj, form, change)
+        HistoryEvent.objects.create(name=obj.name, value=obj.value, edit_at=timezone.now(), edit_by=user)
+
+
+@admin.register(HistoryEvent)
+class HistoryEventAdmin(admin.ModelAdmin):
+    list_display = ("name", "value", "edit_at", "edit_by")
+    readonly_fields = list_display
+    search_fields = ("name",)
+    list_filter = ("name", "edit_at")
 
 
 admin.site.register(ConfigRow, ConfigRowAdmin)
```

### Comparing `django_liveconfigs-1.0.2/src/liveconfigs/filters.py` & `django_liveconfigs-1.0.3/src/liveconfigs/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.contrib.admin import SimpleListFilter
 from django.utils.translation import gettext_lazy as _
 
 
-class ArrayFieldListFilter(SimpleListFilter):
+class JSONFieldListFilter(SimpleListFilter):
     """An admin list filter for ArrayFields."""
 
     def lookups(self, request, model_admin):
         """Return the filtered queryset."""
         queryset_values = model_admin.model.objects.values_list(
             self.parameter_name, flat=True
         )
@@ -81,16 +81,16 @@
     def queryset(self, request, queryset):
         """Return the filtered queryset."""
         lookup_value = self.value()
         if lookup_value:
             lookup_filter = (
                 {"{}__isnull".format(self.parameter_name): True}
                 if lookup_value == "null"
-                else {"{}__overlap".format(self.parameter_name): lookup_value}
+                else {"{}__has_any_keys".format(self.parameter_name): lookup_value}
             )
             queryset = queryset.filter(**lookup_filter)
         return queryset
 
 
-class TagsListFilter(ArrayFieldListFilter):
+class TagsListFilter(JSONFieldListFilter):
     title = "tags"
     parameter_name = "tags"
```

### Comparing `django_liveconfigs-1.0.2/src/liveconfigs/forms.py` & `django_liveconfigs-1.0.3/src/liveconfigs/forms.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,31 +18,27 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         instance_type = self.instance.registered_row_types.get(self.instance.name)
         if settings.LC_ENABLE_PRETTY_INPUT and not isinstance(instance_type, UnionType):
             max_len = settings.LC_MAX_STR_LENGTH_DISPLAYED_AS_TEXTINPUT or 50
             val = self.instance.value
-            if isinstance(val, bool):
+            if instance_type is bool:
                 self.fields["value"] = forms.BooleanField(
                     required=False,
                 )
-            elif isinstance(val, int):
+            elif instance_type is int:
                 self.fields["value"] = forms.IntegerField(
                     required=False,
                 )
-            elif isinstance(val, float):
+            elif instance_type is float:
                 self.fields["value"] = forms.FloatField(
                     required=False,
                     widget=forms.NumberInput(attrs={"step": "0.1"}),
                 )
-            elif isinstance(val, Decimal):
-                self.fields["value"] = forms.DecimalField(
-                    required=False,
-                )
-            elif isinstance(val, str):
+            elif instance_type is str:
                 if len(val) <= max_len:
                     self.fields["value"] = forms.CharField(
                         required=False, widget=forms.TextInput({"size": max_len})
                     )
             elif isinstance(val, (list, dict)):
                 self.fields["value"] = forms.JSONField(encoder=PrettyJSONEncoder)
```

### Comparing `django_liveconfigs-1.0.2/src/liveconfigs/management/commands/delete_unused_configs.py` & `django_liveconfigs-1.0.3/src/liveconfigs/management/commands/delete_unused_configs.py`

 * *Files identical despite different names*

### Comparing `django_liveconfigs-1.0.2/src/liveconfigs/management/commands/load_config.py` & `django_liveconfigs-1.0.3/src/liveconfigs/management/commands/load_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,33 +16,34 @@
         db_row = ConfigRow.objects.get(name=instance_row.config_name)
         if reset or db_row.value is None:
             db_row.value = instance_row.last_value
             db_row.last_set = dt.datetime.now(tz=dt.timezone.utc)
         db_row.description = instance_row.description
         db_row.tags = instance_row.tags
         db_row.topic = instance_row.topic
+        db_row.default_value = instance_row.default_value
         db_row.save()
     except exceptions.ObjectDoesNotExist:
         ConfigRow.objects.create(
             name=instance_row.config_name,
             value=instance_row.last_value,
             description=instance_row.description,
             tags=instance_row.tags,
             topic=instance_row.topic,
-            last_set=dt.datetime.now(tz=dt.timezone.utc)
+            last_set=dt.datetime.now(tz=dt.timezone.utc),
+            default_value=instance_row.default_value,
         )
 
 
 def load_config(reset=False, **kwargs):
     subclasses = set(BaseConfig.__subclasses__())
     for config in subclasses:
         for name, row in config.__dict__.items():
             if not any(
-                [name.startswith('__'), name.endswith(DESCRIPTION_SUFFIX),
-                 name.endswith(TAGS_SUFFIX), name.endswith(VALIDATORS_SUFFIX)]
+                [name.startswith('__'), name.endswith((DESCRIPTION_SUFFIX, TAGS_SUFFIX, VALIDATORS_SUFFIX))]
             ):
                 save_row(row, reset=reset)
         logger.info(f"Config '{config.__name__}' load successfully")
 
 
 class Command(BaseCommand):
     help = 'Загрузка дефолтных конфигов для админки (существующие параметры не перезаписываются)'
```

### Comparing `django_liveconfigs-1.0.2/src/liveconfigs/migrations/0001_initial.py` & `django_liveconfigs-1.0.3/src/liveconfigs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_liveconfigs-1.0.2/src/liveconfigs/models/descriptors.py` & `django_liveconfigs-1.0.3/src/liveconfigs/models/descriptors.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 logger = logging.getLogger()
 
 DESCRIPTION_SUFFIX = "_DESCRIPTION"
 TAGS_SUFFIX = "_TAGS"
 VALIDATORS_SUFFIX = "_VALIDATORS"
 
 
-CACHE_TTL = 1
+CACHE_TTL = getattr(settings, 'LC_CACHE_TTL', 1)
 
 
 class ConfigRowDescriptor:
     """ Кеширующий дескриптор для работы с конфигами """
 
     def __init__(self, config_name, default_value, description=None, topic=None, tags=None):
         self.config_name = config_name
@@ -42,14 +42,16 @@
                     update_fields['description'] = self.description
                 if db_row.tags != self.tags:
                     update_fields['tags'] = self.tags
                 if db_row.topic != self.topic:
                     update_fields['topic'] = self.topic
                 if db_row.last_read is None or (db_row.last_read < dt_now - dt.timedelta(days=1)):
                     update_fields['last_read'] = dt_now
+                if db_row.default_value != self.default_value:
+                    update_fields['default_value'] = self.default_value
                 if update_fields:
                     config_row_update_signal.send(sender=None, config_name=self.config_name,
                                                   update_fields=update_fields)
                 self.last_value = db_row.value
             except exceptions.ObjectDoesNotExist:
                 logger.warning('no config %s in db, using default value %s',
                                self.config_name, self.default_value)
@@ -57,15 +59,16 @@
                 update_fields = {
                     "name": self.config_name,
                     "value": self.last_value,
                     "description": self.description,
                     "tags": self.tags,
                     "topic": self.topic,
                     "last_read": dt_now,
-                    "last_set": dt_now
+                    "last_set": dt_now,
+                    "default_value": self.default_value,
                 }
                 config_row_update_signal.send(
                     sender=None, config_name=self.config_name, update_fields=update_fields)
 
         self.next_check = now + CACHE_TTL
         return self.last_value
 
@@ -88,32 +91,29 @@
         config_row_types = dict()
         if "__annotations__" in dct:
             config_row_types = dct["__annotations__"]
 
         for n, v in dct.items():
             if (
                 not n.startswith('__')
-                and not any([n.endswith(DESCRIPTION_SUFFIX), n.endswith(TAGS_SUFFIX), n.endswith(VALIDATORS_SUFFIX)])
+                and not n.endswith((DESCRIPTION_SUFFIX, TAGS_SUFFIX, VALIDATORS_SUFFIX))
             ):
                 if prefix and n in config_row_types:
                     config_row_types[prefix + n] = config_row_types.pop(n)
                 dct[n] = ConfigRowDescriptor(prefix + n, v,
                                              description=dct.get(
                                                  n + DESCRIPTION_SUFFIX),
                                              tags=dct.get(n + TAGS_SUFFIX),
                                              topic=topic)
                 validators[n] = dct.get(n + VALIDATORS_SUFFIX)
 
         dct = {
             name: value
             for name, value in dct.items()
-            if not any(
-                [name.endswith(DESCRIPTION_SUFFIX), name.endswith(
-                    TAGS_SUFFIX), name.endswith(VALIDATORS_SUFFIX)]
-            )
+            if not name.endswith((DESCRIPTION_SUFFIX, TAGS_SUFFIX, VALIDATORS_SUFFIX))
         }
 
         ConfigRow.registered_row_types.update(config_row_types)
         ConfigRow.validators.update(validators)
         c = super().__new__(cls, name, bases, dct)
         return c
```

### Comparing `django_liveconfigs-1.0.2/src/liveconfigs/models/models.py` & `django_liveconfigs-1.0.3/src/liveconfigs/models/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 import typing
 
 from django import VERSION
-from django.contrib.postgres.fields import ArrayField
+from django.conf import settings
 from django.core import exceptions
 from django.db import models
 from typeguard import check_type, TypeCheckError
+from django.utils import timezone
 
 if VERSION[0] == 3:
     from django.contrib.postgres.fields import JSONField
 else:
     from django.db.models import JSONField
 
 logger = logging.getLogger()
@@ -18,17 +19,18 @@
 class ConfigRow(models.Model):
     """Простая модель для значения одного конфига"""
 
     name = models.TextField(primary_key=True)
     value = JSONField(blank=True, null=True)
     topic = models.TextField(blank=True, null=True)
     description = models.TextField(blank=True, null=True)
-    tags = ArrayField(models.TextField(blank=True, null=True), blank=True, null=True)
+    tags = JSONField(blank=True, null=True)
     last_read = models.DateTimeField(blank=True, null=True)
     last_set = models.DateTimeField(blank=True, null=True)
+    default_value = JSONField(blank=True, null=True)
     registered_row_types: dict[str, typing.Any] = dict()
     validators: dict[str, typing.Any] = dict()
 
     def validate_type(self):
         config_row_type = self.registered_row_types.get(self.name)
         if not config_row_type:
             return
@@ -53,7 +55,14 @@
         self.validate_value()
 
     def __repr__(self):
         return f"ConfigRow('{self.name}', {self.value})"
 
     def __str__(self):
         return f"Config '{self.name}' = {self.value}, {self.description or ''}"
+
+
+class HistoryEvent(models.Model):
+    name = models.TextField()
+    value = JSONField(blank=True, null=True)
+    edit_at = models.DateTimeField(default=timezone.now)
+    edit_by = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE)
```

### Comparing `django_liveconfigs-1.0.2/src/liveconfigs/utils.py` & `django_liveconfigs-1.0.3/src/liveconfigs/utils.py`

 * *Files identical despite different names*

### Comparing `django_liveconfigs-1.0.2/src/liveconfigs/validators.py` & `django_liveconfigs-1.0.3/src/liveconfigs/validators.py`

 * *Files identical despite different names*

### Comparing `django_liveconfigs-1.0.2/src/liveconfigs/views.py` & `django_liveconfigs-1.0.3/src/liveconfigs/views.py`

 * *Files identical despite different names*

