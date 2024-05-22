# Comparing `tmp/neighborly-2.5.0.tar.gz` & `tmp/neighborly-3.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neighborly-2.5.0.tar", last modified: Mon Mar 25 04:25:57 2024, max compression
+gzip compressed data, was "neighborly-3.0.0.dev1.tar", last modified: Wed May 22 20:11:03 2024, max compression
```

## Comparing `neighborly-2.5.0.tar` & `neighborly-3.0.0.dev1.tar`

### file list

```diff
@@ -1,95 +1,126 @@
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-03-25 04:25:57.208600 neighborly-2.5.0/
--rw-r--r--   0 shijbey    (501) staff       (20)    15917 2024-03-25 04:25:14.000000 neighborly-2.5.0/CHANGELOG.md
--rw-r--r--   0 shijbey    (501) staff       (20)     5224 2022-11-18 22:21:21.000000 neighborly-2.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 shijbey    (501) staff       (20)     1095 2024-03-24 19:18:37.000000 neighborly-2.5.0/LICENSE
--rw-r--r--   0 shijbey    (501) staff       (20)      275 2023-11-05 00:27:21.000000 neighborly-2.5.0/MANIFEST.in
--rw-r--r--   0 shijbey    (501) staff       (20)    10610 2024-03-25 04:25:57.208235 neighborly-2.5.0/PKG-INFO
--rw-r--r--   0 shijbey    (501) staff       (20)     8008 2024-03-18 22:17:51.000000 neighborly-2.5.0/README.md
--rw-r--r--   0 shijbey    (501) staff       (20)     3323 2024-03-24 19:19:18.000000 neighborly-2.5.0/pyproject.toml
--rw-r--r--   0 shijbey    (501) staff       (20)       38 2024-03-25 04:25:57.208658 neighborly-2.5.0/setup.cfg
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-03-25 04:25:57.180938 neighborly-2.5.0/src/
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-03-25 04:25:57.189206 neighborly-2.5.0/src/neighborly/
--rw-r--r--   0 shijbey    (501) staff       (20)      477 2023-10-27 22:45:31.000000 neighborly-2.5.0/src/neighborly/__init__.py
--rw-r--r--   0 shijbey    (501) staff       (20)      156 2024-03-24 19:19:50.000000 neighborly-2.5.0/src/neighborly/__version__.py
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-03-25 04:25:57.193714 neighborly-2.5.0/src/neighborly/components/
--rw-r--r--   0 shijbey    (501) staff       (20)        0 2024-03-23 18:45:03.000000 neighborly-2.5.0/src/neighborly/components/__init__.py
--rw-r--r--   0 shijbey    (501) staff       (20)     9205 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/components/business.py
--rw-r--r--   0 shijbey    (501) staff       (20)     5182 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/components/character.py
--rw-r--r--   0 shijbey    (501) staff       (20)     6431 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/components/location.py
--rw-r--r--   0 shijbey    (501) staff       (20)     9130 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/components/relationship.py
--rw-r--r--   0 shijbey    (501) staff       (20)     5728 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/components/residence.py
--rw-r--r--   0 shijbey    (501) staff       (20)     7552 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/components/settlement.py
--rw-r--r--   0 shijbey    (501) staff       (20)     3532 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/components/skills.py
--rw-r--r--   0 shijbey    (501) staff       (20)     6644 2024-03-24 19:18:37.000000 neighborly-2.5.0/src/neighborly/components/spawn_table.py
--rw-r--r--   0 shijbey    (501) staff       (20)     9725 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/components/stats.py
--rw-r--r--   0 shijbey    (501) staff       (20)     6726 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/components/traits.py
--rw-r--r--   0 shijbey    (501) staff       (20)     1139 2024-03-24 13:38:13.000000 neighborly-2.5.0/src/neighborly/config.py
--rw-r--r--   0 shijbey    (501) staff       (20)    19379 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/data_analysis.py
--rw-r--r--   0 shijbey    (501) staff       (20)     4051 2024-03-24 13:38:13.000000 neighborly-2.5.0/src/neighborly/data_collection.py
--rw-r--r--   0 shijbey    (501) staff       (20)     3546 2023-10-27 22:45:31.000000 neighborly-2.5.0/src/neighborly/datetime.py
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-03-25 04:25:57.194618 neighborly-2.5.0/src/neighborly/defs/
--rw-r--r--   0 shijbey    (501) staff       (20)        0 2023-10-27 22:45:31.000000 neighborly-2.5.0/src/neighborly/defs/__init__.py
--rw-r--r--   0 shijbey    (501) staff       (20)    23030 2024-03-25 04:25:14.000000 neighborly-2.5.0/src/neighborly/defs/base_types.py
--rw-r--r--   0 shijbey    (501) staff       (20)    28637 2024-03-25 04:25:14.000000 neighborly-2.5.0/src/neighborly/defs/defaults.py
--rw-r--r--   0 shijbey    (501) staff       (20)     4173 2024-03-24 19:18:37.000000 neighborly-2.5.0/src/neighborly/defs/definition_compiler.py
--rw-r--r--   0 shijbey    (501) staff       (20)    44656 2024-03-24 13:38:13.000000 neighborly-2.5.0/src/neighborly/ecs.py
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-03-25 04:25:57.195356 neighborly-2.5.0/src/neighborly/effects/
--rw-r--r--   0 shijbey    (501) staff       (20)        0 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/effects/__init__.py
--rw-r--r--   0 shijbey    (501) staff       (20)     1028 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/effects/base_types.py
--rw-r--r--   0 shijbey    (501) staff       (20)     7847 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/effects/effects.py
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-03-25 04:25:57.195765 neighborly-2.5.0/src/neighborly/events/
--rw-r--r--   0 shijbey    (501) staff       (20)        0 2023-10-27 22:45:31.000000 neighborly-2.5.0/src/neighborly/events/__init__.py
--rw-r--r--   0 shijbey    (501) staff       (20)    22660 2024-03-24 13:38:13.000000 neighborly-2.5.0/src/neighborly/events/defaults.py
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-03-25 04:25:57.198799 neighborly-2.5.0/src/neighborly/helpers/
--rw-r--r--   0 shijbey    (501) staff       (20)        0 2023-10-27 22:45:31.000000 neighborly-2.5.0/src/neighborly/helpers/__init__.py
--rw-r--r--   0 shijbey    (501) staff       (20)     1969 2024-03-24 19:18:37.000000 neighborly-2.5.0/src/neighborly/helpers/business.py
--rw-r--r--   0 shijbey    (501) staff       (20)     1482 2024-03-24 19:18:37.000000 neighborly-2.5.0/src/neighborly/helpers/character.py
--rw-r--r--   0 shijbey    (501) staff       (20)     1491 2024-03-24 19:18:37.000000 neighborly-2.5.0/src/neighborly/helpers/content_selection.py
--rw-r--r--   0 shijbey    (501) staff       (20)     1963 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/helpers/location.py
--rw-r--r--   0 shijbey    (501) staff       (20)     7567 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/helpers/relationship.py
--rw-r--r--   0 shijbey    (501) staff       (20)     1248 2024-03-24 19:18:37.000000 neighborly-2.5.0/src/neighborly/helpers/residence.py
--rw-r--r--   0 shijbey    (501) staff       (20)     2852 2024-03-24 19:18:37.000000 neighborly-2.5.0/src/neighborly/helpers/settlement.py
--rw-r--r--   0 shijbey    (501) staff       (20)     1786 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/helpers/skills.py
--rw-r--r--   0 shijbey    (501) staff       (20)     1808 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/helpers/stats.py
--rw-r--r--   0 shijbey    (501) staff       (20)     2292 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/helpers/traits.py
--rw-r--r--   0 shijbey    (501) staff       (20)    25120 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/inspection.py
--rw-r--r--   0 shijbey    (501) staff       (20)     9765 2024-03-24 19:18:37.000000 neighborly-2.5.0/src/neighborly/libraries.py
--rw-r--r--   0 shijbey    (501) staff       (20)    14008 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/life_event.py
--rw-r--r--   0 shijbey    (501) staff       (20)     6585 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/loaders.py
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-03-25 04:25:57.200332 neighborly-2.5.0/src/neighborly/plugins/
--rw-r--r--   0 shijbey    (501) staff       (20)        0 2023-10-27 16:34:16.000000 neighborly-2.5.0/src/neighborly/plugins/__init__.py
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-03-25 04:25:57.202673 neighborly-2.5.0/src/neighborly/plugins/data/
--rw-r--r--   0 shijbey    (501) staff       (20)   300691 2023-11-05 00:27:21.000000 neighborly-2.5.0/src/neighborly/plugins/data/character_names.tracery.json
--rw-r--r--   0 shijbey    (501) staff       (20)    11679 2023-11-05 00:27:21.000000 neighborly-2.5.0/src/neighborly/plugins/data/settlement_names.tracery.json
--rw-r--r--   0 shijbey    (501) staff       (20)    23471 2024-03-24 19:18:37.000000 neighborly-2.5.0/src/neighborly/plugins/data/traits.json
--rw-r--r--   0 shijbey    (501) staff       (20)      381 2023-11-05 00:27:21.000000 neighborly-2.5.0/src/neighborly/plugins/default_character_names.py
--rw-r--r--   0 shijbey    (501) staff       (20)    63772 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/plugins/default_events.py
--rw-r--r--   0 shijbey    (501) staff       (20)      361 2023-11-05 00:27:21.000000 neighborly-2.5.0/src/neighborly/plugins/default_settlement_names.py
--rw-r--r--   0 shijbey    (501) staff       (20)      326 2023-11-05 00:27:21.000000 neighborly-2.5.0/src/neighborly/plugins/default_traits.py
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-03-25 04:25:57.203817 neighborly-2.5.0/src/neighborly/preconditions/
--rw-r--r--   0 shijbey    (501) staff       (20)        0 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/preconditions/__init__.py
--rw-r--r--   0 shijbey    (501) staff       (20)     1305 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/preconditions/base_types.py
--rw-r--r--   0 shijbey    (501) staff       (20)     5274 2024-03-24 13:36:46.000000 neighborly-2.5.0/src/neighborly/preconditions/defaults.py
--rw-r--r--   0 shijbey    (501) staff       (20)        0 2023-03-27 21:19:31.000000 neighborly-2.5.0/src/neighborly/py.typed
--rw-r--r--   0 shijbey    (501) staff       (20)    18320 2024-03-25 04:25:14.000000 neighborly-2.5.0/src/neighborly/simulation.py
--rw-r--r--   0 shijbey    (501) staff       (20)    32601 2024-03-25 04:25:14.000000 neighborly-2.5.0/src/neighborly/systems.py
--rw-r--r--   0 shijbey    (501) staff       (20)     1778 2024-02-16 20:30:20.000000 neighborly-2.5.0/src/neighborly/tracery.py
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-03-25 04:25:57.207192 neighborly-2.5.0/src/neighborly.egg-info/
--rw-r--r--   0 shijbey    (501) staff       (20)    10610 2024-03-25 04:25:57.000000 neighborly-2.5.0/src/neighborly.egg-info/PKG-INFO
--rw-r--r--   0 shijbey    (501) staff       (20)     2606 2024-03-25 04:25:57.000000 neighborly-2.5.0/src/neighborly.egg-info/SOURCES.txt
--rw-r--r--   0 shijbey    (501) staff       (20)        1 2024-03-25 04:25:57.000000 neighborly-2.5.0/src/neighborly.egg-info/dependency_links.txt
--rw-r--r--   0 shijbey    (501) staff       (20)      254 2024-03-25 04:25:57.000000 neighborly-2.5.0/src/neighborly.egg-info/requires.txt
--rw-r--r--   0 shijbey    (501) staff       (20)       11 2024-03-25 04:25:57.000000 neighborly-2.5.0/src/neighborly.egg-info/top_level.txt
-drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-03-25 04:25:57.206941 neighborly-2.5.0/tests/
--rw-r--r--   0 shijbey    (501) staff       (20)     1264 2024-03-24 13:36:46.000000 neighborly-2.5.0/tests/test_business.py
--rw-r--r--   0 shijbey    (501) staff       (20)      752 2024-03-24 19:18:37.000000 neighborly-2.5.0/tests/test_character.py
--rw-r--r--   0 shijbey    (501) staff       (20)     2731 2023-10-27 22:45:31.000000 neighborly-2.5.0/tests/test_datetime.py
--rw-r--r--   0 shijbey    (501) staff       (20)     3380 2024-03-24 13:36:46.000000 neighborly-2.5.0/tests/test_loaders.py
--rw-r--r--   0 shijbey    (501) staff       (20)     2116 2024-03-25 04:25:14.000000 neighborly-2.5.0/tests/test_location_preferences.py
--rw-r--r--   0 shijbey    (501) staff       (20)     3277 2024-03-25 04:25:14.000000 neighborly-2.5.0/tests/test_relationship.py
--rw-r--r--   0 shijbey    (501) staff       (20)     1376 2024-03-24 13:36:46.000000 neighborly-2.5.0/tests/test_residence.py
--rw-r--r--   0 shijbey    (501) staff       (20)     4929 2024-03-24 19:18:37.000000 neighborly-2.5.0/tests/test_settlement.py
--rw-r--r--   0 shijbey    (501) staff       (20)     2784 2024-03-24 13:36:46.000000 neighborly-2.5.0/tests/test_simulation.py
--rw-r--r--   0 shijbey    (501) staff       (20)     2368 2024-03-25 04:25:14.000000 neighborly-2.5.0/tests/test_stats.py
--rw-r--r--   0 shijbey    (501) staff       (20)      695 2024-03-24 19:18:37.000000 neighborly-2.5.0/tests/test_tag_selection.py
--rw-r--r--   0 shijbey    (501) staff       (20)     3571 2024-03-25 04:25:14.000000 neighborly-2.5.0/tests/test_traits.py
+drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-05-22 20:11:03.316426 neighborly-3.0.0.dev1/
+-rw-r--r--   0 shijbey    (501) staff       (20)    17563 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/CHANGELOG.md
+-rw-r--r--   0 shijbey    (501) staff       (20)     5224 2022-11-18 22:21:21.000000 neighborly-3.0.0.dev1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 shijbey    (501) staff       (20)     1095 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/LICENSE.md
+-rw-r--r--   0 shijbey    (501) staff       (20)      278 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/MANIFEST.in
+-rw-r--r--   0 shijbey    (501) staff       (20)    12429 2024-05-22 20:11:03.316079 neighborly-3.0.0.dev1/PKG-INFO
+-rw-r--r--   0 shijbey    (501) staff       (20)     8785 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/README.md
+-rw-r--r--   0 shijbey    (501) staff       (20)     3233 2024-05-21 14:41:04.000000 neighborly-3.0.0.dev1/pyproject.toml
+-rw-r--r--   0 shijbey    (501) staff       (20)       38 2024-05-22 20:11:03.316486 neighborly-3.0.0.dev1/setup.cfg
+drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-05-22 20:11:03.278094 neighborly-3.0.0.dev1/src/
+drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-05-22 20:11:03.285828 neighborly-3.0.0.dev1/src/neighborly/
+-rw-r--r--   0 shijbey    (501) staff       (20)      616 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/__init__.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     1603 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/action.py
+drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-05-22 20:11:03.291447 neighborly-3.0.0.dev1/src/neighborly/components/
+-rw-r--r--   0 shijbey    (501) staff       (20)        0 2024-03-23 18:45:03.000000 neighborly-3.0.0.dev1/src/neighborly/components/__init__.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     5095 2024-05-22 03:51:42.000000 neighborly-3.0.0.dev1/src/neighborly/components/beliefs.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     5574 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/components/business.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     7465 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/components/character.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     6908 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/components/location.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     7239 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/components/relationship.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     1453 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/components/settlement.py
+-rw-r--r--   0 shijbey    (501) staff       (20)      720 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/components/shared.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     2674 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/components/skills.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     4074 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/components/spawn_table.py
+-rw-r--r--   0 shijbey    (501) staff       (20)    13651 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/components/stats.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     6422 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/components/traits.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     1281 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/config.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     4316 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/data_analysis.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     3546 2023-10-27 22:45:31.000000 neighborly-3.0.0.dev1/src/neighborly/datetime.py
+drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-05-22 20:11:03.292331 neighborly-3.0.0.dev1/src/neighborly/defs/
+-rw-r--r--   0 shijbey    (501) staff       (20)        0 2023-10-27 22:45:31.000000 neighborly-3.0.0.dev1/src/neighborly/defs/__init__.py
+-rw-r--r--   0 shijbey    (501) staff       (20)    14285 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/defs/base_types.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     4811 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/defs/definition_compiler.py
+-rw-r--r--   0 shijbey    (501) staff       (20)    48294 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/ecs.py
+drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-05-22 20:11:03.292920 neighborly-3.0.0.dev1/src/neighborly/effects/
+-rw-r--r--   0 shijbey    (501) staff       (20)        0 2024-05-20 20:39:06.000000 neighborly-3.0.0.dev1/src/neighborly/effects/__init__.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     1443 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/effects/base_types.py
+-rw-r--r--   0 shijbey    (501) staff       (20)    12438 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/effects/effects.py
+drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-05-22 20:11:03.293412 neighborly-3.0.0.dev1/src/neighborly/events/
+-rw-r--r--   0 shijbey    (501) staff       (20)        0 2023-10-27 22:45:31.000000 neighborly-3.0.0.dev1/src/neighborly/events/__init__.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     9655 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/events/defaults.py
+drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-05-22 20:11:03.296426 neighborly-3.0.0.dev1/src/neighborly/factories/
+-rw-r--r--   0 shijbey    (501) staff       (20)        0 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/factories/__init__.py
+-rw-r--r--   0 shijbey    (501) staff       (20)      689 2024-05-22 03:51:38.000000 neighborly-3.0.0.dev1/src/neighborly/factories/beliefs.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     2522 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/factories/business.py
+-rw-r--r--   0 shijbey    (501) staff       (20)    12145 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/factories/character.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     1049 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/factories/location.py
+-rw-r--r--   0 shijbey    (501) staff       (20)      441 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/factories/relationships.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     2584 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/factories/settlement.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     1020 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/factories/shared.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     1599 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/factories/skills.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     6550 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/factories/spawn_table.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     5564 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/factories/stats.py
+-rw-r--r--   0 shijbey    (501) staff       (20)      401 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/factories/traits.py
+drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-05-22 20:11:03.298821 neighborly-3.0.0.dev1/src/neighborly/helpers/
+-rw-r--r--   0 shijbey    (501) staff       (20)        0 2023-10-27 22:45:31.000000 neighborly-3.0.0.dev1/src/neighborly/helpers/__init__.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     1041 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/helpers/action.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     5604 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/helpers/business.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     4938 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/helpers/character.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     1495 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/helpers/content_selection.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     3792 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/helpers/location.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     7790 2024-05-22 03:51:38.000000 neighborly-3.0.0.dev1/src/neighborly/helpers/relationship.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     1887 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/helpers/settlement.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     1501 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/helpers/skills.py
+-rw-r--r--   0 shijbey    (501) staff       (20)      937 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/helpers/stats.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     8049 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/helpers/traits.py
+-rw-r--r--   0 shijbey    (501) staff       (20)    30485 2024-05-22 03:51:38.000000 neighborly-3.0.0.dev1/src/neighborly/inspection.py
+-rw-r--r--   0 shijbey    (501) staff       (20)    18249 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/libraries.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     4520 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/life_event.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     7040 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/loaders.py
+drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-05-22 20:11:03.303209 neighborly-3.0.0.dev1/src/neighborly/plugins/
+-rw-r--r--   0 shijbey    (501) staff       (20)        0 2023-10-27 16:34:16.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/__init__.py
+-rw-r--r--   0 shijbey    (501) staff       (20)    33931 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/actions.py
+drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-05-22 20:11:03.307639 neighborly-3.0.0.dev1/src/neighborly/plugins/data/
+-rw-r--r--   0 shijbey    (501) staff       (20)     1422 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/data/beliefs.json
+-rw-r--r--   0 shijbey    (501) staff       (20)      143 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/data/business_traits.json
+-rw-r--r--   0 shijbey    (501) staff       (20)     3005 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/data/businesses.json
+-rw-r--r--   0 shijbey    (501) staff       (20)     4288 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/data/characters.json
+-rw-r--r--   0 shijbey    (501) staff       (20)     2771 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/data/districts.json
+-rw-r--r--   0 shijbey    (501) staff       (20)     6999 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/data/feminine_first_names.txt
+-rw-r--r--   0 shijbey    (501) staff       (20)     1027 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/data/job_roles.json
+-rw-r--r--   0 shijbey    (501) staff       (20)   106909 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/data/last_names.txt
+-rw-r--r--   0 shijbey    (501) staff       (20)      260 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/data/location_preferences.json
+-rw-r--r--   0 shijbey    (501) staff       (20)     6669 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/data/masculine_first_names.txt
+-rw-r--r--   0 shijbey    (501) staff       (20)     4933 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/data/relationship_traits.json
+-rw-r--r--   0 shijbey    (501) staff       (20)     6111 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/data/settlement_names.txt
+-rw-r--r--   0 shijbey    (501) staff       (20)     1105 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/data/settlements.json
+-rw-r--r--   0 shijbey    (501) staff       (20)      275 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/data/skills.json
+-rw-r--r--   0 shijbey    (501) staff       (20)      623 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/data/species.json
+-rw-r--r--   0 shijbey    (501) staff       (20)    18209 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/data/traits.json
+-rw-r--r--   0 shijbey    (501) staff       (20)      430 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/default_businesses.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     1352 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/default_character_names.py
+-rw-r--r--   0 shijbey    (501) staff       (20)      537 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/default_characters.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     9148 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/default_considerations.py
+-rw-r--r--   0 shijbey    (501) staff       (20)      817 2024-05-21 14:58:34.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/default_content.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     1440 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/default_event_responses.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     9176 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/default_events.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     1012 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/default_settlement_names.py
+-rw-r--r--   0 shijbey    (501) staff       (20)      435 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/default_settlements.py
+-rw-r--r--   0 shijbey    (501) staff       (20)    25803 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/default_systems.py
+-rw-r--r--   0 shijbey    (501) staff       (20)      611 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/plugins/default_traits.py
+drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-05-22 20:11:03.308749 neighborly-3.0.0.dev1/src/neighborly/preconditions/
+-rw-r--r--   0 shijbey    (501) staff       (20)        0 2024-05-20 20:39:06.000000 neighborly-3.0.0.dev1/src/neighborly/preconditions/__init__.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     1813 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/preconditions/base_types.py
+-rw-r--r--   0 shijbey    (501) staff       (20)    10376 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/preconditions/defaults.py
+-rw-r--r--   0 shijbey    (501) staff       (20)        0 2023-03-27 21:19:31.000000 neighborly-3.0.0.dev1/src/neighborly/py.typed
+-rw-r--r--   0 shijbey    (501) staff       (20)    15278 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/simulation.py
+-rw-r--r--   0 shijbey    (501) staff       (20)    33668 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/src/neighborly/systems.py
+drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-05-22 20:11:03.315220 neighborly-3.0.0.dev1/src/neighborly.egg-info/
+-rw-r--r--   0 shijbey    (501) staff       (20)    12429 2024-05-22 20:11:03.000000 neighborly-3.0.0.dev1/src/neighborly.egg-info/PKG-INFO
+-rw-r--r--   0 shijbey    (501) staff       (20)     3898 2024-05-22 20:11:03.000000 neighborly-3.0.0.dev1/src/neighborly.egg-info/SOURCES.txt
+-rw-r--r--   0 shijbey    (501) staff       (20)        1 2024-05-22 20:11:03.000000 neighborly-3.0.0.dev1/src/neighborly.egg-info/dependency_links.txt
+-rw-r--r--   0 shijbey    (501) staff       (20)      178 2024-05-22 20:11:03.000000 neighborly-3.0.0.dev1/src/neighborly.egg-info/requires.txt
+-rw-r--r--   0 shijbey    (501) staff       (20)       11 2024-05-22 20:11:03.000000 neighborly-3.0.0.dev1/src/neighborly.egg-info/top_level.txt
+drwxr-xr-x   0 shijbey    (501) staff       (20)        0 2024-05-22 20:11:03.314814 neighborly-3.0.0.dev1/tests/
+-rw-r--r--   0 shijbey    (501) staff       (20)      761 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/tests/test_business.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     1011 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/tests/test_character.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     2731 2023-10-27 22:45:31.000000 neighborly-3.0.0.dev1/tests/test_datetime.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     2692 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/tests/test_loaders.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     1932 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/tests/test_location_preferences.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     3779 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/tests/test_relationship.py
+-rw-r--r--   0 shijbey    (501) staff       (20)      967 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/tests/test_settlement.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     2343 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/tests/test_simulation.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     2198 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/tests/test_stats.py
+-rw-r--r--   0 shijbey    (501) staff       (20)      695 2024-05-20 20:39:06.000000 neighborly-3.0.0.dev1/tests/test_tag_selection.py
+-rw-r--r--   0 shijbey    (501) staff       (20)     2957 2024-05-21 01:41:58.000000 neighborly-3.0.0.dev1/tests/test_traits.py
```

### Comparing `neighborly-2.5.0/CHANGELOG.md` & `neighborly-3.0.0.dev1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,43 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres mostly to
 [Semantic Versioning](https://semver.org/spec/v2.0.0.html). However, all releases before 1.0.0 have breaking changes
 between minor-version updates.
 
+## [3.0.0] - Unreleased
+
+Neighborly version 3.0 focuses on agent-based modeling, data analysis, and data querying. It boasts a new action system and two database instances (RePraxis and SQL) that help users easily query data for analysis or simulation mechanics. It also consolidates many of the public APIs to shorten code lines. To support this, 3.0 introduces breaking changes to the ECS, content definitions, social rules, location preferences, the life event system, and a few others.
+
+### Changed
+
+- Convert Skills and Traits to an instance-style model
+- Refactor social rules and location preferences to be independent from traits
+- Move social rule and location preference calculation functions to helper modules
+- Component constructors can no longer be called directly as we need to inject the gameobject directly into the `__init__()`.
+- Rename `display_name` attribute for content to `name`.
+- Move version information to top-level `__init__.py` as `__version__` to comply with Python conventions
+- Replace `FrequentedBy` component with `Location` component
+- Convert
+
+### Added
+
+- Add SQLAlchemy back-end to replace the manual table construction in the `data_analysis` module
+- Add `lifespan` option to business definitions
+
+### Removed
+
+- Precondition API in favor of RePraxis queries
+- Data duplication in Trait, JobRole, and Species classes
+- Polars sql context building code from `data_analysis` module
+- `data_collection` module. Users can leverage new SQL database.
+- `OpenToPublic` component
+- `health` and `health_decay` stats in favor of life span system.
+
 ## [2.5.0] - 2024-03-24
 
 This version introduces minor breaking changes to the content authoring pipeline. Please check your YAML and JSON files.
 
 ### Changed
 
 - Convert content definition classes to use Pydantic
@@ -364,14 +393,15 @@
 - Bug in Business operating hours regex that did not recognize AM/PM strings
 - `setup.cfg` did not properly include data files in the wheel build.
 
 ## [0.9.3] - 2022-08-15
 
 _Initial Release._
 
+[3.0.0]: https://github.com/ShiJbey/neighborly/releases/tag/v3.0.0
 [2.5.0]: https://github.com/ShiJbey/neighborly/releases/tag/v2.5.0
 [2.4.1]: https://github.com/ShiJbey/neighborly/releases/tag/v2.4.1
 [2.1.1]: https://github.com/ShiJbey/neighborly/releases/tag/v2.1.1
 [2.1.0]: https://github.com/ShiJbey/neighborly/releases/tag/v2.1.0
 [2.0.0]: https://github.com/ShiJbey/neighborly/releases/tag/v2.0.0
 [1.0.0]: https://github.com/ShiJbey/neighborly/releases/tag/v1.0.0
 [0.11.2]: https://github.com/ShiJbey/neighborly/releases/tag/v0.11.2
```

### Comparing `neighborly-2.5.0/CODE_OF_CONDUCT.md` & `neighborly-3.0.0.dev1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `neighborly-2.5.0/LICENSE` & `neighborly-3.0.0.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neighborly-2.5.0/PKG-INFO` & `neighborly-3.0.0.dev1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,664 +1,777 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e65 6967  : 2.1.Name: neig
 00000020: 6862 6f72 6c79 0a56 6572 7369 6f6e 3a20  hborly.Version: 
-00000030: 322e 352e 300a 5375 6d6d 6172 793a 2041  2.5.0.Summary: A
-00000040: 206e 6172 7261 7469 7665 2d66 6f63 7573   narrative-focus
-00000050: 6564 2061 6765 6e74 2d62 6173 6564 2073  ed agent-based s
-00000060: 6574 746c 656d 656e 7420 7369 6d75 6c61  ettlement simula
-00000070: 7469 6f6e 2066 7261 6d65 776f 726b 2e0a  tion framework..
-00000080: 4175 7468 6f72 2d65 6d61 696c 3a20 5368  Author-email: Sh
-00000090: 6920 4a6f 686e 736f 6e2d 4265 7920 3c73  i Johnson-Bey <s
-000000a0: 6869 6a62 6579 4067 6d61 696c 2e63 6f6d  hijbey@gmail.com
-000000b0: 3e0a 5072 6f6a 6563 742d 5552 4c3a 2048  >.Project-URL: H
-000000c0: 6f6d 6570 6167 652c 2068 7474 7073 3a2f  omepage, https:/
-000000d0: 2f67 6974 6875 622e 636f 6d2f 5368 694a  /github.com/ShiJ
-000000e0: 6265 792f 6e65 6967 6862 6f72 6c79 0a50  bey/neighborly.P
-000000f0: 726f 6a65 6374 2d55 524c 3a20 4275 6720  roject-URL: Bug 
-00000100: 5472 6163 6b65 722c 2068 7474 7073 3a2f  Tracker, https:/
-00000110: 2f67 6974 6875 622e 636f 6d2f 5368 694a  /github.com/ShiJ
-00000120: 6265 792f 6e65 6967 6862 6f72 6c79 2f69  bey/neighborly/i
-00000130: 7373 7565 730a 5072 6f6a 6563 742d 5552  ssues.Project-UR
-00000140: 4c3a 2052 6570 6f73 6974 6f72 792c 2068  L: Repository, h
-00000150: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000160: 6d2f 5368 694a 4265 792f 6e65 6967 6862  m/ShiJBey/neighb
-00000170: 6f72 6c79 2e67 6974 0a50 726f 6a65 6374  orly.git.Project
-00000180: 2d55 524c 3a20 4368 616e 6765 6c6f 672c  -URL: Changelog,
-00000190: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000001a0: 636f 6d2f 5368 694a 6265 792f 6e65 6967  com/ShiJbey/neig
-000001b0: 6862 6f72 6c79 2f62 6c6f 622f 6d61 696e  hborly/blob/main
-000001c0: 2f43 4841 4e47 454c 4f47 2e6d 640a 5072  /CHANGELOG.md.Pr
-000001d0: 6f6a 6563 742d 5552 4c3a 2044 6f63 756d  oject-URL: Docum
-000001e0: 656e 7461 7469 6f6e 2c20 6874 7470 733a  entation, https:
-000001f0: 2f2f 6e65 6967 6862 6f72 6c79 2e72 6561  //neighborly.rea
-00000200: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00000210: 6174 6573 742f 0a4b 6579 776f 7264 733a  atest/.Keywords:
-00000220: 2073 6f63 6961 6c20 7369 6d75 6c61 7469   social simulati
-00000230: 6f6e 2c67 616d 6573 2c73 696d 756c 6174  on,games,simulat
-00000240: 696f 6e2c 6172 7469 6669 6369 616c 2069  ion,artificial i
-00000250: 6e74 656c 6c69 6765 6e63 652c 6167 656e  ntelligence,agen
-00000260: 742d 6261 7365 6420 6d6f 6465 6c69 6e67  t-based modeling
-00000270: 2c6d 756c 7469 6167 656e 7420 7379 7374  ,multiagent syst
-00000280: 656d 732c 656d 6572 6765 6e74 206e 6172  ems,emergent nar
-00000290: 7261 7469 7665 2c6e 6172 7261 7469 7665  rative,narrative
-000002a0: 2067 656e 6572 6174 696f 6e2c 696e 7465   generation,inte
-000002b0: 7261 6374 6976 6520 7374 6f72 7974 656c  ractive storytel
-000002c0: 6c69 6e67 2c73 6574 746c 656d 656e 7420  ling,settlement 
-000002d0: 7369 6d75 6c61 7469 6f6e 0a43 6c61 7373  simulation.Class
-000002e0: 6966 6965 723a 2049 6e74 656e 6465 6420  ifier: Intended 
-000002f0: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
-00000300: 6c6f 7065 7273 0a43 6c61 7373 6966 6965  lopers.Classifie
-00000310: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
-00000320: 656e 6365 203a 3a20 5363 6965 6e63 652f  ence :: Science/
-00000330: 5265 7365 6172 6368 0a43 6c61 7373 6966  Research.Classif
-00000340: 6965 723a 204c 6963 656e 7365 203a 3a20  ier: License :: 
-00000350: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-00000360: 4d49 5420 4c69 6365 6e73 650a 436c 6173  MIT License.Clas
-00000370: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
-00000380: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-00000390: 6e64 6570 656e 6465 6e74 0a43 6c61 7373  ndependent.Class
-000003a0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-000003b0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000003c0: 7974 686f 6e20 3a3a 2033 203a 3a20 4f6e  ython :: 3 :: On
-000003d0: 6c79 0a43 6c61 7373 6966 6965 723a 2050  ly.Classifier: P
-000003e0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000003f0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000400: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
-00000410: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000420: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000430: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
-00000440: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000450: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000460: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
-00000470: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000480: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000490: 7468 6f6e 203a 3a20 332e 3131 0a43 6c61  thon :: 3.11.Cla
-000004a0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-000004b0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000004c0: 2050 7974 686f 6e20 3a3a 2033 2e31 320a   Python :: 3.12.
-000004d0: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
-000004e0: 6320 3a3a 2047 616d 6573 2f45 6e74 6572  c :: Games/Enter
-000004f0: 7461 696e 6d65 6e74 203a 3a20 5369 6d75  tainment :: Simu
-00000500: 6c61 7469 6f6e 0a43 6c61 7373 6966 6965  lation.Classifie
-00000510: 723a 2054 6f70 6963 203a 3a20 5363 6965  r: Topic :: Scie
-00000520: 6e74 6966 6963 2f45 6e67 696e 6565 7269  ntific/Engineeri
-00000530: 6e67 0a43 6c61 7373 6966 6965 723a 2054  ng.Classifier: T
-00000540: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
-00000550: 6963 2f45 6e67 696e 6565 7269 6e67 203a  ic/Engineering :
-00000560: 3a20 4172 7469 6669 6369 616c 2049 6e74  : Artificial Int
-00000570: 656c 6c69 6765 6e63 650a 436c 6173 7369  elligence.Classi
-00000580: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
-00000590: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
-000005a0: 6572 696e 6720 3a3a 2041 7274 6966 6963  ering :: Artific
-000005b0: 6961 6c20 4c69 6665 0a43 6c61 7373 6966  ial Life.Classif
-000005c0: 6965 723a 2054 6f70 6963 203a 3a20 536f  ier: Topic :: So
-000005d0: 6369 6f6c 6f67 790a 436c 6173 7369 6669  ciology.Classifi
-000005e0: 6572 3a20 546f 7069 6320 3a3a 2053 6f66  er: Topic :: Sof
-000005f0: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
-00000600: 7420 3a3a 204c 6962 7261 7269 6573 0a43  t :: Libraries.C
-00000610: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-00000620: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
-00000630: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
-00000640: 6172 6965 7320 3a3a 2041 7070 6c69 6361  aries :: Applica
-00000650: 7469 6f6e 2046 7261 6d65 776f 726b 730a  tion Frameworks.
-00000660: 436c 6173 7369 6669 6572 3a20 5479 7069  Classifier: Typi
-00000670: 6e67 203a 3a20 5479 7065 640a 5265 7175  ng :: Typed.Requ
-00000680: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
-00000690: 2e38 0a44 6573 6372 6970 7469 6f6e 2d43  .8.Description-C
-000006a0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-000006b0: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
-000006c0: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-000006d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000006e0: 6573 7065 723d 3d32 2e2a 0a52 6571 7569  esper==2.*.Requi
-000006f0: 7265 732d 4469 7374 3a20 6f72 6465 7265  res-Dist: ordere
-00000700: 642d 7365 743d 3d34 2e2a 0a52 6571 7569  d-set==4.*.Requi
-00000710: 7265 732d 4469 7374 3a20 7472 6163 6572  res-Dist: tracer
-00000720: 7933 3d3d 312e 2a0a 5265 7175 6972 6573  y3==1.*.Requires
-00000730: 2d44 6973 743a 2070 6f6c 6172 733d 3d30  -Dist: polars==0
-00000740: 2e31 392e 2a0a 5265 7175 6972 6573 2d44  .19.*.Requires-D
-00000750: 6973 743a 2074 6162 756c 6174 653d 3d30  ist: tabulate==0
-00000760: 2e39 2e2a 0a52 6571 7569 7265 732d 4469  .9.*.Requires-Di
-00000770: 7374 3a20 5079 5941 4d4c 3d3d 362e 302e  st: PyYAML==6.0.
-00000780: 2a0a 5265 7175 6972 6573 2d44 6973 743a  *.Requires-Dist:
-00000790: 2074 7164 6d3d 3d34 2e2a 0a52 6571 7569   tqdm==4.*.Requi
-000007a0: 7265 732d 4469 7374 3a20 7079 6461 6e74  res-Dist: pydant
-000007b0: 6963 3d3d 322e 2a0a 5072 6f76 6964 6573  ic==2.*.Provides
-000007c0: 2d45 7874 7261 3a20 7361 6d70 6c65 730a  -Extra: samples.
-000007d0: 5265 7175 6972 6573 2d44 6973 743a 206a  Requires-Dist: j
-000007e0: 7570 7974 6572 6c61 623b 2065 7874 7261  upyterlab; extra
-000007f0: 203d 3d20 2273 616d 706c 6573 220a 5265   == "samples".Re
-00000800: 7175 6972 6573 2d44 6973 743a 206d 6174  quires-Dist: mat
-00000810: 706c 6f74 6c69 623b 2065 7874 7261 203d  plotlib; extra =
-00000820: 3d20 2273 616d 706c 6573 220a 5265 7175  = "samples".Requ
-00000830: 6972 6573 2d44 6973 743a 2069 7079 7769  ires-Dist: ipywi
-00000840: 6467 6574 733b 2065 7874 7261 203d 3d20  dgets; extra == 
-00000850: 2273 616d 706c 6573 220a 5072 6f76 6964  "samples".Provid
-00000860: 6573 2d45 7874 7261 3a20 6465 7665 6c6f  es-Extra: develo
-00000870: 706d 656e 740a 5265 7175 6972 6573 2d44  pment.Requires-D
-00000880: 6973 743a 2069 736f 7274 3b20 6578 7472  ist: isort; extr
-00000890: 6120 3d3d 2022 6465 7665 6c6f 706d 656e  a == "developmen
-000008a0: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
-000008b0: 3a20 626c 6163 6b3b 2065 7874 7261 203d  : black; extra =
-000008c0: 3d20 2264 6576 656c 6f70 6d65 6e74 220a  = "development".
-000008d0: 5265 7175 6972 6573 2d44 6973 743a 2062  Requires-Dist: b
-000008e0: 6c61 636b 5b64 5d3b 2065 7874 7261 203d  lack[d]; extra =
-000008f0: 3d20 2264 6576 656c 6f70 6d65 6e74 220a  = "development".
-00000900: 5265 7175 6972 6573 2d44 6973 743a 2062  Requires-Dist: b
-00000910: 6c61 636b 5b6a 7570 7974 6572 5d3b 2065  lack[jupyter]; e
-00000920: 7874 7261 203d 3d20 2264 6576 656c 6f70  xtra == "develop
-00000930: 6d65 6e74 220a 5265 7175 6972 6573 2d44  ment".Requires-D
-00000940: 6973 743a 2062 7569 6c64 3b20 6578 7472  ist: build; extr
-00000950: 6120 3d3d 2022 6465 7665 6c6f 706d 656e  a == "developmen
-00000960: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
-00000970: 3a20 7079 7465 7374 3b20 6578 7472 6120  : pytest; extra 
-00000980: 3d3d 2022 6465 7665 6c6f 706d 656e 7422  == "development"
-00000990: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000009a0: 7079 7465 7374 2d63 6f76 3b20 6578 7472  pytest-cov; extr
-000009b0: 6120 3d3d 2022 6465 7665 6c6f 706d 656e  a == "developmen
-000009c0: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
-000009d0: 3a20 7370 6869 6e78 3b20 6578 7472 6120  : sphinx; extra 
-000009e0: 3d3d 2022 6465 7665 6c6f 706d 656e 7422  == "development"
-000009f0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000a00: 7370 6869 6e78 5f72 7464 5f74 6865 6d65  sphinx_rtd_theme
-00000a10: 3b20 6578 7472 6120 3d3d 2022 6465 7665  ; extra == "deve
-00000a20: 6c6f 706d 656e 7422 0a0a 3c68 3120 616c  lopment"..<h1 al
-00000a30: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
-00000a40: 3c69 6d67 0a20 2020 2077 6964 7468 3d22  <img.    width="
-00000a50: 3135 3022 0a20 2020 2068 6569 6768 743d  150".    height=
-00000a60: 2231 3530 220a 2020 2020 7372 633d 2268  "150".    src="h
-00000a70: 7474 7073 3a2f 2f75 7365 722d 696d 6167  ttps://user-imag
-00000a80: 6573 2e67 6974 6875 6275 7365 7263 6f6e  es.githubusercon
-00000a90: 7465 6e74 2e63 6f6d 2f31 3130 3736 3532  tent.com/1107652
-00000aa0: 352f 3136 3538 3336 3137 312d 3966 6664  5/165836171-9ffd
-00000ab0: 6561 3665 2d31 3633 332d 3434 3063 2d62  ea6e-1633-440c-b
-00000ac0: 6530 362d 6234 3665 3165 3365 3465 3034  e06-b46e1e3e4e04
-00000ad0: 2e70 6e67 220a 2020 3e0a 2020 3c62 723e  .png".  >.  <br>
-00000ae0: 0a20 204e 6569 6768 626f 726c 790a 3c2f  .  Neighborly.</
-00000af0: 6831 3e0a 0a3c 7020 616c 6967 6e3d 2263  h1>..<p align="c
-00000b00: 656e 7465 7222 3e0a 2020 3c69 6d67 2073  enter">.  <img s
-00000b10: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000b20: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000b30: 762f 6e65 6967 6862 6f72 6c79 223e 0a20  v/neighborly">. 
-00000b40: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000b50: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000b60: 6f2f 7079 7069 2f70 7976 6572 7369 6f6e  o/pypi/pyversion
-00000b70: 732f 6e65 6967 6862 6f72 6c79 223e 0a20  s/neighborly">. 
-00000b80: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000b90: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000ba0: 6f2f 7079 7069 2f6c 2f6e 6569 6768 626f  o/pypi/l/neighbo
-00000bb0: 726c 7922 3e0a 2020 3c69 6d67 2073 7263  rly">.  <img src
-00000bc0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00000bd0: 6965 6c64 732e 696f 2f70 7970 692f 646d  ields.io/pypi/dm
-00000be0: 2f6e 6569 6768 626f 726c 7922 3e0a 2020  /neighborly">.  
-00000bf0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000c00: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000c10: 2f62 6164 6765 2f63 6f64 6525 3230 7374  /badge/code%20st
-00000c20: 796c 652d 626c 6163 6b2d 626c 6163 6b22  yle-black-black"
-00000c30: 3e0a 2020 3c69 6d67 2073 7263 3d22 6874  >.  <img src="ht
-00000c40: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000c50: 732e 696f 2f62 6164 6765 2f25 3230 696d  s.io/badge/%20im
-00000c60: 706f 7274 732d 6973 6f72 742d 2532 3331  ports-isort-%231
-00000c70: 3637 3462 313f 7374 796c 653d 666c 6174  674b1?style=flat
-00000c80: 266c 6162 656c 436f 6c6f 723d 6566 3833  &labelColor=ef83
-00000c90: 3336 223e 0a3c 2f70 3e0a 0a4e 6569 6768  36">.</p>..Neigh
-00000ca0: 626f 726c 7920 6973 2061 6e20 6578 7465  borly is an exte
-00000cb0: 6e73 6962 6c65 2061 6765 6e74 2d62 6173  nsible agent-bas
-00000cc0: 6564 2073 6574 746c 656d 656e 7420 7369  ed settlement si
-00000cd0: 6d75 6c61 7469 6f6e 2e20 4974 2077 6173  mulation. It was
-00000ce0: 2062 7569 6c74 2074 6f20 6265 2061 2074   built to be a t
-00000cf0: 6f6f 6c20 666f 7220 656d 6572 6765 6e74  ool for emergent
-00000d00: 206e 6172 7261 7469 7665 2073 746f 7279   narrative story
-00000d10: 7465 6c6c 696e 6720 7265 7365 6172 6368  telling research
-00000d20: 2e20 4e65 6967 6862 6f72 6c79 2067 656e  . Neighborly gen
-00000d30: 6572 6174 6573 2061 2076 6972 7475 616c  erates a virtual
-00000d40: 2073 6574 746c 656d 656e 7420 616e 6420   settlement and 
-00000d50: 7369 6d75 6c61 7465 7320 7468 6520 696e  simulates the in
-00000d60: 6469 7669 6475 616c 206c 6976 6573 206f  dividual lives o
-00000d70: 6620 6974 7320 7265 7369 6465 6e74 7320  f its residents 
-00000d80: 6f76 6572 206d 756c 7469 706c 6520 6765  over multiple ge
-00000d90: 6e65 7261 7469 6f6e 732e 2049 7420 6d6f  nerations. It mo
-00000da0: 6465 6c73 2074 6865 2063 6861 7261 6374  dels the charact
-00000db0: 6572 7327 2074 7261 6974 732c 2073 7461  ers' traits, sta
-00000dc0: 7475 7365 732c 2072 656c 6174 696f 6e73  tuses, relations
-00000dd0: 6869 7073 2c20 6f63 6375 7061 7469 6f6e  hips, occupation
-00000de0: 732c 206c 6966 6520 6576 656e 7473 2c20  s, life events, 
-00000df0: 616e 6420 6d6f 7265 2e20 4e65 6967 6862  and more. Neighb
-00000e00: 6f72 6c79 2074 7261 636b 7320 616c 6c20  orly tracks all 
-00000e10: 7468 6520 6c69 6665 2065 7665 6e74 7320  the life events 
-00000e20: 2873 7461 7274 696e 6720 6120 6e65 7720  (starting a new 
-00000e30: 6a6f 622c 2066 616c 6c69 6e67 2069 6e20  job, falling in 
-00000e40: 6c6f 7665 2c20 7475 726e 696e 6720 696e  love, turning in
-00000e50: 746f 2061 2064 656d 6f6e 2c20 6574 632e  to a demon, etc.
-00000e60: 292c 2061 6e64 2074 6865 7365 2062 6563  ), and these bec
-00000e70: 6f6d 6520 7468 6520 6275 696c 6469 6e67  ome the building
-00000e80: 2062 6c6f 636b 7320 666f 7220 6372 6561   blocks for crea
-00000e90: 7469 6e67 2065 6d65 7267 656e 7420 7374  ting emergent st
-00000ea0: 6f72 6965 7320 6162 6f75 7420 6368 6172  ories about char
-00000eb0: 6163 7465 7273 2061 6e64 2074 6865 6972  acters and their
-00000ec0: 206c 6567 6163 6965 732e 2054 6865 2065   legacies. The e
-00000ed0: 6e74 6972 6520 6869 7374 6f72 7920 6f66  ntire history of
-00000ee0: 2074 6865 2073 6574 746c 656d 656e 7420   the settlement 
-00000ef0: 616e 6420 6974 7320 6765 6e65 7261 7469  and its generati
-00000f00: 6f6e 7320 6f66 2063 6861 7261 6374 6572  ons of character
-00000f10: 7320 6973 2074 6865 6e20 6d61 6465 2061  s is then made a
-00000f20: 7661 696c 6162 6c65 2066 6f72 2064 6174  vailable for dat
-00000f30: 6120 616e 616c 7973 6973 206f 7220 6173  a analysis or as
-00000f40: 2063 6f6e 7465 6e74 2066 6f72 206f 7468   content for oth
-00000f50: 6572 2061 7070 6c69 6361 7469 6f6e 7320  er applications 
-00000f60: 7375 6368 2061 7320 6761 6d65 732e 0a0a  such as games...
-00000f70: 4e65 6967 6862 6f72 6c79 2773 2077 6173  Neighborly's was
-00000f80: 2069 6e73 7069 7265 6420 5b5f 5461 6c6b   inspired [_Talk
-00000f90: 206f 6620 7468 6520 546f 776e 5f5d 2868   of the Town_](h
-00000fa0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000fb0: 6d2f 6a61 6d65 732d 6f77 656e 2d72 7961  m/james-owen-rya
-00000fc0: 6e2f 7461 6c6b 746f 776e 292c 2061 6e6f  n/talktown), ano
-00000fd0: 7468 6572 2073 6574 746c 656d 656e 7420  ther settlement 
-00000fe0: 7369 6d75 6c61 7469 6f6e 2066 6f72 2065  simulation for e
-00000ff0: 6d65 7267 656e 7420 6e61 7272 6174 6976  mergent narrativ
-00001000: 6520 7374 6f72 7974 656c 6c69 6e67 2072  e storytelling r
-00001010: 6573 6561 7263 682e 2049 7420 616c 736f  esearch. It also
-00001020: 2064 7261 7773 2069 6e73 7069 7261 7469   draws inspirati
-00001030: 6f6e 2066 726f 6d20 636f 6d6d 6572 6369  on from commerci
-00001040: 616c 2077 6f72 6c64 2d73 696d 756c 6174  al world-simulat
-00001050: 696f 6e20 6761 6d65 7320 6c69 6b65 205f  ion games like _
-00001060: 4361 7665 7320 6f66 2051 7564 5f2c 205f  Caves of Qud_, _
-00001070: 4477 6172 6620 466f 7274 7265 7373 5f2c  Dwarf Fortress_,
-00001080: 205f 4372 7573 6164 6572 204b 696e 6773   _Crusader Kings
-00001090: 5f2c 205f 5269 6d57 6f72 6c64 5f2c 2061  _, _RimWorld_, a
-000010a0: 6e64 205f 576f 726c 6442 6f78 5f2e 2049  nd _WorldBox_. I
-000010b0: 7420 6169 6d73 2074 6f20 6265 2061 6e20  t aims to be an 
-000010c0: 6561 7369 6c79 2063 7573 746f 6d69 7a61  easily customiza
-000010d0: 626c 6520 7369 6d75 6c61 7469 6f6e 2074  ble simulation t
-000010e0: 6861 7420 6361 6e20 6164 6170 7420 746f  hat can adapt to
-000010f0: 2076 6172 696f 7573 206e 6172 7261 7469   various narrati
-00001100: 7665 2073 6574 7469 6e67 7320 616e 6420  ve settings and 
-00001110: 7375 7070 6f72 7420 7265 7365 6172 6368  support research
-00001120: 206f 7220 656e 7465 7274 6169 6e6d 656e   or entertainmen
-00001130: 7420 7072 6f6a 6563 7473 2e0a 0a49 6620  t projects...If 
-00001140: 796f 7520 7573 6520 4e65 6967 6862 6f72  you use Neighbor
-00001150: 6c79 2069 6e20 6120 7072 6f6a 6563 742c  ly in a project,
-00001160: 2070 6c65 6173 6520 5b63 6974 6520 7468   please [cite th
-00001170: 6973 2072 6570 6f73 6974 6f72 795d 282e  is repository](.
-00001180: 2f43 4954 4154 494f 4e2e 6269 6229 2e20  /CITATION.bib). 
-00001190: 596f 7520 6361 6e20 7265 6164 2061 2063  You can read a c
-000011a0: 6f70 7920 6f66 0a4e 6569 6768 626f 726c  opy of.Neighborl
-000011b0: 7927 7320 6173 736f 6369 6174 6564 205b  y's associated [
-000011c0: 7061 7065 725d 2868 7474 7073 3a2f 2f73  paper](https://s
-000011d0: 6869 6a62 6579 2e67 6974 6875 622e 696f  hijbey.github.io
-000011e0: 2f70 7562 6c69 6361 7469 6f6e 732f 4e65  /publications/Ne
-000011f0: 6967 6862 6f72 6c79 2e70 6466 2920 7468  ighborly.pdf) th
-00001200: 6174 2077 6173 2070 7562 6c69 7368 6564  at was published
-00001210: 2069 6e20 7468 650a 7072 6f63 6565 6469   in the.proceedi
-00001220: 6e67 7320 6f66 2074 6865 2032 3032 3220  ngs of the 2022 
-00001230: 4945 4545 2043 6f6e 6665 7265 6e63 6520  IEEE Conference 
-00001240: 4f6e 2047 616d 6573 2e20 e29a a0ef b88f  On Games. ......
-00001250: 202a 2a57 6172 6e69 6e67 2a2a 3a20 506c   **Warning**: Pl
-00001260: 6561 7365 206e 6f74 6520 7468 6174 204e  ease note that N
-00001270: 6569 6768 626f 726c 7927 7320 6375 7272  eighborly's curr
-00001280: 656e 7420 7374 7275 6374 7572 650a 6469  ent structure.di
-00001290: 6666 6572 7320 6772 6561 746c 7920 6672  ffers greatly fr
-000012a0: 6f6d 2074 6865 2076 6572 7369 6f6e 2074  om the version t
-000012b0: 6865 2070 6170 6572 2064 6573 6372 6962  he paper describ
-000012c0: 6573 2e0a 0a23 2043 6f72 6520 4665 6174  es...# Core Feat
-000012d0: 7572 6573 0a0a 2d20 f09f 8f99 efb8 8f20  ures..- ....... 
-000012e0: 5072 6f63 6564 7572 616c 6c79 2067 656e  Procedurally gen
-000012f0: 6572 6174 6573 2061 2073 6574 746c 656d  erates a settlem
-00001300: 656e 7420 616e 6420 7468 6520 6869 7374  ent and the hist
-00001310: 6f72 7920 6f66 2069 7473 2072 6573 6964  ory of its resid
-00001320: 656e 7473 2e0a 2d20 f09f 9a80 2055 7469  ents..- .... Uti
-00001330: 6c69 7a65 2061 206c 6f77 2d66 6964 656c  lize a low-fidel
-00001340: 6974 7920 736f 6369 616c 2073 696d 756c  ity social simul
-00001350: 6174 696f 6e20 746f 2073 696d 756c 6174  ation to simulat
-00001360: 6520 6875 6e64 7265 6473 206f 6620 7965  e hundreds of ye
-00001370: 6172 7320 6f66 2077 6f72 6c64 2068 6973  ars of world his
-00001380: 746f 7279 2077 6974 6869 6e20 6d69 6e75  tory within minu
-00001390: 7465 732e 0a2d 20e2 9a99 efb8 8f20 4275  tes..- ...... Bu
-000013a0: 696c 7420 7573 696e 6720 616e 2065 6e74  ilt using an ent
-000013b0: 6974 792d 636f 6d70 6f6e 656e 7420 7379  ity-component sy
-000013c0: 7374 656d 2028 4543 5329 2061 7263 6869  stem (ECS) archi
-000013d0: 7465 6374 7572 650a 2d20 f09f 93a6 2050  tecture.- .... P
-000013e0: 6c75 6769 6e20 7379 7374 656d 2074 6f20  lugin system to 
-000013f0: 6c6f 6164 2061 6e64 2073 6861 7265 206e  load and share n
-00001400: 6577 2063 6f6e 7465 6e74 2e0a 2d20 f09f  ew content..- ..
-00001410: 9194 2043 6861 7261 6374 6572 7320 6361  .. Characters ca
-00001420: 6e20 7374 6172 7420 6275 7369 6e65 7373  n start business
-00001430: 6573 2061 6e64 2068 6f6c 6420 6a6f 6273  es and hold jobs
-00001440: 2e0a 2d20 efb8 8ff0 9fa7 ac20 4368 6172  ..- ....... Char
-00001450: 6163 7465 7273 2068 6176 6520 7472 6169  acters have trai
-00001460: 7473 2074 6861 7420 6d6f 6469 6679 2074  ts that modify t
-00001470: 6865 6972 2073 7461 7473 2061 6e64 2072  heir stats and r
-00001480: 656c 6174 696f 6e73 6869 7073 2e0a 2d20  elationships..- 
-00001490: e29d a4ef b88f 2043 6861 7261 6374 6572  ...... Character
-000014a0: 7320 666f 726d 2061 6e64 2063 756c 7469  s form and culti
-000014b0: 7661 7465 2072 656c 6174 696f 6e73 6869  vate relationshi
-000014c0: 7073 2062 6173 6564 206f 6e20 726f 6d61  ps based on roma
-000014d0: 6e63 6520 616e 6420 7265 7075 7461 7469  nce and reputati
-000014e0: 6f6e 2e0a 2d20 f09f 92a5 2053 696d 756c  on..- .... Simul
-000014f0: 6174 6520 7261 6e64 6f6d 206c 6966 6520  ate random life 
-00001500: 6576 656e 7473 2074 6861 7420 7370 6963  events that spic
-00001510: 6520 7570 2063 6861 7261 6374 6572 7327  e up characters'
-00001520: 206c 6976 6573 2e0a 2d20 e29a 96ef b88f   lives..- ......
-00001530: 2044 6566 696e 6520 536f 6369 616c 2052   Define Social R
-00001540: 756c 6573 2066 6f72 2068 6f77 2063 6861  ules for how cha
-00001550: 7261 6374 6572 7320 7368 6f75 6c64 2066  racters should f
-00001560: 6565 6c20 6162 6f75 7420 6561 6368 206f  eel about each o
-00001570: 7468 6572 2e0a 2d20 f09f 8fac 2044 6566  ther..- .... Def
-00001580: 696e 6520 6c6f 6361 7469 6f6e 2070 7265  ine location pre
-00001590: 6665 7265 6e63 6520 7275 6c65 7320 666f  ference rules fo
-000015a0: 7220 7768 6174 206c 6f63 6174 696f 6e73  r what locations
-000015b0: 2063 6861 7261 6374 6572 7320 6672 6571   characters freq
-000015c0: 7565 6e74 2e0a 2d20 f09f 9388 2055 7365  uent..- .... Use
-000015d0: 7320 5b50 6f6c 6172 735d 2868 7474 7073  s [Polars](https
-000015e0: 3a2f 2f77 7777 2e70 6f6c 612e 7273 2920  ://www.pola.rs) 
-000015f0: 666f 7220 6661 7374 2064 6174 6120 616e  for fast data an
-00001600: 616c 7973 6973 2e0a 2d20 f09f 939c 2045  alysis..- .... E
-00001610: 7870 6f72 7420 7369 6d75 6c61 7469 6f6e  xport simulation
-00001620: 2064 6174 6120 746f 204a 534f 4e2e 0a0a   data to JSON...
-00001630: 2320 5379 7374 656d 2063 6176 6561 7473  # System caveats
-00001640: 0a0a 2d20 4f6e 6c79 2073 696d 756c 6174  ..- Only simulat
-00001650: 6573 2061 2073 696e 676c 6520 7365 7474  es a single sett
-00001660: 6c65 6d65 6e74 0a2d 2043 6861 7261 6374  lement.- Charact
-00001670: 6572 7320 6361 6e20 6f6e 6c79 2068 6f6c  ers can only hol
-00001680: 6420 6f6e 6520 6f63 6375 7061 7469 6f6e  d one occupation
-00001690: 2061 7420 6120 7469 6d65 2e0a 2d20 446f   at a time..- Do
-000016a0: 6573 206e 6f74 206d 6f64 656c 2074 6865  es not model the
-000016b0: 2065 7861 6374 2070 6f73 6974 696f 6e20   exact position 
-000016c0: 6f66 2065 6e74 6974 6965 732e 0a0a 2320  of entities...# 
-000016d0: 5472 7920 4e65 6967 6862 6f72 6c79 2077  Try Neighborly w
-000016e0: 6974 686f 7574 2069 6e73 7461 6c6c 696e  ithout installin
-000016f0: 670a 0a4e 6569 6768 626f 726c 7920 6973  g..Neighborly is
-00001700: 2061 7661 696c 6162 6c65 2074 6f20 7573   available to us
-00001710: 6520 7769 7468 696e 2074 6869 7320 5b73  e within this [s
-00001720: 616d 706c 6520 476f 6f67 6c65 2043 6f6c  ample Google Col
-00001730: 6162 206e 6f74 6562 6f6f 6b5d 2868 7474  ab notebook](htt
-00001740: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
-00001750: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f64  rch.google.com/d
-00001760: 7269 7665 2f31 5778 5a6e 4352 3861 6665  rive/1WxZnCR8afe
-00001770: 6b66 426c 2d76 4936 5763 4963 5336 4f68  kfBl-vI6WcIcS6Oh
-00001780: 5247 646b 616d 3f75 7370 3d73 6861 7269  RGdkam?usp=shari
-00001790: 6e67 292e 2049 7420 636f 6e74 6169 6e73  ng). It contains
-000017a0: 2061 2062 6173 6963 2077 616c 6b74 6872   a basic walkthr
-000017b0: 6f75 6768 206f 6620 686f 7720 746f 2064  ough of how to d
-000017c0: 6566 696e 6520 636f 6e74 656e 7420 666f  efine content fo
-000017d0: 7220 7468 6520 7369 6d75 6c61 7469 6f6e  r the simulation
-000017e0: 2061 6e64 2069 6e73 7065 6374 2074 6865   and inspect the
-000017f0: 2067 656e 6572 6174 6564 2064 6174 612e   generated data.
-00001800: 0a0a 2320 496e 7374 616c 6c61 7469 6f6e  ..# Installation
-00001810: 0a0a 5468 6520 6c61 7465 7374 206f 6666  ..The latest off
-00001820: 6963 6961 6c20 7265 6c65 6173 6520 6f66  icial release of
-00001830: 204e 6569 6768 626f 726c 7920 6973 2061   Neighborly is a
-00001840: 7661 696c 6162 6c65 2074 6f20 696e 7374  vailable to inst
-00001850: 616c 6c20 6672 6f6d 205b 5079 5049 5d28  all from [PyPI](
-00001860: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00001870: 2f70 726f 6a65 6374 2f6e 6569 6768 626f  /project/neighbo
-00001880: 726c 792f 292e 0a0a 6060 6062 6173 680a  rly/)...```bash.
-00001890: 7069 7020 696e 7374 616c 6c20 6e65 6967  pip install neig
-000018a0: 6862 6f72 6c79 0a60 6060 0a0a 2323 2049  hborly.```..## I
-000018b0: 6e73 7461 6c6c 696e 6720 666f 7220 6c6f  nstalling for lo
-000018c0: 6361 6c20 6465 7665 6c6f 706d 656e 740a  cal development.
-000018d0: 0a49 6620 796f 7520 7769 7368 2074 6f20  .If you wish to 
-000018e0: 646f 776e 6c6f 6164 2061 204e 6569 6768  download a Neigh
-000018f0: 626f 726c 7920 666f 7220 6c6f 6361 6c20  borly for local 
-00001900: 6465 7665 6c6f 706d 656e 7420 6f72 2077  development or w
-00001910: 616e 7420 746f 2070 6c61 7920 6172 6f75  ant to play arou
-00001920: 6e64 2077 6974 680a 616e 7920 6f66 2074  nd with.any of t
-00001930: 6865 2073 616d 706c 6573 2c20 796f 7520  he samples, you 
-00001940: 6e65 6564 2074 6f20 636c 6f6e 6520 6f72  need to clone or
-00001950: 2064 6f77 6e6c 6f61 6420 7468 6973 2072   download this r
-00001960: 6570 6f73 6974 6f72 7920 616e 6420 696e  epository and in
-00001970: 7374 616c 6c0a 7573 696e 6720 7468 6520  stall.using the 
-00001980: 5f65 6469 7461 626c 655f 2066 6c61 6720  _editable_ flag 
-00001990: 282d 6529 2e20 506c 6561 7365 2073 6565  (-e). Please see
-000019a0: 2074 6865 2069 6e73 7472 7563 7469 6f6e   the instruction
-000019b0: 7320 6265 6c6f 772e 2054 6869 7320 636f  s below. This co
-000019c0: 6d6d 616e 6420 7769 6c6c 2069 6e73 7461  mmand will insta
-000019d0: 6c6c 0a61 204e 6569 6768 626f 726c 7920  ll.a Neighborly 
-000019e0: 696e 746f 2074 6865 2076 6972 7475 616c  into the virtual
-000019f0: 2065 6e76 6972 6f6e 6d65 6e74 2061 6c6f   environment alo
-00001a00: 6e67 2077 6974 6820 616c 6c20 6974 7320  ng with all its 
-00001a10: 6465 7065 6e64 656e 6369 6573 2061 6e64  dependencies and
-00001a20: 2061 2066 6577 0a61 6464 6974 696f 6e61   a few.additiona
-00001a30: 6c20 6465 7665 6c6f 706d 656e 7420 616e  l development an
-00001a40: 6420 7465 7374 696e 6720 6465 7065 6e64  d testing depend
-00001a50: 656e 6369 6573 2073 7563 6820 6173 205f  encies such as _
-00001a60: 626c 6163 6b5f 2c20 5f69 736f 7274 5f2c  black_, _isort_,
-00001a70: 2061 6e64 205f 7079 7465 7374 5f2e 0a0a   and _pytest_...
-00001a80: 6060 6062 6173 680a 2320 5374 6570 2031  ```bash.# Step 1
-00001a90: 3a20 436c 6f6e 6520 5265 706f 7369 746f  : Clone Reposito
-00001aa0: 7279 2061 6e64 2063 6861 6e67 6520 696e  ry and change in
-00001ab0: 746f 2070 726f 6a65 6374 2064 6972 6563  to project direc
-00001ac0: 746f 7279 0a67 6974 2063 6c6f 6e65 2068  tory.git clone h
-00001ad0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001ae0: 6d2f 5368 694a 6265 792f 6e65 6967 6862  m/ShiJbey/neighb
-00001af0: 6f72 6c79 2e67 6974 0a63 6420 6e65 6967  orly.git.cd neig
-00001b00: 6862 6f72 6c79 0a0a 2320 5374 6570 2032  hborly..# Step 2
-00001b10: 2028 4d61 634f 532f 4c69 6e75 7829 3a20   (MacOS/Linux): 
-00001b20: 4372 6561 7465 2061 6e64 2061 6374 6976  Create and activ
-00001b30: 6174 6520 6120 5079 7468 6f6e 2076 6972  ate a Python vir
-00001b40: 7475 616c 2065 6e76 6972 6f6e 6d65 6e74  tual environment
-00001b50: 0a70 7974 686f 6e33 202d 6d20 7665 6e76  .python3 -m venv
-00001b60: 2076 656e 760a 736f 7572 6365 202e 2f76   venv.source ./v
-00001b70: 656e 762f 6269 6e2f 6163 7469 7661 7465  env/bin/activate
-00001b80: 0a0a 2320 5374 6570 2032 2028 5769 6e64  ..# Step 2 (Wind
-00001b90: 6f77 7329 3a20 4372 6561 7465 2061 6e64  ows): Create and
-00001ba0: 2061 6374 6976 6174 6520 6120 5079 7468   activate a Pyth
-00001bb0: 6f6e 2076 6972 7475 616c 2065 6e76 6972  on virtual envir
-00001bc0: 6f6e 6d65 6e74 0a70 7974 686f 6e20 2d6d  onment.python -m
-00001bd0: 2076 656e 7620 7665 6e76 0a2e 5c76 656e   venv venv..\ven
-00001be0: 765c 5363 7269 7074 735c 4163 7469 7661  v\Scripts\Activa
-00001bf0: 7465 0a0a 2320 5374 6570 2033 3a20 496e  te..# Step 3: In
-00001c00: 7374 616c 6c20 6c6f 6361 6c20 6275 696c  stall local buil
-00001c10: 6420 616e 6420 6465 7065 6e64 656e 6369  d and dependenci
-00001c20: 6573 0a70 7974 686f 6e20 2d6d 2070 6970  es.python -m pip
-00001c30: 2069 6e73 7461 6c6c 202d 6520 222e 5b64   install -e ".[d
-00001c40: 6576 656c 6f70 6d65 6e74 5d22 0a60 6060  evelopment]".```
-00001c50: 0a0a 2320 5573 6167 650a 0a54 6865 2062  ..# Usage..The b
-00001c60: 6573 7420 7761 7920 746f 206c 6561 726e  est way to learn
-00001c70: 2068 6f77 2074 6f20 7573 6520 4e65 6967   how to use Neig
-00001c80: 6862 6f72 6c79 2069 7320 746f 2065 7870  hborly is to exp
-00001c90: 6c6f 7265 2074 6865 2076 6172 696f 7573  lore the various
-00001ca0: 2073 616d 706c 6573 2069 6e20 7468 6520   samples in the 
-00001cb0: 6073 616d 706c 6573 6020 6469 7265 6374  `samples` direct
-00001cc0: 6f72 790a 7468 6174 2064 656d 6f6e 7374  ory.that demonst
-00001cd0: 7261 7465 2068 6f77 2074 6f20 6372 6561  rate how to crea
-00001ce0: 7465 2063 7573 746f 6d20 7369 6d75 6c61  te custom simula
-00001cf0: 7469 6f6e 7320 616e 6420 636f 6c6c 6563  tions and collec
-00001d00: 7420 616e 6420 7669 7375 616c 697a 6520  t and visualize 
-00001d10: 6461 7461 2e20 496e 7465 7261 6374 6976  data. Interactiv
-00001d20: 6520 7361 6d70 6c65 7320 7769 7468 2074  e samples with t
-00001d30: 6865 2060 2e69 7079 6e62 600a 6578 7465  he `.ipynb`.exte
-00001d40: 6e73 696f 6e20 6172 6520 6d65 616e 7420  nsion are meant 
-00001d50: 746f 2062 6520 7275 6e20 7573 696e 6720  to be run using 
-00001d60: 5b4a 7570 7974 6572 204c 6162 5d28 6874  [Jupyter Lab](ht
-00001d70: 7470 733a 2f2f 6a75 7079 7465 722e 6f72  tps://jupyter.or
-00001d80: 672f 292e 2050 6c65 6173 6520 7275 6e20  g/). Please run 
-00001d90: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
-00001da0: 6d6d 616e 640a 746f 2065 6e73 7572 6520  mmand.to ensure 
-00001db0: 616c 6c20 6465 7065 6e64 656e 6369 6573  all dependencies
-00001dc0: 2061 7265 2069 6e73 7461 6c6c 6564 2066   are installed f
-00001dd0: 6f72 2074 6865 2073 616d 706c 6573 2e20  or the samples. 
-00001de0: 4d61 6b65 2073 7572 6520 7468 6174 2079  Make sure that y
-00001df0: 6f75 2776 6520 6163 7469 7661 7465 6420  ou've activated 
-00001e00: 796f 7572 2050 7974 686f 6e20 7669 7274  your Python virt
-00001e10: 7561 6c0a 656e 7669 726f 6e6d 656e 7420  ual.environment 
-00001e20: 6265 666f 7265 6861 6e64 2e0a 0a60 6060  beforehand...```
-00001e30: 6261 7368 0a70 7974 686f 6e20 2d6d 2070  bash.python -m p
-00001e40: 6970 2069 6e73 7461 6c6c 202d 6520 222e  ip install -e ".
-00001e50: 5b73 616d 706c 6573 5d22 0a60 6060 0a0a  [samples]".```..
-00001e60: 5468 656e 2c20 7275 6e20 7468 6520 666f  Then, run the fo
-00001e70: 6c6c 6f77 696e 6720 636f 6d6d 616e 6473  llowing commands
-00001e80: 2074 6f20 7275 6e20 7468 6520 7361 6d70   to run the samp
-00001e90: 6c65 2073 6372 6970 7473 206f 7220 6e6f  le scripts or no
-00001ea0: 7465 626f 6f6b 732e 0a0a 6060 6062 6173  tebooks...```bas
-00001eb0: 680a 2320 546f 2072 756e 2073 616d 706c  h.# To run sampl
-00001ec0: 6520 7363 7269 7074 732c 2075 7365 3a0a  e scripts, use:.
-00001ed0: 7079 7468 6f6e 202e 2f73 616d 706c 6573  python ./samples
-00001ee0: 2f3c 6e61 6d65 5f6f 665f 7361 6d70 6c65  /<name_of_sample
-00001ef0: 3e2e 7079 0a0a 2320 4578 706c 6f72 6520  >.py..# Explore 
-00001f00: 4950 7974 686f 6e20 6e6f 7465 626f 6f6b  IPython notebook
-00001f10: 7320 7573 696e 6720 4a75 7079 7465 7220  s using Jupyter 
-00001f20: 4c61 623a 0a6a 7570 7974 6572 2d6c 6162  Lab:.jupyter-lab
-00001f30: 0a60 6060 0a0a 2320 506c 7567 696e 730a  .```..# Plugins.
-00001f40: 0a50 6c75 6769 6e73 2061 7265 2069 6d70  .Plugins are imp
-00001f50: 6f72 7461 626c 6520 5079 7468 6f6e 206d  ortable Python m
-00001f60: 6f64 756c 6573 206f 7220 7061 636b 6167  odules or packag
-00001f70: 6573 2074 6861 7420 6164 6420 6e65 7720  es that add new 
-00001f80: 636f 6e74 656e 7420 746f 2061 2073 696d  content to a sim
-00001f90: 756c 6174 696f 6e2e 2054 6865 7920 616c  ulation. They al
-00001fa0: 6c6f 7720 7573 6572 7320 746f 2063 6861  low users to cha
-00001fb0: 6e67 650a 6120 7369 6d75 6c61 7469 6f6e  nge.a simulation
-00001fc0: 2773 2062 6568 6176 696f 7220 7769 7468  's behavior with
-00001fd0: 6f75 7420 6564 6974 696e 6720 7468 6520  out editing the 
-00001fe0: 636f 7265 206c 6962 7261 7279 2063 6f64  core library cod
-00001ff0: 652e 2041 6c6c 2070 6c75 6769 6e73 2073  e. All plugins s
-00002000: 686f 756c 6420 6861 7665 2061 2074 6f70  hould have a top
-00002010: 2d6c 6576 656c 0a60 6c6f 6164 5f70 6c75  -level.`load_plu
-00002020: 6769 6e28 7369 6d29 6020 6675 6e63 7469  gin(sim)` functi
-00002030: 6f6e 2074 6861 7420 6765 7473 2063 616c  on that gets cal
-00002040: 6c65 6420 746f 206c 6f61 6420 696e 2074  led to load in t
-00002050: 6865 2070 6c75 6769 6e20 636f 6e74 656e  he plugin conten
-00002060: 742e 0a0a 4173 2077 6974 6820 616e 7920  t...As with any 
-00002070: 7069 6563 6520 6f66 2073 6f66 7477 6172  piece of softwar
-00002080: 652c 2061 6c77 6179 7320 6578 7072 6573  e, always expres
-00002090: 7320 6361 7574 696f 6e20 7768 656e 2064  s caution when d
-000020a0: 6f77 6e6c 6f61 6469 6e67 2074 6869 7264  ownloading third
-000020b0: 2d70 6172 7479 2070 6c75 6769 6e73 2e20  -party plugins. 
-000020c0: 456e 7375 7265 2074 6865 7920 636f 6d65  Ensure they come
-000020d0: 2066 726f 6d20 610a 736f 7572 6365 2074   from a.source t
-000020e0: 6861 7420 796f 7520 7472 7573 742e 0a0a  hat you trust...
-000020f0: 546f 2072 6561 6420 6d6f 7265 2061 626f  To read more abo
-00002100: 7574 2070 6c75 6769 6e73 2c20 7669 7369  ut plugins, visi
-00002110: 7420 7468 6520 5b50 6c75 6769 6e73 5d28  t the [Plugins](
-00002120: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002130: 6f6d 2f53 6869 4a62 6579 2f6e 6569 6768  om/ShiJbey/neigh
-00002140: 626f 726c 792f 7769 6b69 2f70 6c75 6769  borly/wiki/plugi
-00002150: 6e73 2920 7365 6374 696f 6e20 6f66 2074  ns) section of t
-00002160: 6865 0a77 696b 692e 0a0a 2320 5465 7374  he.wiki...# Test
-00002170: 730a 0a4e 6569 6768 626f 726c 7920 7573  s..Neighborly us
-00002180: 6573 205b 5079 5465 7374 5d28 6874 7470  es [PyTest](http
-00002190: 733a 2f2f 646f 6373 2e70 7974 6573 742e  s://docs.pytest.
-000021a0: 6f72 672f 2920 666f 7220 756e 6974 2074  org/) for unit t
-000021b0: 6573 7469 6e67 2e20 416c 6c20 7465 7374  esting. All test
-000021c0: 7320 6172 6520 6c6f 6361 7465 6420 696e  s are located in
-000021d0: 2074 6865 2060 7465 7374 732f 6020 6469   the `tests/` di
-000021e0: 7265 6374 6f72 792e 2049 0a64 6f20 6d79  rectory. I.do my
-000021f0: 2062 6573 7420 746f 206b 6565 7020 7465   best to keep te
-00002200: 7374 7320 7570 6461 7465 642e 2048 6f77  sts updated. How
-00002210: 6576 6572 2c20 736f 6d65 2074 6573 7473  ever, some tests
-00002220: 206d 6179 206e 6565 6420 746f 2062 650a   may need to be.
-00002230: 6164 6465 6420 6f72 2075 7064 6174 6564  added or updated
-00002240: 2064 7565 2074 6f20 636f 6e73 7461 6e74   due to constant
-00002250: 2062 7265 616b 696e 6720 6368 616e 6765   breaking change
-00002260: 7320 6265 7477 6565 6e20 7265 6c65 6173  s between releas
-00002270: 6573 2e20 4966 2079 6f75 2077 616e 7420  es. If you want 
-00002280: 746f 2063 6f6e 7472 6962 7574 6520 756e  to contribute un
-00002290: 6974 2074 6573 7473 2c20 706c 6561 7365  it tests, please
-000022a0: 2072 6566 6572 0a74 6f20 5b43 4f4e 5452   refer.to [CONTR
-000022b0: 4942 5554 494e 472e 6d64 5d28 2e2f 434f  IBUTING.md](./CO
-000022c0: 4e54 5249 4255 5449 4e47 2e6d 6429 2e0a  NTRIBUTING.md)..
-000022d0: 0a60 6060 6261 7368 0a23 2053 7465 7020  .```bash.# Step 
-000022e0: 313a 2049 6e73 7461 6c6c 2061 6464 6974  1: Install addit
-000022f0: 696f 6e61 6c20 6465 7065 6e64 656e 6369  ional dependenci
-00002300: 6573 2066 6f72 2074 6573 7473 0a70 7974  es for tests.pyt
-00002310: 686f 6e20 2d6d 2070 6970 2069 6e73 7461  hon -m pip insta
-00002320: 6c6c 202d 6520 222e 5b64 6576 656c 6f70  ll -e ".[develop
-00002330: 6d65 6e74 5d22 0a0a 2320 5374 6570 2032  ment]"..# Step 2
-00002340: 3a20 5275 6e20 5079 7465 7374 0a70 7974  : Run Pytest.pyt
-00002350: 6573 740a 0a23 2053 7465 7033 203a 2028  est..# Step3 : (
-00002360: 4f70 7469 6f6e 616c 2920 4765 6e65 7261  Optional) Genera
-00002370: 7465 2061 2074 6573 7420 636f 7665 7261  te a test covera
-00002380: 6765 2072 6570 6f72 740a 7079 7465 7374  ge report.pytest
-00002390: 202d 2d63 6f76 3d6e 6569 6768 626f 726c   --cov=neighborl
-000023a0: 7920 7465 7374 732f 0a60 6060 0a0a 2320  y tests/.```..# 
-000023b0: 446f 6375 6d65 6e74 6174 696f 6e0a 0a54  Documentation..T
-000023c0: 6865 2062 6573 7420 706c 6163 6520 746f  he best place to
-000023d0: 2066 696e 6420 6578 616d 706c 6573 206f   find examples o
-000023e0: 6620 686f 7720 746f 2075 7365 204e 6569  f how to use Nei
-000023f0: 6768 626f 726c 7920 6973 2061 6374 7561  ghborly is actua
-00002400: 6c6c 7920 696e 2074 6865 2060 2e2f 7465  lly in the `./te
-00002410: 7374 7360 2064 6972 6563 746f 7279 2e20  sts` directory. 
-00002420: 5468 6572 6520 796f 7520 7769 6c6c 2066  There you will f
-00002430: 696e 6420 6578 616d 706c 6573 206f 6620  ind examples of 
-00002440: 6c6f 6164 696e 6720 636f 6e74 656e 7420  loading content 
-00002450: 6672 6f6d 2066 696c 6573 2c20 7275 6e6e  from files, runn
-00002460: 696e 6720 6120 7369 6d75 6c61 7469 6f6e  ing a simulation
-00002470: 2c20 616e 6420 7361 7669 6e67 2074 6865  , and saving the
-00002480: 206f 7574 7075 7420 746f 204a 534f 4e2e   output to JSON.
-00002490: 2054 6865 7265 2069 7320 616c 736f 2074   There is also t
-000024a0: 6865 205b 5265 6164 2074 6865 2044 6f63  he [Read the Doc
-000024b0: 735d 2868 7474 7073 3a2f 2f6e 6569 6768  s](https://neigh
-000024c0: 626f 726c 792e 7265 6164 7468 6564 6f63  borly.readthedoc
-000024d0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f69  s.io/en/latest/i
-000024e0: 6e64 6578 2e68 746d 6c29 2e20 486f 7765  ndex.html). Howe
-000024f0: 7665 722c 2074 6865 2064 6f63 7320 6861  ver, the docs ha
-00002500: 7320 6120 7465 6e64 656e 6379 2074 6f20  s a tendency to 
-00002510: 6265 206f 7574 206f 6620 6461 7465 2077  be out of date w
-00002520: 6865 6e20 6e65 772c 2070 6f74 656e 7469  hen new, potenti
-00002530: 616c 6c79 2062 7265 616b 696e 6720 6368  ally breaking ch
-00002540: 616e 6765 7320 6172 6520 6d61 6465 2074  anges are made t
-00002550: 6f20 7468 6520 6672 616d 6577 6f72 6b2e  o the framework.
-00002560: 2048 6f77 6576 6572 2c20 756e 6974 2074   However, unit t
-00002570: 6573 7473 2061 7265 2075 7064 6174 6564  ests are updated
-00002580: 2061 6c6d 6f73 7420 6576 6572 7920 7469   almost every ti
-00002590: 6d65 2061 206e 6577 2066 6561 7475 7265  me a new feature
-000025a0: 2069 7320 6164 6465 642e 0a0a 2320 4765   is added...# Ge
-000025b0: 7474 696e 6720 6865 6c70 2061 6e64 2073  tting help and s
-000025c0: 7562 6d69 7474 696e 6720 6275 6720 7265  ubmitting bug re
-000025d0: 706f 7274 730a 0a49 6620 796f 7520 6861  ports..If you ha
-000025e0: 7665 2061 6e79 2071 7565 7374 696f 6e73  ve any questions
-000025f0: 2c20 6665 6564 6261 636b 2c20 6f72 2070  , feedback, or p
-00002600: 726f 626c 656d 732c 2070 6c65 6173 6520  roblems, please 
-00002610: 6372 6561 7465 2061 206e 6577 2049 7373  create a new Iss
-00002620: 7565 2e20 4920 7769 6c6c 2064 6f20 6d79  ue. I will do my
-00002630: 2062 6573 7420 746f 2061 6e73 7765 7220   best to answer 
-00002640: 6173 2073 6f6f 6e20 6173 2049 0a63 616e  as soon as I.can
-00002650: 2e20 506c 6561 7365 2062 6520 7265 7370  . Please be resp
-00002660: 6563 7466 756c 2c20 616e 6420 4920 6170  ectful, and I ap
-00002670: 7072 6563 6961 7465 2079 6f75 7220 7061  preciate your pa
-00002680: 7469 656e 6365 2e0a 0a23 2043 6f6e 7472  tience...# Contr
-00002690: 6962 7574 696e 670a 0a43 6f6e 7472 6962  ibuting..Contrib
-000026a0: 7574 696f 6e73 2061 7265 2077 656c 636f  utions are welco
-000026b0: 6d65 2e20 506c 6561 7365 2072 6566 6572  me. Please refer
-000026c0: 2074 6f20 5b43 4f4e 5452 4942 5554 494e   to [CONTRIBUTIN
-000026d0: 472e 6d64 5d28 2e2f 434f 4e54 5249 4255  G.md](./CONTRIBU
-000026e0: 5449 4e47 2e6d 6429 2066 6f72 206d 6f72  TING.md) for mor
-000026f0: 6520 696e 666f 726d 6174 696f 6e20 6162  e information ab
-00002700: 6f75 7420 686f 7720 746f 2067 6574 0a69  out how to get.i
-00002710: 6e76 6f6c 7665 642e 0a0a 2320 4c69 6365  nvolved...# Lice
-00002720: 6e73 650a 0a54 6869 7320 7072 6f6a 6563  nse..This projec
-00002730: 7420 6973 206c 6963 656e 7365 6420 756e  t is licensed un
-00002740: 6465 7220 7468 6520 5b4d 4954 204c 6963  der the [MIT Lic
-00002750: 656e 7365 5d28 2e2f 4c49 4345 4e53 4529  ense](./LICENSE)
-00002760: 2e0a 0a23 2044 4d43 4120 5374 6174 656d  ...# DMCA Statem
-00002770: 656e 740a 0a55 706f 6e20 7265 6365 6970  ent..Upon receip
-00002780: 7420 6f66 2061 206e 6f74 6963 6520 616c  t of a notice al
-00002790: 6c65 6769 6e67 2063 6f70 7972 6967 6874  leging copyright
-000027a0: 2069 6e66 7269 6e67 656d 656e 742c 2049   infringement, I
-000027b0: 2077 696c 6c20 7461 6b65 2077 6861 7465   will take whate
-000027c0: 7665 7220 6163 7469 6f6e 2069 7420 6465  ver action it de
-000027d0: 656d 7320 6170 7072 6f70 7269 6174 6520  ems appropriate 
-000027e0: 7769 7468 696e 2069 7473 0a73 6f6c 6520  within its.sole 
-000027f0: 6469 7363 7265 7469 6f6e 2c20 696e 636c  discretion, incl
-00002800: 7564 696e 6720 7265 6d6f 7661 6c20 6f66  uding removal of
-00002810: 2074 6865 2061 6c6c 6567 6564 6c79 2069   the allegedly i
-00002820: 6e66 7269 6e67 696e 6720 6d61 7465 7269  nfringing materi
-00002830: 616c 732e 0a0a 5468 6520 7265 706f 2069  als...The repo i
-00002840: 6d61 6765 2069 7320 736f 6d65 7468 696e  mage is somethin
-00002850: 6720 6675 6e20 7468 6174 2049 206d 6164  g fun that I mad
-00002860: 652e 2049 206c 6f76 6520 5f54 6865 2053  e. I love _The S
-00002870: 696d 7073 6f6e 735f 2c20 616e 6420 4920  impsons_, and I 
-00002880: 636f 756c 646e 2774 2074 6869 6e6b 206f  couldn't think o
-00002890: 6620 616e 796f 6e65 206d 6f72 6520 6e65  f anyone more ne
-000028a0: 6967 6862 6f72 6c79 2074 6861 6e0a 4e65  ighborly than.Ne
-000028b0: 6420 466c 616e 6465 7273 2e20 4966 2074  d Flanders. If t
-000028c0: 6865 2063 6f70 7972 6967 6874 206f 776e  he copyright own
-000028d0: 6572 2066 6f72 205f 5468 6520 5369 6d70  er for _The Simp
-000028e0: 736f 6e73 5f20 776f 756c 6420 6c69 6b65  sons_ would like
-000028f0: 206d 6520 746f 2074 616b 6520 6974 2064   me to take it d
-00002900: 6f77 6e2c 2070 6c65 6173 6520 636f 6e74  own, please cont
-00002910: 6163 7420 6d65 2e20 5468 6520 7361 6d65  act me. The same
-00002920: 0a74 616b 6564 6f77 6e20 706f 6c69 6379  .takedown policy
-00002930: 2061 7070 6c69 6573 2074 6f20 636f 6465   applies to code
-00002940: 2073 616d 706c 6573 2069 6e73 7069 7265   samples inspire
-00002950: 6420 6279 2054 5620 7368 6f77 732c 206d  d by TV shows, m
-00002960: 6f76 6965 732c 2061 6e64 2067 616d 6573  ovies, and games
-00002970: 2e0a                                     ..
+00000030: 332e 302e 302e 6465 7631 0a53 756d 6d61  3.0.0.dev1.Summa
+00000040: 7279 3a20 4120 6368 6172 6163 7465 722d  ry: A character-
+00000050: 666f 6375 7365 6420 7365 7474 6c65 6d65  focused settleme
+00000060: 6e74 2067 656e 6572 6174 6f72 2075 7469  nt generator uti
+00000070: 6c69 7a69 6e67 2061 6765 6e74 2d62 6173  lizing agent-bas
+00000080: 6564 2073 6f63 6961 6c20 7369 6d75 6c61  ed social simula
+00000090: 7469 6f6e 2e0a 4175 7468 6f72 2d65 6d61  tion..Author-ema
+000000a0: 696c 3a20 5368 6920 4a6f 686e 736f 6e2d  il: Shi Johnson-
+000000b0: 4265 7920 3c73 6869 6a62 6579 4067 6d61  Bey <shijbey@gma
+000000c0: 696c 2e63 6f6d 3e0a 4c69 6365 6e73 653a  il.com>.License:
+000000d0: 2023 204d 4954 204c 4943 454e 5345 0a20   # MIT LICENSE. 
+000000e0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000000f0: 436f 7079 7269 6768 7420 3230 3232 2d32  Copyright 2022-2
+00000100: 3032 3420 5368 6920 4a6f 686e 736f 6e2d  024 Shi Johnson-
+00000110: 4265 7920 3c73 6869 6a62 6579 4067 6d61  Bey <shijbey@gma
+00000120: 696c 2e63 6f6d 3e0a 2020 2020 2020 2020  il.com>.        
+00000130: 0a20 2020 2020 2020 2050 6572 6d69 7373  .        Permiss
+00000140: 696f 6e20 6973 2068 6572 6562 7920 6772  ion is hereby gr
+00000150: 616e 7465 642c 2066 7265 6520 6f66 2063  anted, free of c
+00000160: 6861 7267 652c 2074 6f20 616e 7920 7065  harge, to any pe
+00000170: 7273 6f6e 206f 6274 6169 6e69 6e67 2061  rson obtaining a
+00000180: 2063 6f70 7920 6f66 2074 6869 730a 2020   copy of this.  
+00000190: 2020 2020 2020 736f 6674 7761 7265 2061        software a
+000001a0: 6e64 2061 7373 6f63 6961 7465 6420 646f  nd associated do
+000001b0: 6375 6d65 6e74 6174 696f 6e20 6669 6c65  cumentation file
+000001c0: 7320 2874 6865 2022 536f 6674 7761 7265  s (the "Software
+000001d0: 2229 2c20 746f 2064 6561 6c20 696e 2074  "), to deal in t
+000001e0: 6865 2053 6f66 7477 6172 650a 2020 2020  he Software.    
+000001f0: 2020 2020 7769 7468 6f75 7420 7265 7374      without rest
+00000200: 7269 6374 696f 6e2c 2069 6e63 6c75 6469  riction, includi
+00000210: 6e67 2077 6974 686f 7574 206c 696d 6974  ng without limit
+00000220: 6174 696f 6e20 7468 6520 7269 6768 7473  ation the rights
+00000230: 2074 6f20 7573 652c 2063 6f70 792c 206d   to use, copy, m
+00000240: 6f64 6966 792c 0a20 2020 2020 2020 206d  odify,.        m
+00000250: 6572 6765 2c20 7075 626c 6973 682c 2064  erge, publish, d
+00000260: 6973 7472 6962 7574 652c 2073 7562 6c69  istribute, subli
+00000270: 6365 6e73 652c 2061 6e64 2f6f 7220 7365  cense, and/or se
+00000280: 6c6c 2063 6f70 6965 7320 6f66 2074 6865  ll copies of the
+00000290: 2053 6f66 7477 6172 652c 2061 6e64 2074   Software, and t
+000002a0: 6f0a 2020 2020 2020 2020 7065 726d 6974  o.        permit
+000002b0: 2070 6572 736f 6e73 2074 6f20 7768 6f6d   persons to whom
+000002c0: 2074 6865 2053 6f66 7477 6172 6520 6973   the Software is
+000002d0: 2066 7572 6e69 7368 6564 2074 6f20 646f   furnished to do
+000002e0: 2073 6f2c 2073 7562 6a65 6374 2074 6f20   so, subject to 
+000002f0: 7468 6520 666f 6c6c 6f77 696e 670a 2020  the following.  
+00000300: 2020 2020 2020 636f 6e64 6974 696f 6e73        conditions
+00000310: 3a0a 2020 2020 2020 2020 0a20 2020 2020  :.        .     
+00000320: 2020 2054 6865 2061 626f 7665 2063 6f70     The above cop
+00000330: 7972 6967 6874 206e 6f74 6963 6520 616e  yright notice an
+00000340: 6420 7468 6973 2070 6572 6d69 7373 696f  d this permissio
+00000350: 6e20 6e6f 7469 6365 2073 6861 6c6c 2062  n notice shall b
+00000360: 6520 696e 636c 7564 6564 2069 6e20 616c  e included in al
+00000370: 6c20 636f 7069 6573 0a20 2020 2020 2020  l copies.       
+00000380: 206f 7220 7375 6273 7461 6e74 6961 6c20   or substantial 
+00000390: 706f 7274 696f 6e73 206f 6620 7468 6520  portions of the 
+000003a0: 536f 6674 7761 7265 2e0a 2020 2020 2020  Software..      
+000003b0: 2020 0a20 2020 2020 2020 2054 4845 2053    .        THE S
+000003c0: 4f46 5457 4152 4520 4953 2050 524f 5649  OFTWARE IS PROVI
+000003d0: 4445 4420 2241 5320 4953 222c 2057 4954  DED "AS IS", WIT
+000003e0: 484f 5554 2057 4152 5241 4e54 5920 4f46  HOUT WARRANTY OF
+000003f0: 2041 4e59 204b 494e 442c 2045 5850 5245   ANY KIND, EXPRE
+00000400: 5353 204f 5220 494d 504c 4945 442c 0a20  SS OR IMPLIED,. 
+00000410: 2020 2020 2020 2049 4e43 4c55 4449 4e47         INCLUDING
+00000420: 2042 5554 204e 4f54 204c 494d 4954 4544   BUT NOT LIMITED
+00000430: 2054 4f20 5448 4520 5741 5252 414e 5449   TO THE WARRANTI
+00000440: 4553 204f 4620 4d45 5243 4841 4e54 4142  ES OF MERCHANTAB
+00000450: 494c 4954 592c 2046 4954 4e45 5353 2046  ILITY, FITNESS F
+00000460: 4f52 2041 0a20 2020 2020 2020 2050 4152  OR A.        PAR
+00000470: 5449 4355 4c41 5220 5055 5250 4f53 4520  TICULAR PURPOSE 
+00000480: 414e 4420 4e4f 4e49 4e46 5249 4e47 454d  AND NONINFRINGEM
+00000490: 454e 542e 2049 4e20 4e4f 2045 5645 4e54  ENT. IN NO EVENT
+000004a0: 2053 4841 4c4c 2054 4845 2041 5554 484f   SHALL THE AUTHO
+000004b0: 5253 204f 5220 434f 5059 5249 4748 540a  RS OR COPYRIGHT.
+000004c0: 2020 2020 2020 2020 484f 4c44 4552 5320          HOLDERS 
+000004d0: 4245 204c 4941 424c 4520 464f 5220 414e  BE LIABLE FOR AN
+000004e0: 5920 434c 4149 4d2c 2044 414d 4147 4553  Y CLAIM, DAMAGES
+000004f0: 204f 5220 4f54 4845 5220 4c49 4142 494c   OR OTHER LIABIL
+00000500: 4954 592c 2057 4845 5448 4552 2049 4e20  ITY, WHETHER IN 
+00000510: 414e 2041 4354 494f 4e20 4f46 0a20 2020  AN ACTION OF.   
+00000520: 2020 2020 2043 4f4e 5452 4143 542c 2054       CONTRACT, T
+00000530: 4f52 5420 4f52 204f 5448 4552 5749 5345  ORT OR OTHERWISE
+00000540: 2c20 4152 4953 494e 4720 4652 4f4d 2c20  , ARISING FROM, 
+00000550: 4f55 5420 4f46 204f 5220 494e 2043 4f4e  OUT OF OR IN CON
+00000560: 4e45 4354 494f 4e20 5749 5448 2054 4845  NECTION WITH THE
+00000570: 2053 4f46 5457 4152 450a 2020 2020 2020   SOFTWARE.      
+00000580: 2020 4f52 2054 4845 2055 5345 204f 5220    OR THE USE OR 
+00000590: 4f54 4845 5220 4445 414c 494e 4753 2049  OTHER DEALINGS I
+000005a0: 4e20 5448 4520 534f 4654 5741 5245 2e0a  N THE SOFTWARE..
+000005b0: 2020 2020 2020 2020 0a50 726f 6a65 6374          .Project
+000005c0: 2d55 524c 3a20 486f 6d65 7061 6765 2c20  -URL: Homepage, 
+000005d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000005e0: 6f6d 2f53 6869 4a62 6579 2f6e 6569 6768  om/ShiJbey/neigh
+000005f0: 626f 726c 790a 5072 6f6a 6563 742d 5552  borly.Project-UR
+00000600: 4c3a 2042 7567 2054 7261 636b 6572 2c20  L: Bug Tracker, 
+00000610: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000620: 6f6d 2f53 6869 4a62 6579 2f6e 6569 6768  om/ShiJbey/neigh
+00000630: 626f 726c 792f 6973 7375 6573 0a50 726f  borly/issues.Pro
+00000640: 6a65 6374 2d55 524c 3a20 5265 706f 7369  ject-URL: Reposi
+00000650: 746f 7279 2c20 6874 7470 733a 2f2f 6769  tory, https://gi
+00000660: 7468 7562 2e63 6f6d 2f53 6869 4a42 6579  thub.com/ShiJBey
+00000670: 2f6e 6569 6768 626f 726c 792e 6769 740a  /neighborly.git.
+00000680: 5072 6f6a 6563 742d 5552 4c3a 2043 6861  Project-URL: Cha
+00000690: 6e67 656c 6f67 2c20 6874 7470 733a 2f2f  ngelog, https://
+000006a0: 6769 7468 7562 2e63 6f6d 2f53 6869 4a62  github.com/ShiJb
+000006b0: 6579 2f6e 6569 6768 626f 726c 792f 626c  ey/neighborly/bl
+000006c0: 6f62 2f6d 6169 6e2f 4348 414e 4745 4c4f  ob/main/CHANGELO
+000006d0: 472e 6d64 0a50 726f 6a65 6374 2d55 524c  G.md.Project-URL
+000006e0: 3a20 446f 6375 6d65 6e74 6174 696f 6e2c  : Documentation,
+000006f0: 2068 7474 7073 3a2f 2f6e 6569 6768 626f   https://neighbo
+00000700: 726c 792e 7265 6164 7468 6564 6f63 732e  rly.readthedocs.
+00000710: 696f 2f65 6e2f 6c61 7465 7374 2f0a 4b65  io/en/latest/.Ke
+00000720: 7977 6f72 6473 3a20 736f 6369 616c 2073  ywords: social s
+00000730: 696d 756c 6174 696f 6e2c 6761 6d65 732c  imulation,games,
+00000740: 7369 6d75 6c61 7469 6f6e 2c61 7274 6966  simulation,artif
+00000750: 6963 6961 6c20 696e 7465 6c6c 6967 656e  icial intelligen
+00000760: 6365 2c61 6765 6e74 2d62 6173 6564 206d  ce,agent-based m
+00000770: 6f64 656c 696e 672c 6d75 6c74 6961 6765  odeling,multiage
+00000780: 6e74 2073 7973 7465 6d73 2c65 6d65 7267  nt systems,emerg
+00000790: 656e 7420 6e61 7272 6174 6976 652c 6e61  ent narrative,na
+000007a0: 7272 6174 6976 6520 6765 6e65 7261 7469  rrative generati
+000007b0: 6f6e 2c69 6e74 6572 6163 7469 7665 2073  on,interactive s
+000007c0: 746f 7279 7465 6c6c 696e 672c 7365 7474  torytelling,sett
+000007d0: 6c65 6d65 6e74 2073 696d 756c 6174 696f  lement simulatio
+000007e0: 6e0a 436c 6173 7369 6669 6572 3a20 496e  n.Classifier: In
+000007f0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000800: 3a3a 2044 6576 656c 6f70 6572 730a 436c  :: Developers.Cl
+00000810: 6173 7369 6669 6572 3a20 496e 7465 6e64  assifier: Intend
+00000820: 6564 2041 7564 6965 6e63 6520 3a3a 2053  ed Audience :: S
+00000830: 6369 656e 6365 2f52 6573 6561 7263 680a  cience/Research.
+00000840: 436c 6173 7369 6669 6572 3a20 4c69 6365  Classifier: Lice
+00000850: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000860: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+00000870: 7365 0a43 6c61 7373 6966 6965 723a 204f  se.Classifier: O
+00000880: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000890: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+000008a0: 740a 436c 6173 7369 6669 6572 3a20 5072  t.Classifier: Pr
+000008b0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000008c0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000008d0: 3320 3a3a 204f 6e6c 790a 436c 6173 7369  3 :: Only.Classi
+000008e0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000008f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000900: 7468 6f6e 203a 3a20 332e 380a 436c 6173  thon :: 3.8.Clas
+00000910: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000920: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000930: 5079 7468 6f6e 203a 3a20 332e 390a 436c  Python :: 3.9.Cl
+00000940: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000950: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000960: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+00000970: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000980: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000990: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000009a0: 2e31 310a 436c 6173 7369 6669 6572 3a20  .11.Classifier: 
+000009b0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000009c0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000009d0: 3a20 332e 3132 0a43 6c61 7373 6966 6965  : 3.12.Classifie
+000009e0: 723a 2054 6f70 6963 203a 3a20 4761 6d65  r: Topic :: Game
+000009f0: 732f 456e 7465 7274 6169 6e6d 656e 7420  s/Entertainment 
+00000a00: 3a3a 2053 696d 756c 6174 696f 6e0a 436c  :: Simulation.Cl
+00000a10: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
+00000a20: 3a3a 2053 6369 656e 7469 6669 632f 456e  :: Scientific/En
+00000a30: 6769 6e65 6572 696e 670a 436c 6173 7369  gineering.Classi
+00000a40: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
+00000a50: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
+00000a60: 6572 696e 6720 3a3a 2041 7274 6966 6963  ering :: Artific
+00000a70: 6961 6c20 496e 7465 6c6c 6967 656e 6365  ial Intelligence
+00000a80: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+00000a90: 6963 203a 3a20 5363 6965 6e74 6966 6963  ic :: Scientific
+00000aa0: 2f45 6e67 696e 6565 7269 6e67 203a 3a20  /Engineering :: 
+00000ab0: 4172 7469 6669 6369 616c 204c 6966 650a  Artificial Life.
+00000ac0: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+00000ad0: 6320 3a3a 2053 6f63 696f 6c6f 6779 0a43  c :: Sociology.C
+00000ae0: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
+00000af0: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
+00000b00: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
+00000b10: 6172 6965 730a 436c 6173 7369 6669 6572  aries.Classifier
+00000b20: 3a20 546f 7069 6320 3a3a 2053 6f66 7477  : Topic :: Softw
+00000b30: 6172 6520 4465 7665 6c6f 706d 656e 7420  are Development 
+00000b40: 3a3a 204c 6962 7261 7269 6573 203a 3a20  :: Libraries :: 
+00000b50: 4170 706c 6963 6174 696f 6e20 4672 616d  Application Fram
+00000b60: 6577 6f72 6b73 0a43 6c61 7373 6966 6965  eworks.Classifie
+00000b70: 723a 2054 7970 696e 6720 3a3a 2054 7970  r: Typing :: Typ
+00000b80: 6564 0a52 6571 7569 7265 732d 5079 7468  ed.Requires-Pyth
+00000b90: 6f6e 3a20 3e3d 332e 380a 4465 7363 7269  on: >=3.8.Descri
+00000ba0: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
+00000bb0: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
+00000bc0: 6e0a 4c69 6365 6e73 652d 4669 6c65 3a20  n.License-File: 
+00000bd0: 4c49 4345 4e53 452e 6d64 0a52 6571 7569  LICENSE.md.Requi
+00000be0: 7265 732d 4469 7374 3a20 6573 7065 723d  res-Dist: esper=
+00000bf0: 3d32 2e2a 0a52 6571 7569 7265 732d 4469  =2.*.Requires-Di
+00000c00: 7374 3a20 6f72 6465 7265 642d 7365 743d  st: ordered-set=
+00000c10: 3d34 2e2a 0a52 6571 7569 7265 732d 4469  =4.*.Requires-Di
+00000c20: 7374 3a20 7461 6275 6c61 7465 3d3d 302e  st: tabulate==0.
+00000c30: 392e 2a0a 5265 7175 6972 6573 2d44 6973  9.*.Requires-Dis
+00000c40: 743a 2050 7959 414d 4c3d 3d36 2e30 2e2a  t: PyYAML==6.0.*
+00000c50: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000c60: 7471 646d 3d3d 342e 2a0a 5265 7175 6972  tqdm==4.*.Requir
+00000c70: 6573 2d44 6973 743a 2070 7964 616e 7469  es-Dist: pydanti
+00000c80: 633d 3d32 2e2a 0a52 6571 7569 7265 732d  c==2.*.Requires-
+00000c90: 4469 7374 3a20 7061 6e64 6173 3d3d 322e  Dist: pandas==2.
+00000ca0: 2a0a 5072 6f76 6964 6573 2d45 7874 7261  *.Provides-Extra
+00000cb0: 3a20 6465 7665 6c6f 706d 656e 740a 5265  : development.Re
+00000cc0: 7175 6972 6573 2d44 6973 743a 2069 736f  quires-Dist: iso
+00000cd0: 7274 3b20 6578 7472 6120 3d3d 2022 6465  rt; extra == "de
+00000ce0: 7665 6c6f 706d 656e 7422 0a52 6571 7569  velopment".Requi
+00000cf0: 7265 732d 4469 7374 3a20 626c 6163 6b3b  res-Dist: black;
+00000d00: 2065 7874 7261 203d 3d20 2264 6576 656c   extra == "devel
+00000d10: 6f70 6d65 6e74 220a 5265 7175 6972 6573  opment".Requires
+00000d20: 2d44 6973 743a 2062 6c61 636b 5b64 5d3b  -Dist: black[d];
+00000d30: 2065 7874 7261 203d 3d20 2264 6576 656c   extra == "devel
+00000d40: 6f70 6d65 6e74 220a 5265 7175 6972 6573  opment".Requires
+00000d50: 2d44 6973 743a 2062 7569 6c64 3b20 6578  -Dist: build; ex
+00000d60: 7472 6120 3d3d 2022 6465 7665 6c6f 706d  tra == "developm
+00000d70: 656e 7422 0a52 6571 7569 7265 732d 4469  ent".Requires-Di
+00000d80: 7374 3a20 7079 7465 7374 3b20 6578 7472  st: pytest; extr
+00000d90: 6120 3d3d 2022 6465 7665 6c6f 706d 656e  a == "developmen
+00000da0: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
+00000db0: 3a20 7079 7465 7374 2d63 6f76 3b20 6578  : pytest-cov; ex
+00000dc0: 7472 6120 3d3d 2022 6465 7665 6c6f 706d  tra == "developm
+00000dd0: 656e 7422 0a52 6571 7569 7265 732d 4469  ent".Requires-Di
+00000de0: 7374 3a20 7370 6869 6e78 3b20 6578 7472  st: sphinx; extr
+00000df0: 6120 3d3d 2022 6465 7665 6c6f 706d 656e  a == "developmen
+00000e00: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
+00000e10: 3a20 7370 6869 6e78 5f72 7464 5f74 6865  : sphinx_rtd_the
+00000e20: 6d65 3b20 6578 7472 6120 3d3d 2022 6465  me; extra == "de
+00000e30: 7665 6c6f 706d 656e 7422 0a0a 3c68 3120  velopment"..<h1 
+00000e40: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00000e50: 2020 3c69 6d67 0a20 2020 2077 6964 7468    <img.    width
+00000e60: 3d22 3135 3022 0a20 2020 2068 6569 6768  ="150".    heigh
+00000e70: 743d 2231 3530 220a 2020 2020 7372 633d  t="150".    src=
+00000e80: 2268 7474 7073 3a2f 2f75 7365 722d 696d  "https://user-im
+00000e90: 6167 6573 2e67 6974 6875 6275 7365 7263  ages.githubuserc
+00000ea0: 6f6e 7465 6e74 2e63 6f6d 2f31 3130 3736  ontent.com/11076
+00000eb0: 3532 352f 3136 3538 3336 3137 312d 3966  525/165836171-9f
+00000ec0: 6664 6561 3665 2d31 3633 332d 3434 3063  fdea6e-1633-440c
+00000ed0: 2d62 6530 362d 6234 3665 3165 3365 3465  -be06-b46e1e3e4e
+00000ee0: 3034 2e70 6e67 220a 2020 3e0a 2020 3c62  04.png".  >.  <b
+00000ef0: 723e 0a20 204e 6569 6768 626f 726c 790a  r>.  Neighborly.
+00000f00: 3c2f 6831 3e0a 0a3c 7020 616c 6967 6e3d  </h1>..<p align=
+00000f10: 2263 656e 7465 7222 3e0a 2020 3c61 2068  "center">.  <a h
+00000f20: 7265 663d 2268 7474 7073 3a2f 2f6e 6569  ref="https://nei
+00000f30: 6768 626f 726c 792e 7265 6164 7468 6564  ghborly.readthed
+00000f40: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00000f50: 2f69 6e64 6578 2e68 746d 6c22 3e44 6f63  /index.html">Doc
+00000f60: 756d 656e 7461 7469 6f6e 3c2f 613e 207c  umentation</a> |
+00000f70: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000f80: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000f90: 6a65 6374 2f6e 6569 6768 626f 726c 7922  ject/neighborly"
+00000fa0: 3e50 7950 493c 2f61 3e20 7c20 3c61 2068  >PyPI</a> | <a h
+00000fb0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000fc0: 6875 622e 636f 6d2f 5368 694a 6265 792f  hub.com/ShiJbey/
+00000fd0: 6e65 6967 6862 6f72 6c79 223e 4769 7448  neighborly">GitH
+00000fe0: 7562 3c2f 613e 0a3c 2f70 3e0a 0a3c 7020  ub</a>.</p>..<p 
+00000ff0: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00001000: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00001010: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00001020: 696f 2f70 7970 692f 762f 6e65 6967 6862  io/pypi/v/neighb
+00001030: 6f72 6c79 2220 616c 743d 2250 7950 4920  orly" alt="PyPI 
+00001040: 7665 7273 696f 6e20 6261 6467 6522 3e0a  version badge">.
+00001050: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00001060: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00001070: 696f 2f70 7970 692f 7079 7665 7273 696f  io/pypi/pyversio
+00001080: 6e73 2f6e 6569 6768 626f 726c 7922 2061  ns/neighborly" a
+00001090: 6c74 3d22 5375 7070 6f72 7465 6420 5079  lt="Supported Py
+000010a0: 7468 6f6e 2056 6572 7369 6f6e 7320 6261  thon Versions ba
+000010b0: 6467 6522 3e0a 2020 3c69 6d67 2073 7263  dge">.  <img src
+000010c0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000010d0: 6965 6c64 732e 696f 2f70 7970 692f 6c2f  ields.io/pypi/l/
+000010e0: 6e65 6967 6862 6f72 6c79 2220 616c 743d  neighborly" alt=
+000010f0: 224d 4954 204c 6963 656e 7365 2062 6164  "MIT License bad
+00001100: 6765 223e 0a20 203c 696d 6720 7372 633d  ge">.  <img src=
+00001110: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00001120: 656c 6473 2e69 6f2f 7079 7069 2f64 6d2f  elds.io/pypi/dm/
+00001130: 6e65 6967 6862 6f72 6c79 2220 616c 743d  neighborly" alt=
+00001140: 2250 7950 4920 646f 776e 6c6f 6164 7320  "PyPI downloads 
+00001150: 6261 6467 6522 3e0a 2020 3c69 6d67 2073  badge">.  <img s
+00001160: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00001170: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00001180: 2f63 6f64 6525 3230 7374 796c 652d 626c  /code%20style-bl
+00001190: 6163 6b2d 626c 6163 6b22 2061 6c74 3d22  ack-black" alt="
+000011a0: 426c 6163 6b20 666f 726d 6174 7465 7220  Black formatter 
+000011b0: 6261 6467 6522 3e0a 2020 3c69 6d67 2073  badge">.  <img s
+000011c0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+000011d0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+000011e0: 2f25 3230 696d 706f 7274 732d 6973 6f72  /%20imports-isor
+000011f0: 742d 2532 3331 3637 3462 313f 7374 796c  t-%231674b1?styl
+00001200: 653d 666c 6174 266c 6162 656c 436f 6c6f  e=flat&labelColo
+00001210: 723d 6566 3833 3336 2220 616c 743d 2249  r=ef8336" alt="I
+00001220: 536f 7274 2062 6164 6765 223e 0a3c 2f70  Sort badge">.</p
+00001230: 3e0a 0a4e 6569 6768 626f 726c 7920 6973  >..Neighborly is
+00001240: 2061 6e20 6167 656e 742d 6261 7365 6420   an agent-based 
+00001250: 7365 7474 6c65 6d65 6e74 2073 696d 756c  settlement simul
+00001260: 6174 696f 6e20 7468 6174 2067 656e 6572  ation that gener
+00001270: 6174 6573 2062 6163 6b73 746f 7279 2064  ates backstory d
+00001280: 6174 6120 666f 7220 6368 6172 6163 7465  ata for characte
+00001290: 7273 206c 6976 696e 6720 696e 2061 2070  rs living in a p
+000012a0: 726f 6365 6475 7261 6c6c 7920 6765 6e65  rocedurally gene
+000012b0: 7261 7465 6420 7365 7474 6c65 6d65 6e74  rated settlement
+000012c0: 2e20 4974 2077 6173 2062 7569 6c74 2074  . It was built t
+000012d0: 6f20 6265 2061 2074 6f6f 6c20 666f 7220  o be a tool for 
+000012e0: 656d 6572 6765 6e74 206e 6172 7261 7469  emergent narrati
+000012f0: 7665 2073 746f 7279 7465 6c6c 696e 6720  ve storytelling 
+00001300: 7265 7365 6172 6368 2e20 4e65 6967 6862  research. Neighb
+00001310: 6f72 6c79 206d 6f64 656c 7320 7468 6520  orly models the 
+00001320: 6368 6172 6163 7465 7273 2720 7472 6169  characters' trai
+00001330: 7473 2c20 7374 6174 7573 6573 2c20 7265  ts, statuses, re
+00001340: 6c61 7469 6f6e 7368 6970 732c 206f 6363  lationships, occ
+00001350: 7570 6174 696f 6e73 2c20 6c69 6665 2065  upations, life e
+00001360: 7665 6e74 732c 2065 7463 2e20 6f76 6572  vents, etc. over
+00001370: 2064 6563 6164 6573 206f 6620 7369 6d75   decades of simu
+00001380: 6c61 7465 6420 7469 6d65 2e20 5468 6520  lated time. The 
+00001390: 656e 7469 7265 2068 6973 746f 7279 206f  entire history o
+000013a0: 6620 7468 6520 7365 7474 6c65 6d65 6e74  f the settlement
+000013b0: 2061 6e64 2069 7473 2067 656e 6572 6174   and its generat
+000013c0: 696f 6e73 206f 6620 6368 6172 6163 7465  ions of characte
+000013d0: 7273 2069 7320 6d61 6465 2061 7661 696c  rs is made avail
+000013e0: 6162 6c65 2066 6f72 2064 6174 6120 616e  able for data an
+000013f0: 616c 7973 6973 2061 6e64 2065 7870 6f72  alysis and expor
+00001400: 7469 6e67 2e20 4e65 6967 6862 6f72 6c79  ting. Neighborly
+00001410: 2061 696d 7320 746f 2062 6520 616e 2065   aims to be an e
+00001420: 6173 696c 7920 6375 7374 6f6d 697a 6162  asily customizab
+00001430: 6c65 2073 696d 756c 6174 696f 6e20 7468  le simulation th
+00001440: 6174 2063 616e 2061 6461 7074 2074 6f20  at can adapt to 
+00001450: 7661 7269 6f75 7320 6e61 7272 6174 6976  various narrativ
+00001460: 6520 7365 7474 696e 6773 2061 6e64 2073  e settings and s
+00001470: 7570 706f 7274 2072 6573 6561 7263 6820  upport research 
+00001480: 6f72 2065 6e74 6572 7461 696e 6d65 6e74  or entertainment
+00001490: 2070 726f 6a65 6374 732e 0a0a 4e65 6967   projects...Neig
+000014a0: 6862 6f72 6c79 2773 2077 6173 2069 6e73  hborly's was ins
+000014b0: 7069 7265 6420 5b5f 5461 6c6b 206f 6620  pired [_Talk of 
+000014c0: 7468 6520 546f 776e 5f5d 2868 7474 7073  the Town_](https
+000014d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a61  ://github.com/ja
+000014e0: 6d65 732d 6f77 656e 2d72 7961 6e2f 7461  mes-owen-ryan/ta
+000014f0: 6c6b 746f 776e 292c 2061 6e6f 7468 6572  lktown), another
+00001500: 2073 6574 746c 656d 656e 7420 7369 6d75   settlement simu
+00001510: 6c61 7469 6f6e 2066 6f72 2065 6d65 7267  lation for emerg
+00001520: 656e 7420 6e61 7272 6174 6976 6520 7374  ent narrative st
+00001530: 6f72 7974 656c 6c69 6e67 2072 6573 6561  orytelling resea
+00001540: 7263 682e 2049 7420 616c 736f 2064 7261  rch. It also dra
+00001550: 7773 2069 6e73 7069 7261 7469 6f6e 2066  ws inspiration f
+00001560: 726f 6d20 636f 6d6d 6572 6369 616c 2077  rom commercial w
+00001570: 6f72 6c64 2d73 696d 756c 6174 696f 6e20  orld-simulation 
+00001580: 6761 6d65 7320 6c69 6b65 205f 4361 7665  games like _Cave
+00001590: 7320 6f66 2051 7564 5f2c 205f 4477 6172  s of Qud_, _Dwar
+000015a0: 6620 466f 7274 7265 7373 5f2c 205f 4372  f Fortress_, _Cr
+000015b0: 7573 6164 6572 204b 696e 6773 5f2c 205f  usader Kings_, _
+000015c0: 5269 6d57 6f72 6c64 5f2c 2061 6e64 205f  RimWorld_, and _
+000015d0: 576f 726c 6442 6f78 5f2e 0a0a 4966 2079  WorldBox_...If y
+000015e0: 6f75 2075 7365 204e 6569 6768 626f 726c  ou use Neighborl
+000015f0: 7920 696e 2061 2070 726f 6a65 6374 2c20  y in a project, 
+00001600: 706c 6561 7365 2063 6974 6520 7468 6973  please cite this
+00001610: 2072 6570 6f73 6974 6f72 792e 2059 6f75   repository. You
+00001620: 2063 616e 2072 6561 640a 4e65 6967 6862   can read.Neighb
+00001630: 6f72 6c79 2773 2061 7373 6f63 6961 7465  orly's associate
+00001640: 6420 5b70 6170 6572 5d28 6874 7470 733a  d [paper](https:
+00001650: 2f2f 7368 696a 6265 792e 6769 7468 7562  //shijbey.github
+00001660: 2e69 6f2f 7075 626c 6963 6174 696f 6e73  .io/publications
+00001670: 2f4e 6569 6768 626f 726c 792e 7064 6629  /Neighborly.pdf)
+00001680: 2074 6861 7420 7761 7320 7075 626c 6973   that was publis
+00001690: 6865 6420 696e 2074 6865 0a70 726f 6365  hed in the.proce
+000016a0: 6564 696e 6773 206f 6620 7468 6520 3230  edings of the 20
+000016b0: 3232 2049 4545 4520 436f 6e66 6572 656e  22 IEEE Conferen
+000016c0: 6365 204f 6e20 4761 6d65 732e 0a0a 6060  ce On Games...``
+000016d0: 6074 6578 740a 4069 6e70 726f 6365 6564  `text.@inproceed
+000016e0: 696e 6773 7b6a 6f68 6e73 6f6e 6265 7932  ings{johnsonbey2
+000016f0: 3032 326e 6569 6768 626f 726c 792c 0a20  022neighborly,. 
+00001700: 2020 2074 6974 6c65 203d 207b 4e65 6967     title = {Neig
+00001710: 6862 6f72 6c79 3a20 4120 5361 6e64 626f  hborly: A Sandbo
+00001720: 7820 666f 7220 5369 6d75 6c61 7469 6f6e  x for Simulation
+00001730: 2d62 6173 6564 2045 6d65 7267 656e 7420  -based Emergent 
+00001740: 4e61 7272 6174 6976 657d 2c0a 2020 2020  Narrative},.    
+00001750: 6175 7468 6f72 203d 207b 4a6f 686e 736f  author = {Johnso
+00001760: 6e2d 4265 792c 2053 6869 2061 6e64 204e  n-Bey, Shi and N
+00001770: 656c 736f 6e2c 204d 6172 6b20 4a20 616e  elson, Mark J an
+00001780: 6420 4d61 7465 6173 2c20 4d69 6368 6165  d Mateas, Michae
+00001790: 6c7d 2c0a 2020 2020 626f 6f6b 7469 746c  l},.    booktitl
+000017a0: 6520 3d20 7b32 3032 3220 4945 4545 2043  e = {2022 IEEE C
+000017b0: 6f6e 6665 7265 6e63 6520 6f6e 2047 616d  onference on Gam
+000017c0: 6573 2028 436f 4729 7d2c 0a20 2020 2070  es (CoG)},.    p
+000017d0: 6167 6573 203d 207b 3432 352d 2d34 3332  ages = {425--432
+000017e0: 7d2c 0a20 2020 2079 6561 7220 3d20 7b32  },.    year = {2
+000017f0: 3032 327d 2c0a 2020 2020 6f72 6761 6e69  022},.    organi
+00001800: 7a61 7469 6f6e 203d 207b 4945 4545 7d0a  zation = {IEEE}.
+00001810: 7d0a 6060 600a 0a3e 205b 2149 4d50 4f52  }.```..> [!IMPOR
+00001820: 5441 4e54 5d0a 3e20 4e65 6967 6862 6f72  TANT].> Neighbor
+00001830: 6c79 2773 2063 7572 7265 6e74 2061 7263  ly's current arc
+00001840: 6869 7465 6374 7572 6520 6469 6666 6572  hitecture differ
+00001850: 7320 6672 6f6d 2077 6861 7420 6973 2064  s from what is d
+00001860: 6573 6372 6962 6564 2069 6e20 7468 6520  escribed in the 
+00001870: 7061 7065 722e 2050 6c65 6173 6520 7365  paper. Please se
+00001880: 6520 7468 6520 5b44 6966 6665 7265 6e63  e the [Differenc
+00001890: 6573 2066 726f 6d20 7468 6520 5061 7065  es from the Pape
+000018a0: 725d 2823 e284 b9ef b88f 2d64 6966 6665  r](#......-diffe
+000018b0: 7265 6e63 6573 2d66 726f 6d2d 7468 652d  rences-from-the-
+000018c0: 7061 7065 7229 2073 6563 7469 6f6e 2062  paper) section b
+000018d0: 656c 6f77 2e0a 0a23 2320 f09f 8eaf 2043  elow...## .... C
+000018e0: 6f72 6520 4665 6174 7572 6573 0a0a 2d20  ore Features..- 
+000018f0: f09f 92be 202a 2a44 6174 612d 6472 6976  .... **Data-driv
+00001900: 656e 2a2a 2e20 4375 7374 6f6d 697a 6520  en**. Customize 
+00001910: 7468 6520 7369 6d75 6c61 7469 6f6e 2066  the simulation f
+00001920: 6f72 2064 6966 6665 7265 6e74 206e 6172  or different nar
+00001930: 7261 7469 7665 2073 6574 7469 6e67 730a  rative settings.
+00001940: 2d20 f09f a496 202a 2a41 6765 6e74 2d62  - .... **Agent-b
+00001950: 6173 6564 2a2a 2e20 5365 7474 6c65 6d65  ased**. Settleme
+00001960: 6e74 2061 6e64 2063 6861 7261 6374 6572  nt and character
+00001970: 2068 6973 746f 7269 6573 2061 7265 2067   histories are g
+00001980: 656e 6572 6174 6564 2062 6f74 746f 6d2d  enerated bottom-
+00001990: 7570 2066 726f 6d20 6368 6172 6163 7465  up from characte
+000019a0: 7220 6265 6861 7669 6f72 2e0a 2d20 f09f  r behavior..- ..
+000019b0: 93a6 202a 2a45 6e74 6974 792d 436f 6d70  .. **Entity-Comp
+000019c0: 6f6e 656e 7420 5379 7374 656d 2a2a 2e20  onent System**. 
+000019d0: 4167 656e 7473 2061 7265 2063 6f6d 706f  Agents are compo
+000019e0: 7365 6420 6f66 206d 6f64 756c 6172 2063  sed of modular c
+000019f0: 6f6d 706f 6e65 6e74 732e 0a2d 20f0 9f91  omponents..- ...
+00001a00: 9420 2a2a 5374 6174 2026 2053 6b69 6c6c  . **Stat & Skill
+00001a10: 2053 7973 7465 6d73 2a2a 2e20 5472 6163   Systems**. Trac
+00001a20: 6b20 6368 6172 6163 7465 7220 7072 6f66  k character prof
+00001a30: 6963 6965 6e63 6965 7320 616e 6420 5250  iciencies and RP
+00001a40: 472d 6c69 6b65 2073 7461 7473 2e0a 2d20  G-like stats..- 
+00001a50: efb8 8ff0 9f8f b7ef b88f 202a 2a54 7261  .......... **Tra
+00001a60: 6974 2053 7973 7465 6d2a 2a2e 2054 6167  it System**. Tag
+00001a70: 2047 616d 654f 626a 6563 7473 2077 6974   GameObjects wit
+00001a80: 6820 7472 6169 7473 2074 6861 7420 6d6f  h traits that mo
+00001a90: 6469 6679 2074 6865 6972 2073 7461 7473  dify their stats
+00001aa0: 2061 6e64 2072 656c 6174 696f 6e73 6869   and relationshi
+00001ab0: 7073 2e0a 2d20 e29d a4ef b88f 202a 2a52  ps..- ...... **R
+00001ac0: 656c 6174 696f 6e73 6869 7020 5379 7374  elationship Syst
+00001ad0: 656d 2a2a 2e20 4368 6172 6163 7465 7273  em**. Characters
+00001ae0: 2063 756c 7469 7661 7465 2072 656c 6174   cultivate relat
+00001af0: 696f 6e73 6869 7073 2062 6173 6564 206f  ionships based o
+00001b00: 6e20 726f 6d61 6e63 6520 616e 6420 7265  n romance and re
+00001b10: 7075 7461 7469 6f6e 2e0a 2d20 f09f 92a5  putation..- ....
+00001b20: 202a 2a41 6374 696f 6e20 2620 4576 656e   **Action & Even
+00001b30: 7420 5379 7374 656d 2a2a 2e20 4167 656e  t System**. Agen
+00001b40: 7473 2074 616b 6520 6163 7469 6f6e 7320  ts take actions 
+00001b50: 7468 6174 2062 7569 6c64 2075 7020 6869  that build up hi
+00001b60: 7374 6f72 6965 7320 6f66 206c 6966 6520  stories of life 
+00001b70: 6576 656e 7473 2e0a 2d20 e29a 96ef b88f  events..- ......
+00001b80: 202a 2a42 656c 6965 6620 5379 7374 656d   **Belief System
+00001b90: 2a2a 2e20 4368 6172 6163 7465 7227 7320  **. Character's 
+00001ba0: 6265 6c69 6566 7320 696e 666c 7565 6e63  beliefs influenc
+00001bb0: 6520 686f 7720 7468 6579 2066 6565 6c20  e how they feel 
+00001bc0: 6162 6f75 7420 6f74 6865 7273 2e0a 2d20  about others..- 
+00001bd0: f09f 8fac 202a 2a4c 6f63 6174 696f 6e20  .... **Location 
+00001be0: 5072 6566 6572 656e 6365 2053 7973 7465  Preference Syste
+00001bf0: 6d2a 2a2e 204d 6f64 656c 2077 6861 7420  m**. Model what 
+00001c00: 6c6f 6361 7469 6f6e 7320 6120 6368 6172  locations a char
+00001c10: 6163 7465 7220 6d69 6768 7420 6672 6571  acter might freq
+00001c20: 7565 6e74 2067 6976 656e 2074 6865 6972  uent given their
+00001c30: 2074 7261 6974 732e 0a2d 20f0 9f93 8820   traits..- .... 
+00001c40: 2a2a 5265 6164 7920 666f 7220 6461 7461  **Ready for data
+00001c50: 2073 6369 656e 6365 2a2a 2e20 4578 7472   science**. Extr
+00001c60: 6163 7420 616e 6420 616e 616c 797a 6520  act and analyze 
+00001c70: 6461 7461 2077 6974 6820 5b50 616e 6461  data with [Panda
+00001c80: 735d 2868 7474 7073 3a2f 2f70 616e 6461  s](https://panda
+00001c90: 732e 7079 6461 7461 2e6f 7267 2f29 2e0a  s.pydata.org/)..
+00001ca0: 0a23 2320 f09f 9a80 2048 6f77 2074 6f20  .## .... How to 
+00001cb0: 496e 7374 616c 6c0a 0a54 6865 206c 6174  Install..The lat
+00001cc0: 6573 7420 6f66 6669 6369 616c 2072 656c  est official rel
+00001cd0: 6561 7365 206f 6620 4e65 6967 6862 6f72  ease of Neighbor
+00001ce0: 6c79 2069 7320 6176 6169 6c61 626c 6520  ly is available 
+00001cf0: 746f 2069 6e73 7461 6c6c 2066 726f 6d20  to install from 
+00001d00: 5b50 7950 495d 2868 7474 7073 3a2f 2f70  [PyPI](https://p
+00001d10: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+00001d20: 6e65 6967 6862 6f72 6c79 2f29 2e0a 0a60  neighborly/)...`
+00001d30: 6060 6261 7368 0a70 6970 2069 6e73 7461  ``bash.pip insta
+00001d40: 6c6c 206e 6569 6768 626f 726c 790a 6060  ll neighborly.``
+00001d50: 600a 0a23 2323 2054 7279 204e 6569 6768  `..### Try Neigh
+00001d60: 626f 726c 7920 5769 7468 6f75 7420 496e  borly Without In
+00001d70: 7374 616c 6c69 6e67 0a0a 4e65 6967 6862  stalling..Neighb
+00001d80: 6f72 6c79 2069 7320 6176 6169 6c61 626c  orly is availabl
+00001d90: 6520 746f 2075 7365 2077 6974 6869 6e20  e to use within 
+00001da0: 7468 6973 205b 7361 6d70 6c65 2047 6f6f  this [sample Goo
+00001db0: 676c 6520 436f 6c61 6220 6e6f 7465 626f  gle Colab notebo
+00001dc0: 6f6b 5d28 6874 7470 733a 2f2f 636f 6c61  ok](https://cola
+00001dd0: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
+00001de0: 652e 636f 6d2f 6472 6976 652f 3157 785a  e.com/drive/1WxZ
+00001df0: 6e43 5238 6166 656b 6642 6c2d 7649 3657  nCR8afekfBl-vI6W
+00001e00: 6349 6353 364f 6852 4764 6b61 6d3f 7573  cIcS6OhRGdkam?us
+00001e10: 703d 7368 6172 696e 6729 2e20 4974 2063  p=sharing). It c
+00001e20: 6f6e 7461 696e 7320 6120 6261 7369 6320  ontains a basic 
+00001e30: 7761 6c6b 7468 726f 7567 6820 6f66 2068  walkthrough of h
+00001e40: 6f77 2074 6f20 6465 6669 6e65 2063 6f6e  ow to define con
+00001e50: 7465 6e74 2066 6f72 2074 6865 2073 696d  tent for the sim
+00001e60: 756c 6174 696f 6e20 616e 6420 696e 7370  ulation and insp
+00001e70: 6563 7420 7468 6520 6765 6e65 7261 7465  ect the generate
+00001e80: 6420 6461 7461 2e0a 0a23 2323 2049 6e73  d data...### Ins
+00001e90: 7461 6c6c 696e 6720 666f 7220 4c6f 6361  talling for Loca
+00001ea0: 6c20 4465 7665 6c6f 706d 656e 740a 0a54  l Development..T
+00001eb0: 6f20 646f 776e 6c6f 6164 2061 204e 6569  o download a Nei
+00001ec0: 6768 626f 726c 7920 666f 7220 6c6f 6361  ghborly for loca
+00001ed0: 6c20 6465 7665 6c6f 706d 656e 7420 6f72  l development or
+00001ee0: 2070 6c61 7920 6172 6f75 6e64 2077 6974   play around wit
+00001ef0: 6820 616e 7920 6f66 2074 6865 2073 616d  h any of the sam
+00001f00: 706c 6573 2c20 796f 7520 6e65 6564 2074  ples, you need t
+00001f10: 6f20 636c 6f6e 6520 6f72 2064 6f77 6e6c  o clone or downl
+00001f20: 6f61 6420 7468 6973 2072 6570 6f73 6974  oad this reposit
+00001f30: 6f72 7920 616e 6420 696e 7374 616c 6c20  ory and install 
+00001f40: 6974 2075 7369 6e67 2074 6865 205f 6564  it using the _ed
+00001f50: 6974 6162 6c65 5f20 666c 6167 2028 2d65  itable_ flag (-e
+00001f60: 292e 2050 6c65 6173 6520 7365 6520 7468  ). Please see th
+00001f70: 6520 696e 7374 7275 6374 696f 6e73 2062  e instructions b
+00001f80: 656c 6f77 2e20 5468 6973 2063 6f6d 6d61  elow. This comma
+00001f90: 6e64 2077 696c 6c20 696e 7374 616c 6c20  nd will install 
+00001fa0: 6120 4e65 6967 6862 6f72 6c79 2069 6e74  a Neighborly int
+00001fb0: 6f20 7468 6520 7669 7274 7561 6c20 656e  o the virtual en
+00001fc0: 7669 726f 6e6d 656e 7420 616c 6f6e 6720  vironment along 
+00001fd0: 7769 7468 2061 6c6c 2069 7473 2064 6570  with all its dep
+00001fe0: 656e 6465 6e63 6965 7320 616e 6420 6120  endencies and a 
+00001ff0: 6665 7720 6164 6469 7469 6f6e 616c 2064  few additional d
+00002000: 6576 656c 6f70 6d65 6e74 2061 6e64 2074  evelopment and t
+00002010: 6573 7469 6e67 2064 6570 656e 6465 6e63  esting dependenc
+00002020: 6965 7320 7375 6368 2061 7320 5f62 6c61  ies such as _bla
+00002030: 636b 5f2c 205f 6973 6f72 745f 2c20 616e  ck_, _isort_, an
+00002040: 6420 5f70 7974 6573 745f 2e0a 0a60 6060  d _pytest_...```
+00002050: 6261 7368 0a23 2053 7465 7020 313a 2043  bash.# Step 1: C
+00002060: 6c6f 6e65 2052 6570 6f73 6974 6f72 7920  lone Repository 
+00002070: 616e 6420 6368 616e 6765 2069 6e74 6f20  and change into 
+00002080: 7072 6f6a 6563 7420 6469 7265 6374 6f72  project director
+00002090: 790a 6769 7420 636c 6f6e 6520 6874 7470  y.git clone http
+000020a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
+000020b0: 6869 4a62 6579 2f6e 6569 6768 626f 726c  hiJbey/neighborl
+000020c0: 792e 6769 740a 6364 206e 6569 6768 626f  y.git.cd neighbo
+000020d0: 726c 790a 0a23 2053 7465 7020 3220 284d  rly..# Step 2 (M
+000020e0: 6163 4f53 2f4c 696e 7578 293a 2043 7265  acOS/Linux): Cre
+000020f0: 6174 6520 616e 6420 6163 7469 7661 7465  ate and activate
+00002100: 2061 2050 7974 686f 6e20 7669 7274 7561   a Python virtua
+00002110: 6c20 656e 7669 726f 6e6d 656e 740a 7079  l environment.py
+00002120: 7468 6f6e 3320 2d6d 2076 656e 7620 7665  thon3 -m venv ve
+00002130: 6e76 0a73 6f75 7263 6520 2e2f 7665 6e76  nv.source ./venv
+00002140: 2f62 696e 2f61 6374 6976 6174 650a 0a23  /bin/activate..#
+00002150: 2053 7465 7020 3220 2857 696e 646f 7773   Step 2 (Windows
+00002160: 293a 2043 7265 6174 6520 616e 6420 6163  ): Create and ac
+00002170: 7469 7661 7465 2061 2050 7974 686f 6e20  tivate a Python 
+00002180: 7669 7274 7561 6c20 656e 7669 726f 6e6d  virtual environm
+00002190: 656e 740a 7079 7468 6f6e 202d 6d20 7665  ent.python -m ve
+000021a0: 6e76 2076 656e 760a 2e5c 7665 6e76 5c53  nv venv..\venv\S
+000021b0: 6372 6970 7473 5c41 6374 6976 6174 650a  cripts\Activate.
+000021c0: 0a23 2053 7465 7020 333a 2049 6e73 7461  .# Step 3: Insta
+000021d0: 6c6c 206e 6569 6768 626f 726c 7920 616e  ll neighborly an
+000021e0: 6420 6465 7065 6e64 656e 6369 6573 0a70  d dependencies.p
+000021f0: 7974 686f 6e20 2d6d 2070 6970 2069 6e73  ython -m pip ins
+00002200: 7461 6c6c 202d 6520 222e 5b64 6576 656c  tall -e ".[devel
+00002210: 6f70 6d65 6e74 5d22 0a60 6060 0a0a 2323  opment]".```..##
+00002220: 20f0 9f8d aa20 5275 6e6e 696e 6720 7468   .... Running th
+00002230: 6520 5361 6d70 6c65 730a 0a45 7861 6d70  e Samples..Examp
+00002240: 6c65 2073 696d 756c 6174 696f 6e73 2063  le simulations c
+00002250: 616e 2062 6520 666f 756e 6420 696e 2074  an be found in t
+00002260: 6865 2060 7361 6d70 6c65 7360 2064 6972  he `samples` dir
+00002270: 6563 746f 7279 2e20 5468 656e 2074 6865  ectory. Then the
+00002280: 2063 6f6d 6d61 6e64 7320 6265 6c6f 7720   commands below 
+00002290: 7769 6c6c 2067 6574 2079 6f75 2073 7461  will get you sta
+000022a0: 7274 6564 2077 6974 6820 7275 6e6e 696e  rted with runnin
+000022b0: 6720 7468 6520 7361 6d70 6c65 2073 696d  g the sample sim
+000022c0: 756c 6174 696f 6e73 2e0a 0a60 6060 6261  ulations...```ba
+000022d0: 7368 0a23 2053 7465 7020 313a 2049 6e73  sh.# Step 1: Ins
+000022e0: 7461 6c6c 206e 6569 6768 626f 726c 7920  tall neighborly 
+000022f0: 6c6f 6361 6c6c 7920 616e 6420 616c 6c20  locally and all 
+00002300: 7468 6520 6465 7065 6e64 656e 6369 6573  the dependencies
+00002310: 206e 6565 6465 6420 746f 2072 756e 2074   needed to run t
+00002320: 6865 2073 616d 706c 6520 636f 6e74 656e  he sample conten
+00002330: 742e 0a70 7974 686f 6e20 2d6d 2070 6970  t..python -m pip
+00002340: 2069 6e73 7461 6c6c 2022 2e22 0a0a 2320   install "."..# 
+00002350: 5374 6570 2032 3a20 5275 6e20 6120 7361  Step 2: Run a sa
+00002360: 6d70 6c65 2073 6372 6970 740a 7079 7468  mple script.pyth
+00002370: 6f6e 202e 2f73 616d 706c 6573 2f4e 414d  on ./samples/NAM
+00002380: 455f 4f46 5f53 414d 504c 455f 4649 4c45  E_OF_SAMPLE_FILE
+00002390: 2e70 790a 6060 600a 0a23 2320 f09f a7aa  .py.```..## ....
+000023a0: 2052 756e 6e69 6e67 2074 6865 2054 6573   Running the Tes
+000023b0: 7473 0a0a 4e65 6967 6862 6f72 6c79 2075  ts..Neighborly u
+000023c0: 7365 7320 5b50 7954 6573 745d 2868 7474  ses [PyTest](htt
+000023d0: 7073 3a2f 2f64 6f63 732e 7079 7465 7374  ps://docs.pytest
+000023e0: 2e6f 7267 2f29 2066 6f72 2075 6e69 7420  .org/) for unit 
+000023f0: 7465 7374 696e 672e 2041 6c6c 2074 6573  testing. All tes
+00002400: 7473 2061 7265 206c 6f63 6174 6564 2069  ts are located i
+00002410: 6e20 7468 6520 6074 6573 7473 2f60 2064  n the `tests/` d
+00002420: 6972 6563 746f 7279 2e0a 0a60 6060 6261  irectory...```ba
+00002430: 7368 0a23 2053 7465 7020 313a 2049 6e73  sh.# Step 1: Ins
+00002440: 7461 6c6c 2061 6464 6974 696f 6e61 6c20  tall additional 
+00002450: 6465 7065 6e64 656e 6369 6573 2066 6f72  dependencies for
+00002460: 2074 6573 7469 6e67 2061 6e64 2064 6576   testing and dev
+00002470: 656c 6f70 6d65 6e74 0a70 7974 686f 6e20  elopment.python 
+00002480: 2d6d 2070 6970 2069 6e73 7461 6c6c 202d  -m pip install -
+00002490: 6520 222e 5b64 6576 656c 6f70 6d65 6e74  e ".[development
+000024a0: 5d22 0a0a 2320 5374 6570 2032 3a20 5275  ]"..# Step 2: Ru
+000024b0: 6e20 5079 7465 7374 0a70 7974 6573 740a  n Pytest.pytest.
+000024c0: 0a23 2053 7465 7020 333a 2028 4f70 7469  .# Step 3: (Opti
+000024d0: 6f6e 616c 2920 4765 6e65 7261 7465 2061  onal) Generate a
+000024e0: 2074 6573 7420 636f 7665 7261 6765 2072   test coverage r
+000024f0: 6570 6f72 740a 7079 7465 7374 202d 2d63  eport.pytest --c
+00002500: 6f76 3d6e 6569 6768 626f 726c 7920 7465  ov=neighborly te
+00002510: 7374 732f 0a60 6060 0a0a 2323 20f0 9f93  sts/.```..## ...
+00002520: 9a20 446f 6375 6d65 6e74 6174 696f 6e0a  . Documentation.
+00002530: 0a4e 6569 6768 626f 726c 7927 7320 646f  .Neighborly's do
+00002540: 6375 6d65 6e74 6174 696f 6e20 6361 6e20  cumentation can 
+00002550: 6265 2066 6f75 6e64 2061 7420 5b52 6561  be found at [Rea
+00002560: 6420 7468 6520 446f 6373 5d28 6874 7470  d the Docs](http
+00002570: 733a 2f2f 6e65 6967 6862 6f72 6c79 2e72  s://neighborly.r
+00002580: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00002590: 2f6c 6174 6573 742f 696e 6465 782e 6874  /latest/index.ht
+000025a0: 6d6c 292e 0a0a 2323 20f0 9fa4 9d20 436f  ml)...## .... Co
+000025b0: 6e74 7269 6275 7469 6e67 0a0a 436f 6e74  ntributing..Cont
+000025c0: 7269 6275 7469 6f6e 7320 6172 6520 7765  ributions are we
+000025d0: 6c63 6f6d 652e 2050 6c65 6173 6520 7265  lcome. Please re
+000025e0: 6665 7220 746f 205b 434f 4e54 5249 4255  fer to [CONTRIBU
+000025f0: 5449 4e47 2e6d 645d 282e 2f43 4f4e 5452  TING.md](./CONTR
+00002600: 4942 5554 494e 472e 6d64 2920 666f 7220  IBUTING.md) for 
+00002610: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+00002620: 2061 626f 7574 2068 6f77 2074 6f20 6765   about how to ge
+00002630: 7420 696e 766f 6c76 6564 2e0a 0a23 2320  t involved...## 
+00002640: f09f 9384 204c 6963 656e 7365 0a0a 5468  .... License..Th
+00002650: 6973 2070 726f 6a65 6374 2069 7320 6c69  is project is li
+00002660: 6365 6e73 6564 2075 6e64 6572 2074 6865  censed under the
+00002670: 205b 4d49 5420 4c69 6365 6e73 655d 282e   [MIT License](.
+00002680: 2f4c 4943 454e 5345 292e 0a0a 2323 20e2  /LICENSE)...## .
+00002690: 84b9 efb8 8f20 4469 6666 6572 656e 6365  ..... Difference
+000026a0: 7320 6672 6f6d 2074 6865 2050 6170 6572  s from the Paper
+000026b0: 0a0a 2d20 2a2a 4469 7265 6374 6564 2072  ..- **Directed r
+000026c0: 656c 6174 696f 6e73 6869 7073 206f 6e6c  elationships onl
+000026d0: 792a 2a20 2d20 204e 6569 6768 626f 726c  y** -  Neighborl
+000026e0: 7920 6f6e 6c79 2073 7570 706f 7274 7320  y only supports 
+000026f0: 6469 7265 6374 6564 2072 656c 6174 696f  directed relatio
+00002700: 6e73 6869 7073 2074 6861 7420 7472 6163  nships that trac
+00002710: 6b20 686f 7720 6f6e 6520 6368 6172 6163  k how one charac
+00002720: 7465 7220 6665 656c 7320 6162 6f75 7420  ter feels about 
+00002730: 616e 6f74 6865 722e 2053 7570 706f 7274  another. Support
+00002740: 2066 6f72 2072 6563 6970 726f 6361 6c20   for reciprocal 
+00002750: 7265 6c61 7469 6f6e 7368 6970 7320 7761  relationships wa
+00002760: 7320 7265 6d6f 7665 6420 6265 6361 7573  s removed becaus
+00002770: 6520 6974 2063 6f6d 706c 6963 6174 6564  e it complicated
+00002780: 2074 6865 2073 696d 756c 6174 696f 6e20   the simulation 
+00002790: 6279 2066 6f72 6369 6e67 2075 7365 7273  by forcing users
+000027a0: 2074 6f20 6368 6563 6b20 6d75 6c74 6970   to check multip
+000027b0: 6c65 206c 6f63 6174 696f 6e73 2066 6f72  le locations for
+000027c0: 2072 656c 6174 696f 6e73 6869 7020 6461   relationship da
+000027d0: 7461 2e0a 2d20 2a2a 4e6f 2061 6374 6976  ta..- **No activ
+000027e0: 6974 792f 7365 7276 6963 6520 7379 7374  ity/service syst
+000027f0: 656d 2a2a 202d 2054 6865 2061 6374 6976  em** - The activ
+00002800: 6974 7920 7379 7374 656d 2077 6173 2069  ity system was i
+00002810: 6e74 726f 6475 6365 6420 746f 2068 656c  ntroduced to hel
+00002820: 7020 6368 6172 6163 7465 7273 2064 6563  p characters dec
+00002830: 6964 6520 7768 6572 6520 746f 2066 7265  ide where to fre
+00002840: 7175 656e 7420 6f75 7473 6964 6520 6f66  quent outside of
+00002850: 2077 6f72 6b2f 686f 6d65 2e20 5468 6973   work/home. This
+00002860: 2073 7973 7465 6d20 7761 7320 7265 706c   system was repl
+00002870: 6163 6564 2077 6974 6820 5f6c 6f63 6174  aced with _locat
+00002880: 696f 6e20 7072 6566 6572 656e 6365 735f  ion preferences_
+00002890: 2c20 7768 6963 6820 6172 6520 6d6f 7265  , which are more
+000028a0: 2066 6c65 7869 626c 652e 2054 6865 2061   flexible. The a
+000028b0: 6374 6976 6974 7920 7379 7374 656d 2063  ctivity system c
+000028c0: 616e 2062 6520 656d 756c 6174 6564 2062  an be emulated b
+000028d0: 7920 6173 736f 6369 6174 696e 6720 6365  y associating ce
+000028e0: 7274 6169 6e20 7472 6169 7473 2077 6974  rtain traits wit
+000028f0: 6820 6c6f 6361 7469 6f6e 732e 0a2d 202a  h locations..- *
+00002900: 2a4e 6f20 372d 6461 7920 7765 656b 6c79  *No 7-day weekly
+00002910: 2072 6f75 7469 6e65 732a 2a20 2d20 526f   routines** - Ro
+00002920: 7574 696e 6573 2077 6572 6520 7465 6469  utines were tedi
+00002930: 6f75 7320 746f 2063 7265 6174 6520 616e  ous to create an
+00002940: 6420 6265 6361 6d65 2069 7272 656c 6576  d became irrelev
+00002950: 616e 7420 7768 656e 204e 6569 6768 626f  ant when Neighbo
+00002960: 726c 7927 7320 7469 6d65 2073 7465 7020  rly's time step 
+00002970: 7363 616c 6520 6368 616e 6765 6420 6672  scale changed fr
+00002980: 6f6d 2069 6e63 7265 6d65 6e74 696e 6720  om incrementing 
+00002990: 7468 6520 6461 7465 2062 7920 6120 6665  the date by a fe
+000029a0: 7720 686f 7572 7320 746f 2069 6e63 7265  w hours to incre
+000029b0: 6d65 6e74 696e 6720 6279 2061 2073 696e  menting by a sin
+000029c0: 676c 6520 6d6f 6e74 682e 0a2d 202a 2a4e  gle month..- **N
+000029d0: 6f20 6469 7265 6374 2073 7570 706f 7274  o direct support
+000029e0: 2066 6f72 2064 6966 6665 7269 6e67 2041   for differing A
+000029f0: 4920 7374 7261 7465 6769 6573 2a2a 202d  I strategies** -
+00002a00: 2057 6520 696e 7465 6e64 6564 2074 6f20   We intended to 
+00002a10: 7375 7070 6f72 7420 7661 7269 6f75 7320  support various 
+00002a20: 6368 6172 6163 7465 7220 6465 6369 7369  character decisi
+00002a30: 6f6e 2d6d 616b 696e 6720 616c 676f 7269  on-making algori
+00002a40: 7468 6d73 2062 7574 206d 6164 6520 6265  thms but made be
+00002a50: 6861 7669 6f72 2061 7574 686f 7269 6e67  havior authoring
+00002a60: 2074 6f6f 2074 6564 696f 7573 2061 6e64   too tedious and
+00002a70: 2074 6f6f 6b20 656d 7068 6173 6973 2061   took emphasis a
+00002a80: 7761 7920 6672 6f6d 2074 6865 2063 6f6e  way from the con
+00002a90: 7465 6e74 2061 7574 686f 7269 6e67 2061  tent authoring a
+00002aa0: 6e64 2064 6174 6120 6765 6e65 7261 7469  nd data generati
+00002ab0: 6f6e 2061 7370 6563 7473 206f 6620 4e65  on aspects of Ne
+00002ac0: 6967 6862 6f72 6c79 2e0a 2d20 2a2a 4576  ighborly..- **Ev
+00002ad0: 656e 7420 7379 7374 656d 2072 6570 6c61  ent system repla
+00002ae0: 6365 6420 7769 7468 2061 6374 696f 6e20  ced with action 
+00002af0: 6f62 6a65 6374 7320 616e 6420 7574 696c  objects and util
+00002b00: 6974 7920 7363 6f72 6573 2a2a 202d 2053  ity scores** - S
+00002b10: 696e 6365 204e 6569 6768 626f 726c 7920  ince Neighborly 
+00002b20: 646f 6573 206e 6f74 206e 6565 6420 746f  does not need to
+00002b30: 2073 7570 706f 7274 2075 7365 722d 7375   support user-su
+00002b40: 7070 6c69 6564 2063 6861 7261 6374 6572  pplied character
+00002b50: 2064 6563 6973 696f 6e2d 6d61 6b69 6e67   decision-making
+00002b60: 206c 6f67 6963 2c20 6974 206d 6164 6520   logic, it made 
+00002b70: 6265 6861 7669 6f72 206d 6f64 656c 696e  behavior modelin
+00002b80: 6720 6d75 6368 2073 696d 706c 6572 2e20  g much simpler. 
+00002b90: 5468 6520 6f6c 6420 6c69 6665 2065 7665  The old life eve
+00002ba0: 6e74 2073 7973 7465 6d20 7265 7175 6972  nt system requir
+00002bb0: 6564 2075 7365 7273 2074 6f20 7370 6563  ed users to spec
+00002bc0: 6966 7920 6576 656e 7420 6566 6665 6374  ify event effect
+00002bd0: 7320 666f 7220 6561 6368 2064 6966 6665  s for each diffe
+00002be0: 7265 6e74 2074 7970 6520 6f66 2061 6765  rent type of age
+00002bf0: 6e74 2c20 616e 6420 7468 6973 206e 6174  nt, and this nat
+00002c00: 7572 616c 6c79 2063 6f6d 706c 6963 6174  urally complicat
+00002c10: 6564 2074 6869 6e67 732e 2043 7572 7265  ed things. Curre
+00002c20: 6e74 6c79 2c20 6167 656e 7420 6265 6861  ntly, agent beha
+00002c30: 7669 6f72 2069 7320 696d 706c 656d 656e  vior is implemen
+00002c40: 7465 6420 7573 696e 6720 6120 636f 6d62  ted using a comb
+00002c50: 696e 6174 696f 6e20 6f66 2053 7973 7465  ination of Syste
+00002c60: 6d73 2c20 6163 7469 6f6e 732c 2061 6e64  ms, actions, and
+00002c70: 206c 6966 6520 6576 656e 7473 2e0a 2d20   life events..- 
+00002c80: 2a2a 4e6f 2062 6568 6176 696f 7220 7472  **No behavior tr
+00002c90: 6565 732a 2a20 2d20 4265 6861 7669 6f72  ees** - Behavior
+00002ca0: 2074 7265 6573 2061 6464 6564 2063 6f6d   trees added com
+00002cb0: 706c 6578 6974 7920 746f 2074 6865 2073  plexity to the s
+00002cc0: 7973 7465 6d2e 2049 7420 7761 7320 7265  ystem. It was re
+00002cd0: 6d6f 7665 6420 746f 2073 696d 706c 6966  moved to simplif
+00002ce0: 7920 7468 696e 6773 2e0a 2d20 2a2a 4e6f  y things..- **No
+00002cf0: 2063 6861 7261 6374 6572 2076 616c 7565   character value
+00002d00: 732a 2a20 2d20 4f76 6572 2074 696d 652c  s** - Over time,
+00002d10: 2074 6865 2063 6861 7261 6374 6572 2076   the character v
+00002d20: 616c 7565 2073 7973 7465 6d20 616e 6420  alue system and 
+00002d30: 7065 7273 6f6e 616c 6974 7920 6d6f 6465  personality mode
+00002d40: 6c73 2077 6572 6520 636f 6d62 696e 6564  ls were combined
+00002d50: 2069 6e74 6f20 6120 7369 6e67 6c65 2073   into a single s
+00002d60: 7461 7420 7379 7374 656d 2e20 5265 6d6f  tat system. Remo
+00002d70: 7669 6e67 2074 6865 6d20 7369 6d70 6c69  ving them simpli
+00002d80: 6669 6564 206d 7563 6820 6f66 2074 6865  fied much of the
+00002d90: 2061 6765 6e74 206d 6f64 656c 696e 6720   agent modeling 
+00002da0: 616e 6420 616c 6c6f 7765 6420 666f 7220  and allowed for 
+00002db0: 7468 6520 6d6f 7374 2066 6c65 7869 6269  the most flexibi
+00002dc0: 6c69 7479 2e0a 2d20 2a2a 4e6f 2063 6861  lity..- **No cha
+00002dd0: 7261 6374 6572 206d 6f76 656d 656e 742a  racter movement*
+00002de0: 2a20 2d20 4368 6172 6163 7465 7273 2064  * - Characters d
+00002df0: 6f20 6e6f 7420 6d6f 7665 2062 6574 7765  o not move betwe
+00002e00: 656e 206c 6f63 6174 696f 6e73 2e20 5468  en locations. Th
+00002e10: 6973 2061 6464 6564 2061 6464 6974 696f  is added additio
+00002e20: 6e61 6c20 7072 6f63 6573 7369 6e67 206f  nal processing o
+00002e30: 7665 7268 6561 6420 616e 6420 6265 6361  verhead and beca
+00002e40: 6d65 2075 6e6e 6563 6573 7361 7279 2077  me unnecessary w
+00002e50: 6865 6e20 6d6f 7669 6e67 2074 6f20 6120  hen moving to a 
+00002e60: 6f6e 652d 6d6f 6e74 6820 7469 6d65 2073  one-month time s
+00002e70: 7465 7073 2e0a 0a23 2320 c2a9 efb8 8f20  teps...## ..... 
+00002e80: 444d 4341 2053 7461 7465 6d65 6e74 0a0a  DMCA Statement..
+00002e90: 5570 6f6e 2072 6563 6569 7074 206f 6620  Upon receipt of 
+00002ea0: 6120 6e6f 7469 6365 2061 6c6c 6567 696e  a notice allegin
+00002eb0: 6720 636f 7079 7269 6768 7420 696e 6672  g copyright infr
+00002ec0: 696e 6765 6d65 6e74 2c20 4920 7769 6c6c  ingement, I will
+00002ed0: 2074 616b 6520 7768 6174 6576 6572 2061   take whatever a
+00002ee0: 6374 696f 6e20 6974 2064 6565 6d73 2061  ction it deems a
+00002ef0: 7070 726f 7072 6961 7465 2077 6974 6869  ppropriate withi
+00002f00: 6e20 6974 7320 736f 6c65 2064 6973 6372  n its sole discr
+00002f10: 6574 696f 6e2c 2069 6e63 6c75 6469 6e67  etion, including
+00002f20: 2072 656d 6f76 616c 206f 6620 7468 6520   removal of the 
+00002f30: 616c 6c65 6765 646c 7920 696e 6672 696e  allegedly infrin
+00002f40: 6769 6e67 206d 6174 6572 6961 6c73 2e0a  ging materials..
+00002f50: 0a54 6865 2072 6570 6f20 696d 6167 6520  .The repo image 
+00002f60: 6973 2073 6f6d 6574 6869 6e67 2066 756e  is something fun
+00002f70: 2074 6861 7420 4920 6d61 6465 2e20 4920   that I made. I 
+00002f80: 6c6f 7665 205f 5468 6520 5369 6d70 736f  love _The Simpso
+00002f90: 6e73 5f2c 2061 6e64 2049 2063 6f75 6c64  ns_, and I could
+00002fa0: 6e27 7420 7468 696e 6b20 6f66 2061 6e79  n't think of any
+00002fb0: 6f6e 6520 6d6f 7265 206e 6569 6768 626f  one more neighbo
+00002fc0: 726c 7920 7468 616e 204e 6564 2046 6c61  rly than Ned Fla
+00002fd0: 6e64 6572 732e 2049 6620 7468 6520 636f  nders. If the co
+00002fe0: 7079 7269 6768 7420 6f77 6e65 7220 666f  pyright owner fo
+00002ff0: 7220 5f54 6865 2053 696d 7073 6f6e 735f  r _The Simpsons_
+00003000: 2077 6f75 6c64 206c 696b 6520 6d65 2074   would like me t
+00003010: 6f20 7461 6b65 2069 7420 646f 776e 2c20  o take it down, 
+00003020: 706c 6561 7365 2063 6f6e 7461 6374 206d  please contact m
+00003030: 652e 2054 6865 2073 616d 6520 7461 6b65  e. The same take
+00003040: 646f 776e 2070 6f6c 6963 7920 6170 706c  down policy appl
+00003050: 6965 7320 746f 2063 6f64 6520 7361 6d70  ies to code samp
+00003060: 6c65 7320 696e 7370 6972 6564 2062 7920  les inspired by 
+00003070: 5456 2073 686f 7773 2c20 6d6f 7669 6573  TV shows, movies
+00003080: 2c20 616e 6420 6761 6d65 732e 0a         , and games..
```

### Comparing `neighborly-2.5.0/README.md` & `neighborly-3.0.0.dev1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -8,494 +8,543 @@
 00000070: 3130 3736 3532 352f 3136 3538 3336 3137  1076525/16583617
 00000080: 312d 3966 6664 6561 3665 2d31 3633 332d  1-9ffdea6e-1633-
 00000090: 3434 3063 2d62 6530 362d 6234 3665 3165  440c-be06-b46e1e
 000000a0: 3365 3465 3034 2e70 6e67 220a 2020 3e0a  3e4e04.png".  >.
 000000b0: 2020 3c62 723e 0a20 204e 6569 6768 626f    <br>.  Neighbo
 000000c0: 726c 790a 3c2f 6831 3e0a 0a3c 7020 616c  rly.</h1>..<p al
 000000d0: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
-000000e0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-000000f0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000100: 2f70 7970 692f 762f 6e65 6967 6862 6f72  /pypi/v/neighbor
-00000110: 6c79 223e 0a20 203c 696d 6720 7372 633d  ly">.  <img src=
-00000120: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-00000130: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
-00000140: 6572 7369 6f6e 732f 6e65 6967 6862 6f72  ersions/neighbor
-00000150: 6c79 223e 0a20 203c 696d 6720 7372 633d  ly">.  <img src=
-00000160: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-00000170: 656c 6473 2e69 6f2f 7079 7069 2f6c 2f6e  elds.io/pypi/l/n
-00000180: 6569 6768 626f 726c 7922 3e0a 2020 3c69  eighborly">.  <i
-00000190: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-000001a0: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-000001b0: 7970 692f 646d 2f6e 6569 6768 626f 726c  ypi/dm/neighborl
-000001c0: 7922 3e0a 2020 3c69 6d67 2073 7263 3d22  y">.  <img src="
+000000e0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000000f0: 2f6e 6569 6768 626f 726c 792e 7265 6164  /neighborly.read
+00000100: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00000110: 7465 7374 2f69 6e64 6578 2e68 746d 6c22  test/index.html"
+00000120: 3e44 6f63 756d 656e 7461 7469 6f6e 3c2f  >Documentation</
+00000130: 613e 207c 0a20 203c 6120 6872 6566 3d22  a> |.  <a href="
+00000140: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000150: 2f70 726f 6a65 6374 2f6e 6569 6768 626f  /project/neighbo
+00000160: 726c 7922 3e50 7950 493c 2f61 3e20 7c20  rly">PyPI</a> | 
+00000170: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000180: 2f67 6974 6875 622e 636f 6d2f 5368 694a  /github.com/ShiJ
+00000190: 6265 792f 6e65 6967 6862 6f72 6c79 223e  bey/neighborly">
+000001a0: 4769 7448 7562 3c2f 613e 0a3c 2f70 3e0a  GitHub</a>.</p>.
+000001b0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+000001c0: 7222 3e0a 2020 3c69 6d67 2073 7263 3d22  r">.  <img src="
 000001d0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000001e0: 6c64 732e 696f 2f62 6164 6765 2f63 6f64  lds.io/badge/cod
-000001f0: 6525 3230 7374 796c 652d 626c 6163 6b2d  e%20style-black-
-00000200: 626c 6163 6b22 3e0a 2020 3c69 6d67 2073  black">.  <img s
-00000210: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000220: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000230: 2f25 3230 696d 706f 7274 732d 6973 6f72  /%20imports-isor
-00000240: 742d 2532 3331 3637 3462 313f 7374 796c  t-%231674b1?styl
-00000250: 653d 666c 6174 266c 6162 656c 436f 6c6f  e=flat&labelColo
-00000260: 723d 6566 3833 3336 223e 0a3c 2f70 3e0a  r=ef8336">.</p>.
-00000270: 0a4e 6569 6768 626f 726c 7920 6973 2061  .Neighborly is a
-00000280: 6e20 6578 7465 6e73 6962 6c65 2061 6765  n extensible age
-00000290: 6e74 2d62 6173 6564 2073 6574 746c 656d  nt-based settlem
-000002a0: 656e 7420 7369 6d75 6c61 7469 6f6e 2e20  ent simulation. 
-000002b0: 4974 2077 6173 2062 7569 6c74 2074 6f20  It was built to 
-000002c0: 6265 2061 2074 6f6f 6c20 666f 7220 656d  be a tool for em
-000002d0: 6572 6765 6e74 206e 6172 7261 7469 7665  ergent narrative
-000002e0: 2073 746f 7279 7465 6c6c 696e 6720 7265   storytelling re
-000002f0: 7365 6172 6368 2e20 4e65 6967 6862 6f72  search. Neighbor
-00000300: 6c79 2067 656e 6572 6174 6573 2061 2076  ly generates a v
-00000310: 6972 7475 616c 2073 6574 746c 656d 656e  irtual settlemen
-00000320: 7420 616e 6420 7369 6d75 6c61 7465 7320  t and simulates 
-00000330: 7468 6520 696e 6469 7669 6475 616c 206c  the individual l
-00000340: 6976 6573 206f 6620 6974 7320 7265 7369  ives of its resi
-00000350: 6465 6e74 7320 6f76 6572 206d 756c 7469  dents over multi
-00000360: 706c 6520 6765 6e65 7261 7469 6f6e 732e  ple generations.
-00000370: 2049 7420 6d6f 6465 6c73 2074 6865 2063   It models the c
-00000380: 6861 7261 6374 6572 7327 2074 7261 6974  haracters' trait
-00000390: 732c 2073 7461 7475 7365 732c 2072 656c  s, statuses, rel
-000003a0: 6174 696f 6e73 6869 7073 2c20 6f63 6375  ationships, occu
-000003b0: 7061 7469 6f6e 732c 206c 6966 6520 6576  pations, life ev
-000003c0: 656e 7473 2c20 616e 6420 6d6f 7265 2e20  ents, and more. 
-000003d0: 4e65 6967 6862 6f72 6c79 2074 7261 636b  Neighborly track
-000003e0: 7320 616c 6c20 7468 6520 6c69 6665 2065  s all the life e
-000003f0: 7665 6e74 7320 2873 7461 7274 696e 6720  vents (starting 
-00000400: 6120 6e65 7720 6a6f 622c 2066 616c 6c69  a new job, falli
-00000410: 6e67 2069 6e20 6c6f 7665 2c20 7475 726e  ng in love, turn
-00000420: 696e 6720 696e 746f 2061 2064 656d 6f6e  ing into a demon
-00000430: 2c20 6574 632e 292c 2061 6e64 2074 6865  , etc.), and the
-00000440: 7365 2062 6563 6f6d 6520 7468 6520 6275  se become the bu
-00000450: 696c 6469 6e67 2062 6c6f 636b 7320 666f  ilding blocks fo
-00000460: 7220 6372 6561 7469 6e67 2065 6d65 7267  r creating emerg
-00000470: 656e 7420 7374 6f72 6965 7320 6162 6f75  ent stories abou
-00000480: 7420 6368 6172 6163 7465 7273 2061 6e64  t characters and
-00000490: 2074 6865 6972 206c 6567 6163 6965 732e   their legacies.
-000004a0: 2054 6865 2065 6e74 6972 6520 6869 7374   The entire hist
-000004b0: 6f72 7920 6f66 2074 6865 2073 6574 746c  ory of the settl
-000004c0: 656d 656e 7420 616e 6420 6974 7320 6765  ement and its ge
-000004d0: 6e65 7261 7469 6f6e 7320 6f66 2063 6861  nerations of cha
-000004e0: 7261 6374 6572 7320 6973 2074 6865 6e20  racters is then 
-000004f0: 6d61 6465 2061 7661 696c 6162 6c65 2066  made available f
-00000500: 6f72 2064 6174 6120 616e 616c 7973 6973  or data analysis
-00000510: 206f 7220 6173 2063 6f6e 7465 6e74 2066   or as content f
-00000520: 6f72 206f 7468 6572 2061 7070 6c69 6361  or other applica
-00000530: 7469 6f6e 7320 7375 6368 2061 7320 6761  tions such as ga
-00000540: 6d65 732e 0a0a 4e65 6967 6862 6f72 6c79  mes...Neighborly
-00000550: 2773 2077 6173 2069 6e73 7069 7265 6420  's was inspired 
-00000560: 5b5f 5461 6c6b 206f 6620 7468 6520 546f  [_Talk of the To
-00000570: 776e 5f5d 2868 7474 7073 3a2f 2f67 6974  wn_](https://git
-00000580: 6875 622e 636f 6d2f 6a61 6d65 732d 6f77  hub.com/james-ow
-00000590: 656e 2d72 7961 6e2f 7461 6c6b 746f 776e  en-ryan/talktown
-000005a0: 292c 2061 6e6f 7468 6572 2073 6574 746c  ), another settl
-000005b0: 656d 656e 7420 7369 6d75 6c61 7469 6f6e  ement simulation
-000005c0: 2066 6f72 2065 6d65 7267 656e 7420 6e61   for emergent na
-000005d0: 7272 6174 6976 6520 7374 6f72 7974 656c  rrative storytel
-000005e0: 6c69 6e67 2072 6573 6561 7263 682e 2049  ling research. I
-000005f0: 7420 616c 736f 2064 7261 7773 2069 6e73  t also draws ins
-00000600: 7069 7261 7469 6f6e 2066 726f 6d20 636f  piration from co
-00000610: 6d6d 6572 6369 616c 2077 6f72 6c64 2d73  mmercial world-s
-00000620: 696d 756c 6174 696f 6e20 6761 6d65 7320  imulation games 
-00000630: 6c69 6b65 205f 4361 7665 7320 6f66 2051  like _Caves of Q
-00000640: 7564 5f2c 205f 4477 6172 6620 466f 7274  ud_, _Dwarf Fort
-00000650: 7265 7373 5f2c 205f 4372 7573 6164 6572  ress_, _Crusader
-00000660: 204b 696e 6773 5f2c 205f 5269 6d57 6f72   Kings_, _RimWor
-00000670: 6c64 5f2c 2061 6e64 205f 576f 726c 6442  ld_, and _WorldB
-00000680: 6f78 5f2e 2049 7420 6169 6d73 2074 6f20  ox_. It aims to 
-00000690: 6265 2061 6e20 6561 7369 6c79 2063 7573  be an easily cus
-000006a0: 746f 6d69 7a61 626c 6520 7369 6d75 6c61  tomizable simula
-000006b0: 7469 6f6e 2074 6861 7420 6361 6e20 6164  tion that can ad
-000006c0: 6170 7420 746f 2076 6172 696f 7573 206e  apt to various n
-000006d0: 6172 7261 7469 7665 2073 6574 7469 6e67  arrative setting
-000006e0: 7320 616e 6420 7375 7070 6f72 7420 7265  s and support re
-000006f0: 7365 6172 6368 206f 7220 656e 7465 7274  search or entert
-00000700: 6169 6e6d 656e 7420 7072 6f6a 6563 7473  ainment projects
-00000710: 2e0a 0a49 6620 796f 7520 7573 6520 4e65  ...If you use Ne
-00000720: 6967 6862 6f72 6c79 2069 6e20 6120 7072  ighborly in a pr
-00000730: 6f6a 6563 742c 2070 6c65 6173 6520 5b63  oject, please [c
-00000740: 6974 6520 7468 6973 2072 6570 6f73 6974  ite this reposit
-00000750: 6f72 795d 282e 2f43 4954 4154 494f 4e2e  ory](./CITATION.
-00000760: 6269 6229 2e20 596f 7520 6361 6e20 7265  bib). You can re
-00000770: 6164 2061 2063 6f70 7920 6f66 0a4e 6569  ad a copy of.Nei
-00000780: 6768 626f 726c 7927 7320 6173 736f 6369  ghborly's associ
-00000790: 6174 6564 205b 7061 7065 725d 2868 7474  ated [paper](htt
-000007a0: 7073 3a2f 2f73 6869 6a62 6579 2e67 6974  ps://shijbey.git
-000007b0: 6875 622e 696f 2f70 7562 6c69 6361 7469  hub.io/publicati
-000007c0: 6f6e 732f 4e65 6967 6862 6f72 6c79 2e70  ons/Neighborly.p
-000007d0: 6466 2920 7468 6174 2077 6173 2070 7562  df) that was pub
-000007e0: 6c69 7368 6564 2069 6e20 7468 650a 7072  lished in the.pr
-000007f0: 6f63 6565 6469 6e67 7320 6f66 2074 6865  oceedings of the
-00000800: 2032 3032 3220 4945 4545 2043 6f6e 6665   2022 IEEE Confe
-00000810: 7265 6e63 6520 4f6e 2047 616d 6573 2e20  rence On Games. 
-00000820: e29a a0ef b88f 202a 2a57 6172 6e69 6e67  ...... **Warning
-00000830: 2a2a 3a20 506c 6561 7365 206e 6f74 6520  **: Please note 
-00000840: 7468 6174 204e 6569 6768 626f 726c 7927  that Neighborly'
-00000850: 7320 6375 7272 656e 7420 7374 7275 6374  s current struct
-00000860: 7572 650a 6469 6666 6572 7320 6772 6561  ure.differs grea
-00000870: 746c 7920 6672 6f6d 2074 6865 2076 6572  tly from the ver
-00000880: 7369 6f6e 2074 6865 2070 6170 6572 2064  sion the paper d
-00000890: 6573 6372 6962 6573 2e0a 0a23 2043 6f72  escribes...# Cor
-000008a0: 6520 4665 6174 7572 6573 0a0a 2d20 f09f  e Features..- ..
-000008b0: 8f99 efb8 8f20 5072 6f63 6564 7572 616c  ..... Procedural
-000008c0: 6c79 2067 656e 6572 6174 6573 2061 2073  ly generates a s
-000008d0: 6574 746c 656d 656e 7420 616e 6420 7468  ettlement and th
-000008e0: 6520 6869 7374 6f72 7920 6f66 2069 7473  e history of its
-000008f0: 2072 6573 6964 656e 7473 2e0a 2d20 f09f   residents..- ..
-00000900: 9a80 2055 7469 6c69 7a65 2061 206c 6f77  .. Utilize a low
-00000910: 2d66 6964 656c 6974 7920 736f 6369 616c  -fidelity social
-00000920: 2073 696d 756c 6174 696f 6e20 746f 2073   simulation to s
-00000930: 696d 756c 6174 6520 6875 6e64 7265 6473  imulate hundreds
-00000940: 206f 6620 7965 6172 7320 6f66 2077 6f72   of years of wor
-00000950: 6c64 2068 6973 746f 7279 2077 6974 6869  ld history withi
-00000960: 6e20 6d69 6e75 7465 732e 0a2d 20e2 9a99  n minutes..- ...
-00000970: efb8 8f20 4275 696c 7420 7573 696e 6720  ... Built using 
-00000980: 616e 2065 6e74 6974 792d 636f 6d70 6f6e  an entity-compon
-00000990: 656e 7420 7379 7374 656d 2028 4543 5329  ent system (ECS)
-000009a0: 2061 7263 6869 7465 6374 7572 650a 2d20   architecture.- 
-000009b0: f09f 93a6 2050 6c75 6769 6e20 7379 7374  .... Plugin syst
-000009c0: 656d 2074 6f20 6c6f 6164 2061 6e64 2073  em to load and s
-000009d0: 6861 7265 206e 6577 2063 6f6e 7465 6e74  hare new content
-000009e0: 2e0a 2d20 f09f 9194 2043 6861 7261 6374  ..- .... Charact
-000009f0: 6572 7320 6361 6e20 7374 6172 7420 6275  ers can start bu
-00000a00: 7369 6e65 7373 6573 2061 6e64 2068 6f6c  sinesses and hol
-00000a10: 6420 6a6f 6273 2e0a 2d20 efb8 8ff0 9fa7  d jobs..- ......
-00000a20: ac20 4368 6172 6163 7465 7273 2068 6176  . Characters hav
-00000a30: 6520 7472 6169 7473 2074 6861 7420 6d6f  e traits that mo
-00000a40: 6469 6679 2074 6865 6972 2073 7461 7473  dify their stats
-00000a50: 2061 6e64 2072 656c 6174 696f 6e73 6869   and relationshi
-00000a60: 7073 2e0a 2d20 e29d a4ef b88f 2043 6861  ps..- ...... Cha
-00000a70: 7261 6374 6572 7320 666f 726d 2061 6e64  racters form and
-00000a80: 2063 756c 7469 7661 7465 2072 656c 6174   cultivate relat
-00000a90: 696f 6e73 6869 7073 2062 6173 6564 206f  ionships based o
-00000aa0: 6e20 726f 6d61 6e63 6520 616e 6420 7265  n romance and re
-00000ab0: 7075 7461 7469 6f6e 2e0a 2d20 f09f 92a5  putation..- ....
-00000ac0: 2053 696d 756c 6174 6520 7261 6e64 6f6d   Simulate random
-00000ad0: 206c 6966 6520 6576 656e 7473 2074 6861   life events tha
-00000ae0: 7420 7370 6963 6520 7570 2063 6861 7261  t spice up chara
-00000af0: 6374 6572 7327 206c 6976 6573 2e0a 2d20  cters' lives..- 
-00000b00: e29a 96ef b88f 2044 6566 696e 6520 536f  ...... Define So
-00000b10: 6369 616c 2052 756c 6573 2066 6f72 2068  cial Rules for h
-00000b20: 6f77 2063 6861 7261 6374 6572 7320 7368  ow characters sh
-00000b30: 6f75 6c64 2066 6565 6c20 6162 6f75 7420  ould feel about 
-00000b40: 6561 6368 206f 7468 6572 2e0a 2d20 f09f  each other..- ..
-00000b50: 8fac 2044 6566 696e 6520 6c6f 6361 7469  .. Define locati
-00000b60: 6f6e 2070 7265 6665 7265 6e63 6520 7275  on preference ru
-00000b70: 6c65 7320 666f 7220 7768 6174 206c 6f63  les for what loc
-00000b80: 6174 696f 6e73 2063 6861 7261 6374 6572  ations character
-00000b90: 7320 6672 6571 7565 6e74 2e0a 2d20 f09f  s frequent..- ..
-00000ba0: 9388 2055 7365 7320 5b50 6f6c 6172 735d  .. Uses [Polars]
-00000bb0: 2868 7474 7073 3a2f 2f77 7777 2e70 6f6c  (https://www.pol
-00000bc0: 612e 7273 2920 666f 7220 6661 7374 2064  a.rs) for fast d
-00000bd0: 6174 6120 616e 616c 7973 6973 2e0a 2d20  ata analysis..- 
-00000be0: f09f 939c 2045 7870 6f72 7420 7369 6d75  .... Export simu
-00000bf0: 6c61 7469 6f6e 2064 6174 6120 746f 204a  lation data to J
-00000c00: 534f 4e2e 0a0a 2320 5379 7374 656d 2063  SON...# System c
-00000c10: 6176 6561 7473 0a0a 2d20 4f6e 6c79 2073  aveats..- Only s
-00000c20: 696d 756c 6174 6573 2061 2073 696e 676c  imulates a singl
-00000c30: 6520 7365 7474 6c65 6d65 6e74 0a2d 2043  e settlement.- C
-00000c40: 6861 7261 6374 6572 7320 6361 6e20 6f6e  haracters can on
-00000c50: 6c79 2068 6f6c 6420 6f6e 6520 6f63 6375  ly hold one occu
-00000c60: 7061 7469 6f6e 2061 7420 6120 7469 6d65  pation at a time
-00000c70: 2e0a 2d20 446f 6573 206e 6f74 206d 6f64  ..- Does not mod
-00000c80: 656c 2074 6865 2065 7861 6374 2070 6f73  el the exact pos
-00000c90: 6974 696f 6e20 6f66 2065 6e74 6974 6965  ition of entitie
-00000ca0: 732e 0a0a 2320 5472 7920 4e65 6967 6862  s...# Try Neighb
-00000cb0: 6f72 6c79 2077 6974 686f 7574 2069 6e73  orly without ins
-00000cc0: 7461 6c6c 696e 670a 0a4e 6569 6768 626f  talling..Neighbo
-00000cd0: 726c 7920 6973 2061 7661 696c 6162 6c65  rly is available
-00000ce0: 2074 6f20 7573 6520 7769 7468 696e 2074   to use within t
-00000cf0: 6869 7320 5b73 616d 706c 6520 476f 6f67  his [sample Goog
-00000d00: 6c65 2043 6f6c 6162 206e 6f74 6562 6f6f  le Colab noteboo
-00000d10: 6b5d 2868 7474 7073 3a2f 2f63 6f6c 6162  k](https://colab
-00000d20: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
-00000d30: 2e63 6f6d 2f64 7269 7665 2f31 5778 5a6e  .com/drive/1WxZn
-00000d40: 4352 3861 6665 6b66 426c 2d76 4936 5763  CR8afekfBl-vI6Wc
-00000d50: 4963 5336 4f68 5247 646b 616d 3f75 7370  IcS6OhRGdkam?usp
-00000d60: 3d73 6861 7269 6e67 292e 2049 7420 636f  =sharing). It co
-00000d70: 6e74 6169 6e73 2061 2062 6173 6963 2077  ntains a basic w
-00000d80: 616c 6b74 6872 6f75 6768 206f 6620 686f  alkthrough of ho
-00000d90: 7720 746f 2064 6566 696e 6520 636f 6e74  w to define cont
-00000da0: 656e 7420 666f 7220 7468 6520 7369 6d75  ent for the simu
-00000db0: 6c61 7469 6f6e 2061 6e64 2069 6e73 7065  lation and inspe
-00000dc0: 6374 2074 6865 2067 656e 6572 6174 6564  ct the generated
-00000dd0: 2064 6174 612e 0a0a 2320 496e 7374 616c   data...# Instal
-00000de0: 6c61 7469 6f6e 0a0a 5468 6520 6c61 7465  lation..The late
-00000df0: 7374 206f 6666 6963 6961 6c20 7265 6c65  st official rele
-00000e00: 6173 6520 6f66 204e 6569 6768 626f 726c  ase of Neighborl
-00000e10: 7920 6973 2061 7661 696c 6162 6c65 2074  y is available t
-00000e20: 6f20 696e 7374 616c 6c20 6672 6f6d 205b  o install from [
-00000e30: 5079 5049 5d28 6874 7470 733a 2f2f 7079  PyPI](https://py
-00000e40: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6e  pi.org/project/n
-00000e50: 6569 6768 626f 726c 792f 292e 0a0a 6060  eighborly/)...``
-00000e60: 6062 6173 680a 7069 7020 696e 7374 616c  `bash.pip instal
-00000e70: 6c20 6e65 6967 6862 6f72 6c79 0a60 6060  l neighborly.```
-00000e80: 0a0a 2323 2049 6e73 7461 6c6c 696e 6720  ..## Installing 
-00000e90: 666f 7220 6c6f 6361 6c20 6465 7665 6c6f  for local develo
-00000ea0: 706d 656e 740a 0a49 6620 796f 7520 7769  pment..If you wi
-00000eb0: 7368 2074 6f20 646f 776e 6c6f 6164 2061  sh to download a
-00000ec0: 204e 6569 6768 626f 726c 7920 666f 7220   Neighborly for 
-00000ed0: 6c6f 6361 6c20 6465 7665 6c6f 706d 656e  local developmen
-00000ee0: 7420 6f72 2077 616e 7420 746f 2070 6c61  t or want to pla
-00000ef0: 7920 6172 6f75 6e64 2077 6974 680a 616e  y around with.an
-00000f00: 7920 6f66 2074 6865 2073 616d 706c 6573  y of the samples
-00000f10: 2c20 796f 7520 6e65 6564 2074 6f20 636c  , you need to cl
-00000f20: 6f6e 6520 6f72 2064 6f77 6e6c 6f61 6420  one or download 
-00000f30: 7468 6973 2072 6570 6f73 6974 6f72 7920  this repository 
-00000f40: 616e 6420 696e 7374 616c 6c0a 7573 696e  and install.usin
-00000f50: 6720 7468 6520 5f65 6469 7461 626c 655f  g the _editable_
-00000f60: 2066 6c61 6720 282d 6529 2e20 506c 6561   flag (-e). Plea
-00000f70: 7365 2073 6565 2074 6865 2069 6e73 7472  se see the instr
-00000f80: 7563 7469 6f6e 7320 6265 6c6f 772e 2054  uctions below. T
-00000f90: 6869 7320 636f 6d6d 616e 6420 7769 6c6c  his command will
-00000fa0: 2069 6e73 7461 6c6c 0a61 204e 6569 6768   install.a Neigh
-00000fb0: 626f 726c 7920 696e 746f 2074 6865 2076  borly into the v
-00000fc0: 6972 7475 616c 2065 6e76 6972 6f6e 6d65  irtual environme
-00000fd0: 6e74 2061 6c6f 6e67 2077 6974 6820 616c  nt along with al
-00000fe0: 6c20 6974 7320 6465 7065 6e64 656e 6369  l its dependenci
-00000ff0: 6573 2061 6e64 2061 2066 6577 0a61 6464  es and a few.add
-00001000: 6974 696f 6e61 6c20 6465 7665 6c6f 706d  itional developm
-00001010: 656e 7420 616e 6420 7465 7374 696e 6720  ent and testing 
-00001020: 6465 7065 6e64 656e 6369 6573 2073 7563  dependencies suc
-00001030: 6820 6173 205f 626c 6163 6b5f 2c20 5f69  h as _black_, _i
-00001040: 736f 7274 5f2c 2061 6e64 205f 7079 7465  sort_, and _pyte
-00001050: 7374 5f2e 0a0a 6060 6062 6173 680a 2320  st_...```bash.# 
-00001060: 5374 6570 2031 3a20 436c 6f6e 6520 5265  Step 1: Clone Re
-00001070: 706f 7369 746f 7279 2061 6e64 2063 6861  pository and cha
-00001080: 6e67 6520 696e 746f 2070 726f 6a65 6374  nge into project
-00001090: 2064 6972 6563 746f 7279 0a67 6974 2063   directory.git c
-000010a0: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
-000010b0: 6875 622e 636f 6d2f 5368 694a 6265 792f  hub.com/ShiJbey/
-000010c0: 6e65 6967 6862 6f72 6c79 2e67 6974 0a63  neighborly.git.c
-000010d0: 6420 6e65 6967 6862 6f72 6c79 0a0a 2320  d neighborly..# 
-000010e0: 5374 6570 2032 2028 4d61 634f 532f 4c69  Step 2 (MacOS/Li
-000010f0: 6e75 7829 3a20 4372 6561 7465 2061 6e64  nux): Create and
-00001100: 2061 6374 6976 6174 6520 6120 5079 7468   activate a Pyth
-00001110: 6f6e 2076 6972 7475 616c 2065 6e76 6972  on virtual envir
-00001120: 6f6e 6d65 6e74 0a70 7974 686f 6e33 202d  onment.python3 -
-00001130: 6d20 7665 6e76 2076 656e 760a 736f 7572  m venv venv.sour
-00001140: 6365 202e 2f76 656e 762f 6269 6e2f 6163  ce ./venv/bin/ac
-00001150: 7469 7661 7465 0a0a 2320 5374 6570 2032  tivate..# Step 2
-00001160: 2028 5769 6e64 6f77 7329 3a20 4372 6561   (Windows): Crea
-00001170: 7465 2061 6e64 2061 6374 6976 6174 6520  te and activate 
-00001180: 6120 5079 7468 6f6e 2076 6972 7475 616c  a Python virtual
-00001190: 2065 6e76 6972 6f6e 6d65 6e74 0a70 7974   environment.pyt
-000011a0: 686f 6e20 2d6d 2076 656e 7620 7665 6e76  hon -m venv venv
-000011b0: 0a2e 5c76 656e 765c 5363 7269 7074 735c  ..\venv\Scripts\
-000011c0: 4163 7469 7661 7465 0a0a 2320 5374 6570  Activate..# Step
-000011d0: 2033 3a20 496e 7374 616c 6c20 6c6f 6361   3: Install loca
-000011e0: 6c20 6275 696c 6420 616e 6420 6465 7065  l build and depe
-000011f0: 6e64 656e 6369 6573 0a70 7974 686f 6e20  ndencies.python 
-00001200: 2d6d 2070 6970 2069 6e73 7461 6c6c 202d  -m pip install -
-00001210: 6520 222e 5b64 6576 656c 6f70 6d65 6e74  e ".[development
-00001220: 5d22 0a60 6060 0a0a 2320 5573 6167 650a  ]".```..# Usage.
-00001230: 0a54 6865 2062 6573 7420 7761 7920 746f  .The best way to
-00001240: 206c 6561 726e 2068 6f77 2074 6f20 7573   learn how to us
-00001250: 6520 4e65 6967 6862 6f72 6c79 2069 7320  e Neighborly is 
-00001260: 746f 2065 7870 6c6f 7265 2074 6865 2076  to explore the v
-00001270: 6172 696f 7573 2073 616d 706c 6573 2069  arious samples i
-00001280: 6e20 7468 6520 6073 616d 706c 6573 6020  n the `samples` 
-00001290: 6469 7265 6374 6f72 790a 7468 6174 2064  directory.that d
-000012a0: 656d 6f6e 7374 7261 7465 2068 6f77 2074  emonstrate how t
-000012b0: 6f20 6372 6561 7465 2063 7573 746f 6d20  o create custom 
-000012c0: 7369 6d75 6c61 7469 6f6e 7320 616e 6420  simulations and 
-000012d0: 636f 6c6c 6563 7420 616e 6420 7669 7375  collect and visu
-000012e0: 616c 697a 6520 6461 7461 2e20 496e 7465  alize data. Inte
-000012f0: 7261 6374 6976 6520 7361 6d70 6c65 7320  ractive samples 
-00001300: 7769 7468 2074 6865 2060 2e69 7079 6e62  with the `.ipynb
-00001310: 600a 6578 7465 6e73 696f 6e20 6172 6520  `.extension are 
-00001320: 6d65 616e 7420 746f 2062 6520 7275 6e20  meant to be run 
-00001330: 7573 696e 6720 5b4a 7570 7974 6572 204c  using [Jupyter L
-00001340: 6162 5d28 6874 7470 733a 2f2f 6a75 7079  ab](https://jupy
-00001350: 7465 722e 6f72 672f 292e 2050 6c65 6173  ter.org/). Pleas
-00001360: 6520 7275 6e20 7468 6520 666f 6c6c 6f77  e run the follow
-00001370: 696e 6720 636f 6d6d 616e 640a 746f 2065  ing command.to e
-00001380: 6e73 7572 6520 616c 6c20 6465 7065 6e64  nsure all depend
-00001390: 656e 6369 6573 2061 7265 2069 6e73 7461  encies are insta
-000013a0: 6c6c 6564 2066 6f72 2074 6865 2073 616d  lled for the sam
-000013b0: 706c 6573 2e20 4d61 6b65 2073 7572 6520  ples. Make sure 
-000013c0: 7468 6174 2079 6f75 2776 6520 6163 7469  that you've acti
-000013d0: 7661 7465 6420 796f 7572 2050 7974 686f  vated your Pytho
-000013e0: 6e20 7669 7274 7561 6c0a 656e 7669 726f  n virtual.enviro
-000013f0: 6e6d 656e 7420 6265 666f 7265 6861 6e64  nment beforehand
-00001400: 2e0a 0a60 6060 6261 7368 0a70 7974 686f  ...```bash.pytho
-00001410: 6e20 2d6d 2070 6970 2069 6e73 7461 6c6c  n -m pip install
-00001420: 202d 6520 222e 5b73 616d 706c 6573 5d22   -e ".[samples]"
-00001430: 0a60 6060 0a0a 5468 656e 2c20 7275 6e20  .```..Then, run 
-00001440: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
-00001450: 6d6d 616e 6473 2074 6f20 7275 6e20 7468  mmands to run th
-00001460: 6520 7361 6d70 6c65 2073 6372 6970 7473  e sample scripts
-00001470: 206f 7220 6e6f 7465 626f 6f6b 732e 0a0a   or notebooks...
-00001480: 6060 6062 6173 680a 2320 546f 2072 756e  ```bash.# To run
-00001490: 2073 616d 706c 6520 7363 7269 7074 732c   sample scripts,
-000014a0: 2075 7365 3a0a 7079 7468 6f6e 202e 2f73   use:.python ./s
-000014b0: 616d 706c 6573 2f3c 6e61 6d65 5f6f 665f  amples/<name_of_
-000014c0: 7361 6d70 6c65 3e2e 7079 0a0a 2320 4578  sample>.py..# Ex
-000014d0: 706c 6f72 6520 4950 7974 686f 6e20 6e6f  plore IPython no
-000014e0: 7465 626f 6f6b 7320 7573 696e 6720 4a75  tebooks using Ju
-000014f0: 7079 7465 7220 4c61 623a 0a6a 7570 7974  pyter Lab:.jupyt
-00001500: 6572 2d6c 6162 0a60 6060 0a0a 2320 506c  er-lab.```..# Pl
-00001510: 7567 696e 730a 0a50 6c75 6769 6e73 2061  ugins..Plugins a
-00001520: 7265 2069 6d70 6f72 7461 626c 6520 5079  re importable Py
-00001530: 7468 6f6e 206d 6f64 756c 6573 206f 7220  thon modules or 
-00001540: 7061 636b 6167 6573 2074 6861 7420 6164  packages that ad
-00001550: 6420 6e65 7720 636f 6e74 656e 7420 746f  d new content to
-00001560: 2061 2073 696d 756c 6174 696f 6e2e 2054   a simulation. T
-00001570: 6865 7920 616c 6c6f 7720 7573 6572 7320  hey allow users 
-00001580: 746f 2063 6861 6e67 650a 6120 7369 6d75  to change.a simu
-00001590: 6c61 7469 6f6e 2773 2062 6568 6176 696f  lation's behavio
-000015a0: 7220 7769 7468 6f75 7420 6564 6974 696e  r without editin
-000015b0: 6720 7468 6520 636f 7265 206c 6962 7261  g the core libra
-000015c0: 7279 2063 6f64 652e 2041 6c6c 2070 6c75  ry code. All plu
-000015d0: 6769 6e73 2073 686f 756c 6420 6861 7665  gins should have
-000015e0: 2061 2074 6f70 2d6c 6576 656c 0a60 6c6f   a top-level.`lo
-000015f0: 6164 5f70 6c75 6769 6e28 7369 6d29 6020  ad_plugin(sim)` 
-00001600: 6675 6e63 7469 6f6e 2074 6861 7420 6765  function that ge
-00001610: 7473 2063 616c 6c65 6420 746f 206c 6f61  ts called to loa
-00001620: 6420 696e 2074 6865 2070 6c75 6769 6e20  d in the plugin 
-00001630: 636f 6e74 656e 742e 0a0a 4173 2077 6974  content...As wit
-00001640: 6820 616e 7920 7069 6563 6520 6f66 2073  h any piece of s
-00001650: 6f66 7477 6172 652c 2061 6c77 6179 7320  oftware, always 
-00001660: 6578 7072 6573 7320 6361 7574 696f 6e20  express caution 
-00001670: 7768 656e 2064 6f77 6e6c 6f61 6469 6e67  when downloading
-00001680: 2074 6869 7264 2d70 6172 7479 2070 6c75   third-party plu
-00001690: 6769 6e73 2e20 456e 7375 7265 2074 6865  gins. Ensure the
-000016a0: 7920 636f 6d65 2066 726f 6d20 610a 736f  y come from a.so
-000016b0: 7572 6365 2074 6861 7420 796f 7520 7472  urce that you tr
-000016c0: 7573 742e 0a0a 546f 2072 6561 6420 6d6f  ust...To read mo
-000016d0: 7265 2061 626f 7574 2070 6c75 6769 6e73  re about plugins
-000016e0: 2c20 7669 7369 7420 7468 6520 5b50 6c75  , visit the [Plu
-000016f0: 6769 6e73 5d28 6874 7470 733a 2f2f 6769  gins](https://gi
-00001700: 7468 7562 2e63 6f6d 2f53 6869 4a62 6579  thub.com/ShiJbey
-00001710: 2f6e 6569 6768 626f 726c 792f 7769 6b69  /neighborly/wiki
-00001720: 2f70 6c75 6769 6e73 2920 7365 6374 696f  /plugins) sectio
-00001730: 6e20 6f66 2074 6865 0a77 696b 692e 0a0a  n of the.wiki...
-00001740: 2320 5465 7374 730a 0a4e 6569 6768 626f  # Tests..Neighbo
-00001750: 726c 7920 7573 6573 205b 5079 5465 7374  rly uses [PyTest
-00001760: 5d28 6874 7470 733a 2f2f 646f 6373 2e70  ](https://docs.p
-00001770: 7974 6573 742e 6f72 672f 2920 666f 7220  ytest.org/) for 
-00001780: 756e 6974 2074 6573 7469 6e67 2e20 416c  unit testing. Al
-00001790: 6c20 7465 7374 7320 6172 6520 6c6f 6361  l tests are loca
-000017a0: 7465 6420 696e 2074 6865 2060 7465 7374  ted in the `test
-000017b0: 732f 6020 6469 7265 6374 6f72 792e 2049  s/` directory. I
-000017c0: 0a64 6f20 6d79 2062 6573 7420 746f 206b  .do my best to k
-000017d0: 6565 7020 7465 7374 7320 7570 6461 7465  eep tests update
-000017e0: 642e 2048 6f77 6576 6572 2c20 736f 6d65  d. However, some
-000017f0: 2074 6573 7473 206d 6179 206e 6565 6420   tests may need 
-00001800: 746f 2062 650a 6164 6465 6420 6f72 2075  to be.added or u
-00001810: 7064 6174 6564 2064 7565 2074 6f20 636f  pdated due to co
-00001820: 6e73 7461 6e74 2062 7265 616b 696e 6720  nstant breaking 
-00001830: 6368 616e 6765 7320 6265 7477 6565 6e20  changes between 
-00001840: 7265 6c65 6173 6573 2e20 4966 2079 6f75  releases. If you
-00001850: 2077 616e 7420 746f 2063 6f6e 7472 6962   want to contrib
-00001860: 7574 6520 756e 6974 2074 6573 7473 2c20  ute unit tests, 
-00001870: 706c 6561 7365 2072 6566 6572 0a74 6f20  please refer.to 
-00001880: 5b43 4f4e 5452 4942 5554 494e 472e 6d64  [CONTRIBUTING.md
-00001890: 5d28 2e2f 434f 4e54 5249 4255 5449 4e47  ](./CONTRIBUTING
-000018a0: 2e6d 6429 2e0a 0a60 6060 6261 7368 0a23  .md)...```bash.#
-000018b0: 2053 7465 7020 313a 2049 6e73 7461 6c6c   Step 1: Install
-000018c0: 2061 6464 6974 696f 6e61 6c20 6465 7065   additional depe
-000018d0: 6e64 656e 6369 6573 2066 6f72 2074 6573  ndencies for tes
-000018e0: 7473 0a70 7974 686f 6e20 2d6d 2070 6970  ts.python -m pip
-000018f0: 2069 6e73 7461 6c6c 202d 6520 222e 5b64   install -e ".[d
-00001900: 6576 656c 6f70 6d65 6e74 5d22 0a0a 2320  evelopment]"..# 
-00001910: 5374 6570 2032 3a20 5275 6e20 5079 7465  Step 2: Run Pyte
-00001920: 7374 0a70 7974 6573 740a 0a23 2053 7465  st.pytest..# Ste
-00001930: 7033 203a 2028 4f70 7469 6f6e 616c 2920  p3 : (Optional) 
-00001940: 4765 6e65 7261 7465 2061 2074 6573 7420  Generate a test 
-00001950: 636f 7665 7261 6765 2072 6570 6f72 740a  coverage report.
-00001960: 7079 7465 7374 202d 2d63 6f76 3d6e 6569  pytest --cov=nei
-00001970: 6768 626f 726c 7920 7465 7374 732f 0a60  ghborly tests/.`
-00001980: 6060 0a0a 2320 446f 6375 6d65 6e74 6174  ``..# Documentat
-00001990: 696f 6e0a 0a54 6865 2062 6573 7420 706c  ion..The best pl
-000019a0: 6163 6520 746f 2066 696e 6420 6578 616d  ace to find exam
-000019b0: 706c 6573 206f 6620 686f 7720 746f 2075  ples of how to u
-000019c0: 7365 204e 6569 6768 626f 726c 7920 6973  se Neighborly is
-000019d0: 2061 6374 7561 6c6c 7920 696e 2074 6865   actually in the
-000019e0: 2060 2e2f 7465 7374 7360 2064 6972 6563   `./tests` direc
-000019f0: 746f 7279 2e20 5468 6572 6520 796f 7520  tory. There you 
-00001a00: 7769 6c6c 2066 696e 6420 6578 616d 706c  will find exampl
-00001a10: 6573 206f 6620 6c6f 6164 696e 6720 636f  es of loading co
-00001a20: 6e74 656e 7420 6672 6f6d 2066 696c 6573  ntent from files
-00001a30: 2c20 7275 6e6e 696e 6720 6120 7369 6d75  , running a simu
-00001a40: 6c61 7469 6f6e 2c20 616e 6420 7361 7669  lation, and savi
-00001a50: 6e67 2074 6865 206f 7574 7075 7420 746f  ng the output to
-00001a60: 204a 534f 4e2e 2054 6865 7265 2069 7320   JSON. There is 
-00001a70: 616c 736f 2074 6865 205b 5265 6164 2074  also the [Read t
-00001a80: 6865 2044 6f63 735d 2868 7474 7073 3a2f  he Docs](https:/
-00001a90: 2f6e 6569 6768 626f 726c 792e 7265 6164  /neighborly.read
-00001aa0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00001ab0: 7465 7374 2f69 6e64 6578 2e68 746d 6c29  test/index.html)
-00001ac0: 2e20 486f 7765 7665 722c 2074 6865 2064  . However, the d
-00001ad0: 6f63 7320 6861 7320 6120 7465 6e64 656e  ocs has a tenden
-00001ae0: 6379 2074 6f20 6265 206f 7574 206f 6620  cy to be out of 
-00001af0: 6461 7465 2077 6865 6e20 6e65 772c 2070  date when new, p
-00001b00: 6f74 656e 7469 616c 6c79 2062 7265 616b  otentially break
-00001b10: 696e 6720 6368 616e 6765 7320 6172 6520  ing changes are 
-00001b20: 6d61 6465 2074 6f20 7468 6520 6672 616d  made to the fram
-00001b30: 6577 6f72 6b2e 2048 6f77 6576 6572 2c20  ework. However, 
-00001b40: 756e 6974 2074 6573 7473 2061 7265 2075  unit tests are u
-00001b50: 7064 6174 6564 2061 6c6d 6f73 7420 6576  pdated almost ev
-00001b60: 6572 7920 7469 6d65 2061 206e 6577 2066  ery time a new f
-00001b70: 6561 7475 7265 2069 7320 6164 6465 642e  eature is added.
-00001b80: 0a0a 2320 4765 7474 696e 6720 6865 6c70  ..# Getting help
-00001b90: 2061 6e64 2073 7562 6d69 7474 696e 6720   and submitting 
-00001ba0: 6275 6720 7265 706f 7274 730a 0a49 6620  bug reports..If 
-00001bb0: 796f 7520 6861 7665 2061 6e79 2071 7565  you have any que
-00001bc0: 7374 696f 6e73 2c20 6665 6564 6261 636b  stions, feedback
-00001bd0: 2c20 6f72 2070 726f 626c 656d 732c 2070  , or problems, p
-00001be0: 6c65 6173 6520 6372 6561 7465 2061 206e  lease create a n
-00001bf0: 6577 2049 7373 7565 2e20 4920 7769 6c6c  ew Issue. I will
-00001c00: 2064 6f20 6d79 2062 6573 7420 746f 2061   do my best to a
-00001c10: 6e73 7765 7220 6173 2073 6f6f 6e20 6173  nswer as soon as
-00001c20: 2049 0a63 616e 2e20 506c 6561 7365 2062   I.can. Please b
-00001c30: 6520 7265 7370 6563 7466 756c 2c20 616e  e respectful, an
-00001c40: 6420 4920 6170 7072 6563 6961 7465 2079  d I appreciate y
-00001c50: 6f75 7220 7061 7469 656e 6365 2e0a 0a23  our patience...#
-00001c60: 2043 6f6e 7472 6962 7574 696e 670a 0a43   Contributing..C
-00001c70: 6f6e 7472 6962 7574 696f 6e73 2061 7265  ontributions are
-00001c80: 2077 656c 636f 6d65 2e20 506c 6561 7365   welcome. Please
-00001c90: 2072 6566 6572 2074 6f20 5b43 4f4e 5452   refer to [CONTR
-00001ca0: 4942 5554 494e 472e 6d64 5d28 2e2f 434f  IBUTING.md](./CO
-00001cb0: 4e54 5249 4255 5449 4e47 2e6d 6429 2066  NTRIBUTING.md) f
-00001cc0: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
-00001cd0: 696f 6e20 6162 6f75 7420 686f 7720 746f  ion about how to
-00001ce0: 2067 6574 0a69 6e76 6f6c 7665 642e 0a0a   get.involved...
-00001cf0: 2320 4c69 6365 6e73 650a 0a54 6869 7320  # License..This 
-00001d00: 7072 6f6a 6563 7420 6973 206c 6963 656e  project is licen
-00001d10: 7365 6420 756e 6465 7220 7468 6520 5b4d  sed under the [M
-00001d20: 4954 204c 6963 656e 7365 5d28 2e2f 4c49  IT License](./LI
-00001d30: 4345 4e53 4529 2e0a 0a23 2044 4d43 4120  CENSE)...# DMCA 
-00001d40: 5374 6174 656d 656e 740a 0a55 706f 6e20  Statement..Upon 
-00001d50: 7265 6365 6970 7420 6f66 2061 206e 6f74  receipt of a not
-00001d60: 6963 6520 616c 6c65 6769 6e67 2063 6f70  ice alleging cop
-00001d70: 7972 6967 6874 2069 6e66 7269 6e67 656d  yright infringem
-00001d80: 656e 742c 2049 2077 696c 6c20 7461 6b65  ent, I will take
-00001d90: 2077 6861 7465 7665 7220 6163 7469 6f6e   whatever action
-00001da0: 2069 7420 6465 656d 7320 6170 7072 6f70   it deems approp
-00001db0: 7269 6174 6520 7769 7468 696e 2069 7473  riate within its
-00001dc0: 0a73 6f6c 6520 6469 7363 7265 7469 6f6e  .sole discretion
-00001dd0: 2c20 696e 636c 7564 696e 6720 7265 6d6f  , including remo
-00001de0: 7661 6c20 6f66 2074 6865 2061 6c6c 6567  val of the alleg
-00001df0: 6564 6c79 2069 6e66 7269 6e67 696e 6720  edly infringing 
-00001e00: 6d61 7465 7269 616c 732e 0a0a 5468 6520  materials...The 
-00001e10: 7265 706f 2069 6d61 6765 2069 7320 736f  repo image is so
-00001e20: 6d65 7468 696e 6720 6675 6e20 7468 6174  mething fun that
-00001e30: 2049 206d 6164 652e 2049 206c 6f76 6520   I made. I love 
-00001e40: 5f54 6865 2053 696d 7073 6f6e 735f 2c20  _The Simpsons_, 
-00001e50: 616e 6420 4920 636f 756c 646e 2774 2074  and I couldn't t
-00001e60: 6869 6e6b 206f 6620 616e 796f 6e65 206d  hink of anyone m
-00001e70: 6f72 6520 6e65 6967 6862 6f72 6c79 2074  ore neighborly t
-00001e80: 6861 6e0a 4e65 6420 466c 616e 6465 7273  han.Ned Flanders
-00001e90: 2e20 4966 2074 6865 2063 6f70 7972 6967  . If the copyrig
-00001ea0: 6874 206f 776e 6572 2066 6f72 205f 5468  ht owner for _Th
-00001eb0: 6520 5369 6d70 736f 6e73 5f20 776f 756c  e Simpsons_ woul
-00001ec0: 6420 6c69 6b65 206d 6520 746f 2074 616b  d like me to tak
-00001ed0: 6520 6974 2064 6f77 6e2c 2070 6c65 6173  e it down, pleas
-00001ee0: 6520 636f 6e74 6163 7420 6d65 2e20 5468  e contact me. Th
-00001ef0: 6520 7361 6d65 0a74 616b 6564 6f77 6e20  e same.takedown 
-00001f00: 706f 6c69 6379 2061 7070 6c69 6573 2074  policy applies t
-00001f10: 6f20 636f 6465 2073 616d 706c 6573 2069  o code samples i
-00001f20: 6e73 7069 7265 6420 6279 2054 5620 7368  nspired by TV sh
-00001f30: 6f77 732c 206d 6f76 6965 732c 2061 6e64  ows, movies, and
-00001f40: 2067 616d 6573 2e0a                       games..
+000001e0: 6c64 732e 696f 2f70 7970 692f 762f 6e65  lds.io/pypi/v/ne
+000001f0: 6967 6862 6f72 6c79 2220 616c 743d 2250  ighborly" alt="P
+00000200: 7950 4920 7665 7273 696f 6e20 6261 6467  yPI version badg
+00000210: 6522 3e0a 2020 3c69 6d67 2073 7263 3d22  e">.  <img src="
+00000220: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000230: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
+00000240: 7273 696f 6e73 2f6e 6569 6768 626f 726c  rsions/neighborl
+00000250: 7922 2061 6c74 3d22 5375 7070 6f72 7465  y" alt="Supporte
+00000260: 6420 5079 7468 6f6e 2056 6572 7369 6f6e  d Python Version
+00000270: 7320 6261 6467 6522 3e0a 2020 3c69 6d67  s badge">.  <img
+00000280: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000290: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+000002a0: 692f 6c2f 6e65 6967 6862 6f72 6c79 2220  i/l/neighborly" 
+000002b0: 616c 743d 224d 4954 204c 6963 656e 7365  alt="MIT License
+000002c0: 2062 6164 6765 223e 0a20 203c 696d 6720   badge">.  <img 
+000002d0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+000002e0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+000002f0: 2f64 6d2f 6e65 6967 6862 6f72 6c79 2220  /dm/neighborly" 
+00000300: 616c 743d 2250 7950 4920 646f 776e 6c6f  alt="PyPI downlo
+00000310: 6164 7320 6261 6467 6522 3e0a 2020 3c69  ads badge">.  <i
+00000320: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000330: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000340: 6164 6765 2f63 6f64 6525 3230 7374 796c  adge/code%20styl
+00000350: 652d 626c 6163 6b2d 626c 6163 6b22 2061  e-black-black" a
+00000360: 6c74 3d22 426c 6163 6b20 666f 726d 6174  lt="Black format
+00000370: 7465 7220 6261 6467 6522 3e0a 2020 3c69  ter badge">.  <i
+00000380: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000390: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+000003a0: 6164 6765 2f25 3230 696d 706f 7274 732d  adge/%20imports-
+000003b0: 6973 6f72 742d 2532 3331 3637 3462 313f  isort-%231674b1?
+000003c0: 7374 796c 653d 666c 6174 266c 6162 656c  style=flat&label
+000003d0: 436f 6c6f 723d 6566 3833 3336 2220 616c  Color=ef8336" al
+000003e0: 743d 2249 536f 7274 2062 6164 6765 223e  t="ISort badge">
+000003f0: 0a3c 2f70 3e0a 0a4e 6569 6768 626f 726c  .</p>..Neighborl
+00000400: 7920 6973 2061 6e20 6167 656e 742d 6261  y is an agent-ba
+00000410: 7365 6420 7365 7474 6c65 6d65 6e74 2073  sed settlement s
+00000420: 696d 756c 6174 696f 6e20 7468 6174 2067  imulation that g
+00000430: 656e 6572 6174 6573 2062 6163 6b73 746f  enerates backsto
+00000440: 7279 2064 6174 6120 666f 7220 6368 6172  ry data for char
+00000450: 6163 7465 7273 206c 6976 696e 6720 696e  acters living in
+00000460: 2061 2070 726f 6365 6475 7261 6c6c 7920   a procedurally 
+00000470: 6765 6e65 7261 7465 6420 7365 7474 6c65  generated settle
+00000480: 6d65 6e74 2e20 4974 2077 6173 2062 7569  ment. It was bui
+00000490: 6c74 2074 6f20 6265 2061 2074 6f6f 6c20  lt to be a tool 
+000004a0: 666f 7220 656d 6572 6765 6e74 206e 6172  for emergent nar
+000004b0: 7261 7469 7665 2073 746f 7279 7465 6c6c  rative storytell
+000004c0: 696e 6720 7265 7365 6172 6368 2e20 4e65  ing research. Ne
+000004d0: 6967 6862 6f72 6c79 206d 6f64 656c 7320  ighborly models 
+000004e0: 7468 6520 6368 6172 6163 7465 7273 2720  the characters' 
+000004f0: 7472 6169 7473 2c20 7374 6174 7573 6573  traits, statuses
+00000500: 2c20 7265 6c61 7469 6f6e 7368 6970 732c  , relationships,
+00000510: 206f 6363 7570 6174 696f 6e73 2c20 6c69   occupations, li
+00000520: 6665 2065 7665 6e74 732c 2065 7463 2e20  fe events, etc. 
+00000530: 6f76 6572 2064 6563 6164 6573 206f 6620  over decades of 
+00000540: 7369 6d75 6c61 7465 6420 7469 6d65 2e20  simulated time. 
+00000550: 5468 6520 656e 7469 7265 2068 6973 746f  The entire histo
+00000560: 7279 206f 6620 7468 6520 7365 7474 6c65  ry of the settle
+00000570: 6d65 6e74 2061 6e64 2069 7473 2067 656e  ment and its gen
+00000580: 6572 6174 696f 6e73 206f 6620 6368 6172  erations of char
+00000590: 6163 7465 7273 2069 7320 6d61 6465 2061  acters is made a
+000005a0: 7661 696c 6162 6c65 2066 6f72 2064 6174  vailable for dat
+000005b0: 6120 616e 616c 7973 6973 2061 6e64 2065  a analysis and e
+000005c0: 7870 6f72 7469 6e67 2e20 4e65 6967 6862  xporting. Neighb
+000005d0: 6f72 6c79 2061 696d 7320 746f 2062 6520  orly aims to be 
+000005e0: 616e 2065 6173 696c 7920 6375 7374 6f6d  an easily custom
+000005f0: 697a 6162 6c65 2073 696d 756c 6174 696f  izable simulatio
+00000600: 6e20 7468 6174 2063 616e 2061 6461 7074  n that can adapt
+00000610: 2074 6f20 7661 7269 6f75 7320 6e61 7272   to various narr
+00000620: 6174 6976 6520 7365 7474 696e 6773 2061  ative settings a
+00000630: 6e64 2073 7570 706f 7274 2072 6573 6561  nd support resea
+00000640: 7263 6820 6f72 2065 6e74 6572 7461 696e  rch or entertain
+00000650: 6d65 6e74 2070 726f 6a65 6374 732e 0a0a  ment projects...
+00000660: 4e65 6967 6862 6f72 6c79 2773 2077 6173  Neighborly's was
+00000670: 2069 6e73 7069 7265 6420 5b5f 5461 6c6b   inspired [_Talk
+00000680: 206f 6620 7468 6520 546f 776e 5f5d 2868   of the Town_](h
+00000690: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000006a0: 6d2f 6a61 6d65 732d 6f77 656e 2d72 7961  m/james-owen-rya
+000006b0: 6e2f 7461 6c6b 746f 776e 292c 2061 6e6f  n/talktown), ano
+000006c0: 7468 6572 2073 6574 746c 656d 656e 7420  ther settlement 
+000006d0: 7369 6d75 6c61 7469 6f6e 2066 6f72 2065  simulation for e
+000006e0: 6d65 7267 656e 7420 6e61 7272 6174 6976  mergent narrativ
+000006f0: 6520 7374 6f72 7974 656c 6c69 6e67 2072  e storytelling r
+00000700: 6573 6561 7263 682e 2049 7420 616c 736f  esearch. It also
+00000710: 2064 7261 7773 2069 6e73 7069 7261 7469   draws inspirati
+00000720: 6f6e 2066 726f 6d20 636f 6d6d 6572 6369  on from commerci
+00000730: 616c 2077 6f72 6c64 2d73 696d 756c 6174  al world-simulat
+00000740: 696f 6e20 6761 6d65 7320 6c69 6b65 205f  ion games like _
+00000750: 4361 7665 7320 6f66 2051 7564 5f2c 205f  Caves of Qud_, _
+00000760: 4477 6172 6620 466f 7274 7265 7373 5f2c  Dwarf Fortress_,
+00000770: 205f 4372 7573 6164 6572 204b 696e 6773   _Crusader Kings
+00000780: 5f2c 205f 5269 6d57 6f72 6c64 5f2c 2061  _, _RimWorld_, a
+00000790: 6e64 205f 576f 726c 6442 6f78 5f2e 0a0a  nd _WorldBox_...
+000007a0: 4966 2079 6f75 2075 7365 204e 6569 6768  If you use Neigh
+000007b0: 626f 726c 7920 696e 2061 2070 726f 6a65  borly in a proje
+000007c0: 6374 2c20 706c 6561 7365 2063 6974 6520  ct, please cite 
+000007d0: 7468 6973 2072 6570 6f73 6974 6f72 792e  this repository.
+000007e0: 2059 6f75 2063 616e 2072 6561 640a 4e65   You can read.Ne
+000007f0: 6967 6862 6f72 6c79 2773 2061 7373 6f63  ighborly's assoc
+00000800: 6961 7465 6420 5b70 6170 6572 5d28 6874  iated [paper](ht
+00000810: 7470 733a 2f2f 7368 696a 6265 792e 6769  tps://shijbey.gi
+00000820: 7468 7562 2e69 6f2f 7075 626c 6963 6174  thub.io/publicat
+00000830: 696f 6e73 2f4e 6569 6768 626f 726c 792e  ions/Neighborly.
+00000840: 7064 6629 2074 6861 7420 7761 7320 7075  pdf) that was pu
+00000850: 626c 6973 6865 6420 696e 2074 6865 0a70  blished in the.p
+00000860: 726f 6365 6564 696e 6773 206f 6620 7468  roceedings of th
+00000870: 6520 3230 3232 2049 4545 4520 436f 6e66  e 2022 IEEE Conf
+00000880: 6572 656e 6365 204f 6e20 4761 6d65 732e  erence On Games.
+00000890: 0a0a 6060 6074 6578 740a 4069 6e70 726f  ..```text.@inpro
+000008a0: 6365 6564 696e 6773 7b6a 6f68 6e73 6f6e  ceedings{johnson
+000008b0: 6265 7932 3032 326e 6569 6768 626f 726c  bey2022neighborl
+000008c0: 792c 0a20 2020 2074 6974 6c65 203d 207b  y,.    title = {
+000008d0: 4e65 6967 6862 6f72 6c79 3a20 4120 5361  Neighborly: A Sa
+000008e0: 6e64 626f 7820 666f 7220 5369 6d75 6c61  ndbox for Simula
+000008f0: 7469 6f6e 2d62 6173 6564 2045 6d65 7267  tion-based Emerg
+00000900: 656e 7420 4e61 7272 6174 6976 657d 2c0a  ent Narrative},.
+00000910: 2020 2020 6175 7468 6f72 203d 207b 4a6f      author = {Jo
+00000920: 686e 736f 6e2d 4265 792c 2053 6869 2061  hnson-Bey, Shi a
+00000930: 6e64 204e 656c 736f 6e2c 204d 6172 6b20  nd Nelson, Mark 
+00000940: 4a20 616e 6420 4d61 7465 6173 2c20 4d69  J and Mateas, Mi
+00000950: 6368 6165 6c7d 2c0a 2020 2020 626f 6f6b  chael},.    book
+00000960: 7469 746c 6520 3d20 7b32 3032 3220 4945  title = {2022 IE
+00000970: 4545 2043 6f6e 6665 7265 6e63 6520 6f6e  EE Conference on
+00000980: 2047 616d 6573 2028 436f 4729 7d2c 0a20   Games (CoG)},. 
+00000990: 2020 2070 6167 6573 203d 207b 3432 352d     pages = {425-
+000009a0: 2d34 3332 7d2c 0a20 2020 2079 6561 7220  -432},.    year 
+000009b0: 3d20 7b32 3032 327d 2c0a 2020 2020 6f72  = {2022},.    or
+000009c0: 6761 6e69 7a61 7469 6f6e 203d 207b 4945  ganization = {IE
+000009d0: 4545 7d0a 7d0a 6060 600a 0a3e 205b 2149  EE}.}.```..> [!I
+000009e0: 4d50 4f52 5441 4e54 5d0a 3e20 4e65 6967  MPORTANT].> Neig
+000009f0: 6862 6f72 6c79 2773 2063 7572 7265 6e74  hborly's current
+00000a00: 2061 7263 6869 7465 6374 7572 6520 6469   architecture di
+00000a10: 6666 6572 7320 6672 6f6d 2077 6861 7420  ffers from what 
+00000a20: 6973 2064 6573 6372 6962 6564 2069 6e20  is described in 
+00000a30: 7468 6520 7061 7065 722e 2050 6c65 6173  the paper. Pleas
+00000a40: 6520 7365 6520 7468 6520 5b44 6966 6665  e see the [Diffe
+00000a50: 7265 6e63 6573 2066 726f 6d20 7468 6520  rences from the 
+00000a60: 5061 7065 725d 2823 e284 b9ef b88f 2d64  Paper](#......-d
+00000a70: 6966 6665 7265 6e63 6573 2d66 726f 6d2d  ifferences-from-
+00000a80: 7468 652d 7061 7065 7229 2073 6563 7469  the-paper) secti
+00000a90: 6f6e 2062 656c 6f77 2e0a 0a23 2320 f09f  on below...## ..
+00000aa0: 8eaf 2043 6f72 6520 4665 6174 7572 6573  .. Core Features
+00000ab0: 0a0a 2d20 f09f 92be 202a 2a44 6174 612d  ..- .... **Data-
+00000ac0: 6472 6976 656e 2a2a 2e20 4375 7374 6f6d  driven**. Custom
+00000ad0: 697a 6520 7468 6520 7369 6d75 6c61 7469  ize the simulati
+00000ae0: 6f6e 2066 6f72 2064 6966 6665 7265 6e74  on for different
+00000af0: 206e 6172 7261 7469 7665 2073 6574 7469   narrative setti
+00000b00: 6e67 730a 2d20 f09f a496 202a 2a41 6765  ngs.- .... **Age
+00000b10: 6e74 2d62 6173 6564 2a2a 2e20 5365 7474  nt-based**. Sett
+00000b20: 6c65 6d65 6e74 2061 6e64 2063 6861 7261  lement and chara
+00000b30: 6374 6572 2068 6973 746f 7269 6573 2061  cter histories a
+00000b40: 7265 2067 656e 6572 6174 6564 2062 6f74  re generated bot
+00000b50: 746f 6d2d 7570 2066 726f 6d20 6368 6172  tom-up from char
+00000b60: 6163 7465 7220 6265 6861 7669 6f72 2e0a  acter behavior..
+00000b70: 2d20 f09f 93a6 202a 2a45 6e74 6974 792d  - .... **Entity-
+00000b80: 436f 6d70 6f6e 656e 7420 5379 7374 656d  Component System
+00000b90: 2a2a 2e20 4167 656e 7473 2061 7265 2063  **. Agents are c
+00000ba0: 6f6d 706f 7365 6420 6f66 206d 6f64 756c  omposed of modul
+00000bb0: 6172 2063 6f6d 706f 6e65 6e74 732e 0a2d  ar components..-
+00000bc0: 20f0 9f91 9420 2a2a 5374 6174 2026 2053   .... **Stat & S
+00000bd0: 6b69 6c6c 2053 7973 7465 6d73 2a2a 2e20  kill Systems**. 
+00000be0: 5472 6163 6b20 6368 6172 6163 7465 7220  Track character 
+00000bf0: 7072 6f66 6963 6965 6e63 6965 7320 616e  proficiencies an
+00000c00: 6420 5250 472d 6c69 6b65 2073 7461 7473  d RPG-like stats
+00000c10: 2e0a 2d20 efb8 8ff0 9f8f b7ef b88f 202a  ..- .......... *
+00000c20: 2a54 7261 6974 2053 7973 7465 6d2a 2a2e  *Trait System**.
+00000c30: 2054 6167 2047 616d 654f 626a 6563 7473   Tag GameObjects
+00000c40: 2077 6974 6820 7472 6169 7473 2074 6861   with traits tha
+00000c50: 7420 6d6f 6469 6679 2074 6865 6972 2073  t modify their s
+00000c60: 7461 7473 2061 6e64 2072 656c 6174 696f  tats and relatio
+00000c70: 6e73 6869 7073 2e0a 2d20 e29d a4ef b88f  nships..- ......
+00000c80: 202a 2a52 656c 6174 696f 6e73 6869 7020   **Relationship 
+00000c90: 5379 7374 656d 2a2a 2e20 4368 6172 6163  System**. Charac
+00000ca0: 7465 7273 2063 756c 7469 7661 7465 2072  ters cultivate r
+00000cb0: 656c 6174 696f 6e73 6869 7073 2062 6173  elationships bas
+00000cc0: 6564 206f 6e20 726f 6d61 6e63 6520 616e  ed on romance an
+00000cd0: 6420 7265 7075 7461 7469 6f6e 2e0a 2d20  d reputation..- 
+00000ce0: f09f 92a5 202a 2a41 6374 696f 6e20 2620  .... **Action & 
+00000cf0: 4576 656e 7420 5379 7374 656d 2a2a 2e20  Event System**. 
+00000d00: 4167 656e 7473 2074 616b 6520 6163 7469  Agents take acti
+00000d10: 6f6e 7320 7468 6174 2062 7569 6c64 2075  ons that build u
+00000d20: 7020 6869 7374 6f72 6965 7320 6f66 206c  p histories of l
+00000d30: 6966 6520 6576 656e 7473 2e0a 2d20 e29a  ife events..- ..
+00000d40: 96ef b88f 202a 2a42 656c 6965 6620 5379  .... **Belief Sy
+00000d50: 7374 656d 2a2a 2e20 4368 6172 6163 7465  stem**. Characte
+00000d60: 7227 7320 6265 6c69 6566 7320 696e 666c  r's beliefs infl
+00000d70: 7565 6e63 6520 686f 7720 7468 6579 2066  uence how they f
+00000d80: 6565 6c20 6162 6f75 7420 6f74 6865 7273  eel about others
+00000d90: 2e0a 2d20 f09f 8fac 202a 2a4c 6f63 6174  ..- .... **Locat
+00000da0: 696f 6e20 5072 6566 6572 656e 6365 2053  ion Preference S
+00000db0: 7973 7465 6d2a 2a2e 204d 6f64 656c 2077  ystem**. Model w
+00000dc0: 6861 7420 6c6f 6361 7469 6f6e 7320 6120  hat locations a 
+00000dd0: 6368 6172 6163 7465 7220 6d69 6768 7420  character might 
+00000de0: 6672 6571 7565 6e74 2067 6976 656e 2074  frequent given t
+00000df0: 6865 6972 2074 7261 6974 732e 0a2d 20f0  heir traits..- .
+00000e00: 9f93 8820 2a2a 5265 6164 7920 666f 7220  ... **Ready for 
+00000e10: 6461 7461 2073 6369 656e 6365 2a2a 2e20  data science**. 
+00000e20: 4578 7472 6163 7420 616e 6420 616e 616c  Extract and anal
+00000e30: 797a 6520 6461 7461 2077 6974 6820 5b50  yze data with [P
+00000e40: 616e 6461 735d 2868 7474 7073 3a2f 2f70  andas](https://p
+00000e50: 616e 6461 732e 7079 6461 7461 2e6f 7267  andas.pydata.org
+00000e60: 2f29 2e0a 0a23 2320 f09f 9a80 2048 6f77  /)...## .... How
+00000e70: 2074 6f20 496e 7374 616c 6c0a 0a54 6865   to Install..The
+00000e80: 206c 6174 6573 7420 6f66 6669 6369 616c   latest official
+00000e90: 2072 656c 6561 7365 206f 6620 4e65 6967   release of Neig
+00000ea0: 6862 6f72 6c79 2069 7320 6176 6169 6c61  hborly is availa
+00000eb0: 626c 6520 746f 2069 6e73 7461 6c6c 2066  ble to install f
+00000ec0: 726f 6d20 5b50 7950 495d 2868 7474 7073  rom [PyPI](https
+00000ed0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000ee0: 6563 742f 6e65 6967 6862 6f72 6c79 2f29  ect/neighborly/)
+00000ef0: 2e0a 0a60 6060 6261 7368 0a70 6970 2069  ...```bash.pip i
+00000f00: 6e73 7461 6c6c 206e 6569 6768 626f 726c  nstall neighborl
+00000f10: 790a 6060 600a 0a23 2323 2054 7279 204e  y.```..### Try N
+00000f20: 6569 6768 626f 726c 7920 5769 7468 6f75  eighborly Withou
+00000f30: 7420 496e 7374 616c 6c69 6e67 0a0a 4e65  t Installing..Ne
+00000f40: 6967 6862 6f72 6c79 2069 7320 6176 6169  ighborly is avai
+00000f50: 6c61 626c 6520 746f 2075 7365 2077 6974  lable to use wit
+00000f60: 6869 6e20 7468 6973 205b 7361 6d70 6c65  hin this [sample
+00000f70: 2047 6f6f 676c 6520 436f 6c61 6220 6e6f   Google Colab no
+00000f80: 7465 626f 6f6b 5d28 6874 7470 733a 2f2f  tebook](https://
+00000f90: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
+00000fa0: 6f6f 676c 652e 636f 6d2f 6472 6976 652f  oogle.com/drive/
+00000fb0: 3157 785a 6e43 5238 6166 656b 6642 6c2d  1WxZnCR8afekfBl-
+00000fc0: 7649 3657 6349 6353 364f 6852 4764 6b61  vI6WcIcS6OhRGdka
+00000fd0: 6d3f 7573 703d 7368 6172 696e 6729 2e20  m?usp=sharing). 
+00000fe0: 4974 2063 6f6e 7461 696e 7320 6120 6261  It contains a ba
+00000ff0: 7369 6320 7761 6c6b 7468 726f 7567 6820  sic walkthrough 
+00001000: 6f66 2068 6f77 2074 6f20 6465 6669 6e65  of how to define
+00001010: 2063 6f6e 7465 6e74 2066 6f72 2074 6865   content for the
+00001020: 2073 696d 756c 6174 696f 6e20 616e 6420   simulation and 
+00001030: 696e 7370 6563 7420 7468 6520 6765 6e65  inspect the gene
+00001040: 7261 7465 6420 6461 7461 2e0a 0a23 2323  rated data...###
+00001050: 2049 6e73 7461 6c6c 696e 6720 666f 7220   Installing for 
+00001060: 4c6f 6361 6c20 4465 7665 6c6f 706d 656e  Local Developmen
+00001070: 740a 0a54 6f20 646f 776e 6c6f 6164 2061  t..To download a
+00001080: 204e 6569 6768 626f 726c 7920 666f 7220   Neighborly for 
+00001090: 6c6f 6361 6c20 6465 7665 6c6f 706d 656e  local developmen
+000010a0: 7420 6f72 2070 6c61 7920 6172 6f75 6e64  t or play around
+000010b0: 2077 6974 6820 616e 7920 6f66 2074 6865   with any of the
+000010c0: 2073 616d 706c 6573 2c20 796f 7520 6e65   samples, you ne
+000010d0: 6564 2074 6f20 636c 6f6e 6520 6f72 2064  ed to clone or d
+000010e0: 6f77 6e6c 6f61 6420 7468 6973 2072 6570  ownload this rep
+000010f0: 6f73 6974 6f72 7920 616e 6420 696e 7374  ository and inst
+00001100: 616c 6c20 6974 2075 7369 6e67 2074 6865  all it using the
+00001110: 205f 6564 6974 6162 6c65 5f20 666c 6167   _editable_ flag
+00001120: 2028 2d65 292e 2050 6c65 6173 6520 7365   (-e). Please se
+00001130: 6520 7468 6520 696e 7374 7275 6374 696f  e the instructio
+00001140: 6e73 2062 656c 6f77 2e20 5468 6973 2063  ns below. This c
+00001150: 6f6d 6d61 6e64 2077 696c 6c20 696e 7374  ommand will inst
+00001160: 616c 6c20 6120 4e65 6967 6862 6f72 6c79  all a Neighborly
+00001170: 2069 6e74 6f20 7468 6520 7669 7274 7561   into the virtua
+00001180: 6c20 656e 7669 726f 6e6d 656e 7420 616c  l environment al
+00001190: 6f6e 6720 7769 7468 2061 6c6c 2069 7473  ong with all its
+000011a0: 2064 6570 656e 6465 6e63 6965 7320 616e   dependencies an
+000011b0: 6420 6120 6665 7720 6164 6469 7469 6f6e  d a few addition
+000011c0: 616c 2064 6576 656c 6f70 6d65 6e74 2061  al development a
+000011d0: 6e64 2074 6573 7469 6e67 2064 6570 656e  nd testing depen
+000011e0: 6465 6e63 6965 7320 7375 6368 2061 7320  dencies such as 
+000011f0: 5f62 6c61 636b 5f2c 205f 6973 6f72 745f  _black_, _isort_
+00001200: 2c20 616e 6420 5f70 7974 6573 745f 2e0a  , and _pytest_..
+00001210: 0a60 6060 6261 7368 0a23 2053 7465 7020  .```bash.# Step 
+00001220: 313a 2043 6c6f 6e65 2052 6570 6f73 6974  1: Clone Reposit
+00001230: 6f72 7920 616e 6420 6368 616e 6765 2069  ory and change i
+00001240: 6e74 6f20 7072 6f6a 6563 7420 6469 7265  nto project dire
+00001250: 6374 6f72 790a 6769 7420 636c 6f6e 6520  ctory.git clone 
+00001260: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001270: 6f6d 2f53 6869 4a62 6579 2f6e 6569 6768  om/ShiJbey/neigh
+00001280: 626f 726c 792e 6769 740a 6364 206e 6569  borly.git.cd nei
+00001290: 6768 626f 726c 790a 0a23 2053 7465 7020  ghborly..# Step 
+000012a0: 3220 284d 6163 4f53 2f4c 696e 7578 293a  2 (MacOS/Linux):
+000012b0: 2043 7265 6174 6520 616e 6420 6163 7469   Create and acti
+000012c0: 7661 7465 2061 2050 7974 686f 6e20 7669  vate a Python vi
+000012d0: 7274 7561 6c20 656e 7669 726f 6e6d 656e  rtual environmen
+000012e0: 740a 7079 7468 6f6e 3320 2d6d 2076 656e  t.python3 -m ven
+000012f0: 7620 7665 6e76 0a73 6f75 7263 6520 2e2f  v venv.source ./
+00001300: 7665 6e76 2f62 696e 2f61 6374 6976 6174  venv/bin/activat
+00001310: 650a 0a23 2053 7465 7020 3220 2857 696e  e..# Step 2 (Win
+00001320: 646f 7773 293a 2043 7265 6174 6520 616e  dows): Create an
+00001330: 6420 6163 7469 7661 7465 2061 2050 7974  d activate a Pyt
+00001340: 686f 6e20 7669 7274 7561 6c20 656e 7669  hon virtual envi
+00001350: 726f 6e6d 656e 740a 7079 7468 6f6e 202d  ronment.python -
+00001360: 6d20 7665 6e76 2076 656e 760a 2e5c 7665  m venv venv..\ve
+00001370: 6e76 5c53 6372 6970 7473 5c41 6374 6976  nv\Scripts\Activ
+00001380: 6174 650a 0a23 2053 7465 7020 333a 2049  ate..# Step 3: I
+00001390: 6e73 7461 6c6c 206e 6569 6768 626f 726c  nstall neighborl
+000013a0: 7920 616e 6420 6465 7065 6e64 656e 6369  y and dependenci
+000013b0: 6573 0a70 7974 686f 6e20 2d6d 2070 6970  es.python -m pip
+000013c0: 2069 6e73 7461 6c6c 202d 6520 222e 5b64   install -e ".[d
+000013d0: 6576 656c 6f70 6d65 6e74 5d22 0a60 6060  evelopment]".```
+000013e0: 0a0a 2323 20f0 9f8d aa20 5275 6e6e 696e  ..## .... Runnin
+000013f0: 6720 7468 6520 5361 6d70 6c65 730a 0a45  g the Samples..E
+00001400: 7861 6d70 6c65 2073 696d 756c 6174 696f  xample simulatio
+00001410: 6e73 2063 616e 2062 6520 666f 756e 6420  ns can be found 
+00001420: 696e 2074 6865 2060 7361 6d70 6c65 7360  in the `samples`
+00001430: 2064 6972 6563 746f 7279 2e20 5468 656e   directory. Then
+00001440: 2074 6865 2063 6f6d 6d61 6e64 7320 6265   the commands be
+00001450: 6c6f 7720 7769 6c6c 2067 6574 2079 6f75  low will get you
+00001460: 2073 7461 7274 6564 2077 6974 6820 7275   started with ru
+00001470: 6e6e 696e 6720 7468 6520 7361 6d70 6c65  nning the sample
+00001480: 2073 696d 756c 6174 696f 6e73 2e0a 0a60   simulations...`
+00001490: 6060 6261 7368 0a23 2053 7465 7020 313a  ``bash.# Step 1:
+000014a0: 2049 6e73 7461 6c6c 206e 6569 6768 626f   Install neighbo
+000014b0: 726c 7920 6c6f 6361 6c6c 7920 616e 6420  rly locally and 
+000014c0: 616c 6c20 7468 6520 6465 7065 6e64 656e  all the dependen
+000014d0: 6369 6573 206e 6565 6465 6420 746f 2072  cies needed to r
+000014e0: 756e 2074 6865 2073 616d 706c 6520 636f  un the sample co
+000014f0: 6e74 656e 742e 0a70 7974 686f 6e20 2d6d  ntent..python -m
+00001500: 2070 6970 2069 6e73 7461 6c6c 2022 2e22   pip install "."
+00001510: 0a0a 2320 5374 6570 2032 3a20 5275 6e20  ..# Step 2: Run 
+00001520: 6120 7361 6d70 6c65 2073 6372 6970 740a  a sample script.
+00001530: 7079 7468 6f6e 202e 2f73 616d 706c 6573  python ./samples
+00001540: 2f4e 414d 455f 4f46 5f53 414d 504c 455f  /NAME_OF_SAMPLE_
+00001550: 4649 4c45 2e70 790a 6060 600a 0a23 2320  FILE.py.```..## 
+00001560: f09f a7aa 2052 756e 6e69 6e67 2074 6865  .... Running the
+00001570: 2054 6573 7473 0a0a 4e65 6967 6862 6f72   Tests..Neighbor
+00001580: 6c79 2075 7365 7320 5b50 7954 6573 745d  ly uses [PyTest]
+00001590: 2868 7474 7073 3a2f 2f64 6f63 732e 7079  (https://docs.py
+000015a0: 7465 7374 2e6f 7267 2f29 2066 6f72 2075  test.org/) for u
+000015b0: 6e69 7420 7465 7374 696e 672e 2041 6c6c  nit testing. All
+000015c0: 2074 6573 7473 2061 7265 206c 6f63 6174   tests are locat
+000015d0: 6564 2069 6e20 7468 6520 6074 6573 7473  ed in the `tests
+000015e0: 2f60 2064 6972 6563 746f 7279 2e0a 0a60  /` directory...`
+000015f0: 6060 6261 7368 0a23 2053 7465 7020 313a  ``bash.# Step 1:
+00001600: 2049 6e73 7461 6c6c 2061 6464 6974 696f   Install additio
+00001610: 6e61 6c20 6465 7065 6e64 656e 6369 6573  nal dependencies
+00001620: 2066 6f72 2074 6573 7469 6e67 2061 6e64   for testing and
+00001630: 2064 6576 656c 6f70 6d65 6e74 0a70 7974   development.pyt
+00001640: 686f 6e20 2d6d 2070 6970 2069 6e73 7461  hon -m pip insta
+00001650: 6c6c 202d 6520 222e 5b64 6576 656c 6f70  ll -e ".[develop
+00001660: 6d65 6e74 5d22 0a0a 2320 5374 6570 2032  ment]"..# Step 2
+00001670: 3a20 5275 6e20 5079 7465 7374 0a70 7974  : Run Pytest.pyt
+00001680: 6573 740a 0a23 2053 7465 7020 333a 2028  est..# Step 3: (
+00001690: 4f70 7469 6f6e 616c 2920 4765 6e65 7261  Optional) Genera
+000016a0: 7465 2061 2074 6573 7420 636f 7665 7261  te a test covera
+000016b0: 6765 2072 6570 6f72 740a 7079 7465 7374  ge report.pytest
+000016c0: 202d 2d63 6f76 3d6e 6569 6768 626f 726c   --cov=neighborl
+000016d0: 7920 7465 7374 732f 0a60 6060 0a0a 2323  y tests/.```..##
+000016e0: 20f0 9f93 9a20 446f 6375 6d65 6e74 6174   .... Documentat
+000016f0: 696f 6e0a 0a4e 6569 6768 626f 726c 7927  ion..Neighborly'
+00001700: 7320 646f 6375 6d65 6e74 6174 696f 6e20  s documentation 
+00001710: 6361 6e20 6265 2066 6f75 6e64 2061 7420  can be found at 
+00001720: 5b52 6561 6420 7468 6520 446f 6373 5d28  [Read the Docs](
+00001730: 6874 7470 733a 2f2f 6e65 6967 6862 6f72  https://neighbor
+00001740: 6c79 2e72 6561 6474 6865 646f 6373 2e69  ly.readthedocs.i
+00001750: 6f2f 656e 2f6c 6174 6573 742f 696e 6465  o/en/latest/inde
+00001760: 782e 6874 6d6c 292e 0a0a 2323 20f0 9fa4  x.html)...## ...
+00001770: 9d20 436f 6e74 7269 6275 7469 6e67 0a0a  . Contributing..
+00001780: 436f 6e74 7269 6275 7469 6f6e 7320 6172  Contributions ar
+00001790: 6520 7765 6c63 6f6d 652e 2050 6c65 6173  e welcome. Pleas
+000017a0: 6520 7265 6665 7220 746f 205b 434f 4e54  e refer to [CONT
+000017b0: 5249 4255 5449 4e47 2e6d 645d 282e 2f43  RIBUTING.md](./C
+000017c0: 4f4e 5452 4942 5554 494e 472e 6d64 2920  ONTRIBUTING.md) 
+000017d0: 666f 7220 6d6f 7265 2069 6e66 6f72 6d61  for more informa
+000017e0: 7469 6f6e 2061 626f 7574 2068 6f77 2074  tion about how t
+000017f0: 6f20 6765 7420 696e 766f 6c76 6564 2e0a  o get involved..
+00001800: 0a23 2320 f09f 9384 204c 6963 656e 7365  .## .... License
+00001810: 0a0a 5468 6973 2070 726f 6a65 6374 2069  ..This project i
+00001820: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
+00001830: 2074 6865 205b 4d49 5420 4c69 6365 6e73   the [MIT Licens
+00001840: 655d 282e 2f4c 4943 454e 5345 292e 0a0a  e](./LICENSE)...
+00001850: 2323 20e2 84b9 efb8 8f20 4469 6666 6572  ## ...... Differ
+00001860: 656e 6365 7320 6672 6f6d 2074 6865 2050  ences from the P
+00001870: 6170 6572 0a0a 2d20 2a2a 4469 7265 6374  aper..- **Direct
+00001880: 6564 2072 656c 6174 696f 6e73 6869 7073  ed relationships
+00001890: 206f 6e6c 792a 2a20 2d20 204e 6569 6768   only** -  Neigh
+000018a0: 626f 726c 7920 6f6e 6c79 2073 7570 706f  borly only suppo
+000018b0: 7274 7320 6469 7265 6374 6564 2072 656c  rts directed rel
+000018c0: 6174 696f 6e73 6869 7073 2074 6861 7420  ationships that 
+000018d0: 7472 6163 6b20 686f 7720 6f6e 6520 6368  track how one ch
+000018e0: 6172 6163 7465 7220 6665 656c 7320 6162  aracter feels ab
+000018f0: 6f75 7420 616e 6f74 6865 722e 2053 7570  out another. Sup
+00001900: 706f 7274 2066 6f72 2072 6563 6970 726f  port for recipro
+00001910: 6361 6c20 7265 6c61 7469 6f6e 7368 6970  cal relationship
+00001920: 7320 7761 7320 7265 6d6f 7665 6420 6265  s was removed be
+00001930: 6361 7573 6520 6974 2063 6f6d 706c 6963  cause it complic
+00001940: 6174 6564 2074 6865 2073 696d 756c 6174  ated the simulat
+00001950: 696f 6e20 6279 2066 6f72 6369 6e67 2075  ion by forcing u
+00001960: 7365 7273 2074 6f20 6368 6563 6b20 6d75  sers to check mu
+00001970: 6c74 6970 6c65 206c 6f63 6174 696f 6e73  ltiple locations
+00001980: 2066 6f72 2072 656c 6174 696f 6e73 6869   for relationshi
+00001990: 7020 6461 7461 2e0a 2d20 2a2a 4e6f 2061  p data..- **No a
+000019a0: 6374 6976 6974 792f 7365 7276 6963 6520  ctivity/service 
+000019b0: 7379 7374 656d 2a2a 202d 2054 6865 2061  system** - The a
+000019c0: 6374 6976 6974 7920 7379 7374 656d 2077  ctivity system w
+000019d0: 6173 2069 6e74 726f 6475 6365 6420 746f  as introduced to
+000019e0: 2068 656c 7020 6368 6172 6163 7465 7273   help characters
+000019f0: 2064 6563 6964 6520 7768 6572 6520 746f   decide where to
+00001a00: 2066 7265 7175 656e 7420 6f75 7473 6964   frequent outsid
+00001a10: 6520 6f66 2077 6f72 6b2f 686f 6d65 2e20  e of work/home. 
+00001a20: 5468 6973 2073 7973 7465 6d20 7761 7320  This system was 
+00001a30: 7265 706c 6163 6564 2077 6974 6820 5f6c  replaced with _l
+00001a40: 6f63 6174 696f 6e20 7072 6566 6572 656e  ocation preferen
+00001a50: 6365 735f 2c20 7768 6963 6820 6172 6520  ces_, which are 
+00001a60: 6d6f 7265 2066 6c65 7869 626c 652e 2054  more flexible. T
+00001a70: 6865 2061 6374 6976 6974 7920 7379 7374  he activity syst
+00001a80: 656d 2063 616e 2062 6520 656d 756c 6174  em can be emulat
+00001a90: 6564 2062 7920 6173 736f 6369 6174 696e  ed by associatin
+00001aa0: 6720 6365 7274 6169 6e20 7472 6169 7473  g certain traits
+00001ab0: 2077 6974 6820 6c6f 6361 7469 6f6e 732e   with locations.
+00001ac0: 0a2d 202a 2a4e 6f20 372d 6461 7920 7765  .- **No 7-day we
+00001ad0: 656b 6c79 2072 6f75 7469 6e65 732a 2a20  ekly routines** 
+00001ae0: 2d20 526f 7574 696e 6573 2077 6572 6520  - Routines were 
+00001af0: 7465 6469 6f75 7320 746f 2063 7265 6174  tedious to creat
+00001b00: 6520 616e 6420 6265 6361 6d65 2069 7272  e and became irr
+00001b10: 656c 6576 616e 7420 7768 656e 204e 6569  elevant when Nei
+00001b20: 6768 626f 726c 7927 7320 7469 6d65 2073  ghborly's time s
+00001b30: 7465 7020 7363 616c 6520 6368 616e 6765  tep scale change
+00001b40: 6420 6672 6f6d 2069 6e63 7265 6d65 6e74  d from increment
+00001b50: 696e 6720 7468 6520 6461 7465 2062 7920  ing the date by 
+00001b60: 6120 6665 7720 686f 7572 7320 746f 2069  a few hours to i
+00001b70: 6e63 7265 6d65 6e74 696e 6720 6279 2061  ncrementing by a
+00001b80: 2073 696e 676c 6520 6d6f 6e74 682e 0a2d   single month..-
+00001b90: 202a 2a4e 6f20 6469 7265 6374 2073 7570   **No direct sup
+00001ba0: 706f 7274 2066 6f72 2064 6966 6665 7269  port for differi
+00001bb0: 6e67 2041 4920 7374 7261 7465 6769 6573  ng AI strategies
+00001bc0: 2a2a 202d 2057 6520 696e 7465 6e64 6564  ** - We intended
+00001bd0: 2074 6f20 7375 7070 6f72 7420 7661 7269   to support vari
+00001be0: 6f75 7320 6368 6172 6163 7465 7220 6465  ous character de
+00001bf0: 6369 7369 6f6e 2d6d 616b 696e 6720 616c  cision-making al
+00001c00: 676f 7269 7468 6d73 2062 7574 206d 6164  gorithms but mad
+00001c10: 6520 6265 6861 7669 6f72 2061 7574 686f  e behavior autho
+00001c20: 7269 6e67 2074 6f6f 2074 6564 696f 7573  ring too tedious
+00001c30: 2061 6e64 2074 6f6f 6b20 656d 7068 6173   and took emphas
+00001c40: 6973 2061 7761 7920 6672 6f6d 2074 6865  is away from the
+00001c50: 2063 6f6e 7465 6e74 2061 7574 686f 7269   content authori
+00001c60: 6e67 2061 6e64 2064 6174 6120 6765 6e65  ng and data gene
+00001c70: 7261 7469 6f6e 2061 7370 6563 7473 206f  ration aspects o
+00001c80: 6620 4e65 6967 6862 6f72 6c79 2e0a 2d20  f Neighborly..- 
+00001c90: 2a2a 4576 656e 7420 7379 7374 656d 2072  **Event system r
+00001ca0: 6570 6c61 6365 6420 7769 7468 2061 6374  eplaced with act
+00001cb0: 696f 6e20 6f62 6a65 6374 7320 616e 6420  ion objects and 
+00001cc0: 7574 696c 6974 7920 7363 6f72 6573 2a2a  utility scores**
+00001cd0: 202d 2053 696e 6365 204e 6569 6768 626f   - Since Neighbo
+00001ce0: 726c 7920 646f 6573 206e 6f74 206e 6565  rly does not nee
+00001cf0: 6420 746f 2073 7570 706f 7274 2075 7365  d to support use
+00001d00: 722d 7375 7070 6c69 6564 2063 6861 7261  r-supplied chara
+00001d10: 6374 6572 2064 6563 6973 696f 6e2d 6d61  cter decision-ma
+00001d20: 6b69 6e67 206c 6f67 6963 2c20 6974 206d  king logic, it m
+00001d30: 6164 6520 6265 6861 7669 6f72 206d 6f64  ade behavior mod
+00001d40: 656c 696e 6720 6d75 6368 2073 696d 706c  eling much simpl
+00001d50: 6572 2e20 5468 6520 6f6c 6420 6c69 6665  er. The old life
+00001d60: 2065 7665 6e74 2073 7973 7465 6d20 7265   event system re
+00001d70: 7175 6972 6564 2075 7365 7273 2074 6f20  quired users to 
+00001d80: 7370 6563 6966 7920 6576 656e 7420 6566  specify event ef
+00001d90: 6665 6374 7320 666f 7220 6561 6368 2064  fects for each d
+00001da0: 6966 6665 7265 6e74 2074 7970 6520 6f66  ifferent type of
+00001db0: 2061 6765 6e74 2c20 616e 6420 7468 6973   agent, and this
+00001dc0: 206e 6174 7572 616c 6c79 2063 6f6d 706c   naturally compl
+00001dd0: 6963 6174 6564 2074 6869 6e67 732e 2043  icated things. C
+00001de0: 7572 7265 6e74 6c79 2c20 6167 656e 7420  urrently, agent 
+00001df0: 6265 6861 7669 6f72 2069 7320 696d 706c  behavior is impl
+00001e00: 656d 656e 7465 6420 7573 696e 6720 6120  emented using a 
+00001e10: 636f 6d62 696e 6174 696f 6e20 6f66 2053  combination of S
+00001e20: 7973 7465 6d73 2c20 6163 7469 6f6e 732c  ystems, actions,
+00001e30: 2061 6e64 206c 6966 6520 6576 656e 7473   and life events
+00001e40: 2e0a 2d20 2a2a 4e6f 2062 6568 6176 696f  ..- **No behavio
+00001e50: 7220 7472 6565 732a 2a20 2d20 4265 6861  r trees** - Beha
+00001e60: 7669 6f72 2074 7265 6573 2061 6464 6564  vior trees added
+00001e70: 2063 6f6d 706c 6578 6974 7920 746f 2074   complexity to t
+00001e80: 6865 2073 7973 7465 6d2e 2049 7420 7761  he system. It wa
+00001e90: 7320 7265 6d6f 7665 6420 746f 2073 696d  s removed to sim
+00001ea0: 706c 6966 7920 7468 696e 6773 2e0a 2d20  plify things..- 
+00001eb0: 2a2a 4e6f 2063 6861 7261 6374 6572 2076  **No character v
+00001ec0: 616c 7565 732a 2a20 2d20 4f76 6572 2074  alues** - Over t
+00001ed0: 696d 652c 2074 6865 2063 6861 7261 6374  ime, the charact
+00001ee0: 6572 2076 616c 7565 2073 7973 7465 6d20  er value system 
+00001ef0: 616e 6420 7065 7273 6f6e 616c 6974 7920  and personality 
+00001f00: 6d6f 6465 6c73 2077 6572 6520 636f 6d62  models were comb
+00001f10: 696e 6564 2069 6e74 6f20 6120 7369 6e67  ined into a sing
+00001f20: 6c65 2073 7461 7420 7379 7374 656d 2e20  le stat system. 
+00001f30: 5265 6d6f 7669 6e67 2074 6865 6d20 7369  Removing them si
+00001f40: 6d70 6c69 6669 6564 206d 7563 6820 6f66  mplified much of
+00001f50: 2074 6865 2061 6765 6e74 206d 6f64 656c   the agent model
+00001f60: 696e 6720 616e 6420 616c 6c6f 7765 6420  ing and allowed 
+00001f70: 666f 7220 7468 6520 6d6f 7374 2066 6c65  for the most fle
+00001f80: 7869 6269 6c69 7479 2e0a 2d20 2a2a 4e6f  xibility..- **No
+00001f90: 2063 6861 7261 6374 6572 206d 6f76 656d   character movem
+00001fa0: 656e 742a 2a20 2d20 4368 6172 6163 7465  ent** - Characte
+00001fb0: 7273 2064 6f20 6e6f 7420 6d6f 7665 2062  rs do not move b
+00001fc0: 6574 7765 656e 206c 6f63 6174 696f 6e73  etween locations
+00001fd0: 2e20 5468 6973 2061 6464 6564 2061 6464  . This added add
+00001fe0: 6974 696f 6e61 6c20 7072 6f63 6573 7369  itional processi
+00001ff0: 6e67 206f 7665 7268 6561 6420 616e 6420  ng overhead and 
+00002000: 6265 6361 6d65 2075 6e6e 6563 6573 7361  became unnecessa
+00002010: 7279 2077 6865 6e20 6d6f 7669 6e67 2074  ry when moving t
+00002020: 6f20 6120 6f6e 652d 6d6f 6e74 6820 7469  o a one-month ti
+00002030: 6d65 2073 7465 7073 2e0a 0a23 2320 c2a9  me steps...## ..
+00002040: efb8 8f20 444d 4341 2053 7461 7465 6d65  ... DMCA Stateme
+00002050: 6e74 0a0a 5570 6f6e 2072 6563 6569 7074  nt..Upon receipt
+00002060: 206f 6620 6120 6e6f 7469 6365 2061 6c6c   of a notice all
+00002070: 6567 696e 6720 636f 7079 7269 6768 7420  eging copyright 
+00002080: 696e 6672 696e 6765 6d65 6e74 2c20 4920  infringement, I 
+00002090: 7769 6c6c 2074 616b 6520 7768 6174 6576  will take whatev
+000020a0: 6572 2061 6374 696f 6e20 6974 2064 6565  er action it dee
+000020b0: 6d73 2061 7070 726f 7072 6961 7465 2077  ms appropriate w
+000020c0: 6974 6869 6e20 6974 7320 736f 6c65 2064  ithin its sole d
+000020d0: 6973 6372 6574 696f 6e2c 2069 6e63 6c75  iscretion, inclu
+000020e0: 6469 6e67 2072 656d 6f76 616c 206f 6620  ding removal of 
+000020f0: 7468 6520 616c 6c65 6765 646c 7920 696e  the allegedly in
+00002100: 6672 696e 6769 6e67 206d 6174 6572 6961  fringing materia
+00002110: 6c73 2e0a 0a54 6865 2072 6570 6f20 696d  ls...The repo im
+00002120: 6167 6520 6973 2073 6f6d 6574 6869 6e67  age is something
+00002130: 2066 756e 2074 6861 7420 4920 6d61 6465   fun that I made
+00002140: 2e20 4920 6c6f 7665 205f 5468 6520 5369  . I love _The Si
+00002150: 6d70 736f 6e73 5f2c 2061 6e64 2049 2063  mpsons_, and I c
+00002160: 6f75 6c64 6e27 7420 7468 696e 6b20 6f66  ouldn't think of
+00002170: 2061 6e79 6f6e 6520 6d6f 7265 206e 6569   anyone more nei
+00002180: 6768 626f 726c 7920 7468 616e 204e 6564  ghborly than Ned
+00002190: 2046 6c61 6e64 6572 732e 2049 6620 7468   Flanders. If th
+000021a0: 6520 636f 7079 7269 6768 7420 6f77 6e65  e copyright owne
+000021b0: 7220 666f 7220 5f54 6865 2053 696d 7073  r for _The Simps
+000021c0: 6f6e 735f 2077 6f75 6c64 206c 696b 6520  ons_ would like 
+000021d0: 6d65 2074 6f20 7461 6b65 2069 7420 646f  me to take it do
+000021e0: 776e 2c20 706c 6561 7365 2063 6f6e 7461  wn, please conta
+000021f0: 6374 206d 652e 2054 6865 2073 616d 6520  ct me. The same 
+00002200: 7461 6b65 646f 776e 2070 6f6c 6963 7920  takedown policy 
+00002210: 6170 706c 6965 7320 746f 2063 6f64 6520  applies to code 
+00002220: 7361 6d70 6c65 7320 696e 7370 6972 6564  samples inspired
+00002230: 2062 7920 5456 2073 686f 7773 2c20 6d6f   by TV shows, mo
+00002240: 7669 6573 2c20 616e 6420 6761 6d65 732e  vies, and games.
+00002250: 0a                                       .
```

### Comparing `neighborly-2.5.0/pyproject.toml` & `neighborly-3.0.0.dev1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neighborly"
-description = "A narrative-focused agent-based settlement simulation framework."
+description = "A character-focused settlement generator utilizing agent-based social simulation."
 authors = [{ name = "Shi Johnson-Bey", email = "shijbey@gmail.com" }]
 readme = "README.md"
 dynamic = ["version"]
 requires-python = ">=3.8"
 keywords = [
     "social simulation",
     "games",
@@ -41,29 +41,26 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Typing :: Typed",
 ]
 dependencies = [
     "esper==2.*",
     "ordered-set==4.*",
-    "tracery3==1.*",
-    "polars==0.19.*",
     "tabulate==0.9.*",
     "PyYAML==6.0.*",
     "tqdm==4.*",
     "pydantic==2.*",
+    "pandas==2.*",
 ]
 
 [project.optional-dependencies]
-samples = ["jupyterlab", "matplotlib", "ipywidgets"]
 development = [
     "isort",
     "black",
     "black[d]",
-    "black[jupyter]",
     "build",
     "pytest",
     "pytest-cov",
     "sphinx",
     "sphinx_rtd_theme",
 ]
 
@@ -71,15 +68,15 @@
 "Homepage" = "https://github.com/ShiJbey/neighborly"
 "Bug Tracker" = "https://github.com/ShiJbey/neighborly/issues"
 "Repository" = "https://github.com/ShiJBey/neighborly.git"
 "Changelog" = "https://github.com/ShiJbey/neighborly/blob/main/CHANGELOG.md"
 "Documentation" = "https://neighborly.readthedocs.io/en/latest/"
 
 [tool.setuptools.dynamic]
-version = { attr = "neighborly.__version__.VERSION" }
+version = { attr = "neighborly.__version__" }
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.black]
 line-length = 88
```

### Comparing `neighborly-2.5.0/src/neighborly/components/character.py` & `neighborly-3.0.0.dev1/src/neighborly/components/character.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Components for representing Characters.
 
 """
 
 from __future__ import annotations
 
 import enum
-from typing import Any
+from typing import Any, Optional
+
+import attrs
 
-from neighborly.components.traits import Trait
 from neighborly.datetime import SimDate
 from neighborly.ecs import Component, GameObject
 
 
 class LifeStage(enum.IntEnum):
     """An enumeration of all the various life stages aging characters pass through."""
 
@@ -26,148 +27,137 @@
     """The characters current sex."""
 
     MALE = enum.auto()
     FEMALE = enum.auto()
     NOT_SPECIFIED = enum.auto()
 
 
-class Species(Component):
+@attrs.define
+class SpeciesType:
     """Configuration information about a character's species."""
 
-    __slots__ = (
-        "adolescent_age",
-        "young_adult_age",
-        "adult_age",
-        "senior_age",
-        "lifespan",
-        "can_physically_age",
-    )
+    definition_id: str
+    """The unique ID of this species definition."""
+    name: str
+    """The name of this species."""
+    description: str
+    """A short text description."""
+    adolescent_age: int
+    """The age when this species is considered an adolescent."""
+    young_adult_age: int
+    """The age when this species is considered a young adult."""
+    adult_age: int
+    """The age when this species is considered an adult."""
+    senior_age: int
+    """The age when this species is considered a senior."""
+    lifespan: tuple[int, int]
+    """A lifespan interval for characters of this species."""
+    can_physically_age: bool
+    """Can characters of this species age."""
+    traits: list[str]
+    """IDs of traits characters of this species get at creation."""
+    adolescent_male_fertility: int
+    """Max fertility for adolescent males."""
+    young_adult_male_fertility: int
+    """Max fertility for young adult males."""
+    adult_male_fertility: int
+    """Max fertility for adult males."""
+    senior_male_fertility: int
+    """Max fertility for senior males."""
+    adolescent_female_fertility: int
+    """Max fertility for adolescent females."""
+    young_adult_female_fertility: int
+    """Max fertility for young adult females."""
+    adult_female_fertility: int
+    """Max fertility for adult females."""
+    senior_female_fertility: int
+    """Max fertility for senior females."""
+    fertility_cost_per_child: int
+    """Fertility reduction each time a character births a child."""
+
+    def get_life_stage_for_age(self, age: int) -> LifeStage:
+        """Get the life stage for a character with a given species and age."""
+
+        if age >= self.senior_age:
+            return LifeStage.SENIOR
+        elif age >= self.adult_age:
+            return LifeStage.ADULT
+        elif age >= self.young_adult_age:
+            return LifeStage.YOUNG_ADULT
+        elif age >= self.adolescent_age:
+            return LifeStage.ADOLESCENT
 
-    def __init__(
-        self,
-        adolescent_age: int,
-        young_adult_age: int,
-        adult_age: int,
-        senior_age: int,
-        lifespan: int,
-        can_physically_age: bool,
-    ) -> None:
-        super().__init__()
-        self.adolescent_age = adolescent_age
-        self.young_adult_age = young_adult_age
-        self.adult_age = adult_age
-        self.senior_age = senior_age
-        self.lifespan = lifespan
-        self.can_physically_age = can_physically_age
-
-    def to_dict(self) -> dict[str, Any]:
-        return {}
+        return LifeStage.CHILD
 
 
 class Character(Component):
     """A character within the story world."""
 
-    __slots__ = ("_first_name", "_last_name", "_sex", "_age", "_life_stage", "species")
+    __slots__ = ("first_name", "last_name", "sex", "life_stage")
 
-    _first_name: str
+    first_name: str
     """The character's first name."""
-    _last_name: str
+    last_name: str
     """The character's last name or family name."""
-    _age: float
-    """the character's current age."""
-    _sex: Sex
+    sex: Sex
     """The physical sex of the character."""
-    _life_stage: LifeStage
+    life_stage: LifeStage
     """The character's current life stage."""
-    species: GameObject
-    """The character's species"""
 
     def __init__(
-        self, first_name: str, last_name: str, sex: Sex, species: GameObject
+        self,
+        first_name: str,
+        last_name: str,
+        sex: Sex,
     ) -> None:
         super().__init__()
-        self._first_name = first_name
-        self._last_name = last_name
-        self._sex = sex
-        self._age = 0
-        self._life_stage = LifeStage.CHILD
-        self.species = species
-
-    @property
-    def first_name(self) -> str:
-        """The character's first name."""
-        return self._first_name
-
-    @first_name.setter
-    def first_name(self, value: str) -> None:
-        """Set the character's first name."""
-        self._first_name = value
-        self.gameobject.name = self.full_name
-
-    @property
-    def last_name(self) -> str:
-        """The character's last name."""
-        return self._last_name
-
-    @last_name.setter
-    def last_name(self, value: str) -> None:
-        """Set the character's last name."""
-        self._last_name = value
-        self.gameobject.name = self.full_name
+        self.first_name = first_name
+        self.last_name = last_name
+        self.sex = sex
+        self.life_stage = LifeStage.CHILD
 
     @property
     def full_name(self) -> str:
         """The combined full name of the character."""
-        return f"{self._first_name} {self._last_name}"
-
-    @property
-    def age(self) -> float:
-        """Get the character's age."""
-        return self._age
-
-    @age.setter
-    def age(self, value: float) -> None:
-        """Set the character's age."""
-        self._age = value
-
-    @property
-    def sex(self) -> Sex:
-        """Get the characters sex."""
-        return self._sex
-
-    @property
-    def life_stage(self) -> LifeStage:
-        """Get the character's life stage."""
-        return self._life_stage
-
-    @life_stage.setter
-    def life_stage(self, value: LifeStage) -> None:
-        """Set the character's life stage."""
-        self._life_stage = value
+        return f"{self.first_name} {self.last_name}"
 
     def to_dict(self) -> dict[str, Any]:
         return {
-            "first_name": self._first_name,
-            "last_name": self._last_name,
+            "first_name": self.first_name,
+            "last_name": self.last_name,
             "sex": self.sex.name,
-            "age": int(self.age),
             "life_stage": self.life_stage.name,
-            "species": self.species.get_component(Trait).definition_id,
         }
 
     def __repr__(self) -> str:
         return (
-            f"{self.__class__.__name__}(name={self.full_name}, sex={self.sex}, "
-            f"age={self.age}({self.life_stage}), species={self.species.name})"
+            f"Character(name={self.full_name!r}, sex={self.sex!r}, "
+            f"life_stage={self.life_stage!r})"
         )
 
     def __str__(self) -> str:
         return self.full_name
 
 
+class Species(Component):
+    """Tracks the species a character belongs to."""
+
+    __slots__ = ("species",)
+
+    species: SpeciesType
+    """The species the character belongs to."""
+
+    def __init__(self, species: SpeciesType) -> None:
+        super().__init__()
+        self.species = species
+
+    def to_dict(self) -> dict[str, Any]:
+        return {"species": self.species.definition_id}
+
+
 class Pregnant(Component):
     """Tags a character as pregnant and tracks relevant information."""
 
     __slots__ = "partner", "due_date"
 
     partner: GameObject
     """The GameObject ID of the character that impregnated this character."""
@@ -176,18 +166,97 @@
 
     def __init__(self, partner: GameObject, due_date: SimDate) -> None:
         super().__init__()
         self.partner = partner
         self.due_date = due_date.copy()
 
     def __str__(self) -> str:
-        return f"{type(self).__name__}(partner={self.partner.name})"
+        return f"Pregnant(partner={self.partner.name!r}, due_date={self.due_date})"
 
     def __repr__(self) -> str:
-        return f"{type(self).__name__}(partner={self.partner.name})"
+        return f"Pregnant(partner={self.partner.name!r}, due_date={self.due_date})"
 
     def to_dict(self) -> dict[str, Any]:
         return {
-            **super().to_dict(),
             "partner": self.partner.uid,
             "due_date": str(self.due_date),
         }
+
+
+class Household(Component):
+    """A collection of characters that all live together."""
+
+    __slots__ = ("head", "spouse", "members")
+
+    head: Optional[GameObject]
+    """The head of the household."""
+    spouse: Optional[GameObject]
+    """The spouse of the head of the household."""
+    members: list[GameObject]
+    """Other members of the household."""
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.head = None
+        self.spouse = None
+        self.members = []
+
+    def to_dict(self) -> dict[str, Any]:
+        return {
+            "head": self.head.uid if self.head is not None else -1,
+            "spouse": self.spouse.uid if self.spouse is not None else -1,
+            "members": [m.uid for m in self.members],
+        }
+
+
+class MemberOfHousehold(Component):
+    """Marks a GameObject as being a member of a household."""
+
+    __slots__ = ("household",)
+
+    household: GameObject
+    """The household they belong to."""
+
+    def __init__(self, household: GameObject) -> None:
+        super().__init__()
+        self.household = household
+
+    def to_dict(self) -> dict[str, Any]:
+        return {"household": self.household.uid}
+
+
+class HeadOfHousehold(Component):
+    """Marks a character as being the head of a household."""
+
+    __slots__ = ("household",)
+
+    household: GameObject
+    """The household they are the head of."""
+
+    def __init__(self, household: GameObject) -> None:
+        super().__init__()
+        self.household = household
+
+    def to_dict(self) -> dict[str, Any]:
+        return {"household": self.household.uid}
+
+
+class ResidentOf(Component):
+    """A Component attached to characters that tracks where they live."""
+
+    __slots__ = ("settlement",)
+
+    settlement: GameObject
+    """The settlement they live in."""
+
+    def __init__(self, settlement: GameObject) -> None:
+        super().__init__()
+        self.settlement = settlement
+
+    def to_dict(self) -> dict[str, Any]:
+        return {"settlement": self.settlement.uid}
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(settlement={self.settlement.name!r})"
+
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__}(settlement={self.settlement.name!r})"
```

### Comparing `neighborly-2.5.0/src/neighborly/components/location.py` & `neighborly-3.0.0.dev1/src/neighborly/components/location.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,91 +3,100 @@
 This module contains classes and functions that help characters decide where within the
 settlement they spend most of their time. Since the simulation does not model
 characters' positions throughout the settlement, this is a way of tracking who
 characters have the highest likelihood of interacting with during a time step.
 
 """
 
-from typing import Any, Iterator
+from collections import defaultdict
+from typing import Any, Iterable, Iterator
 
-import attrs
 from ordered_set import OrderedSet
 
 from neighborly.ecs import Component, GameObject
 from neighborly.preconditions.base_types import Precondition
 
 
-class FrequentedBy(Component):
+class Location(Component):
     """Tracks the characters that frequent a location."""
 
-    __slots__ = ("_characters",)
+    __slots__ = ("frequented_by", "is_private")
 
-    _characters: OrderedSet[GameObject]
+    is_private: bool
+    """Can this location be frequented by any character."""
+    frequented_by: OrderedSet[GameObject]
     """GameObject IDs of characters that frequent the location."""
 
-    def __init__(self) -> None:
+    def __init__(
+        self,
+        is_private: bool = False,
+    ) -> None:
         super().__init__()
-        self._characters = OrderedSet([])
+        self.is_private = is_private
+        self.frequented_by = OrderedSet([])
 
     def add_character(self, character: GameObject) -> None:
         """Add a character.
 
         Parameters
         ----------
         character
             The GameObject reference to a character.
         """
-        self._characters.add(character)
+        self.frequented_by.add(character)
 
     def remove_character(self, character: GameObject) -> bool:
         """Remove a character.
 
         Parameters
         ----------
         character
             The character to remove.
 
         Returns
         -------
         bool
             Returns True if a character was removed. False otherwise.
         """
-        if character in self._characters:
-            self._characters.remove(character)
+        if character in self.frequented_by:
+            self.frequented_by.remove(character)
+
             return True
 
         return False
 
     def to_dict(self) -> dict[str, Any]:
         return {
-            "characters": [entry.uid for entry in self._characters],
+            "frequented_by": [entry.uid for entry in self.frequented_by],
         }
 
     def __contains__(self, item: GameObject) -> bool:
-        return item in self._characters
+        return item in self.frequented_by
 
     def __iter__(self) -> Iterator[GameObject]:
-        return iter(self._characters)
+        return iter(self.frequented_by)
 
     def __str__(self):
         return repr(self)
 
     def __repr__(self):
-        return f"{self.__class__.__name__}({self._characters})"
+        return f"Location({self.frequented_by!r})"
 
 
 class FrequentedLocations(Component):
     """Tracks the locations that a character frequents."""
 
     __slots__ = ("_locations",)
 
     _locations: OrderedSet[GameObject]
     """A set of GameObject IDs of locations."""
 
-    def __init__(self) -> None:
+    def __init__(
+        self,
+    ) -> None:
         super().__init__()
         self._locations = OrderedSet([])
 
     def add_location(self, location: GameObject) -> None:
         """Add a new location.
 
         Parameters
@@ -108,14 +117,15 @@
         Returns
         -------
         bool
             Returns True of a location was removed. False otherwise.
         """
         if location in self._locations:
             self._locations.remove(location)
+
             return True
         return False
 
     def to_dict(self) -> dict[str, Any]:
         return {"locations": [entry.uid for entry in self._locations]}
 
     def __contains__(self, item: GameObject) -> bool:
@@ -130,100 +140,117 @@
     def __len__(self) -> int:
         return len(self._locations)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({repr(self._locations)})"
 
 
-@attrs.define
 class LocationPreferenceRule:
     """A rule that helps characters score how they feel about locations to frequent."""
 
+    __slots__ = ("rule_id", "description", "preconditions", "probability")
+
+    rule_id: str
+    """A unique ID for this rule."""
+    description: str
+    """A description of the preference."""
     preconditions: list[Precondition]
-    """Precondition functions to run when scoring a location."""
+    """Precondition to run when scoring a location."""
     probability: float
     """The amount to apply to the score."""
-    source: object
-    """The source of this location."""
 
-    def __call__(self, gameobject: GameObject) -> float:
-        """Check all preconditions and return a weight modifier.
+    def __init__(
+        self,
+        rule_id: str,
+        description: str,
+        preconditions: list[Precondition],
+        probability: float,
+    ) -> None:
+        self.rule_id = rule_id
+        self.description = description
+        self.preconditions = preconditions
+        self.probability = probability
+
+    def check_preconditions(self, character: GameObject, location: GameObject) -> bool:
+        """Check the preconditions against the given location."""
+
+        for precondition in self.preconditions:
+            if (
+                precondition.check({"location": location, "character": character})
+                is False
+            ):
+                return False
 
-        Parameters
-        ----------
-        gameobject
-            A location to score.
-
-        Returns
-        -------
-        float
-            A probability score from [0.0, 1.0] of the character frequenting the
-            location. Or -1 if it does not pass the preconditions.
-        """
-
-        if all(p(gameobject) for p in self.preconditions):
-            return self.probability
-
-        return -1.0
+        return True
 
 
 class LocationPreferences(Component):
     """A component that manages a character's location preference rules."""
 
     __slots__ = ("_rules",)
 
-    _rules: list[LocationPreferenceRule]
-    """Rules added to the location preferences."""
+    _rules: defaultdict[str, int]
+    """Rules IDs mapped to reference counts."""
 
-    def __init__(self) -> None:
+    def __init__(
+        self,
+    ) -> None:
         super().__init__()
-        self._rules = []
+        self._rules = defaultdict(lambda: 0)
 
-    def add_rule(self, rule: LocationPreferenceRule) -> None:
-        """Add a location preference rule."""
-        self._rules.append(rule)
-
-    def remove_rule(self, rule: LocationPreferenceRule) -> None:
-        """Remove a location preference rule."""
-        self._rules.remove(rule)
-
-    def remove_rules_from_source(self, source: object) -> None:
-        """Remove all preference rules from the given source."""
-        self._rules = [rule for rule in self._rules if rule.source != source]
+    @property
+    def rules(self) -> Iterable[str]:
+        """Rules applied to the owning GameObject's relationships."""
+        return self._rules
+
+    def add_rule(self, rule_id: str) -> None:
+        """Add a rule to the rule collection."""
+        self._rules[rule_id] += 1
+
+    def has_rule(self, rule_id: str) -> bool:
+        """Check if a rule is present."""
+        return rule_id in self._rules
+
+    def remove_rule(self, rule_id: str) -> bool:
+        """Remove a rule from the rules collection."""
+        if rule_id in self._rules:
+            self._rules[rule_id] -= 1
 
-    def score_location(self, location: GameObject) -> float:
-        """Calculate a score for a character choosing to frequent this location.
+            if self._rules[rule_id] <= 0:
+                del self._rules[rule_id]
 
-        Parameters
-        ----------
-        location
-            A location to score
+            return True
 
-        Returns
-        -------
-        float
-            A probability score from [0.0, 1.0]
-        """
+        return False
+
+    def to_dict(self) -> dict[str, Any]:
+        return {"rules": [r for r in self._rules]}
 
-        cumulative_score: float = 0.5
-        consideration_count: int = 1
 
-        for rule in self._rules:
-            consideration_score = rule(location)
+class CurrentSettlement(Component):
+    """Tracks the current settlement a GameObject is in."""
 
-            # Scores greater than zero are added to the cumulative score
-            if consideration_score > 0:
-                cumulative_score += consideration_score
-                consideration_count += 1
-
-            # Scores equal to zero make the entire score zero (make zero a veto value)
-            elif consideration_score == 0.0:
-                cumulative_score = 0.0
-                break
+    __slots__ = ("settlement",)
 
-        # Scores are averaged using the arithmetic mean
-        final_score = cumulative_score / consideration_count
+    settlement: GameObject
+
+    def __init__(self, settlement: GameObject) -> None:
+        super().__init__()
+        self.settlement = settlement
 
-        return final_score
+    def to_dict(self) -> dict[str, Any]:
+        return {"settlement": self.settlement.uid}
+
+
+class CurrentDistrict(Component):
+    """Tracks the current district a GameObject is in."""
+
+    __slots__ = ("district",)
+
+    district: GameObject
+
+    def __init__(self, district: GameObject) -> None:
+        super().__init__()
+        self.district = district
 
     def to_dict(self) -> dict[str, Any]:
-        return {}
+        return {"district": self.district.uid}
```

### Comparing `neighborly-2.5.0/src/neighborly/components/relationship.py` & `neighborly-3.0.0.dev1/src/neighborly/components/relationship.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,27 +4,24 @@
 Relationships are represented as independent GameObjects. Together they form a directed
 graph.
 
 """
 
 from __future__ import annotations
 
-from typing import Any, Iterable, Mapping, Optional
-
-import attrs
+from typing import Any, Mapping
 
+from neighborly.components.stats import StatComponent
 from neighborly.ecs import Component, GameObject
-from neighborly.effects.base_types import Effect
-from neighborly.preconditions.base_types import Precondition
 
 
 class Relationship(Component):
     """Tags a GameObject as a relationship and tracks the owner and target."""
 
-    __slots__ = "_target", "_owner"
+    __slots__ = "_target", "_owner", "active_rules"
 
     _owner: GameObject
     """Who owns this relationship."""
     _target: GameObject
     """Who is the relationship directed toward."""
 
     def __init__(
@@ -76,15 +73,17 @@
     )
 
     _incoming: dict[GameObject, GameObject]
     """Relationship owners mapped to the Relationship GameObjects."""
     _outgoing: dict[GameObject, GameObject]
     """Relationship targets mapped to the Relationship GameObjects."""
 
-    def __init__(self) -> None:
+    def __init__(
+        self,
+    ) -> None:
         super().__init__()
         self._incoming = {}
         self._outgoing = {}
 
     @property
     def outgoing(self) -> Mapping[GameObject, GameObject]:
         """Returns a mapping of the outgoing relationship collection."""
@@ -247,82 +246,29 @@
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(outgoing={self._outgoing}, "
             f"incoming={self._incoming})"
         )
 
 
-@attrs.define
-class SocialRule:
-    """A rule that modifies a relationship depending on some preconditions."""
-
-    preconditions: list[Precondition]
-    """Conditions that need to be met to apply the rule."""
-    effects: list[Effect]
-    """Side-effects of the rule applied to a relationship."""
-    is_outgoing: bool = True
-    """True if this rule is applied to outgoing relationships."""
-    source: Optional[object] = None
-    """The object responsible for adding this rule."""
-
-    def check_preconditions(self, relationship: GameObject) -> bool:
-        """Check that a relationship passes all the preconditions."""
-        return all(p(relationship) for p in self.preconditions)
-
-    def apply(self, relationship: GameObject) -> None:
-        """Apply the effects of the social rule.
-
-        Parameters
-        ----------
-        relationship
-            The relationship to apply the effects to.
-        """
-        for effect in self.effects:
-            effect.apply(relationship)
+class Reputation(StatComponent):
+    """Tracks a relationship's reputations stat."""
 
-    def remove(self, relationship: GameObject) -> None:
-        """Remove the effects of the social rule.
+    __stat_name__ = "reputation"
 
-        Parameters
-        ----------
-        relationship
-            The relationship to remove the effects from.
-        """
-        for effect in self.effects:
-            effect.remove(relationship)
-
-
-class SocialRules(Component):
-    """Tracks all the social rules that a GameObject abides by."""
+    def __init__(
+        self,
+        base_value: float = 0,
+    ) -> None:
+        super().__init__(base_value, (-50, 50), True)
 
-    __slots__ = ("_rules",)
 
-    _rules: list[SocialRule]
-    """Rules applied to the owning GameObject's relationships."""
+class Romance(StatComponent):
+    """Tracks a relationship's romance stat."""
 
-    def __init__(self) -> None:
-        super().__init__()
-        self._rules = []
+    __stat_name__ = "romance"
 
-    @property
-    def rules(self) -> Iterable[SocialRule]:
-        """Rules applied to the owning GameObject's relationships."""
-        return self._rules
-
-    def add_rule(self, rule: SocialRule) -> None:
-        """Add a rule to the rule collection."""
-        self._rules.append(rule)
-
-    def has_rule(self, rule: SocialRule) -> bool:
-        """Check if a rule is present."""
-        return rule in self._rules
-
-    def remove_rule(self, rule: SocialRule) -> bool:
-        """Remove a rule from the rules collection."""
-        try:
-            self._rules.remove(rule)
-            return True
-        except ValueError:
-            return False
-
-    def to_dict(self) -> dict[str, Any]:
-        return {}
+    def __init__(
+        self,
+        base_value: float = 0,
+    ) -> None:
+        super().__init__(base_value, (-50, 50), True)
```

### Comparing `neighborly-2.5.0/src/neighborly/components/stats.py` & `neighborly-3.0.0.dev1/src/neighborly/components/stats.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,24 +7,33 @@
 The code for the stat class is based on Kryzarel's tutorial on YouTube:
 https://www.youtube.com/watch?v=SH25f3cXBVc.
 
 """
 
 from __future__ import annotations
 
+import dataclasses
 import enum
 import math
 import sys
-from typing import Any, Iterator, Optional
+from abc import ABC
+from typing import Any, ClassVar, Iterable, Optional
 
 import attrs
 
 from neighborly.ecs import Component
 
 
+@dataclasses.dataclass
+class StatValueChangeEvent:
+    """An even triggered when a stats value changes."""
+
+    value: float
+
+
 class Stat:
     """A stat such as strength, reputation, or attraction.
 
     Parameters
     ----------
     base_value
         The value of the stat with no modifiers applied.
@@ -56,15 +65,15 @@
     _max_value: float
     """The maximum score the overall stat is clamped to."""
     _is_discrete: bool
     """Should the final calculated stat value be converted to an int."""
 
     def __init__(
         self,
-        base_value: float,
+        base_value: float = 0,
         bounds: Optional[tuple[float, float]] = None,
         is_discrete: bool = False,
     ) -> None:
         self._base_value = base_value
         self._value = base_value
         self._modifiers = []
         self._is_dirty = False
@@ -205,21 +214,25 @@
         """Get the normalized value from 0.0 to 1.0."""
         if self.is_bounded:
             return (self.value - self._min_value) / (self._max_value - self._min_value)
 
         raise ValueError("Cannot calculate normalized value of an unbound stat.")
 
     def __str__(self) -> str:
-        return str(self.value)
+        return (
+            f"Stat(value={self.value!r}, base={self.base_value!r}, "
+            f"max={self._max_value!r}, min={self._min_value!r}, "
+            f"modifiers={self._modifiers!r})"
+        )
 
     def __repr__(self) -> str:
         return (
-            f"{self.__class__.__name__}(value={self.value}, base={self.base_value}, "
-            f"max={self._max_value}, min={self._min_value}, "
-            f"modifiers={self._modifiers})"
+            f"Stat(value={self.value!r}, base={self.base_value!r}, "
+            f"max={self._max_value!r}, min={self._min_value!r}, "
+            f"modifiers={self._modifiers!r})"
         )
 
 
 class StatModifierType(enum.IntEnum):
     """Specifies how the value of a StatModifier is applied in stat calculation."""
 
     FLAT = 100
@@ -262,36 +275,86 @@
             "value": self.value,
             "modifier_type": self.modifier_type.name,
             "order": self.order,
             "source": str(self.source) if self.source is not None else "",
         }
 
 
+class StatComponent(Component, ABC):
+    """A component that represents a numerical stat associated with a GameObject."""
+
+    __stat_name__: ClassVar[str] = ""
+
+    __slots__ = ("stat",)
+
+    stat: Stat
+    """stat data"""
+
+    def __init__(
+        self,
+        base_value: float = 0,
+        bounds: Optional[tuple[float, float]] = None,
+        is_discrete: bool = False,
+    ) -> None:
+        super().__init__()
+
+        if not self.__stat_name__:
+            raise ValueError(
+                f"Please specify __stat_name__ class attribute for {type(self)}."
+            )
+
+        self.stat = Stat(base_value=base_value, bounds=bounds, is_discrete=is_discrete)
+
+    @property
+    def stat_name(self) -> str:
+        """The name associated with this stat."""
+        return self.__stat_name__
+
+    def on_add(self) -> None:
+        self.gameobject.get_component(Stats).add_stat(self)
+
+    def on_remove(self) -> None:
+        if stats_comp := self.gameobject.try_component(Stats):
+            stats_comp.remove_stat(self.stat_name)
+
+    def to_dict(self) -> dict[str, Any]:
+        return {"value": self.stat.value}
+
+
 class Stats(Component):
     """Tracks all the various stats for a GameObject."""
 
     __slots__ = ("_stats",)
 
-    _stats: dict[str, Stat]
-    """Map of Stat IDs to Stat instances."""
+    _stats: dict[str, StatComponent]
+    """Map of Stat IDs to Stat components."""
 
-    def __init__(self) -> None:
+    def __init__(
+        self,
+    ) -> None:
         super().__init__()
         self._stats = {}
 
-    def add_stat(self, stat_id: str, stat: Stat) -> None:
+    @property
+    def stats(self) -> Iterable[StatComponent]:
+        """Stat instances."""
+        return self._stats.values()
+
+    def add_stat(
+        self,
+        stat: StatComponent,
+    ) -> None:
         """Add a new stat.
 
         Parameters
         ----------
-        stat_id
-            A string ID to associate with the stat.
         stat
-            A stat instance.
+            A stat component instance.
         """
+        stat_id = stat.stat_name
         self._stats[stat_id] = stat
 
     def has_stat(self, stat_id: str) -> bool:
         """Check if a stat exists.
 
         Parameters
         ----------
@@ -314,33 +377,156 @@
             A string ID associated with a stat.
 
         Returns
         -------
         Stat
             The Stat instance associated with the given ID.
         """
-        return self._stats[stat_id]
+        return self._stats[stat_id].stat
 
     def remove_stat(self, stat_id: str) -> bool:
         """Remove a stat.
 
         Parameters
         ----------
         stat_id
-            A string ID associated with a stat
+            A string ID associated with a stat.
 
         Returns
         -------
         bool
-            True if the stat was removed successfully, False otherwise.
+            True is successful, False otherwise.
         """
         if stat_id in self._stats:
+
             del self._stats[stat_id]
+
             return True
 
         return False
 
-    def __iter__(self) -> Iterator[tuple[str, Stat]]:
-        return iter(self._stats.items())
-
     def to_dict(self) -> dict[str, Any]:
-        return {stat_id: stat.value for stat_id, stat in self._stats.items()}
+        return {}
+
+
+class Lifespan(StatComponent):
+    """Tracks a GameObject's lifespan."""
+
+    __stat_name__ = "lifespan"
+
+    def __init__(
+        self,
+        base_value: float = 0,
+    ) -> None:
+        super().__init__(base_value, (0, 999_999), True)
+
+
+class Fertility(StatComponent):
+    """Tracks a GameObject's fertility."""
+
+    __stat_name__ = "fertility"
+
+    MAX_VALUE: int = 100
+
+    def __init__(
+        self,
+        base_value: float = 0,
+    ) -> None:
+        super().__init__(base_value, (0, self.MAX_VALUE), True)
+
+
+class Kindness(StatComponent):
+    """Tracks a GameObject's kindness."""
+
+    __stat_name__ = "kindness"
+
+    MAX_VALUE: int = 100
+
+    def __init__(
+        self,
+        base_value: float = 0,
+    ) -> None:
+        super().__init__(base_value, (0, self.MAX_VALUE), True)
+
+
+class Courage(StatComponent):
+    """Tracks a GameObject's courage."""
+
+    __stat_name__ = "courage"
+
+    MAX_VALUE: int = 100
+
+    def __init__(
+        self,
+        base_value: float = 0,
+    ) -> None:
+        super().__init__(base_value, (0, self.MAX_VALUE), True)
+
+
+class Stewardship(StatComponent):
+    """Tracks a GameObject's stewardship."""
+
+    __stat_name__ = "stewardship"
+
+    MAX_VALUE: int = 100
+
+    def __init__(
+        self,
+        base_value: float = 0,
+    ) -> None:
+        super().__init__(base_value, (0, self.MAX_VALUE), True)
+
+
+class Sociability(StatComponent):
+    """Tracks a GameObject's sociability."""
+
+    __stat_name__ = "sociability"
+
+    MAX_VALUE: int = 100
+
+    def __init__(
+        self,
+        base_value: float = 0,
+    ) -> None:
+        super().__init__(base_value, (0, self.MAX_VALUE), True)
+
+
+class Intelligence(StatComponent):
+    """Tracks a GameObject's intelligence."""
+
+    __stat_name__ = "intelligence"
+
+    MAX_VALUE: int = 100
+
+    def __init__(
+        self,
+        base_value: float = 0,
+    ) -> None:
+        super().__init__(base_value, (0, self.MAX_VALUE), True)
+
+
+class Discipline(StatComponent):
+    """Tracks a GameObject's discipline."""
+
+    __stat_name__ = "discipline"
+
+    MAX_VALUE: int = 100
+
+    def __init__(
+        self,
+        base_value: float = 0,
+    ) -> None:
+        super().__init__(base_value, (0, self.MAX_VALUE), True)
+
+
+class Charm(StatComponent):
+    """Tracks a GameObject's charm."""
+
+    __stat_name__ = "charm"
+
+    MAX_VALUE: int = 100
+
+    def __init__(
+        self,
+        base_value: float = 0,
+    ) -> None:
+        super().__init__(base_value, (0, self.MAX_VALUE), True)
```

### Comparing `neighborly-2.5.0/src/neighborly/components/traits.py` & `neighborly-3.0.0.dev1/src/neighborly/components/traits.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,234 +2,214 @@
 
 This module contains class definitions for implementing the trait system.
 
 """
 
 from __future__ import annotations
 
-from typing import Any, Iterable
+import enum
+from typing import Any, Union
 
-from ordered_set import OrderedSet
+import attrs
 
-from neighborly.ecs import Component, GameObject
+from neighborly.datetime import SimDate
+from neighborly.ecs import Component
 from neighborly.effects.base_types import Effect
 
 
-class Trait(Component):
-    """Additional state associated with characters, businesses, and other GameObjects.
+class TraitType(enum.Enum):
+    """Enumeration of all possible trait types."""
 
-    Users can use traits as another way to make runtime-changes to character behavior
-    and component data. This class interface offers a more traditional object-oriented
-    programming way of representing traits.
-
-    This component is attached to a GameObject that represents a trait and should not
-    be added directly to a character or business.
-    """
-
-    __slots__ = (
-        "_definition_id",
-        "_description",
-        "_display_name",
-        "_effects",
-        "_conflicting_traits",
-    )
+    AGENT = enum.auto()
+    RELATIONSHIP = enum.auto()
 
-    _definition_id: str
+
+@attrs.define
+class Trait:
+    """Additional state associated with characters, businesses, and other GameObjects."""
+
+    definition_id: str
     """The ID of this tag definition."""
-    _description: str
+    description: str
     """A short description of the tag."""
-    _display_name: str
+    name: str
     """The name of this tag printed."""
-    _effects: list[Effect]
+    trait_type: TraitType
+    """The kind of GameObject the trait can attach to."""
+    effects: list[Effect]
     """Effects to apply when the tag is added."""
-    _conflicting_traits: OrderedSet[str]
+    conflicting_traits: set[str]
     """traits that this trait conflicts with."""
+    incoming_relationship_effects: list[Effect]
+    """(Agents only) Effects to incoming relationships."""
+    outgoing_relationship_effects: list[Effect]
+    """(Agents only) Effects to outgoing relationships."""
+    owner_effects: list[Effect]
+    """(Relationships only) Effects to the owner of a relationship."""
+    target_effects: list[Effect]
+    """(Relationships only) Effects to the target of a relationship."""
+    spawn_frequency: int = 0
+    """(Agents only) The relative frequency of an agent spawning with this trait."""
+    is_inheritable: bool = False
+    """(Agents only) Is the trait inheritable."""
+    inheritance_chance_single: float = 0.0
+    """(Agents only) The probability of inheriting this trait if one parent has it."""
+    inheritance_chance_both: float = 0.0
+    """(Agents only) The probability of inheriting this trait if both parents have it."""
 
-    def __init__(
-        self,
-        definition_id: str,
-        display_name: str,
-        description: str,
-        effects: list[Effect],
-        conflicting_traits: Iterable[str],
-    ) -> None:
-        super().__init__()
-        self._definition_id = definition_id
-        self._display_name = display_name
-        self._description = description
-        self._effects = effects
-        self._conflicting_traits = OrderedSet(conflicting_traits)
-
-    @property
-    def definition_id(self) -> str:
-        """The ID of this tag definition."""
-        return self._definition_id
-
-    @property
-    def display_name(self) -> str:
-        """The name of this tag printed."""
-        return self._display_name
-
-    @property
-    def description(self) -> str:
-        """A short description of the tag."""
-        return self._description
-
-    @property
-    def effects(self) -> Iterable[Effect]:
-        """The effects associated with the trait."""
-        return self._effects
-
-    @property
-    def conflicting_traits(self) -> Iterable[str]:
-        """A set of names of this trait's conflicts."""
-        return self._conflicting_traits
+    def __str__(self) -> str:
+        return self.name
 
-    def apply(self, target: GameObject) -> None:
-        """Callback method executed when the trait is added.
+    def __repr__(self) -> str:
+        return f"{type(self)}({self.definition_id})"
 
-        Parameters
-        ----------
-        target
-            The gameobject with the trait
-        """
-        for effect in self._effects:
-            effect.apply(target)
 
-    def remove(self, target: GameObject) -> None:
-        """Callback method executed when the trait is removed.
+class TraitInstance:
+    """An instance of a trait being attached to a GameObject."""
 
-        Parameters
-        ----------
-        target
-            The gameobject with the trait
-        """
-        for effect in self._effects:
-            effect.remove(target)
+    __slots__ = ("trait", "description", "duration", "has_duration", "timestamp")
+
+    trait: Trait
+    """The trait attached to the GameObject."""
+    description: str
+    """A description of the trait or why it was added."""
+    duration: int
+    """The remaining number of time steps this trait is active for."""
+    has_duration: bool
+    """Does the trait have a duration time."""
+    timestamp: SimDate
+    """When was this trait acquired."""
+
+    def __init__(
+        self, trait: Trait, timestamp: SimDate, description: str = "", duration: int = 0
+    ) -> None:
+        self.trait = trait
+        self.description = description
+        self.has_duration = duration > 0
+        self.duration = duration
+        self.timestamp = timestamp
 
     def __str__(self) -> str:
-        return self.display_name
+        return (
+            f"TraitInstance(trait={self.trait.definition_id!r}, "
+            f"duration={self.duration!r}, description={self.description!r}, "
+            f"timestamp={self.timestamp})"
+        )
 
     def __repr__(self) -> str:
-        return f"{type(self)}({self.definition_id})"
+        return (
+            f"TraitInstance(trait={self.trait.definition_id!r}, "
+            f"duration={self.duration!r}, description={self.description!r}, "
+            f"timestamp={self.timestamp})"
+        )
 
     def to_dict(self) -> dict[str, Any]:
+        """Return as serialized dict."""
         return {
-            "definition_id": self.definition_id,
-            "display_name": self.display_name,
+            "trait": self.trait.definition_id,
             "description": self.description,
-            "conflicts_with": list(self.conflicting_traits),
+            "has_duration": self.has_duration,
+            "duration": self.duration,
+            "timestamp": self.timestamp.to_iso_str(),
         }
 
 
 class Traits(Component):
     """Tracks the traits attached to a GameObject."""
 
-    __slots__ = "_traits", "_conflicting_traits"
+    __slots__ = ("traits",)
 
-    _traits: OrderedSet[GameObject]
+    traits: dict[str, TraitInstance]
     """References to traits attached to the GameObject."""
-    _conflicting_traits: set[str]
-    """IDs of all traits that conflict with the equipped traits."""
 
-    def __init__(self) -> None:
+    def __init__(
+        self,
+    ) -> None:
         super().__init__()
-        self._traits = OrderedSet([])
-        self._conflicting_traits = set()
-
-    @property
-    def traits(self) -> Iterable[GameObject]:
-        """Return an iterator for the trait collection."""
-        return self._traits
-
-    def has_trait(self, trait: GameObject) -> bool:
-        """Check if a trait is present."""
-        return trait in self._traits
+        self.traits = {}
 
-    def add_trait(self, trait: GameObject) -> bool:
+    def add_trait(
+        self, trait: Trait, duration: int = -1, description: str = ""
+    ) -> bool:
         """Add a trait to the tracker.
 
         Parameters
         ----------
         trait
-            A trait to add.
+            The trait to add.
+        duration
+            How long to add the trait.
+        description
+            A string description to about the trait.
 
-        Return
-        ------
+        Returns
+        -------
         bool
-            True if the trait was added successfully, False if already present or
-            if the trait conflict with existing traits.
+            True if successful; False otherwise.
         """
-
-        if trait in self._traits:
+        if trait.definition_id in self.traits:
             return False
 
         if self.has_conflicting_trait(trait):
             return False
 
-        self._traits.add(trait)
-        self._conflicting_traits = self._conflicting_traits.union(
-            trait.get_component(Trait).conflicting_traits
+        instance = TraitInstance(
+            trait=trait,
+            timestamp=self.gameobject.world.resources.get_resource(SimDate).copy(),
+            duration=duration,
+            description=description if description else trait.description,
         )
-        trait.get_component(Trait).apply(self.gameobject)
-        return True
 
-    def remove_trait(self, trait: GameObject) -> bool:
-        """Remove a trait from the tracker.
+        self.traits[instance.trait.definition_id] = instance
 
-        Parameters
-        ----------
-        trait
-            The trait to remove.
+        return True
 
-        Return
-        ------
-        bool
-            True if a trait was successfully removed. False otherwise.
-        """
-        if trait in self._traits:
-            self._traits.remove(trait)
+    def remove_trait(self, trait: Trait) -> bool:
+        """Remove a trait from the tracker."""
 
-            self._conflicting_traits = set()
-            for remaining_trait in self._traits:
-                self._conflicting_traits = self._conflicting_traits.union(
-                    remaining_trait.get_component(Trait).conflicting_traits
-                )
+        if trait.definition_id in self.traits:
 
-            trait.get_component(Trait).remove(self.gameobject)
+            del self.traits[trait.definition_id]
 
             return True
 
         return False
 
-    def has_conflicting_trait(self, trait: GameObject) -> bool:
+    def has_trait(self, trait: Union[str, Trait]) -> bool:
+        """Check if the GameObject has a given trait."""
+        if isinstance(trait, str):
+            return trait in self.traits
+
+        return trait.definition_id in self.traits
+
+    def has_conflicting_trait(self, trait: Trait) -> bool:
         """Check if a trait conflicts with current traits.
 
         Parameters
         ----------
         trait
             The trait to check.
 
         Returns
         -------
         bool
             True if the trait conflicts with any of the current traits or if any current
             traits conflict with the given trait. False otherwise.
         """
-        if trait.get_component(Trait).definition_id in self._conflicting_traits:
-            return True
+        for instance in self.traits.values():
 
-        incoming_trait_conflicts = trait.get_component(Trait).conflicting_traits
+            if instance.trait.definition_id in trait.conflicting_traits:
+                return True
 
-        return any(
-            t.get_component(Trait).definition_id in incoming_trait_conflicts
-            for t in self._traits
-        )
+            if trait.definition_id in instance.trait.conflicting_traits:
+                return True
+
+        return False
 
     def __str__(self) -> str:
-        return f"{type(self).__name__}({list(self._traits)})"
+        return f"Traits(traits={list(self.traits.keys())!r})"
 
     def __repr__(self) -> str:
-        return f"{type(self).__name__}({list(self._traits)})"
+        return f"Traits(traits={list(self.traits.keys())!r})"
 
     def to_dict(self) -> dict[str, Any]:
-        return {"traits": [t.uid for t in self._traits]}
+        return {"instances": [t.to_dict() for t in self.traits.values()]}
```

### Comparing `neighborly-2.5.0/src/neighborly/config.py` & `neighborly-3.0.0.dev1/src/neighborly/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,9 +33,15 @@
 
     seed: Union[str, int] = attrs.field(factory=lambda: random.randint(0, 9999999))
     """Value used for pseudo-random number generation."""
 
     logging: LoggingConfig = attrs.field(factory=LoggingConfig)
     """Configuration settings for logging."""
 
-    settlement: Union[str, list[str]] = attrs.field(factory=list[str])
-    """Settlement definition ID to instantiate during simulation initialization."""
+    growth_factor: float = 0.5
+    """Probability of a district spawning a new character."""
+
+    num_districts: int = 4
+    """The number of districts to generate in the settlement."""
+
+    theme_tags: list[str] = attrs.field(factory=list)
+    """Content tags to guide settlement development."""
```

### Comparing `neighborly-2.5.0/src/neighborly/data_collection.py` & `neighborly-3.0.0.dev1/src/neighborly/data_analysis.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,135 +1,136 @@
-"""Data collection.
+"""Data Analysis and Experimentation
 
-This module contains functionality for collecting and exporting data from a simulation.
-
-Its structure is informed by the data collection layer of Mesa, an agent-based modeling
-library written in Python. Here we adapt their functionality to fit the ECS architecture
-of the simulation.
+This module contains classes and helper functions for performing experiments and
+data analysis on one or more simulation runs. Data analysis is closely integrated with
+the Pandas data frame library.
 
 """
 
 from __future__ import annotations
 
-from typing import Any, Iterator, Optional, Sequence
-
-import polars as pl
-
-from neighborly.ecs import SystemGroup
+from abc import ABC, abstractmethod
+from typing import Callable, Sequence
 
+import pandas as pd
+import tqdm
 
-class DataTablesIterator:
-    """Iterator for DataTables resource."""
+from neighborly.simulation import Simulation
 
-    __slots__ = ("table_names", "tables", "idx")
 
-    table_names: tuple[str, ...]
-    """table names to iterate over."""
-    tables: DataTables
-    """Tables to iterate over."""
-    idx: int
-    """The current index in the table names tuple."""
+class Metric(ABC):
+    """Extracts and aggregates data from a BatchRunner."""
 
-    def __init__(self, table_names: Sequence[str], tables: DataTables) -> None:
-        self.table_names = tuple(table_names)
-        self.tables = tables
-        self.idx = 0
+    __slots__ = ("_tables", "collection_interval", "collect_at_end", "cooldown")
 
-    def __iter__(self) -> Iterator[tuple[str, pl.DataFrame]]:
-        return self
+    _tables: list[list[pd.DataFrame]]
+    """Data frames extracted from simulation instances."""
+    collection_interval: int
+    """The number of timesteps between collections."""
+    collect_at_end: bool
+    """Should this metric collect data when the simulation ends."""
+    cooldown: int
+    """The number of timesteps until the metric runs again."""
 
-    def __next__(self) -> tuple[str, pl.DataFrame]:
-        if self.idx < len(self.table_names):
-            name = self.table_names[self.idx]
-            df = self.tables.get_data_frame(name)
-            self.idx += 1
-            return name, df
-        raise StopIteration
-
-
-class DataTables:
-    """A shared resource that collects data from the simulation into tables."""
+    def __init__(
+        self, collection_interval: int = -1, collect_at_end: bool = True
+    ) -> None:
+        super().__init__()
+        self._tables = [[]]
+        self.collection_interval = collection_interval
+        self.collect_at_end = collect_at_end
+        self.cooldown = 0
+
+    @property
+    def tables(self) -> Sequence[Sequence[pd.DataFrame]]:
+        """Get the data tables for the metric."""
+        return self._tables
+
+    def increment_table_batch(self) -> None:
+        """Add a new collection of tables for another batch run."""
+        self._tables.append([])
+
+    def add_table(self, table: pd.DataFrame) -> None:
+        """Add a table to the Metric's collection of tables."""
+        self._tables[-1].append(table)
+
+    @abstractmethod
+    def extract_data(self, sim: Simulation) -> pd.DataFrame:
+        """Extract a table of data from the simulation instance."""
+        raise NotImplementedError()
+
+    @abstractmethod
+    def get_aggregate_data(self) -> pd.DataFrame:
+        """Aggregate the tables extracted from the simulations instances."""
+        raise NotImplementedError()
+
+    def clear(self) -> None:
+        """Clears all data from the metric."""
+        self._tables.clear()
+        self._tables.append([])
+
+
+class BatchRunner:
+    """Runs multiple simulation instances and collects data during each run.
+
+    Parameters
+    ----------
+    factory
+        A function used to create new simulation instances.
+    n_instances
+        The number of simulation instances to run.
+    years
+        The number of simulated years to run each simulation instance.
+    """
 
-    __slots__ = ("_tables",)
+    __slots__ = ("factory", "n_instances", "years", "_metrics")
 
-    _tables: dict[str, dict[str, list[Any]]]
-    """Table names mapped to dicts with column names mapped to data entries."""
+    factory: Callable[[], Simulation]
+    """A function used to create new simulation instances."""
+    n_instances: int
+    """The number of simulation instances to run."""
+    years: int
+    """The number of simulated years to run each simulation instance."""
+    _metrics: list[Metric]
+    """Metrics to run after a simulation instance finishes running."""
 
     def __init__(
         self,
-        tables: Optional[dict[str, tuple[str, ...]]] = None,
+        factory: Callable[[], Simulation],
+        n_instances: int,
+        years: int,
     ) -> None:
-        """
-        Parameters
-        ----------
-        tables
-            Table names mapped to dicts with column names mapped to data entries.
-        """
-        self._tables = {}
-
-        # Construct all the tables
-        if tables:
-            for table_name, column_names in tables.items():
-                self.create_table(table_name, column_names)
-
-    def create_table(self, table_name: str, column_names: tuple[str, ...]) -> None:
-        """Create a new table for data collection.
-
-        Parameters
-        ----------
-        table_name
-            The name of the new table.
-        column_names
-            The names of columns within the table.
-        """
-        new_table: dict[str, list[Any]] = {column: [] for column in column_names}
-        self._tables[table_name] = new_table
-
-    def add_data_row(self, table_name: str, row_data: dict[str, Any]) -> None:
-        """Add a new row of data to a table.
-
-        Parameters
-        ----------
-        table_name
-            The table to add the row to.
-        row_data
-            A row of data to add to the table where each dict key is the
-            name of the column.
-        """
-        if table_name not in self._tables:
-            raise ValueError(f"Could not find table with name: {table_name}")
-
-        for column in self._tables[table_name]:
-            if column in row_data:
-                self._tables[table_name][column].append(row_data[column])
-            else:
-                raise KeyError(f"Row data is missing column: {column}")
-
-    def get_data_frame(self, table_name: str) -> pl.DataFrame:
-        """Create a Polars data frame from a table.
-
-        Parameters
-        ----------
-        table_name
-            The name of the table to retrieve.
-
-        Returns
-        -------
-        pl.DataFrame
-            A polars DataFrame.
-        """
-        return pl.DataFrame(self._tables[table_name])
-
-    def __iter__(self) -> Iterator[tuple[str, pl.DataFrame]]:
-        return DataTablesIterator(list(self._tables.keys()), self)
-
-    def to_dict(self) -> dict[str, Any]:
-        """Serialize the object to a JSON-serializable dict."""
-        return {**self._tables}
-
-
-class DataCollectionSystems(SystemGroup):
-    """System group for collecting data.
-
-    Any system that collects data during the course of the simulation should
-    belong to this group.
-    """
+        self.factory = factory
+        self.n_instances = n_instances
+        self.years = years
+        self._metrics = []
+
+    def add_metric(self, metric: Metric) -> None:
+        """Add a data analysis metric to the runner."""
+        self._metrics.append(metric)
+
+    def run(self) -> None:
+        """Run the simulation batch."""
+
+        for _ in range(self.n_instances):
+            sim = self.factory()
+
+            num_time_steps = 12 * self.years
+
+            for _ in tqdm.tqdm(range(num_time_steps)):
+                sim.step()
+
+                for metric in self._metrics:
+                    metric.cooldown -= 1
+                    if metric.cooldown <= 0 and metric.collection_interval > 0:
+                        metric.add_table(metric.extract_data(sim))
+                        metric.cooldown = metric.collection_interval
+
+            for metric in self._metrics:
+                if metric.collect_at_end:
+                    metric.add_table(metric.extract_data(sim))
+                metric.increment_table_batch()
+
+    def reset(self) -> None:
+        """Resets the internal data caches for another run."""
+        for metric in self._metrics:
+            metric.clear()
```

### Comparing `neighborly-2.5.0/src/neighborly/datetime.py` & `neighborly-3.0.0.dev1/src/neighborly/datetime.py`

 * *Files identical despite different names*

### Comparing `neighborly-2.5.0/src/neighborly/defs/defaults.py` & `neighborly-3.0.0.dev1/src/neighborly/plugins/default_systems.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,826 +1,712 @@
-"""Default Content Definitions.
-
-This module contains default implementations of concrete definition classes that
-inherit from those found in neighborly.defs.base_types. These definitions are loaded
-into ever Neighborly instance when it is constructed.
+"""Default systems to include into a simulation.
 
 """
 
-from __future__ import annotations
-
 import random
-from typing import Callable, ClassVar, Optional
+from collections import defaultdict
+from typing import ClassVar, Optional
 
-from neighborly.components.business import Business, JobRole, OpenToPublic
-from neighborly.components.character import Character, LifeStage, Sex, Species
-from neighborly.components.location import (
-    FrequentedBy,
-    FrequentedLocations,
-    LocationPreferences,
-)
-from neighborly.components.relationship import Relationships, SocialRules
-from neighborly.components.residence import ResidentialBuilding, ResidentialUnit, Vacant
-from neighborly.components.settlement import District, Settlement
-from neighborly.components.skills import Skill, Skills
-from neighborly.components.spawn_table import (
-    BusinessSpawnTable,
-    BusinessSpawnTableEntry,
-    CharacterSpawnTable,
-    CharacterSpawnTableEntry,
-    ResidenceSpawnTable,
-    ResidenceSpawnTableEntry,
+from neighborly.components.business import Business, BusinessStatus, JobRole, Occupation
+from neighborly.components.character import (
+    Character,
+    Household,
+    LifeStage,
+    MemberOfHousehold,
+    Pregnant,
+    ResidentOf,
+    Sex,
 )
-from neighborly.components.stats import Stat, Stats
-from neighborly.components.traits import Trait, Traits
-from neighborly.defs.base_types import (
-    BusinessDef,
-    BusinessGenOptions,
-    CharacterDef,
-    CharacterGenOptions,
-    DistrictDef,
-    DistrictGenOptions,
-    JobRoleDef,
-    ResidenceDef,
-    ResidenceGenOptions,
-    SettlementDef,
-    SettlementGenOptions,
-    SkillDef,
-    TraitDef,
+from neighborly.components.location import FrequentedLocations, Location
+from neighborly.components.relationship import Relationship, Relationships, Romance
+from neighborly.components.settlement import Settlement
+from neighborly.components.spawn_table import BusinessSpawnTable
+from neighborly.components.stats import Sociability
+from neighborly.ecs import Active, GameObject, System, World
+from neighborly.helpers.action import get_action_probability
+from neighborly.helpers.character import (
+    add_character_to_household,
+    create_household,
+    remove_character_from_household,
+    set_household_head,
 )
-from neighborly.ecs import GameObject, World
-from neighborly.helpers.settlement import create_district
-from neighborly.helpers.skills import add_skill
-from neighborly.helpers.stats import add_stat
-from neighborly.helpers.traits import add_trait
-from neighborly.libraries import (
-    BusinessLibrary,
-    CharacterLibrary,
-    DistrictLibrary,
-    EffectLibrary,
-    JobRoleLibrary,
-    ResidenceLibrary,
-    SkillLibrary,
-    TraitLibrary,
+from neighborly.helpers.relationship import add_relationship, has_relationship
+from neighborly.helpers.traits import get_relationships_with_traits
+from neighborly.libraries import JobRoleLibrary
+from neighborly.plugins.actions import (
+    BreakUp,
+    Divorce,
+    FireEmployee,
+    FormCrush,
+    GetMarried,
+    GetPregnant,
+    HireEmployee,
+    PromoteEmployee,
+    Retire,
+    StartBusiness,
+    StartDating,
 )
-from neighborly.life_event import PersonalEventHistory
-from neighborly.tracery import Tracery
+from neighborly.simulation import Simulation
+from neighborly.systems import UpdateSystems
 
 
-class DefaultSkillDef(SkillDef):
-    """The default implementation of a skill definition."""
+class FindJobSystem(System):
+    """Unemployed characters try to find work."""
 
-    def instantiate(self, world: World) -> GameObject:
-        skill = world.gameobject_manager.spawn_gameobject(name=self.display_name)
-        tracery = skill.world.resource_manager.get_resource(Tracery)
-        skill.add_component(
-            Skill(
-                definition_id=self.definition_id,
-                display_name=tracery.generate(self.display_name),
-                description=tracery.generate(self.description),
-            )
-        )
-        return skill
+    def on_update(self, world: World) -> None:
 
+        rng = world.resources.get_resource(random.Random)
 
-class DefaultTraitDef(TraitDef):
-    """A definition for a trait type."""
+        library = world.resources.get_resource(JobRoleLibrary)
 
-    def instantiate(self, world: World) -> GameObject:
-        trait = world.gameobject_manager.spawn_gameobject(name=self.display_name)
+        active_businesses = [
+            business
+            for _, (business, _) in world.get_components((Business, Active))
+            if business.status == BusinessStatus.OPEN
+        ]
 
-        effect_library = trait.world.resource_manager.get_resource(EffectLibrary)
-        tracery = trait.world.resource_manager.get_resource(Tracery)
+        rng.shuffle(active_businesses)
 
-        effects = [
-            effect_library.create_from_obj(trait.world, entry) for entry in self.effects
-        ]
+        for _, (character_comp, _) in world.get_components((Character, Active)):
+            character = character_comp.gameobject
 
-        trait.add_component(
-            Trait(
-                definition_id=self.definition_id,
-                display_name=tracery.generate(self.display_name),
-                description=tracery.generate(self.description),
-                effects=effects,
-                conflicting_traits=self.conflicts_with,
-            )
-        )
+            if character.has_component(Occupation):
+                continue
 
-        return trait
+            if character_comp.life_stage not in (
+                LifeStage.YOUNG_ADULT,
+                LifeStage.ADULT,
+            ):
+                continue
 
+            potential_hires: list[HireEmployee] = []
 
-class DefaultSpeciesDef(DefaultTraitDef):
-    """A definition for a trait type."""
+            for business in active_businesses:
+                open_positions = business.get_open_positions()
 
-    adolescent_age: int
-    """Age this species reaches adolescence."""
-    young_adult_age: int
-    """Age this species reaches young adulthood."""
-    adult_age: int
-    """Age this species reaches main adulthood."""
-    senior_age: int
-    """Age this species becomes a senior/elder."""
-    lifespan: int
-    """The number of years that this species lives."""
-    can_physically_age: bool
-    """Does this character go through the various life stages."""
-
-    def instantiate(self, world: World) -> GameObject:
-        trait = super().instantiate(world)
-
-        trait.add_component(
-            Species(
-                adolescent_age=self.adolescent_age,
-                young_adult_age=self.young_adult_age,
-                adult_age=self.adult_age,
-                senior_age=self.senior_age,
-                lifespan=self.lifespan,
-                can_physically_age=self.can_physically_age,
-            )
-        )
+                for role_id in open_positions:
+                    job_role = library.get_role(role_id)
 
-        return trait
+                    if job_role.check_requirements(character):
+                        action = HireEmployee(
+                            business=business.gameobject,
+                            character=character,
+                            role=job_role,
+                        )
+                        potential_hires.append(action)
 
+            if not potential_hires:
+                continue
 
-def default_district_name_factory(world: World, _: DistrictGenOptions) -> str:
-    """Generate a new name"""
-    tracery = world.resource_manager.get_resource(Tracery)
-    name = tracery.generate("#settlement_name#")
-    return name
-
-
-class DefaultDistrictDef(DistrictDef):
-    """A definition for a district type specified by the user."""
-
-    name_factories: ClassVar[dict[str, Callable[[World, DistrictGenOptions], str]]] = {
-        "default": default_district_name_factory
-    }
-
-    def instantiate(
-        self,
-        world: World,
-        settlement: GameObject,
-        options: DistrictGenOptions,
-    ) -> GameObject:
-        district = world.gameobject_manager.spawn_gameobject()
-        district.metadata["definition_id"] = self.definition_id
-
-        name = ""
-
-        if self.name:
-            name = self.name
-        elif self.name_factory:
-            name = self.name_factories[self.name_factory](world, options)
-
-        district.add_component(
-            District(
-                name=name,
-                description=self.description,
-                settlement=settlement,
-                residential_slots=self.residential_slots,
-                business_slots=self.business_slots,
-            )
-        )
-        self.initialize_business_spawn_table(district)
-        self.initialize_character_spawn_table(district)
-        self.initialize_residence_spawn_table(district)
-
-        return district
-
-    def initialize_business_spawn_table(self, district: GameObject) -> None:
-        """Create the business spawn table for the district."""
-        world = district.world
-        rng = world.resource_manager.get_resource(random.Random)
-        business_library = world.resource_manager.get_resource(BusinessLibrary)
+            action = rng.choice(potential_hires)
 
-        table_entries: list[BusinessSpawnTableEntry] = []
+            action_probability = get_action_probability(action)
 
-        for entry in self.business_types:
-            if entry.with_id:
-                business_def = business_library.get_definition(entry.with_id)
-                table_entries.append(
-                    BusinessSpawnTableEntry(
-                        name=entry.with_id,
-                        spawn_frequency=business_def.spawn_frequency,
-                        max_instances=business_def.max_instances,
-                        min_population=business_def.min_population,
-                        instances=0,
-                    )
-                )
-            elif entry.with_tags:
-                potential_defs = business_library.get_definition_with_tags(
-                    entry.with_tags
-                )
+            if rng.random() < action_probability:
+                action.execute()
 
-                if not potential_defs:
-                    continue
 
-                business_def = rng.choice(potential_defs)
+class FiredFromJobSystem(System):
+    """Occasionally fire an employee or two."""
 
-                table_entries.append(
-                    BusinessSpawnTableEntry(
-                        name=business_def.definition_id,
-                        spawn_frequency=entry.spawn_frequency,
-                        max_instances=entry.max_instances,
-                        min_population=entry.min_population,
-                        instances=0,
-                    )
+    FIRING_THRESHOLD: ClassVar[float] = 0.8
+    """Utility score required to consider someone for firing."""
+
+    def on_update(self, world: World) -> None:
+
+        rng = world.resources.get_resource(random.Random)
+
+        # This loops through all the active businesses, scores the probability of
+        # firing each of the current employees, and, if any are above the firing
+        # threshold (class var), they are added to a list of potential employees
+        # to fire.
+        # The system selects one character at random from the list using weighted
+        # random selection, and does a probability check on if the character will
+        # actually be fired this time step.
+        for _, (business, _) in world.get_components((Business, Active)):
+            if business.status != BusinessStatus.OPEN:
+                continue
+
+            business_owner = business.owner
+
+            if business_owner is None:
+                continue
+
+            potential_actions: list[tuple[FireEmployee, float]] = []
+            action_utilities: list[float] = []
+
+            # Evaluate firing each employee
+            for employee, _ in business.employees.items():
+
+                action = FireEmployee(business=business.gameobject, character=employee)
+                action_probability = get_action_probability(action)
+
+                if action_probability >= self.FIRING_THRESHOLD:
+                    potential_actions.append((action, action_probability))
+                    action_utilities.append(action_probability)
+
+            if not potential_actions:
+                continue
+
+            chosen_action, action_probability = rng.choices(
+                potential_actions, action_utilities, k=1
+            )[0]
+
+            if rng.random() < action_probability:
+                chosen_action.execute()
+
+
+class JobPromotionSystem(System):
+    """Occasionally promote characters to higher positions at their jobs."""
+
+    PROMOTION_THRESHOLD: ClassVar[float] = 0.8
+    """Probability scored required to consider someone for a promotion."""
+
+    def on_update(self, world: World) -> None:
+
+        rng = world.resources.get_resource(random.Random)
+        job_role_library = world.resources.get_resource(JobRoleLibrary)
+
+        # Similar to firing characters, this systems loops through all the businesses
+        # and scores the probability of promoting each of it's employees. Only employees
+        # with probability scores above the threshold are considered. Once all employees
+        # have been evaluated, one is selected randomly and we perform a "dice roll"
+        # to see if they will actually be promoted this time step.
+        for _, (business, _) in world.get_components((Business, Active)):
+            if business.status != BusinessStatus.OPEN:
+                continue
+
+            business_owner = business.owner
+
+            if business_owner is None:
+                continue
+
+            potential_promotions: list[tuple[PromoteEmployee, float]] = []
+            potential_promotion_scores: list[float] = []
+
+            # Evaluate promoting each employee
+            for employee, current_role in business.employees.items():
+
+                current_job_level = current_role.job_level
+
+                open_positions = business.get_open_positions()
+
+                for role_id in open_positions:
+                    role = job_role_library.get_role(role_id)
+
+                    if current_job_level >= role.job_level:
+                        continue
+
+                    action = PromoteEmployee(business_owner, employee, role)
+                    probability_score = get_action_probability(action)
+
+                    if probability_score > self.PROMOTION_THRESHOLD:
+                        potential_promotions.append((action, probability_score))
+                        potential_promotion_scores.append(probability_score)
+
+            if not potential_promotions:
+                continue
+
+            action, action_probability = rng.choices(
+                potential_promotions, potential_promotion_scores, k=1
+            )[0]
+
+            if rng.random() < action_probability:
+                action.execute()
+
+
+class StartBusinessSystem(System):
+    """Characters have a chance of becoming a business owner."""
+
+    @staticmethod
+    def get_eligible_businesses(
+        settlement: Settlement,
+    ) -> list[tuple[str, GameObject, JobRole]]:
+        """Get all potential businesses that could be built.
+
+        Parameters
+        ----------
+        settlement
+            The settlement where the business will be built.
+
+        Returns
+        -------
+        tuple[str, GameObject, JobRole]
+            The definition ID, district to build, and job role of eligible business
+            definitions.
+        """
+        eligible_business_definitions: list[tuple[str, GameObject, JobRole]] = []
+        weights: list[float] = []
+
+        for district in settlement.districts:
+            spawn_table = district.get_component(BusinessSpawnTable)
+
+            for entry in spawn_table.table.values():
+                if entry.instances >= entry.max_instances:
+                    continue
+                if entry.min_population >= settlement.population:
+                    continue
+
+                eligible_business_definitions.append(
+                    (entry.definition_id, district, entry.owner_role)
                 )
+                weights.append(entry.spawn_frequency)
 
-        district.add_component(BusinessSpawnTable(entries=table_entries))
+        return eligible_business_definitions
+
+    def on_update(self, world: World) -> None:
+        # This system loops through all the adult characters, giving them the option to
+        # start a new business if:
+        # (1) They meet the requirements for the owner role
+        # (2) They are unemployed
+        # (3) At least at the YOUNG_ADULT life stage
+        # (4) They are residents of the settlement
 
-    def initialize_character_spawn_table(self, district: GameObject) -> None:
-        """Create the character spawn table for the district."""
-        world = district.world
         rng = world.resource_manager.get_resource(random.Random)
 
-        character_library = world.resource_manager.get_resource(CharacterLibrary)
+        for _, (character, resident_of, _) in world.get_components(
+            (Character, ResidentOf, Active)
+        ):
+            if character.life_stage not in (LifeStage.YOUNG_ADULT, LifeStage.ADULT):
+                continue
+
+            if character.gameobject.has_component(Occupation):
+                continue
 
-        table_entries: list[CharacterSpawnTableEntry] = []
+            eligible_businesses = self.get_eligible_businesses(
+                resident_of.settlement.get_component(Settlement)
+            )
 
-        for entry in self.character_types:
-            if entry.with_id:
+            actions: list[tuple[StartBusiness, float]] = []
+            action_utilities: list[float] = []
 
-                character_def = character_library.get_definition(entry.with_id)
+            for definition_id, district, owner_role in eligible_businesses:
 
-                table_entries.append(
-                    CharacterSpawnTableEntry(
-                        name=character_def.definition_id,
-                        spawn_frequency=entry.spawn_frequency,
+                if not owner_role.requirements:
+                    action = StartBusiness(
+                        character=character.gameobject,
+                        business_definition_id=definition_id,
+                        district=district,
+                        owner_role=owner_role,
                     )
-                )
+                    action_probability = get_action_probability(action)
 
-            elif entry.with_id:
+                    if action_probability > 0:
+                        actions.append((action, action_probability))
+                        action_utilities.append(action_probability)
 
-                potential_defs = character_library.get_definition_with_tags(
-                    entry.with_tags
-                )
+                else:
+                    if owner_role.check_requirements(character.gameobject):
+                        action = StartBusiness(
+                            character=character.gameobject,
+                            business_definition_id=definition_id,
+                            district=district,
+                            owner_role=owner_role,
+                        )
+                        action_probability = get_action_probability(action)
+
+                        if action_probability > 0:
+                            actions.append((action, action_probability))
+                            action_utilities.append(action_probability)
 
-                if not potential_defs:
+            if not actions:
+                continue
+
+            action, action_probability = rng.choices(actions, action_utilities, k=1)[0]
+
+            if rng.random() < action_probability:
+                action.execute()
+
+
+class CharacterDatingSystem(System):
+    """Characters have a chance of dating their crush."""
+
+    def on_update(self, world: World) -> None:
+        rng = world.resource_manager.get_resource(random.Random)
+
+        for _, (character, relationships, _) in world.get_components(
+            (Character, Relationships, Active)
+        ):
+
+            potential_romances: list[tuple[StartDating, float]] = []
+            potential_romance_scores: list[float] = []
+
+            for partner, relationship in relationships.outgoing.items():
+
+                if not relationship.is_active:
                     continue
 
-                character_def = rng.choice(potential_defs)
+                if partner.is_active is False:
+                    continue
 
-                table_entries.append(
-                    CharacterSpawnTableEntry(
-                        name=character_def.definition_id,
-                        spawn_frequency=entry.spawn_frequency,
-                    )
-                )
+                if not partner.has_component(Character):
+                    continue
+
+                action = StartDating(character=character.gameobject, partner=partner)
+                action_probability = get_action_probability(action)
+
+                if action_probability > 0:
+                    potential_romances.append((action, action_probability))
+                    potential_romance_scores.append(action_probability)
+
+            if not potential_romances:
+                continue
 
-        district.add_component(CharacterSpawnTable(entries=table_entries))
+            action, action_probability = rng.choices(
+                potential_romances, potential_romance_scores, k=1
+            )[0]
 
-    def initialize_residence_spawn_table(self, district: GameObject) -> None:
-        """Create the residence spawn table for the district."""
-        world = district.world
+            if rng.random() < action_probability:
+                action.execute()
+
+
+class CharacterMarriageSystem(System):
+    """Characters have a chance to get married"""
+
+    def on_update(self, world: World) -> None:
         rng = world.resource_manager.get_resource(random.Random)
 
-        residence_library = world.resource_manager.get_resource(ResidenceLibrary)
+        for _, (character, _) in world.get_components((Character, Active)):
 
-        table_entries: list[ResidenceSpawnTableEntry] = []
+            marriages = get_relationships_with_traits(character.gameobject, "spouse")
 
-        for entry in self.residence_types:
-            if entry.with_id:
-                residence_def = residence_library.get_definition(entry.with_id)
-
-                table_entries.append(
-                    ResidenceSpawnTableEntry(
-                        name=residence_def.definition_id,
-                        spawn_frequency=residence_def.spawn_frequency,
-                        instances=0,
-                        required_population=residence_def.required_population,
-                        max_instances=residence_def.max_instances,
-                        is_multifamily=residence_def.is_multifamily,
-                    )
-                )
+            if marriages:
+                continue
+
+            relationships = get_relationships_with_traits(
+                character.gameobject, "dating"
+            )
 
-            elif entry.with_tags:
+            potential_marriages: list[tuple[GetMarried, float]] = []
+            potential_marriage_scores: list[float] = []
 
-                potential_defs = residence_library.get_definition_with_tags(
-                    entry.with_tags
-                )
+            for relationship in relationships:
+                partner = relationship.get_component(Relationship).target
 
-                if not potential_defs:
+                if partner.is_active is False:
                     continue
 
-                residence_def = rng.choice(potential_defs)
+                marriages = get_relationships_with_traits(partner, "spouse")
 
-                table_entries.append(
-                    ResidenceSpawnTableEntry(
-                        name=residence_def.definition_id,
-                        spawn_frequency=residence_def.spawn_frequency,
-                        instances=0,
-                        required_population=residence_def.required_population,
-                        max_instances=residence_def.max_instances,
-                        is_multifamily=residence_def.is_multifamily,
-                    )
-                )
+                if marriages:
+                    continue
 
-        district.add_component(ResidenceSpawnTable(entries=table_entries))
+                action = GetMarried(character=character.gameobject, partner=partner)
+                action_probability = get_action_probability(action)
 
+                if action_probability > 0:
+                    potential_marriages.append((action, action_probability))
+                    potential_marriage_scores.append(action_probability)
 
-def default_settlement_name_factory(world: World, _: SettlementGenOptions) -> str:
-    """Generate a new name"""
-    tracery = world.resource_manager.get_resource(Tracery)
-    name = tracery.generate("#settlement_name#")
-    return name
+            if not potential_marriages:
+                continue
 
+            action, action_probability = rng.choices(
+                potential_marriages, potential_marriage_scores, k=1
+            )[0]
 
-class DefaultSettlementDef(SettlementDef):
-    """A definition for a settlement type specified by the user."""
+            if rng.random() < action_probability:
+                action.execute()
 
-    name_factories: ClassVar[
-        dict[str, Callable[[World, SettlementGenOptions], str]]
-    ] = {"default": default_settlement_name_factory}
 
-    def instantiate(self, world: World, options: SettlementGenOptions) -> GameObject:
-        settlement = world.gameobject_manager.spawn_gameobject()
-        settlement.metadata["definition_id"] = self.definition_id
+class CharacterDivorceSystem(System):
+    """Characters in marriages may choose to divorce their spouse."""
 
-        name = ""
+    def on_update(self, world: World) -> None:
 
-        if self.display_name:
-            name = self.display_name
+        rng = world.resource_manager.get_resource(random.Random)
 
-        elif self.name_factory:
-            name = self.name_factories[self.name_factory](world, options)
+        for _, (character, _) in world.get_components((Character, Active)):
 
-        settlement.add_component(Settlement(name=name))
-        self.initialize_districts(settlement)
-        return settlement
+            marriages = get_relationships_with_traits(character.gameobject, "spouse")
 
-    def initialize_districts(self, settlement: GameObject) -> None:
-        """Instantiates the settlement's districts."""
+            potential_divorces: list[tuple[Divorce, float]] = []
+            potential_divorce_scores: list[float] = []
 
-        library = settlement.world.resource_manager.get_resource(DistrictLibrary)
-        rng = settlement.world.resource_manager.get_resource(random.Random)
+            for relationship in marriages:
+                partner = relationship.get_component(Relationship).target
 
-        for district_entry in self.districts:
-            if district_entry.with_id:
-                district = create_district(
-                    settlement.world,
-                    settlement,
-                    district_entry.with_id,
-                )
-                settlement.add_child(district)
-            elif district_entry.with_tags:
-                matching_districts = library.get_definition_with_tags(
-                    district_entry.with_tags
-                )
+                if partner.is_active is False:
+                    continue
 
-                if matching_districts:
-                    chosen_district = rng.choice(matching_districts)
-                    district = create_district(
-                        settlement.world,
-                        settlement,
-                        chosen_district.definition_id,
-                    )
-                    settlement.add_child(district)
+                action = Divorce(character=character.gameobject, partner=partner)
+                action_probability = get_action_probability(action)
 
+                if action_probability > 0:
+                    potential_divorces.append((action, action_probability))
+                    potential_divorce_scores.append(action_probability)
 
-class DefaultResidenceDef(ResidenceDef):
-    """A default implementation of a Residence Definition."""
+            if not potential_divorces:
+                continue
 
-    def instantiate(
-        self, world: World, district: GameObject, options: ResidenceGenOptions
-    ) -> GameObject:
+            action, action_probability = rng.choices(
+                potential_divorces, potential_divorce_scores, k=1
+            )[0]
 
-        residence = world.gameobject_manager.spawn_gameobject()
-        residence.metadata["definition_id"] = self.definition_id
+            if rng.random() < action_probability:
+                action.execute()
 
-        world = residence.world
 
-        building = residence.add_component(ResidentialBuilding(district=district))
-        residence.add_component(Traits())
-        residence.add_component(Stats())
+class DatingBreakUpSystem(System):
+    """Characters in dating relationships may choose to break-up with their partner."""
 
-        residence.name = self.display_name
+    def on_update(self, world: World) -> None:
 
-        for _ in range(self.residential_units):
-            residential_unit = world.gameobject_manager.spawn_gameobject(
-                components=[Traits()], name="ResidentialUnit"
-            )
-            residence.add_child(residential_unit)
-            residential_unit.add_component(
-                ResidentialUnit(building=residence, district=district)
+        rng = world.resources.get_resource(random.Random)
+
+        for _, (character, _) in world.get_components((Character, Active)):
+
+            dating_relationships = get_relationships_with_traits(
+                character.gameobject, "dating"
             )
-            building.add_residential_unit(residential_unit)
-            residential_unit.add_component(Vacant())
 
-        return residence
+            potential_break_ups: list[tuple[BreakUp, float]] = []
+            potential_break_up_scores: list[float] = []
 
+            if dating_relationships:
+                relationship = rng.choice(dating_relationships)
 
-def generate_any_first_name(world: World, _: CharacterGenOptions) -> str:
-    """Generate a first name for a character"""
+                if relationship.is_active is False:
+                    return None
 
-    tracery = world.resource_manager.get_resource(Tracery)
-    rng = world.resource_manager.get_resource(random.Random)
+                action = BreakUp(
+                    character=character.gameobject,
+                    partner=relationship.get_component(Relationship).target,
+                )
+                action_probability = get_action_probability(action)
 
-    pattern = rng.choice(["#first_name::feminine#", "#first_name::masculine#"])
+                if action_probability > 0:
+                    potential_break_ups.append((action, action_probability))
+                    potential_break_up_scores.append(action_probability)
 
-    name = tracery.generate(pattern)
+            if not potential_break_ups:
+                continue
 
-    return name
+            action, action_probability = rng.choices(
+                potential_break_ups, potential_break_up_scores, k=1
+            )[0]
 
+            if rng.random() < action_probability:
+                action.execute()
 
-def generate_masculine_first_name(world: World, _: CharacterGenOptions) -> str:
-    """Generate a masculine first name for a character"""
 
-    tracery = world.resource_manager.get_resource(Tracery)
+class PregnancySystem(System):
+    """Female characters in marriages have a chance of getting pregnant."""
 
-    name = tracery.generate("#first_name::masculine#")
+    def on_update(self, world: World) -> None:
 
-    return name
+        rng = world.resources.get_resource(random.Random)
 
+        for _, (character, _) in world.get_components((Character, Active)):
+            if character.sex != Sex.FEMALE:
+                continue
 
-def generate_feminine_first_name(world: World, _: CharacterGenOptions) -> str:
-    """Generate a feminine first name for a character"""
+            if character.gameobject.has_component(Pregnant):
+                continue
 
-    tracery = world.resource_manager.get_resource(Tracery)
+            marriages = get_relationships_with_traits(character.gameobject, "spouse")
 
-    name = tracery.generate("#first_name::feminine#")
+            potential_pregnancies: list[tuple[GetPregnant, float]] = []
+            potential_pregnancy_scores: list[float] = []
 
-    return name
+            for relationship in marriages:
+                partner = relationship.get_component(Relationship).target
 
+                if partner.get_component(Character).sex != Sex.MALE:
+                    continue
 
-def generate_last_name(world: World, _: CharacterGenOptions) -> str:
-    """Generate a last_name for a character."""
+                if partner.is_active is False:
+                    continue
 
-    tracery = world.resource_manager.get_resource(Tracery)
+                action = GetPregnant(character=character.gameobject, partner=partner)
+                action_probability = get_action_probability(action)
 
-    name = tracery.generate("#last_name#")
+                if action_probability > 0:
+                    potential_pregnancies.append((action, action_probability))
+                    potential_pregnancy_scores.append(action_probability)
 
-    return name
+            if not potential_pregnancies:
+                continue
 
+            action, action_probability = rng.choices(
+                potential_pregnancies, potential_pregnancy_scores, k=1
+            )[0]
 
-class DefaultCharacterDef(CharacterDef):
-    """Default implementation for character definitions."""
+            if rng.random() < action_probability:
+                action.execute()
 
-    first_name_factories: ClassVar[
-        dict[str, Callable[[World, CharacterGenOptions], str]]
-    ] = {
-        "default": generate_any_first_name,
-        "masculine": generate_masculine_first_name,
-        "feminine": generate_feminine_first_name,
-    }
 
-    last_name_factories: ClassVar[
-        dict[str, Callable[[World, CharacterGenOptions], str]]
-    ] = {"default": generate_last_name}
+class RetirementSystem(System):
+    """Senior characters working a job can consider if they want to retire."""
 
-    def instantiate(
-        self,
-        world: World,
-        options: CharacterGenOptions,
-    ) -> GameObject:
+    def on_update(self, world: World) -> None:
 
-        character = world.gameobject_manager.spawn_gameobject()
-        character.metadata["definition_id"] = self.definition_id
+        rng = world.resources.get_resource(random.Random)
 
-        rng = world.resource_manager.get_resource(random.Random)
+        for _, (character, _, _) in world.get_components(
+            (Character, Occupation, Active)
+        ):
+            if character.life_stage < LifeStage.SENIOR:
+                continue
 
-        library = character.world.resource_manager.get_resource(TraitLibrary)
-        species = library.get_trait(self.species)
+            if not character.gameobject.has_component(Occupation):
+                continue
 
-        character.add_component(
-            Character(
-                first_name="",
-                last_name="",
-                sex=rng.choice((Sex.MALE, Sex.FEMALE)),
-                species=species,
-            )
-        )
-        character.add_component(Traits())
-        character.add_component(Skills())
-        character.add_component(Stats())
-        character.add_component(FrequentedLocations())
-        character.add_component(Relationships())
-        character.add_component(LocationPreferences())
-        character.add_component(SocialRules())
-        character.add_component(PersonalEventHistory())
-
-        self.initialize_name(character, options)
-        self.initialize_character_age(character, options)
-        self.initialize_character_stats(character)
-        self.initialize_traits(character, options)
-        self.initialize_character_skills(character)
-
-        return character
-
-    def initialize_name(
-        self, character: GameObject, options: CharacterGenOptions
-    ) -> None:
-        """Initialize the character's name.
+            action = Retire(character.gameobject)
 
-        Parameters
-        ----------
-        character
-            The character to initialize.
-        """
-        character_comp = character.get_component(Character)
+            action_probability = get_action_probability(action)
 
-        if options.first_name:
-            character_comp.first_name = options.first_name
-        else:
-            factory = self.first_name_factories[self.first_name_factory]
-            character_comp.first_name = factory(character.world, options)
-
-        if options.last_name:
-            character_comp.last_name = options.last_name
-        else:
-            factory = self.last_name_factories[self.last_name_factory]
-            character_comp.last_name = factory(character.world, options)
-
-    def initialize_character_age(
-        self, character: GameObject, options: CharacterGenOptions
-    ) -> None:
-        """Initializes the characters age."""
-        rng = character.world.resource_manager.get_resource(random.Random)
-
-        character_comp = character.get_component(Character)
-        species = character.get_component(Character).species.get_component(Species)
-
-        if options.life_stage is not "":
-
-            life_stage: Optional[LifeStage] = LifeStage[options.life_stage]
-
-            character_comp.life_stage = life_stage
-
-            # Generate an age for this character
-            if life_stage == LifeStage.CHILD:
-                character_comp.age = rng.randint(0, species.adolescent_age - 1)
-            elif life_stage == LifeStage.ADOLESCENT:
-                character_comp.age = rng.randint(
-                    species.adolescent_age,
-                    species.young_adult_age - 1,
-                )
-            elif life_stage == LifeStage.YOUNG_ADULT:
-                character_comp.age = rng.randint(
-                    species.young_adult_age,
-                    species.adult_age - 1,
-                )
-            elif life_stage == LifeStage.ADULT:
-                character_comp.age = rng.randint(
-                    species.adult_age,
-                    species.senior_age - 1,
-                )
-            else:
-                character_comp.age = character_comp.age = rng.randint(
-                    species.senior_age,
-                    species.lifespan - 1,
-                )
+            if rng.random() < action_probability:
+                action.execute()
 
-    def initialize_traits(
-        self, character: GameObject, options: CharacterGenOptions
-    ) -> None:
-        """Set the traits for a character."""
-        character.add_component(Traits())
-        rng = character.world.resource_manager.get_resource(random.Random)
-        trait_library = character.world.resource_manager.get_resource(TraitLibrary)
-
-        # Loop through the trait entries in the definition and get by ID or select
-        # randomly if using tags
-        for entry in self.traits:
-            if entry.with_id:
-                add_trait(character, entry.with_id)
-            elif entry.with_tags:
-                potential_traits = trait_library.get_definition_with_tags(
-                    entry.with_tags
-                )
 
-                traits: list[str] = []
-                trait_weights: list[int] = []
+class AdultsFormOwnHouseholdSystem(System):
+    """Characters may chose to start their own households.
 
-                for trait_def in potential_traits:
-                    if trait_def.spawn_frequency >= 1:
-                        traits.append(trait_def.definition_id)
-                        trait_weights.append(trait_def.spawn_frequency)
-
-                if len(traits) == 0:
-                    continue
-
-                chosen_trait = rng.choices(
-                    population=traits, weights=trait_weights, k=1
-                )[0]
-
-                add_trait(character, chosen_trait)
-
-        # Add traits specified in options
-        for trait in options.traits:
-            add_trait(character, trait)
-
-    def initialize_character_stats(self, character: GameObject) -> None:
-        """Initializes a characters stats with random values."""
-        rng = character.world.resource_manager.get_resource(random.Random)
-
-        # By adding any stats from the definition
-        for entry in self.stats:
-            base_value = 0
-            if entry.value is not None:
-                base_value = entry.value
-            elif entry.value_range:
-                min_value, max_value = (
-                    int(x.strip()) for x in entry.value_range.split("-")
-                )
-                base_value = rng.randint(min_value, max_value)
+    Adult characters who are not the head or spouse of a household, may start their own
+    households.
+    """
+
+    def on_update(self, world: World) -> None:
+        for _, (character, member_of_household, _) in world.get_components(
+            (Character, MemberOfHousehold, Active)
+        ):
+            if character.life_stage < LifeStage.YOUNG_ADULT:
+                continue
 
-            add_stat(
-                character,
-                entry.stat,
-                Stat(base_value=base_value, bounds=(entry.min_value, entry.max_value)),
+            household = member_of_household.household.get_component(Household)
+
+            is_regular_member = (
+                character.gameobject != household.head
+                and character.gameobject != household.spouse
             )
 
-        character_comp = character.get_component(Character)
-        species = character.get_component(Character).species.get_component(Species)
+            if not is_regular_member:
+                continue
 
-        health = add_stat(
-            character, "health", Stat(base_value=1000, bounds=(0, 999_999))
-        )
-        health_decay = add_stat(
-            character,
-            "health_decay",
-            Stat(base_value=1000.0 / species.lifespan, bounds=(0, 999_999)),
-        )
-        fertility = add_stat(
-            character,
-            "fertility",
-            Stat(base_value=round(rng.uniform(0.0, 1.0)), bounds=(0, 1.0)),
-        )
-        add_stat(
-            character,
-            "boldness",
-            Stat(
-                base_value=float(rng.randint(0, 255)), bounds=(0, 255), is_discrete=True
-            ),
-        )
-        add_stat(
-            character,
-            "stewardship",
-            Stat(
-                base_value=float(rng.randint(0, 255)), bounds=(0, 255), is_discrete=True
-            ),
-        )
-        add_stat(
-            character,
-            "sociability",
-            Stat(
-                base_value=float(rng.randint(0, 255)), bounds=(0, 255), is_discrete=True
-            ),
-        )
-        add_stat(
-            character,
-            "attractiveness",
-            Stat(
-                base_value=float(rng.randint(0, 255)), bounds=(0, 255), is_discrete=True
-            ),
-        )
-        add_stat(
-            character,
-            "intelligence",
-            Stat(
-                base_value=float(rng.randint(0, 255)), bounds=(0, 255), is_discrete=True
-            ),
-        )
-        add_stat(
-            character,
-            "reliability",
-            Stat(
-                base_value=float(rng.randint(0, 255)), bounds=(0, 255), is_discrete=True
-            ),
-        )
-
-        # Adjust health for current age
-        health.base_value -= character_comp.age * health_decay.value
-
-        # Adjust fertility for current life stage
-        if character_comp.sex == Sex.MALE:
-            if character_comp.life_stage == LifeStage.SENIOR:
-                fertility.base_value = fertility.base_value * 0.5
-            if character_comp.life_stage == LifeStage.ADULT:
-                fertility.base_value = fertility.base_value * 0.8
-        elif character_comp.sex == Sex.FEMALE:
-            if character_comp.life_stage == LifeStage.SENIOR:
-                fertility.base_value = 0
-            if character_comp.life_stage == LifeStage.ADULT:
-                fertility.base_value = fertility.base_value * 0.4
-
-    def initialize_character_skills(self, character: GameObject) -> None:
-        """Add default skills to the character."""
-        rng = character.world.resource_manager.get_resource(random.Random)
-        skill_library = character.world.resource_manager.get_resource(SkillLibrary)
-
-        for entry in self.skills:
-            base_value = 0
-            if entry.value is not None:
-                base_value = entry.value
-            elif entry.value_range:
-                min_value, max_value = (
-                    int(x.strip()) for x in entry.value_range.split("-")
-                )
-                base_value = rng.randint(min_value, max_value)
+            new_household = create_household(world).get_component(Household)
+            set_household_head(new_household, character)
+            remove_character_from_household(household, character)
+            add_character_to_household(new_household, character)
 
-            if entry.with_id:
-                add_skill(character, entry.with_id, base_value=base_value)
 
-            elif entry.with_tags:
-                potential_skills = skill_library.get_definition_with_tags(
-                    entry.with_tags
-                )
+class CrushFormationSystem(System):
+    """Every timestep there is a possibility that a character might form a new crush.
 
-                if not potential_skills:
-                    continue
+    This system is intended to assist with romantic depth within the simulation. It adds
+    an additional layer of nuance to relationships since characters might form crushes
+    on characters that they are not currently in a romantic relationship with.
+    """
 
-                chosen_skill = rng.choice(potential_skills)
+    CRUSH_THRESHOLD: ClassVar[float] = 0.6
+    """Probability score required for someone to form a crush."""
 
-                add_skill(character, chosen_skill.definition_id, base_value=base_value)
+    def on_update(self, world: World) -> None:
+        # 1) Loop through all the active characters
+        # 2) Get their outgoing relationships
+        # 3) Find the person that they have the highest romantic attraction to
+        # 4) Run a probability check
+        # 5) If successful, add a crush trait to the relationship and remove any
+        #    existing crushes.
 
+        rng = world.resources.get_resource(random.Random)
 
-class DefaultJobRoleDef(JobRoleDef):
-    """A default implementation of a Job Role Definition."""
+        for _, (character, relationships, _) in world.get_components(
+            (Character, Relationships, Active)
+        ):
+            potential_crush: Optional[GameObject] = None
+            highest_romance: float = 0
 
-    def instantiate(self, world: World) -> GameObject:
-        role = world.gameobject_manager.spawn_gameobject(name=self.display_name)
+            for target, relationship in relationships.outgoing.items():
 
-        effects_library = world.resource_manager.get_resource(EffectLibrary)
+                if not target.is_active or not relationship.is_active:
+                    continue
 
-        effect_instances = [
-            effects_library.create_from_obj(world, entry) for entry in self.effects
-        ]
+                if not target.has_component(Character):
+                    continue
 
-        monthly_effect_instances = [
-            effects_library.create_from_obj(world, entry)
-            for entry in self.monthly_effects
-        ]
+                romance = relationship.get_component(Romance).stat.value
 
-        role.add_component(
-            JobRole(
-                definition_id=self.definition_id,
-                display_name=self.display_name,
-                description=self.description,
-                job_level=self.job_level,
-                requirements=[],
-                effects=effect_instances,
-                monthly_effects=monthly_effect_instances,
-            )
-        )
+                if romance <= 0:
+                    continue
 
-        return role
+                if romance > highest_romance:
+                    highest_romance = romance
+                    potential_crush = target
 
+            if potential_crush is None:
+                continue
 
-class DefaultBusinessDef(BusinessDef):
-    """A default implementation of a Business Definition."""
+            action = FormCrush(character=character.gameobject, crush=potential_crush)
 
-    name_factories: ClassVar[dict[str, Callable[[World, BusinessGenOptions], str]]] = {}
+            action_probability = get_action_probability(action)
 
-    def instantiate(
-        self, world: World, district: GameObject, options: BusinessGenOptions
-    ) -> GameObject:
+            # if action_probability < self.CRUSH_THRESHOLD:
+            #     continue
 
-        business = world.gameobject_manager.spawn_gameobject()
-        business.metadata["definition_id"] = self.definition_id
+            if rng.random() < action_probability:
+                action.execute()
 
-        job_role_library = world.resource_manager.get_resource(JobRoleLibrary)
 
-        business.add_component(
-            Business(
-                name="",
-                owner_role=job_role_library.get_role(self.owner_role).get_component(
-                    JobRole
-                ),
-                employee_roles={
-                    job_role_library.get_role(role).get_component(JobRole): count
-                    for role, count in self.employee_roles.items()  # pylint: disable=E1101
-                },
-                district=district,
-            )
-        )
+class MeetNewPeopleSystem(System):
+    """Characters introduce themselves to new people that frequent the same places.
+
+    Notes
+    -----
+    This system uses a character's sociability stat score to determine the probability
+    of them introducing themselves to someone else. The goal is for characters with
+    higher sociability scores to form more relationships over the course of their lives.
+    """
+
+    def on_update(self, world: World) -> None:
+        rng = world.resource_manager.get_resource(random.Random)
 
-        business.add_component(Traits())
-        business.add_component(FrequentedBy())
-        business.add_component(PersonalEventHistory())
-        business.add_component(Stats())
-        business.add_component(Relationships())
-        business.add_component(SocialRules())
-
-        self.initialize_name(business, options)
-
-        if self.open_to_public:
-            business.add_component(OpenToPublic())
-
-        for trait in self.traits:
-            add_trait(business, trait)
-
-        return business
-
-    def initialize_name(
-        self, business: GameObject, options: BusinessGenOptions
-    ) -> None:
-        """Generates a name for the business."""
-        if options.name:
-            business.get_component(Business).name = options.name
-
-        elif self.name:
-            business.get_component(Business).name = options.name
-
-        elif self.name_factory:
-            name = self.name_factories[self.name_factory](business.world, options)
-            business.get_component(Business).name = name
+        for _, (character, frequented_locs, sociability, _) in world.get_components(
+            (Character, FrequentedLocations, Sociability, Active)
+        ):
+            probability_meet_someone = sociability.stat.normalized
+
+            if rng.random() < probability_meet_someone:
+                candidate_scores: defaultdict[GameObject, int] = defaultdict(int)
+
+                for loc in frequented_locs:
+                    for other in loc.get_component(Location).frequented_by:
+                        if other != character.gameobject and not has_relationship(
+                            character.gameobject, other
+                        ):
+                            candidate_scores[other] += 1
+
+                if candidate_scores:
+                    rng = world.resource_manager.get_resource(random.Random)
+
+                    acquaintance = rng.choices(
+                        list(candidate_scores.keys()),
+                        weights=list(candidate_scores.values()),
+                        k=1,
+                    )[0]
+
+                    if (
+                        rng.random()
+                        < acquaintance.get_component(Sociability).stat.normalized
+                    ):
+                        add_relationship(character.gameobject, acquaintance)
+                        add_relationship(acquaintance, character.gameobject)
+
+
+def load_plugin(sim: Simulation) -> None:
+    """Load systems into the simulation."""
+
+    sim.world.systems.add_system(FindJobSystem(), system_group=UpdateSystems)
+    sim.world.systems.add_system(FiredFromJobSystem(), system_group=UpdateSystems)
+    sim.world.systems.add_system(JobPromotionSystem(), system_group=UpdateSystems)
+    sim.world.systems.add_system(StartBusinessSystem(), system_group=UpdateSystems)
+    sim.world.systems.add_system(CharacterDatingSystem(), system_group=UpdateSystems)
+    sim.world.systems.add_system(CharacterMarriageSystem(), system_group=UpdateSystems)
+    sim.world.systems.add_system(CharacterDivorceSystem(), system_group=UpdateSystems)
+    sim.world.systems.add_system(DatingBreakUpSystem(), system_group=UpdateSystems)
+    sim.world.systems.add_system(PregnancySystem(), system_group=UpdateSystems)
+    sim.world.systems.add_system(RetirementSystem(), system_group=UpdateSystems)
+    sim.world.systems.add_system(
+        AdultsFormOwnHouseholdSystem(), system_group=UpdateSystems
+    )
+    sim.world.systems.add_system(CrushFormationSystem(), system_group=UpdateSystems)
+    sim.world.systems.add_system(MeetNewPeopleSystem(), system_group=UpdateSystems)
```

### Comparing `neighborly-2.5.0/src/neighborly/defs/definition_compiler.py` & `neighborly-3.0.0.dev1/src/neighborly/defs/definition_compiler.py`

 * *Files 14% similar despite different names*

```diff
@@ -62,57 +62,69 @@
     # and is not excluded from model_dump(...)
     if definition.is_template is False:
         definition.is_template = False
 
     # Variables to hold cumulative definition data
     final_definition_data: dict[str, Any] = {}
     final_definition_tags: set[str] = set()
+    final_definition_components: dict[str, dict[str, Any]] = {}
 
     # Update the final definition data with all the parents data
     for parent_def_id in definition.extends:
         if parent_def_id not in processed_defs:
             _process_definition(
                 definition_type,
                 unprocessed_defs[parent_def_id],
                 unprocessed_defs,
                 processed_defs,
             )
 
         parent_def = processed_defs[parent_def_id]
 
         # Update cumulative variables with parent data
-        final_definition_data.update(parent_def.model_dump(exclude_unset=True))
+        parent_def_raw = parent_def.model_dump(exclude_unset=True)
+        final_definition_data.update(parent_def_raw)
         final_definition_tags = final_definition_tags.union(parent_def.tags)
+        if "components" in parent_def_raw:
+            final_definition_components.update(parent_def_raw["components"])
 
     # Lastly update cumulative variables with the current definition's data
-    final_definition_data.update(definition.model_dump(exclude_unset=True))
+    raw_definition = definition.model_dump(exclude_unset=True)
+    final_definition_data.update(raw_definition)
+    if "components" in raw_definition:
+        final_definition_components.update(raw_definition["components"])
+    final_definition_data["components"] = final_definition_components
     final_definition_data["tags"] = final_definition_tags.union(definition.tags)
 
     # This definition has been processed.
     final_definition = definition_type.model_validate(final_definition_data)
     processed_defs[final_definition.definition_id] = final_definition
 
     # Process any variants
     for variant_def in final_definition.variants:
         # We have to do the following to ensure that 'is_template' has the
         # 'set' flag and is not excluded from model_dump(...)
-        if "name" not in variant_def:
+        if "variant_name" not in variant_def:
             raise ValueError(
                 f"{final_definition.definition_id} has variant that is missing a name."
             )
 
-        variant_name = variant_def["name"]
+        variant_name = variant_def["variant_name"]
         variant_tags: set[str] = set(variant_def.get("tags", []))
 
         variant_definition_data: dict[str, Any] = {}
 
         variant_definition_data.update(final_definition.model_dump(exclude_unset=True))
 
         variant_definition_data.update(variant_def)
 
         variant_id = f"{final_definition.definition_id}.{variant_name}"
         variant_definition_data["definition_id"] = variant_id
         variant_definition_data["tags"] = final_definition.tags.union(variant_tags)
+        variant_definition_data["components"] = {
+            **final_definition_data.get("components", {}),
+            **variant_definition_data.get("components", {}),
+        }
 
         processed_defs[variant_id] = definition_type.model_validate(
             variant_definition_data
         )
```

### Comparing `neighborly-2.5.0/src/neighborly/ecs.py` & `neighborly-3.0.0.dev1/src/neighborly/ecs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=C0302
 """Entity Component System
 
 This ECS implementation blends Unity-style GameObjects with the
 ECS logic from the Python esper library and the Bevy Game Engine.
 
 This ECS implementation is not thread-safe. It assumes that everything happens
 sequentially on the same thread.
@@ -20,33 +21,34 @@
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
 from typing import (
     Any,
     Callable,
+    ClassVar,
+    Generic,
     Iterable,
     Iterator,
     Optional,
+    Protocol,
     Type,
     TypeVar,
     Union,
-    cast,
     overload,
 )
 
 import esper
 from ordered_set import OrderedSet
 
 _LOGGER = logging.getLogger(__name__)
 
 _CT = TypeVar("_CT", bound="Component")
 _RT = TypeVar("_RT", bound="Any")
 _ST = TypeVar("_ST", bound="ISystem")
-_ET_contra = TypeVar("_ET_contra", bound="Event", contravariant=True)
 
 
 class ResourceNotFoundError(Exception):
     """Exception raised when attempting to access a resource that does not exist."""
 
     __slots__ = ("resource_type", "message")
 
@@ -153,124 +155,123 @@
     def __str__(self) -> str:
         return self.message
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(component={self.component_type.__name__})"
 
 
-class Event(ABC):
+class IEvent(Protocol):
+    """Interface implemented by any class that can be emitted as an event."""
+
+    @property
+    @abstractmethod
+    def event_type(self) -> str:
+        """A type name for the event."""
+
+        raise NotImplementedError()
+
+    @abstractmethod
+    def to_dict(self) -> dict[str, Any]:
+        """Serialize the event to a JSON-compliant dict."""
+
+        raise NotImplementedError()
+
+
+class Event:
     """Events signal when things happen in the simulation."""
 
-    __slots__ = ("_world", "_event_id")
+    __slots__ = ("_world", "_event_type", "data")
 
-    _event_id: int
-    """A unique ordinal ID for this event."""
     _world: World
     """The world instance to fire this event on."""
+    _event_type: str
+    """The ID of this event."""
+    data: dict[str, Any]
+    """General metadata."""
 
-    def __init__(self, world: World) -> None:
+    def __init__(self, event_type: str, world: World, **kwargs: Any) -> None:
         self._world = world
-        self._event_id = world.event_manager.get_next_event_id()
+        self._event_type = event_type
+        self.data = {**kwargs}
 
     @property
     def world(self) -> World:
         """The world instance to fire this event on."""
         return self._world
 
     @property
-    def event_id(self) -> int:
-        """A unique ordinal ID for this event."""
-        return self._event_id
-
-    def dispatch(self) -> None:
-        """Dispatch the event to registered event listeners."""
-        self.world.event_manager.dispatch_event(self)
+    def event_type(self) -> str:
+        """The type name for the event."""
+        return self._event_type
 
+    @abstractmethod
     def to_dict(self) -> dict[str, Any]:
         """Serialize the event to a JSON-compliant dict."""
-        return {"event_id": self.event_id, "event_type": self.__class__.__name__}
-
-    def __eq__(self, __o: object) -> bool:
-        if isinstance(__o, Event):
-            return self.event_id == __o.event_id
-        raise TypeError(f"Expected type Event, but was {type(__o)}")
-
-    def __le__(self, other: Event) -> bool:
-        return self.event_id <= other.event_id
-
-    def __lt__(self, other: Event) -> bool:
-        return self.event_id < other.event_id
-
-    def __ge__(self, other: Event) -> bool:
-        return self.event_id >= other.event_id
-
-    def __gt__(self, other: Event) -> bool:
-        return self.event_id > other.event_id
+        return {"event_id": self.event_type, "data": self.data}
 
 
 class GameObject:
     """A reference to an entity within the world.
 
     GameObjects wrap a unique integer identifier and provide an interface to access
     associated components and child/parent gameobjects.
     """
 
     __slots__ = (
-        "_id",
+        "_uid",
         "_name",
-        "_world",
+        "world",
         "children",
         "parent",
-        "_metadata",
+        "metadata",
         "_component_types",
         "_component_manager",
+        "_event_listeners",
     )
 
-    _id: int
-    """A GameObject's unique ID."""
-    _world: World
+    _uid: int
+    """The unique ID of this GameObject."""
+    _name: str
+    """The name of this GameObject."""
+    world: World
     """The world instance a GameObject belongs to."""
     _component_manager: esper.World
     """Reference to Esper ECS instance with all the component data."""
-    _name: str
-    """The name of the GameObject."""
     children: list[GameObject]
     """Child GameObjects below this one in the hierarchy."""
     parent: Optional[GameObject]
     """The parent GameObject that this GameObject is a child of."""
-    _metadata: dict[str, Any]
+    metadata: dict[str, Any]
     """Metadata associated with this GameObject."""
     _component_types: list[Type[Component]]
     """Types of the GameObjects components in order of addition."""
+    _event_listeners: dict[str, OrderedSet[Callable[[IEvent], None]]]
+    """Event listeners that are only called when a specific type of event fires."""
 
     def __init__(
         self,
         unique_id: int,
         world: World,
         component_manager: esper.World,
         name: str = "",
     ) -> None:
-        self._id = unique_id
-        self._world = world
+        self._uid = unique_id
+        self._name = name if name else f"GameObject({unique_id})"
+        self.world = world
         self._component_manager = component_manager
         self.parent = None
         self.children = []
-        self._metadata = {}
+        self.metadata = {}
         self._component_types = []
-        self.name = name if name else "GameObject"
+        self._event_listeners = {}
 
     @property
     def uid(self) -> int:
         """A GameObject's ID."""
-        return self._id
-
-    @property
-    def world(self) -> World:
-        """The World instance to which a GameObject belongs."""
-        return self._world
+        return self._uid
 
     @property
     def exists(self) -> bool:
         """Check if the GameObject still exists in the ECS.
 
         Returns
         -------
@@ -281,19 +282,14 @@
 
     @property
     def is_active(self) -> bool:
         """Check if a GameObject is active."""
         return self.has_component(Active)
 
     @property
-    def metadata(self) -> dict[str, Any]:
-        """Get the metadata associated with this GameObject."""
-        return self._metadata
-
-    @property
     def name(self) -> str:
         """Get the GameObject's name"""
         return self._name
 
     @name.setter
     def name(self, value: str) -> None:
         """Set the GameObject's name"""
@@ -302,22 +298,26 @@
     def activate(self) -> None:
         """Tag the GameObject as active."""
         self.add_component(Active())
 
         for child in self.children:
             child.activate()
 
+        self.dispatch_event(Event("activated", world=self.world, gameobject=self))
+
     def deactivate(self) -> None:
         """Remove the Active tag from a GameObject."""
 
         self.remove_component(Active)
 
         for child in self.children:
             child.deactivate()
 
+        self.dispatch_event(Event("deactivated", world=self.world, gameobject=self))
+
     def get_components(self) -> tuple[Component, ...]:
         """Get all components associated with the GameObject.
 
         Returns
         -------
         tuple[Component, ...]
             Component instances
@@ -347,21 +347,88 @@
             The component.
 
         Returns
         -------
         _CT
             The added component
         """
+
+        if self.has_component(type(component)):
+            raise TypeError(
+                "Cannot have multiple components of same type. "
+                f"Attempted to add {type(component)}."
+            )
+
         component.gameobject = self
         self._component_manager.add_component(self.uid, component)
         self._component_types.append(type(component))
         component.on_add()
 
         return component
 
+    def add_event_listener(
+        self,
+        event_name: str,
+        listener: Callable[[IEvent], None],
+    ) -> None:
+        """Register a listener function to a specific event type.
+
+        Parameters
+        ----------
+        listener
+            A function to be called when the given event type fires.
+        """
+        if event_name not in self._event_listeners:
+            self._event_listeners[event_name] = OrderedSet([])
+
+        listener_set = self._event_listeners[event_name]
+        listener_set.add(listener)
+
+    def remove_event_listener(
+        self, event_name: str, listener: Callable[[IEvent], None]
+    ) -> None:
+        """Remove a listener function from a specific event type.
+
+        Parameters
+        ----------
+        event_name : str
+            The type of event to remove the listener from.
+        callback : Callable[[IEvent], None]
+            The callback function to be removed.
+        """
+        if event_name in self._event_listeners:
+            listener_set = self._event_listeners[event_name]
+            listener_set.discard(listener)
+
+    def remove_all_event_listeners_for_event(self, event_name: str) -> None:
+        """Remove all event listeners for a specific event type.
+
+        Parameters
+        ----------
+        event_name : str
+            The type of event to remove listeners for.
+        """
+        if event_name in self._event_listeners:
+            del self._event_listeners[event_name]
+
+    def remove_all_event_listeners(self) -> None:
+        """Remove all event listeners associated with this GameObject."""
+        self._event_listeners.clear()
+
+    def dispatch_event(self, event: IEvent) -> None:
+        """Fire an event and trigger associated event listeners.
+
+        Parameters
+        ----------
+        event : IEvent
+            The event to fire
+        """
+        for callback_fn in self._event_listeners.get(event.event_type, OrderedSet([])):
+            callback_fn(event)
+
     def remove_component(self, component_type: Type[Component]) -> bool:
         """Remove a component from the GameObject.
 
         Parameters
         ----------
         component_type
             The type of the component to remove.
@@ -586,61 +653,47 @@
 
     def __eq__(self, other: object) -> bool:
         if isinstance(other, GameObject):
             return self.uid == other.uid
         return False
 
     def __int__(self) -> int:
-        return self._id
+        return self.uid
 
     def __hash__(self) -> int:
-        return self._id
+        return self.uid
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(id={self.uid}, name={self.name})"
+        return f"GameObject(id={self.uid!r}, name={self.name!r})"
 
 
 class Component(ABC):
     """A collection of data attributes associated with a GameObject."""
 
-    __slots__ = ("_gameobject", "_has_gameobject")
+    __slots__ = ("_gameobject",)
 
     _gameobject: GameObject
     """The GameObject the component belongs to."""
-    # We need an additional variable to track if the gameobject has been set because
-    # the variable will be initialized outside the __init__ method, and we need to
-    # ensure that it is not set again
-    _has_gameobject: bool
-    """Is the Component's _gameobject field set."""
-
-    def __init__(self) -> None:
-        super().__init__()
-        self._has_gameobject = False
 
     @property
     def gameobject(self) -> GameObject:
         """Get the GameObject instance for this component."""
         return self._gameobject
 
     @gameobject.setter
     def gameobject(self, value: GameObject) -> None:
-        """Sets the component's gameobject reference.
-
-        Notes
-        -----
-        This setter should only be called internally by the ECS when adding new
-        components to gameobjects. Calling this function twice will result in a
-        RuntimeError.
-        """
-        if self._has_gameobject is True:
-            raise RuntimeError("Cannot reassign a component to another GameObject.")
-        self._gameobject = value
+        """Set the GameObject instance."""
+        # This method should only be called by the ECS
+        if not hasattr(self, "_gameobject"):
+            self._gameobject = value
+        else:
+            raise RuntimeError("Cannot reassign the GameObject for a component")
 
     def on_add(self) -> None:
         """Lifecycle method called when the component is added to a GameObject."""
         return
 
     def on_remove(self) -> None:
         """Lifecycle method called when the component is removed from a GameObject."""
@@ -1095,119 +1148,193 @@
         -------
         _RT or None
             The instance of the resource.
         """
         return self._resources.get(resource_type)
 
 
+_T = TypeVar("_T")
+
+
+class EventEmitter(Generic[_T]):
+    """Emits events that observers can listen for."""
+
+    __slots__ = ("listeners",)
+
+    listeners: list[Callable[[object, _T], None]]
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.listeners = []
+
+    def add_listener(
+        self,
+        listener: Callable[[object, _T], None],
+    ) -> None:
+        """Register a listener function to a specific event type.
+
+        Parameters
+        ----------
+        listener
+            A function to be called when the given event type fires.
+        """
+        self.listeners.append(listener)
+
+    def remove_listener(
+        self,
+        listener: Callable[[object, _T], None],
+    ) -> None:
+        """Remove a listener from an event type.
+
+        Parameters
+        ----------
+        listener
+            A listener callback.
+        """
+        self.listeners.remove(listener)
+
+    def remove_all_listeners(self) -> None:
+        """Remove all listeners from an emitter."""
+        self.listeners.clear()
+
+    def dispatch(self, source: object, event: _T) -> None:
+        """Fire an event and trigger associated event listeners.
+
+        Parameters
+        ----------
+        source
+            The source of the event
+        event
+            The event to fire
+        """
+
+        for callback_fn in self.listeners:
+            callback_fn(source, event)
+
+
 class EventManager:
     """Manages event listeners for a single World instance."""
 
     __slots__ = (
         "_general_event_listeners",
         "_event_listeners_by_type",
         "_world",
-        "_next_event_id",
     )
 
     _world: World
     """The world instance associated with the SystemManager."""
-    _next_event_id: int
-    """The ID number to be given to the next constructed event."""
-    _general_event_listeners: OrderedSet[Callable[[Event], None]]
+    _general_event_listeners: OrderedSet[Callable[[IEvent], None]]
     """Event listeners that are called when any event fires."""
-    _event_listeners_by_type: dict[Type[Event], OrderedSet[Callable[[Event], None]]]
+    _event_listeners_by_type: dict[str, OrderedSet[Callable[[IEvent], None]]]
     """Event listeners that are only called when a specific type of event fires."""
 
     def __init__(self, world: World) -> None:
         self._world = world
         self._general_event_listeners = OrderedSet([])
         self._event_listeners_by_type = {}
-        self._next_event_id = 0
 
     def on_event(
         self,
-        event_type: Type[_ET_contra],
-        listener: Callable[[_ET_contra], None],
+        event_type: str,
+        listener: Callable[[IEvent], None],
     ) -> None:
         """Register a listener function to a specific event type.
 
         Parameters
         ----------
         event_type
             The type of event to listen for.
         listener
             A function to be called when the given event type fires.
         """
         if event_type not in self._event_listeners_by_type:
             self._event_listeners_by_type[event_type] = OrderedSet([])
-        listener_set = cast(
-            OrderedSet[Callable[[_ET_contra], None]],
-            self._event_listeners_by_type[event_type],
-        )
+        listener_set = self._event_listeners_by_type[event_type]
         listener_set.add(listener)
 
-    def on_any_event(self, listener: Callable[[Event], None]) -> None:
+    def on_any_event(self, listener: Callable[[IEvent], None]) -> None:
         """Register a listener function to all event types.
 
         Parameters
         ----------
         listener
             A function to be called any time an event fires.
         """
         self._general_event_listeners.append(listener)
 
-    def dispatch_event(self, event: Event) -> None:
+    def dispatch_event(self, event: IEvent) -> None:
         """Fire an event and trigger associated event listeners.
 
         Parameters
         ----------
         event
             The event to fire
         """
 
         for callback_fn in self._event_listeners_by_type.get(
-            type(event), OrderedSet([])
+            event.event_type, OrderedSet([])
         ):
             callback_fn(event)
 
         for callback_fn in self._general_event_listeners:
             callback_fn(event)
 
-    def get_next_event_id(self) -> int:
-        """Get an ID number for a new event instance."""
-        event_id = self._next_event_id
-        self._next_event_id += 1
-        return event_id
+
+class ComponentFactory(ABC):
+    """Creates instances of a component class."""
+
+    __component__: ClassVar[str] = ""
+
+    def __init__(self) -> None:
+        super().__init__()
+        if not self.__component__:
+            raise ValueError(
+                f"Missing '__component__' class attribute for {type(self)}."
+            )
+
+    @property
+    def component_type(self) -> str:
+        """The class name of the component this constructs"""
+        return self.__component__
+
+    @abstractmethod
+    def instantiate(self, world: World, /, **kwargs: Any) -> Component:
+        """Create an instance of the component."""
+
+        raise NotImplementedError()
 
 
 class GameObjectManager:
     """Manages GameObject and Component Data for a single World instance."""
 
     __slots__ = (
         "world",
+        "component_factories",
         "_component_manager",
         "_gameobjects",
         "_dead_gameobjects",
     )
 
     world: World
     """The manager's associated World instance."""
+    component_factories: dict[str, ComponentFactory]
+    """Component class names mapped to factory instances."""
     _component_manager: esper.World
     """Esper ECS instance used for efficiency."""
     _gameobjects: dict[int, GameObject]
     """Mapping of GameObjects to unique identifiers."""
     _dead_gameobjects: OrderedSet[int]
     """IDs of GameObjects to clean-up following destruction."""
 
     def __init__(self, world: World) -> None:
         self.world = world
         self._gameobjects = {}
         self._component_manager = esper.World()
         self._dead_gameobjects = OrderedSet([])
+        self.component_factories = {}
 
     @property
     def component_manager(self) -> esper.World:
         """Get the esper world instance with all the component data."""
         return self._component_manager
 
     @property
@@ -1217,17 +1344,22 @@
         Returns
         -------
         list[GameObject]
             All the GameObjects that exist in the world.
         """
         return self._gameobjects.values()
 
+    def add_component_factory(self, factory: ComponentFactory) -> None:
+        """Register a component type with the ECS."""
+
+        self.component_factories[factory.component_type] = factory
+
     def spawn_gameobject(
         self,
-        components: Optional[list[Component]] = None,
+        components: Optional[dict[str, dict[str, Any]]] = None,
         name: str = "",
     ) -> GameObject:
         """Create a new GameObject and add it to the world.
 
         Parameters
         ----------
         components
@@ -1248,15 +1380,20 @@
             component_manager=self._component_manager,
             name=name,
         )
 
         self._gameobjects[gameobject.uid] = gameobject
 
         if components:
-            for component in components:
+            for component_type, factory_args in components.items():
+
+                component = self.world.gameobjects.component_factories[
+                    component_type
+                ].instantiate(self.world, **factory_args)
+
                 gameobject.add_component(component)
 
         gameobject.activate()
 
         return gameobject
 
     def get_gameobject(self, gameobject_id: int) -> GameObject:
@@ -1307,14 +1444,17 @@
         """
         gameobject = self._gameobjects[gameobject.uid]
 
         self._dead_gameobjects.append(gameobject.uid)
 
         # Deactivate first
         gameobject.deactivate()
+        gameobject.dispatch_event(
+            Event("destroyed", world=self.world, gameobject=gameobject)
+        )
 
         # Destroy all children
         for child in gameobject.children:
             self.destroy_gameobject(child)
 
         # Destroy attached components
         for component_type in reversed(gameobject.get_component_types()):
@@ -1345,54 +1485,54 @@
 _T8 = TypeVar("_T8", bound=Component)
 
 
 class World:
     """Manages Gameobjects, Systems, events, and resources."""
 
     __slots__ = (
-        "_resource_manager",
-        "_gameobject_manager",
-        "_system_manager",
-        "_event_manager",
+        "resources",
+        "gameobjects",
+        "systems",
+        "events",
     )
 
-    _gameobject_manager: GameObjectManager
+    gameobjects: GameObjectManager
     """Manages GameObjects and Component data."""
-    _resource_manager: ResourceManager
+    resources: ResourceManager
     """Global resources shared by systems in the ECS."""
-    _system_manager: SystemManager
+    systems: SystemManager
     """The systems run every simulation step."""
-    _event_manager: EventManager
+    events: EventManager
     """Manages event listeners."""
 
     def __init__(self) -> None:
-        self._resource_manager = ResourceManager(self)
-        self._system_manager = SystemManager(self)
-        self._event_manager = EventManager(self)
-        self._gameobject_manager = GameObjectManager(self)
+        self.resources = ResourceManager(self)
+        self.systems = SystemManager(self)
+        self.events = EventManager(self)
+        self.gameobjects = GameObjectManager(self)
 
     @property
     def system_manager(self) -> SystemManager:
         """Get the world's system manager."""
-        return self._system_manager
+        return self.systems
 
     @property
     def gameobject_manager(self) -> GameObjectManager:
         """Get the world's gameobject manager"""
-        return self._gameobject_manager
+        return self.gameobjects
 
     @property
     def resource_manager(self) -> ResourceManager:
         """Get the world's resource manager"""
-        return self._resource_manager
+        return self.resources
 
     @property
     def event_manager(self) -> EventManager:
         """Get the world's event manager."""
-        return self._event_manager
+        return self.events
 
     def get_component(self, component_type: Type[_CT]) -> list[tuple[int, _CT]]:
         """Get all the GameObjects that have a given component type.
 
         Parameters
         ----------
         component_type
@@ -1400,15 +1540,15 @@
 
         Returns
         -------
         list[tuple[int, _CT]]
             A list of tuples containing the ID of a GameObject and its respective
             component instance.
         """
-        return self._gameobject_manager.component_manager.get_component(  # type: ignore
+        return self.gameobjects.component_manager.get_component(  # type: ignore
             component_type
         )
 
     @overload
     def get_components(
         self, component_types: tuple[Type[_T1]]
     ) -> list[tuple[int, tuple[_T1]]]: ...
@@ -1522,19 +1662,17 @@
             list[tuple[int, tuple[_T1, _T2, _T3, _T4, _T5, _T6]]],
             list[tuple[int, tuple[_T1, _T2, _T3, _T4, _T5, _T6, _T7]]],
             list[tuple[int, tuple[_T1, _T2, _T3, _T4, _T5, _T6, _T7, _T8]]],
         ]
             list of tuples containing a GameObject ID and an additional tuple with
             the instances of the given component types, in-order.
         """
-        ret = self._gameobject_manager.component_manager.get_components(
-            *component_types
-        )
+        ret = self.gameobjects.component_manager.get_components(*component_types)
 
         # We have to ignore the type because of esper's lax type hinting for
         # world.get_components()
         return ret  # type: ignore
 
     def step(self) -> None:
         """Advance the simulation as single tick and call all the systems."""
-        self._gameobject_manager.clear_dead_gameobjects()
-        self._system_manager.update_systems()
+        self.gameobjects.clear_dead_gameobjects()
+        self.systems.update_systems()
```

### Comparing `neighborly-2.5.0/src/neighborly/effects/base_types.py` & `neighborly-3.0.0.dev1/src/neighborly/effects/base_types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 """Abstract base types for implementing Effects.
 
 """
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Any
+from typing import Any, ClassVar
 
 from neighborly.ecs import GameObject, World
 
 
 class Effect(ABC):
     """Abstract base class for all effect objects."""
 
+    __effect_name__: ClassVar[str] = ""
+
+    def __init__(self) -> None:
+        super().__init__()
+        if not self.__effect_name__:
+            raise ValueError(
+                f"Please specify __effect_name__ class attribute for {type(self)}"
+            )
+
     @property
     @abstractmethod
     def description(self) -> str:
         """Get a string description of the effect."""
         raise NotImplementedError()
 
     @abstractmethod
@@ -31,9 +40,14 @@
 
     @classmethod
     @abstractmethod
     def instantiate(cls, world: World, params: dict[str, Any]) -> Effect:
         """Construct a new instance of the effect type using a data dict."""
         raise NotImplementedError()
 
+    @classmethod
+    def effect_name(cls) -> str:
+        """Get the effect name used in data files."""
+        return cls.__effect_name__
+
     def __str__(self) -> str:
         return self.description
```

### Comparing `neighborly-2.5.0/src/neighborly/helpers/content_selection.py` & `neighborly-3.0.0.dev1/src/neighborly/helpers/content_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from typing import Iterable, TypeVar
 
 _T = TypeVar("_T")
 
 
 def get_with_tags(
-    options: list[tuple[_T, Iterable[str]]], tags: Iterable[str]
+    options: Iterable[tuple[_T, Iterable[str]]], tags: Iterable[str]
 ) -> list[_T]:
     """Get a definition from the library with the given tags.
 
     Parameters
     ----------
     options
         Tuples of items with their tags.
```

### Comparing `neighborly-2.5.0/src/neighborly/helpers/relationship.py` & `neighborly-3.0.0.dev1/src/neighborly/helpers/relationship.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Relationship System Helper Functions.
 
 """
 
+from neighborly.components.beliefs import AppliedBeliefs, Belief, HeldBeliefs
 from neighborly.components.relationship import (
     Relationship,
     Relationships,
-    SocialRule,
-    SocialRules,
+    Reputation,
+    Romance,
 )
-from neighborly.components.stats import Stat, Stats
+from neighborly.components.stats import Stats
 from neighborly.components.traits import Traits
-from neighborly.ecs import GameObject
-from neighborly.helpers.stats import add_stat
-from neighborly.helpers.traits import has_trait
+from neighborly.ecs import Event, GameObject
+from neighborly.libraries import BeliefLibrary
 
 
 def add_relationship(owner: GameObject, target: GameObject) -> GameObject:
     """
     Creates a new relationship from the subject to the target
 
     Parameters
@@ -30,47 +30,43 @@
     -------
     GameObject
         The new relationship instance
     """
     if has_relationship(owner, target):
         return get_relationship(owner, target)
 
-    relationship = owner.world.gameobject_manager.spawn_gameobject(
-        components=[
-            Relationship(owner=owner, target=target),
-            Stats(),
-            SocialRules(),
-            Traits(),
-        ],
-    )
+    relationship = owner.world.gameobject_manager.spawn_gameobject()
 
-    add_stat(relationship, "reputation", Stat(base_value=0, bounds=(-100, 100)))
-    add_stat(relationship, "romance", Stat(base_value=0, bounds=(-100, 100)))
-    add_stat(relationship, "compatibility", Stat(base_value=0))
-    add_stat(relationship, "romantic_compatibility", Stat(base_value=0))
-    add_stat(relationship, "interaction_score", Stat(base_value=0, bounds=(0, 10)))
+    relationship.add_component(Relationship(owner=owner, target=target))
+    relationship.add_component(Stats())
+    relationship.add_component(Traits())
+    relationship.add_component(Reputation())
+    relationship.add_component(Romance())
+    relationship.add_component(AppliedBeliefs())
 
-    relationship.name = f"{owner.name} -> {target.name}"
+    relationship.name = f"[{owner.name} -> {target.name}]"
 
     owner.get_component(Relationships).add_outgoing_relationship(target, relationship)
     target.get_component(Relationships).add_incoming_relationship(owner, relationship)
 
-    # Apply outgoing social rules from the owner
-    owner_social_rules = owner.get_component(SocialRules).rules
-    for rule in owner_social_rules:
-        if rule.is_outgoing and rule.check_preconditions(relationship):
-            rule.apply(relationship)
-            relationship.get_component(SocialRules).add_rule(rule)
-
-    # Apply incoming social rules from the target
-    target_social_rules = target.get_component(SocialRules).rules
-    for rule in target_social_rules:
-        if rule.is_outgoing is False and rule.check_preconditions(relationship):
-            rule.apply(relationship)
-            relationship.get_component(SocialRules).add_rule(rule)
+    # Add outgoing relationship effects from owner
+    for trait_instance in owner.get_component(Traits).traits.values():
+        for effect in trait_instance.trait.outgoing_relationship_effects:
+            effect.apply(relationship)
+
+    # Add incoming relationship effects from target
+    for trait_instance in target.get_component(Traits).traits.values():
+        for effect in trait_instance.trait.incoming_relationship_effects:
+            effect.apply(relationship)
+
+    reevaluate_relationship(relationship.get_component(Relationship))
+
+    relationship.world.events.dispatch_event(
+        Event("relationship-added", world=relationship.world, relationship=relationship)
+    )
 
     return relationship
 
 
 def get_relationship(
     owner: GameObject,
     target: GameObject,
@@ -137,110 +133,115 @@
         target.get_component(Relationships).remove_incoming_relationship(owner)
         relationship.destroy()
         return True
 
     return False
 
 
-def get_relationships_with_traits(
-    gameobject: GameObject, *traits: str
-) -> list[GameObject]:
-    """Get all the relationships with the given tags.
+def add_belief(agent: GameObject, belief_id: str) -> None:
+    """Add a belief to an agent.
 
     Parameters
     ----------
-    gameobject
-        The character to check.
-    *traits
-        The trait IDs to check for on relationships.
-
-    Returns
-    -------
-    list[GameObject]
-        Relationships with the given traits.
+    agent
+        The agent that will hold the belief.
+    belief_id
+        The ID of the belief to add.
     """
-    matches: list[GameObject] = []
+    library = agent.world.resource_manager.get_resource(BeliefLibrary)
+    held_beliefs = agent.get_component(HeldBeliefs)
 
-    for _, relationship in gameobject.get_component(Relationships).outgoing.items():
-        if all(has_trait(relationship, trait) for trait in traits):
-            matches.append(relationship)
+    if held_beliefs.has_belief(belief_id):
+        # Add the belief to increment the internal belief reference counter.
+        held_beliefs.add_belief(belief_id)
+        return
 
-    return matches
+    belief = library.get_belief(belief_id)
+    held_beliefs.add_belief(belief_id)
 
+    relationships = agent.get_component(Relationships).outgoing
 
-def add_social_rule(gameobject: GameObject, rule: SocialRule) -> None:
-    """Add a social rule to a GameObject.
+    for _, relationship in relationships.items():
+        if belief.check_preconditions(relationship):
+            belief.apply_effects(relationship)
+
+
+def remove_belief(agent: GameObject, belief_id: str) -> None:
+    """Remove a belief from an agent.
 
     Parameters
     ----------
-    gameobject
-        The GameObject to add the social rule to.
-    rule
-        The rule to add.
+    agent
+        The agent to modify.
+    belief_id
+        The ID of the belief to remove.
     """
-    gameobject.get_component(SocialRules).add_rule(rule)
+    library = agent.world.resource_manager.get_resource(BeliefLibrary)
+    held_beliefs = agent.get_component(HeldBeliefs)
 
-    if rule.is_outgoing:
-        # Apply the rule to outgoing relationships
-        relationships = gameobject.get_component(Relationships).outgoing
-    else:
-        # Apply the rule to incoming relationships
-        relationships = gameobject.get_component(Relationships).incoming
+    if not held_beliefs.has_belief(belief_id):
+        return
 
-    # Apply this rule to all relationships
-    for _, relationship in relationships.items():
-        if rule.check_preconditions(relationship):
-            relationship.get_component(SocialRules).add_rule(rule)
-            rule.apply(relationship)
+    held_beliefs.remove_belief(belief_id)
 
+    # If the agent still has the belief, then there is something else like a trait
+    # that still requires this belief to be present.
+    if held_beliefs.has_belief(belief_id):
+        return
 
-def remove_social_rule(gameobject: GameObject, rule: SocialRule) -> None:
-    """Remove a social rule from a GameObject.
+    # If the belief is no longer held by the agent, remove the effects from all
+    # outgoing relationships.
 
-    Parameters
-    ----------
-    gameobject
-        The GameObject to remove the social rule from.
-    rule
-        The rule to remove.
-    """
-    gameobject.get_component(SocialRules).add_rule(rule)
+    belief = library.get_belief(belief_id)
 
-    if rule.is_outgoing:
-        # Remove the rule from outgoing relationships
-        relationships = gameobject.get_component(Relationships).outgoing
-    else:
-        # Remove the rule from incoming relationships
-        relationships = gameobject.get_component(Relationships).incoming
+    relationships = agent.get_component(Relationships).outgoing
 
     for _, relationship in relationships.items():
-        relationship_rules = relationship.get_component(SocialRules)
-        if relationship_rules.has_rule(rule):
-            rule.remove(relationship)
-            relationship_rules.remove_rule(rule)
+        applied_beliefs = relationship.get_component(AppliedBeliefs)
 
-    gameobject.get_component(SocialRules).remove_rule(rule)
+        if applied_beliefs.has_belief(belief_id):
+            applied_beliefs.remove_belief(belief_id)
+            belief.remove_effects(relationship)
 
 
-def remove_all_social_rules_from_source(gameobject: GameObject, source: object) -> None:
-    """Remove all social rules with a given source.
+def reevaluate_relationship(relationship: Relationship) -> None:
+    """Reevaluate beliefs for a given relationship."""
 
-    Parameters
-    ----------
-    gameobject
-        The GameObject modify.
-    source
-        The source object to check for.
-    """
-    # Remove the effects of this social rule from all current relationships.
-    rules = list(gameobject.get_component(SocialRules).rules)
+    library = relationship.gameobject.world.resource_manager.get_resource(BeliefLibrary)
+
+    applied_beliefs = relationship.gameobject.get_component(AppliedBeliefs)
+
+    held_beliefs = relationship.owner.get_component(HeldBeliefs)
+
+    # Check that existing rules still pass their preconditions
+
+    beliefs_to_remove: list[Belief] = []
+
+    for belief_id in held_beliefs.get_all():
+        belief = library.get_belief(belief_id)
+
+        if belief.check_preconditions(relationship.gameobject):
+            if not applied_beliefs.has_belief(belief_id):
+                applied_beliefs.add_belief(belief_id)
+                belief.apply_effects(relationship.gameobject)
+        else:
+            if applied_beliefs.has_belief(belief_id):
+                beliefs_to_remove.append(belief)
+
+    for belief in beliefs_to_remove:
+        applied_beliefs.remove_belief(belief.belief_id)
+        belief.remove_effects(relationship.gameobject)
+
+    # Check if any global beliefs should be applied
 
-    for rule in rules:
-        if rule.source == source:
-            remove_social_rule(gameobject, rule)
+    for belief_id in library.global_beliefs:
+        belief = library.get_belief(belief_id)
+        if belief.check_preconditions(relationship.gameobject):
+            applied_beliefs.add_belief(belief_id)
+            belief.apply_effects(relationship.gameobject)
 
 
 def deactivate_relationships(gameobject: GameObject) -> None:
     """Deactivates all an objects incoming and outgoing relationships."""
 
     relationships = gameobject.get_component(Relationships)
```

### Comparing `neighborly-2.5.0/src/neighborly/helpers/settlement.py` & `neighborly-3.0.0.dev1/src/neighborly/helpers/settlement.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,111 +1,69 @@
 """Helper functions for managing Settlements.
 
 """
 
 from __future__ import annotations
 
-from typing import Optional
-
-from neighborly.components.settlement import Settlement
-from neighborly.defs.base_types import (
-    DistrictDef,
-    DistrictGenOptions,
-    SettlementDef,
-    SettlementGenOptions,
-)
+from neighborly.components.location import CurrentSettlement
+from neighborly.components.settlement import District, Settlement
 from neighborly.ecs import GameObject, World
 from neighborly.libraries import DistrictLibrary, SettlementLibrary
 
 
-def create_settlement(
-    world: World, definition_id: str, options: Optional[SettlementGenOptions] = None
-) -> GameObject:
+def create_settlement(world: World, definition_id: str) -> GameObject:
     """Create a new settlement.
 
     Parameters
     ----------
     world
         The world instance to spawn the settlement in.
     definition_id
         The ID of the definition to instantiate.
-    options
-        Generation options.
-
     Returns
     -------
     GameObject
         The settlement.
     """
     library = world.resource_manager.get_resource(SettlementLibrary)
 
-    settlement_def = library.get_definition(definition_id)
-
-    options = options if options else SettlementGenOptions()
-
-    settlement = settlement_def.instantiate(world, options)
-
-    return settlement
+    return library.factory.create_settlement(world, definition_id)
 
 
 def create_district(
     world: World,
-    settlement: GameObject,
     definition_id: str,
-    options: Optional[DistrictGenOptions] = None,
 ) -> GameObject:
     """Create a new district GameObject.
 
     Parameters
     ----------
     world
         The world instance spawn the district in.
-    settlement
-        The settlement that owns district belongs to.
     definition_id
         The ID of the definition to instantiate.
-    options
-        Generation options.
 
     Returns
     -------
     GameObject
         The district.
     """
     library = world.resource_manager.get_resource(DistrictLibrary)
 
-    district_def = library.get_definition(definition_id)
-
-    options = options if options else DistrictGenOptions()
-
-    district = district_def.instantiate(world, settlement, options)
-
-    settlement.get_component(Settlement).add_district(district)
+    return library.factory.create_district(world, definition_id)
 
-    return district
 
+def add_district_to_settlement(settlement: Settlement, district: District) -> None:
+    """Add a district to a settlement."""
 
-def register_settlement_def(world: World, definition: SettlementDef) -> None:
-    """Add a new settlement definition for the SettlementLibrary.
-
-    Parameters
-    ----------
-    world
-        The world instance containing the settlement library.
-    definition
-        The definition to add.
-    """
-    world.resource_manager.get_resource(SettlementLibrary).add_definition(definition)
+    settlement.districts.append(district.gameobject)
+    district.gameobject.add_component(
+        CurrentSettlement(settlement=settlement.gameobject)
+    )
 
 
-def register_district_def(world: World, definition: DistrictDef) -> None:
-    """Add a new district definition for the DistrictLibrary.
+def remove_district_from_settlement(settlement: Settlement, district: District) -> None:
+    """Remove a district from this settlement."""
 
-    Parameters
-    ----------
-    world
-        The world instance containing the district library.
-    definition
-        The definition to add.
-    """
-    world.resource_manager.get_resource(DistrictLibrary).add_definition(definition)
-    world.resource_manager.get_resource(DistrictLibrary).add_definition(definition)
+    settlement.districts.remove(district.gameobject)
+    district.gameobject.remove_component(CurrentSettlement)
+    settlement.gameobject.add_child(district.gameobject)
```

### Comparing `neighborly-2.5.0/src/neighborly/helpers/skills.py` & `neighborly-3.0.0.dev1/src/neighborly/helpers/skills.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Skill System Helper Functions.
 
 """
 
-from neighborly.components.skills import Skills
-from neighborly.components.stats import Stat
+from neighborly.components.skills import SkillInstance, Skills
 from neighborly.ecs import GameObject
 from neighborly.libraries import SkillLibrary
 
 
 def add_skill(gameobject: GameObject, skill_id: str, base_value: float = 0.0) -> None:
     """Add a new skill to a character with the given base value.
 
@@ -36,30 +35,25 @@
         The ID of the skill to check for.
 
     Returns
     -------
     bool
         True if the character has the skill, False otherwise.
     """
-    library = gameobject.world.resource_manager.get_resource(SkillLibrary)
-    skill = library.get_skill(skill_id)
-    return gameobject.get_component(Skills).has_skill(skill)
+    return skill_id in gameobject.get_component(Skills).skills
 
 
-def get_skill(gameobject: GameObject, skill_id: str) -> Stat:
+def get_skill(gameobject: GameObject, skill_id: str) -> SkillInstance:
     """Get a character's skill stat.
 
     Parameters
     ----------
     gameobject
         The character to check.
     skill_id
         The ID of the skill to retrieve.
 
     Returns
     -------
-    Stat
-        The stat associated with this skill.
+    SkillInstance
     """
-    library = gameobject.world.resource_manager.get_resource(SkillLibrary)
-    skill = library.get_skill(skill_id)
-    return gameobject.get_component(Skills).get_skill(skill)
+    return gameobject.get_component(Skills).skills[skill_id]
```

### Comparing `neighborly-2.5.0/src/neighborly/helpers/stats.py` & `neighborly-3.0.0.dev1/src/neighborly/helpers/stats.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,39 +4,14 @@
 
 from __future__ import annotations
 
 from neighborly.components.stats import Stat, Stats
 from neighborly.ecs import GameObject
 
 
-def add_stat(
-    gameobject: GameObject,
-    stat_id: str,
-    stat: Stat,
-) -> Stat:
-    """Add a new stat to the gameobject.
-
-    Parameters
-    ----------
-    gameobject
-        The GameObject to add a stat to.
-    stat_id
-        The ID to associate the stat with.
-    stat
-        The stat instance to add.
-
-    Returns
-    -------
-    Stat
-        The newly created stat.
-    """
-    gameobject.get_component(Stats).add_stat(stat_id, stat)
-    return stat
-
-
 def has_stat(gameobject: GameObject, stat_id: str) -> bool:
     """Check if a GameObject has a stat.
 
     Parameters
     ----------
     gameobject
         The GameObject to check.
@@ -63,25 +38,7 @@
 
     Returns
     -------
     Stat
         The stat.
     """
     return gameobject.get_component(Stats).get_stat(stat_id)
-
-
-def remove_stat(gameobject: GameObject, stat_id: str) -> bool:
-    """Remove a stat from a GameObject.
-
-    Parameters
-    ----------
-    gameobject
-        A GameObject.
-    stat_id
-        The definition ID of a stat to remove.
-
-    Returns
-    -------
-    bool
-        True if the stat was removed successfully. False otherwise.
-    """
-    return gameobject.get_component(Stats).remove_stat(stat_id)
```

### Comparing `neighborly-2.5.0/src/neighborly/loaders.py` & `neighborly-3.0.0.dev1/src/neighborly/loaders.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,32 +4,43 @@
 simulation data into a simulation.
 
 """
 
 from __future__ import annotations
 
 import os
-from typing import Any, Type, Union
+from typing import Any, Union
 
 import yaml
 
+from neighborly.defs.base_types import (
+    BeliefDef,
+    BusinessDef,
+    CharacterDef,
+    DistrictDef,
+    JobRoleDef,
+    LocationPreferenceDef,
+    SettlementDef,
+    SkillDef,
+    SpeciesDef,
+    TraitDef,
+)
 from neighborly.libraries import (
+    BeliefLibrary,
     BusinessLibrary,
     CharacterLibrary,
     DistrictLibrary,
     JobRoleLibrary,
-    LifeEventLibrary,
-    ResidenceLibrary,
+    LocationPreferenceLibrary,
     SettlementLibrary,
     SkillLibrary,
+    SpeciesLibrary,
     TraitLibrary,
 )
-from neighborly.life_event import LifeEvent
 from neighborly.simulation import Simulation
-from neighborly.tracery import Tracery
 
 
 def load_districts(
     sim: Simulation, file_path: Union[os.PathLike[str], str, bytes]
 ) -> None:
     """Load settlement district definition data from a data file.
 
@@ -42,39 +53,16 @@
     """
     with open(file_path, "r", encoding="utf8") as file:
         data: dict[str, dict[str, Any]] = yaml.safe_load(file)
 
     district_library = sim.world.resource_manager.get_resource(DistrictLibrary)
 
     for district_id, params in data.items():
-        district_library.add_definition_from_obj(
-            {"definition_id": district_id, **params}
-        )
-
-
-def load_residences(
-    sim: Simulation, file_path: Union[os.PathLike[str], str, bytes]
-) -> None:
-    """Load residential building definition data from a data file.
-
-    Parameters
-    ----------
-    sim
-        The simulation instance to load the data into
-    file_path
-        The path to the data file.
-    """
-    with open(file_path, "r", encoding="utf8") as file:
-        data: dict[str, dict[str, Any]] = yaml.safe_load(file)
-
-    residence_library = sim.world.resource_manager.get_resource(ResidenceLibrary)
-
-    for residence_id, params in data.items():
-        residence_library.add_definition_from_obj(
-            {"definition_id": residence_id, **params}
+        district_library.add_definition(
+            DistrictDef.model_validate({"definition_id": district_id, **params})
         )
 
 
 def load_settlements(
     sim: Simulation, file_path: Union[os.PathLike[str], str, bytes]
 ) -> None:
     """Load settlement definition data from a data file.
@@ -88,16 +76,16 @@
     """
     with open(file_path, "r", encoding="utf8") as file:
         data: dict[str, dict[str, Any]] = yaml.safe_load(file)
 
     settlement_library = sim.world.resource_manager.get_resource(SettlementLibrary)
 
     for settlement_id, params in data.items():
-        settlement_library.add_definition_from_obj(
-            {"definition_id": settlement_id, **params}
+        settlement_library.add_definition(
+            SettlementDef.model_validate({"definition_id": settlement_id, **params})
         )
 
 
 def load_businesses(
     sim: Simulation, file_path: Union[os.PathLike[str], str, bytes]
 ) -> None:
     """Load business definition data from a data file.
@@ -111,16 +99,16 @@
     """
     with open(file_path, "r", encoding="utf8") as file:
         data: dict[str, dict[str, Any]] = yaml.safe_load(file)
 
     business_library = sim.world.resource_manager.get_resource(BusinessLibrary)
 
     for business_id, params in data.items():
-        business_library.add_definition_from_obj(
-            {"definition_id": business_id, **params}
+        business_library.add_definition(
+            BusinessDef.model_validate({"definition_id": business_id, **params})
         )
 
 
 def load_job_roles(
     sim: Simulation, file_path: Union[os.PathLike[str], str, bytes]
 ) -> None:
     """Load business definition data from a data file.
@@ -134,15 +122,17 @@
     """
     with open(file_path, "r", encoding="utf8") as file:
         data: dict[str, dict[str, Any]] = yaml.safe_load(file)
 
     job_role_library = sim.world.resource_manager.get_resource(JobRoleLibrary)
 
     for entry_id, params in data.items():
-        job_role_library.add_definition_from_obj({"definition_id": entry_id, **params})
+        job_role_library.add_definition(
+            JobRoleDef.model_validate({"definition_id": entry_id, **params})
+        )
 
 
 def load_characters(
     sim: Simulation, file_path: Union[os.PathLike[str], str, bytes]
 ) -> None:
     """Load character definition data from a data file.
 
@@ -156,16 +146,16 @@
 
     with open(file_path, "r", encoding="utf8") as file:
         data: dict[str, dict[str, Any]] = yaml.safe_load(file)
 
     character_library = sim.world.resource_manager.get_resource(CharacterLibrary)
 
     for character_id, params in data.items():
-        character_library.add_definition_from_obj(
-            {"definition_id": character_id, **params}
+        character_library.add_definition(
+            CharacterDef.model_validate({"definition_id": character_id, **params})
         )
 
 
 def load_traits(
     sim: Simulation, file_path: Union[os.PathLike[str], str, bytes]
 ) -> None:
     """Load trait definition data from a data file.
@@ -180,32 +170,41 @@
 
     with open(file_path, "r", encoding="utf8") as file:
         data: dict[str, dict[str, Any]] = yaml.safe_load(file)
 
     trait_library = sim.world.resource_manager.get_resource(TraitLibrary)
 
     for trait_id, params in data.items():
-        trait_library.add_definition_from_obj({"definition_id": trait_id, **params})
+        trait_library.add_definition(
+            TraitDef.model_validate({"definition_id": trait_id, **params})
+        )
 
 
-def load_tracery(
+def load_species(
     sim: Simulation, file_path: Union[os.PathLike[str], str, bytes]
 ) -> None:
-    """Loads Tracery rules from a JSON file.
+    """Load species definition data from a data file.
 
     Parameters
     ----------
     sim
-        The simulation instance.
+        The simulation instance to load the data into
     file_path
-        The path of the data file to load.
+        The path to the data file.
     """
+
     with open(file_path, "r", encoding="utf8") as file:
-        rule_data: dict[str, list[str]] = yaml.safe_load(file)
-        sim.world.resource_manager.get_resource(Tracery).add_rules(rule_data)
+        data: dict[str, dict[str, Any]] = yaml.safe_load(file)
+
+    library = sim.world.resource_manager.get_resource(SpeciesLibrary)
+
+    for definition_id, params in data.items():
+        library.add_definition(
+            SpeciesDef.model_validate({"definition_id": definition_id, **params})
+        )
 
 
 def load_skills(
     sim: Simulation, file_path: Union[os.PathLike[str], str, bytes]
 ) -> None:
     """Load skill definition data from a data file.
 
@@ -219,15 +218,38 @@
 
     with open(file_path, "r", encoding="utf8") as file:
         data: dict[str, dict[str, Any]] = yaml.safe_load(file)
 
     library = sim.world.resource_manager.get_resource(SkillLibrary)
 
     for definition_id, params in data.items():
-        library.add_definition_from_obj({"definition_id": definition_id, **params})
+        library.add_definition(
+            SkillDef.model_validate({"definition_id": definition_id, **params})
+        )
+
+
+def load_beliefs(
+    sim: Simulation, file_path: Union[os.PathLike[str], str, bytes]
+) -> None:
+    """Load beliefs from a file."""
+
+    with open(file_path, "r", encoding="utf8") as file:
+        data: list[dict[str, Any]] = yaml.safe_load(file)
+
+    library = sim.world.resource_manager.get_resource(BeliefLibrary)
+
+    for entry in data:
+        library.add_definition(BeliefDef.model_validate(entry))
+
+
+def load_location_preferences(
+    sim: Simulation, file_path: Union[os.PathLike[str], str, bytes]
+) -> None:
+    """Load location preference rules from a file."""
+
+    with open(file_path, "r", encoding="utf8") as file:
+        data: list[dict[str, Any]] = yaml.safe_load(file)
 
+    library = sim.world.resource_manager.get_resource(LocationPreferenceLibrary)
 
-def register_life_event_type(sim: Simulation, life_event_type: Type[LifeEvent]) -> None:
-    """Register a LifeEvent subtype with the simulation's library."""
-    sim.world.resource_manager.get_resource(LifeEventLibrary).add_event_type(
-        life_event_type
-    )
+    for entry in data:
+        library.add_definition(LocationPreferenceDef.model_validate(entry))
```

### Comparing `neighborly-2.5.0/src/neighborly/preconditions/base_types.py` & `neighborly-3.0.0.dev1/src/neighborly/preconditions/base_types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 """Abstract base types for implementing preconditions.
 
 """
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Any
+from typing import Any, ClassVar
 
-from neighborly.ecs import GameObject, World
+from neighborly.ecs import World
 
 
 class Precondition(ABC):
     """Abstract base class for all precondition objects."""
 
+    __precondition_name__: ClassVar[str] = ""
+
+    def __init__(self) -> None:
+        super().__init__()
+        if not self.__precondition_name__:
+            raise ValueError(
+                f"Please specify __precondition_name__ class attribute for {type(self)}"
+            )
+
     @property
     @abstractmethod
     def description(self) -> str:
-        """Get a string description of the effect."""
+        """Get a string description of the precondition."""
         raise NotImplementedError()
 
     @abstractmethod
-    def __call__(self, target: GameObject) -> bool:
-        """Check if a GameObject passes the precondition.
+    def check(self, blackboard: dict[str, Any]) -> bool:
+        """Check if the precondition passes given a blackboard of values.
 
         Parameters
         ----------
-        target
-            A GameObject
+        blackboard
+            Information about the context of the precondition.
 
         Returns
         -------
         bool
             True if the gameobject passes the precondition, False otherwise.
         """
         raise NotImplementedError()
@@ -45,9 +54,14 @@
         world
             The simulation's world instance
         params
             Keyword parameters to pass to the precondition.
         """
         raise NotImplementedError()
 
+    @classmethod
+    def precondition_name(cls) -> str:
+        """Get the precondition name used in data files."""
+        return cls.__precondition_name__
+
     def __str__(self) -> str:
         return self.description
```

### Comparing `neighborly-2.5.0/src/neighborly/simulation.py` & `neighborly-3.0.0.dev1/src/neighborly/simulation.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,87 +8,123 @@
 
 import json
 import logging
 import pathlib
 import random
 from typing import Optional
 
+import tqdm
+
 from neighborly.config import SimulationConfig
-from neighborly.data_collection import DataCollectionSystems, DataTables
-from neighborly.datetime import SimDate
-from neighborly.defs.defaults import (
-    DefaultBusinessDef,
-    DefaultCharacterDef,
-    DefaultDistrictDef,
-    DefaultJobRoleDef,
-    DefaultResidenceDef,
-    DefaultSettlementDef,
-    DefaultSkillDef,
-    DefaultSpeciesDef,
-    DefaultTraitDef,
-)
+from neighborly.datetime import MONTHS_PER_YEAR, SimDate
 from neighborly.ecs import World
 from neighborly.effects.effects import (
+    AddBelief,
     AddLocationPreference,
-    AddSocialRule,
-    IncreaseSkill,
-    StatBuff,
+    AddSkillBuff,
+    AddSkillDebuff,
+    AddStatBuff,
+    AddStatDebuff,
+    DecreaseBaseSkill,
+    DecreaseBaseStat,
+    IncreaseBaseSkill,
+    IncreaseBaseStat,
+)
+from neighborly.factories.beliefs import AgentBeliefsFactory, AppliedBeliefsFactory
+from neighborly.factories.business import BusinessFactory, DefaultBusinessFactory
+from neighborly.factories.character import (
+    CharacterFactory,
+    DefaultCharacterFactory,
+    DefaultChildFactory,
+    SpeciesFactory,
+)
+from neighborly.factories.location import (
+    FrequentedLocationsFactory,
+    LocationFactory,
+    LocationPreferencesFactory,
+)
+from neighborly.factories.relationships import RelationshipsFactory
+from neighborly.factories.settlement import (
+    DefaultDistrictFactory,
+    DefaultSettlementFactory,
+    DistrictFactory,
+    SettlementFactory,
 )
-from neighborly.helpers.traits import register_trait_def
+from neighborly.factories.shared import AgeFactory, PersonalEventHistoryFactory
+from neighborly.factories.skills import SkillsFactory
+from neighborly.factories.spawn_table import (
+    BusinessSpawnTableFactory,
+    CharacterSpawnTableFactory,
+    DistrictSpawnTableFactory,
+)
+from neighborly.factories.stats import (
+    CharmFactory,
+    CourageFactory,
+    DisciplineFactory,
+    FertilityFactory,
+    IntelligenceFactory,
+    KindnessFactory,
+    LifespanFactory,
+    SociabilityFactory,
+    StatsFactory,
+    StewardshipFactory,
+)
+from neighborly.factories.traits import TraitsFactory
 from neighborly.libraries import (
+    ActionConsiderationLibrary,
+    BeliefLibrary,
     BusinessLibrary,
+    BusinessNameFactories,
     CharacterLibrary,
+    CharacterNameFactories,
     DistrictLibrary,
+    DistrictNameFactories,
     EffectLibrary,
     JobRoleLibrary,
-    LifeEventLibrary,
+    LocationPreferenceLibrary,
     PreconditionLibrary,
-    ResidenceLibrary,
     SettlementLibrary,
+    SettlementNameFactories,
     SkillLibrary,
+    SpeciesLibrary,
     TraitLibrary,
 )
-from neighborly.life_event import EventConsiderations, GlobalEventHistory
+from neighborly.life_event import GlobalEventHistory
 from neighborly.preconditions.defaults import (
-    AtLeastLifeStage,
+    GenderRequirement,
     HasTrait,
+    LifeStageRequirement,
     SkillRequirement,
-    TargetHasTrait,
-    TargetIsSex,
-    TargetLifeStageLT,
+    StatRequirement,
 )
 from neighborly.systems import (
     AgingSystem,
+    BusinessLifespanSystem,
+    CharacterLifespanSystem,
     ChildBirthSystem,
+    CompileBeliefDefsSystem,
     CompileBusinessDefsSystem,
     CompileCharacterDefsSystem,
     CompileDistrictDefsSystem,
-    CompileResidenceDefsSystem,
+    CompileJobRoleDefsSystem,
+    CompileLocationPreferenceDefsSystem,
     CompileSettlementDefsSystem,
-    DeathSystem,
+    CompileSkillDefsSystem,
+    CompileSpeciesDefsSystem,
+    CompileTraitDefsSystem,
     EarlyUpdateSystems,
-    HealthDecaySystem,
     InitializationSystems,
     InitializeSettlementSystem,
-    InstantiateJobRolesSystem,
-    InstantiateSkillsSystem,
-    InstantiateTraitsSystem,
     JobRoleMonthlyEffectsSystem,
     LateUpdateSystems,
-    LifeEventSystem,
-    MeetNewPeopleSystem,
-    PassiveReputationChange,
-    PassiveRomanceChange,
-    SpawnNewBusinessesSystem,
+    LifeStageSystem,
     SpawnNewResidentSystem,
-    SpawnResidentialBuildingsSystem,
     UpdateFrequentedLocationSystem,
     UpdateSystems,
 )
-from neighborly.tracery import Tracery
 
 
 class Simulation:
     """A Neighborly simulation instance."""
 
     __slots__ = "_config", "_world"
 
@@ -110,72 +146,85 @@
         self._world = World()
 
         # Seed the global rng for third-party packages
         random.seed(self._config.seed)
 
         self._init_resources()
         self._init_systems()
-        self._init_effects()
-        self._init_preconditions()
-        self._init_traits()
         self._init_logging()
+        self._init_component_factories()
+        self._init_effect_precondition_factories()
 
     def _init_resources(self) -> None:
         """Initialize built-in resources."""
         self.world.resource_manager.add_resource(self._config)
         self.world.resource_manager.add_resource(random.Random(self._config.seed))
         self.world.resource_manager.add_resource(SimDate())
-        self.world.resource_manager.add_resource(DataTables())
-        self.world.resource_manager.add_resource(CharacterLibrary(DefaultCharacterDef))
-        self.world.resource_manager.add_resource(JobRoleLibrary(DefaultJobRoleDef))
-        self.world.resource_manager.add_resource(BusinessLibrary(DefaultBusinessDef))
-        self.world.resource_manager.add_resource(ResidenceLibrary(DefaultResidenceDef))
-        self.world.resource_manager.add_resource(DistrictLibrary(DefaultDistrictDef))
         self.world.resource_manager.add_resource(
-            SettlementLibrary(DefaultSettlementDef)
+            CharacterLibrary(
+                factory=DefaultCharacterFactory(), child_factory=DefaultChildFactory()
+            )
         )
-        self.world.resource_manager.add_resource(TraitLibrary(DefaultTraitDef))
-        self.world.resource_manager.get_resource(TraitLibrary).add_definition_type(
-            DefaultSpeciesDef
+        self.world.resource_manager.add_resource(JobRoleLibrary())
+        self.world.resource_manager.add_resource(
+            BusinessLibrary(factory=DefaultBusinessFactory())
+        )
+        self.world.resource_manager.add_resource(
+            DistrictLibrary(factory=DefaultDistrictFactory())
         )
+        self.world.resource_manager.add_resource(
+            SettlementLibrary(factory=DefaultSettlementFactory())
+        )
+        self.world.resource_manager.add_resource(TraitLibrary())
+        self.world.resource_manager.add_resource(SpeciesLibrary())
+        self.world.resource_manager.add_resource(SkillLibrary())
+        self.world.resource_manager.add_resource(BeliefLibrary())
+        self.world.resource_manager.add_resource(LocationPreferenceLibrary())
+        self.world.resource_manager.add_resource(SettlementNameFactories())
         self.world.resource_manager.add_resource(EffectLibrary())
-        self.world.resource_manager.add_resource(SkillLibrary(DefaultSkillDef))
         self.world.resource_manager.add_resource(PreconditionLibrary())
-        self.world.resource_manager.add_resource(LifeEventLibrary())
-        self.world.resource_manager.add_resource(Tracery(self._config.seed))
+        self.world.resource_manager.add_resource(DistrictNameFactories())
+        self.world.resource_manager.add_resource(CharacterNameFactories())
+        self.world.resource_manager.add_resource(BusinessNameFactories())
         self.world.resource_manager.add_resource(GlobalEventHistory())
-        self.world.resource_manager.add_resource(EventConsiderations())
+        self.world.resource_manager.add_resource(ActionConsiderationLibrary())
 
     def _init_systems(self) -> None:
         """Initialize built-in systems."""
         # Add default top-level system groups (in execution order)
         self.world.system_manager.add_system(InitializationSystems())
-        self.world.system_manager.add_system(DataCollectionSystems())
         self.world.system_manager.add_system(EarlyUpdateSystems())
         self.world.system_manager.add_system(UpdateSystems())
         self.world.system_manager.add_system(LateUpdateSystems())
 
         # Add content initialization systems
         self.world.system_manager.add_system(
-            system=InstantiateTraitsSystem(), system_group=InitializationSystems
+            system=CompileTraitDefsSystem(), system_group=InitializationSystems
         )
         self.world.system_manager.add_system(
-            system=InstantiateJobRolesSystem(), system_group=InitializationSystems
+            system=CompileSpeciesDefsSystem(), system_group=InitializationSystems
         )
         self.world.system_manager.add_system(
-            system=InstantiateSkillsSystem(), system_group=InitializationSystems
+            system=CompileBeliefDefsSystem(), system_group=InitializationSystems
         )
         self.world.system_manager.add_system(
-            system=CompileDistrictDefsSystem(), system_group=InitializationSystems
+            system=CompileLocationPreferenceDefsSystem(),
+            system_group=InitializationSystems,
         )
         self.world.system_manager.add_system(
-            system=CompileSettlementDefsSystem(), system_group=InitializationSystems
+            system=CompileJobRoleDefsSystem(), system_group=InitializationSystems
+        )
+        self.world.system_manager.add_system(
+            system=CompileSkillDefsSystem(), system_group=InitializationSystems
+        )
+        self.world.system_manager.add_system(
+            system=CompileDistrictDefsSystem(), system_group=InitializationSystems
         )
         self.world.system_manager.add_system(
-            system=CompileResidenceDefsSystem(), system_group=InitializationSystems
+            system=CompileSettlementDefsSystem(), system_group=InitializationSystems
         )
         self.world.system_manager.add_system(
             system=CompileCharacterDefsSystem(), system_group=InitializationSystems
         )
         self.world.system_manager.add_system(
             system=CompileBusinessDefsSystem(), system_group=InitializationSystems
         )
@@ -184,301 +233,104 @@
         )
 
         # Add core update systems
         self.world.system_manager.add_system(
             system=SpawnNewResidentSystem(), system_group=UpdateSystems
         )
         self.world.system_manager.add_system(
-            system=SpawnResidentialBuildingsSystem(), system_group=UpdateSystems
-        )
-        self.world.system_manager.add_system(
-            system=SpawnNewBusinessesSystem(), system_group=UpdateSystems
-        )
-        self.world.system_manager.add_system(
             system=UpdateFrequentedLocationSystem(), system_group=UpdateSystems
         )
         self.world.system_manager.add_system(
             system=AgingSystem(), system_group=UpdateSystems
         )
         self.world.system_manager.add_system(
-            system=HealthDecaySystem(), system_group=UpdateSystems
+            system=LifeStageSystem(), system_group=UpdateSystems
         )
         self.world.system_manager.add_system(
             system=ChildBirthSystem(), system_group=UpdateSystems
         )
         self.world.system_manager.add_system(
-            system=MeetNewPeopleSystem(), system_group=UpdateSystems
-        )
-        self.world.system_manager.add_system(
-            system=LifeEventSystem(), system_group=UpdateSystems
-        )
-        self.world.system_manager.add_system(
-            system=PassiveReputationChange(), system_group=UpdateSystems
-        )
-        self.world.system_manager.add_system(
-            system=PassiveRomanceChange(), system_group=UpdateSystems
+            system=JobRoleMonthlyEffectsSystem(), system_group=UpdateSystems
         )
         self.world.system_manager.add_system(
-            system=JobRoleMonthlyEffectsSystem(), system_group=UpdateSystems
+            system=CharacterLifespanSystem(), system_group=UpdateSystems
         )
         self.world.system_manager.add_system(
-            system=DeathSystem(), system_group=UpdateSystems
+            system=BusinessLifespanSystem(), system_group=UpdateSystems
         )
 
-    def _init_effects(self) -> None:
-        """Initialize built-in Effect definitions."""
-        self._world.resource_manager.get_resource(EffectLibrary).add_effect_type(
-            StatBuff
-        )
-        self._world.resource_manager.get_resource(EffectLibrary).add_effect_type(
-            IncreaseSkill
-        )
-        self._world.resource_manager.get_resource(EffectLibrary).add_effect_type(
-            AddLocationPreference
-        )
-        self._world.resource_manager.get_resource(EffectLibrary).add_effect_type(
-            AddSocialRule
-        )
-
-    def _init_preconditions(self) -> None:
-        """Initialize built-in precondition definitions."""
-        self.world.resource_manager.get_resource(
-            PreconditionLibrary
-        ).add_precondition_type(HasTrait)
-        self.world.resource_manager.get_resource(
-            PreconditionLibrary
-        ).add_precondition_type(SkillRequirement)
-        self.world.resource_manager.get_resource(
-            PreconditionLibrary
-        ).add_precondition_type(AtLeastLifeStage)
-        self.world.resource_manager.get_resource(
-            PreconditionLibrary
-        ).add_precondition_type(TargetHasTrait)
-        self.world.resource_manager.get_resource(
-            PreconditionLibrary
-        ).add_precondition_type(TargetIsSex)
-        self.world.resource_manager.get_resource(
-            PreconditionLibrary
-        ).add_precondition_type(TargetLifeStageLT)
-
-    def _init_traits(self) -> None:
-        """Initialize built-in trait definitions"""
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="employee",
-                display_name="Employee",
-                description="The target of this relationship is an employee.",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="coworker",
-                display_name="Coworker",
-                description="The target of this relationship is a coworker.",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="departed",
-                display_name="Departed",
-                description="The character has departed the simulation.",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="deceased",
-                display_name="Deceased",
-                description="The character has died.",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="retired",
-                display_name="Retired",
-                description="The character has retired from working.",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="family",
-                display_name="Family",
-                description="These characters are related",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="parent",
-                display_name="Parent",
-                description="The target of this relationship is the owner's parent",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="child",
-                display_name="Child",
-                description="The target of this relationship is the owner's child",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="sibling",
-                display_name="Sibling",
-                description="The target of this relationship is the owner's sibling",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="spouse",
-                display_name="Spouse",
-                description="The target of this relationship is the owner's spouse",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="dating",
-                display_name="dating",
-                description="The relationship target and owner are dating.",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="crush",
-                display_name="Crush",
-                description="The owner of this relationship has a crush on the target.",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="live_together",
-                display_name="Live Together",
-                description="The owner of this relationship lives with the target.",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="friend",
-                display_name="Friend",
-                description="The owner of this relationship is friends with target.",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="enemy",
-                display_name="Enemy",
-                description="The owner of this relationship is enemies with target.",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="widow",
-                display_name="Widow",
-                description="The target of the relationship is the widow of the owner.",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="step_parent",
-                display_name="Step Parent",
-                description="Target is the step parent of the owner.",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="step_child",
-                display_name="Step Child",
-                description="Target is the step child of the owner.",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="step_sibling",
-                display_name="Step Sibling",
-                description="Target is the step sibling of the owner.",
-                spawn_frequency=0,
-            ),
-        )
-
-        register_trait_def(
-            self.world,
-            DefaultTraitDef(
-                definition_id="biological_parent",
-                display_name="Biological Parent",
-                description="Target is the biological parent of the owner.",
-                spawn_frequency=0,
-            ),
-        )
+    def _init_component_factories(self) -> None:
+        """Initialize built-in component factories."""
+        self.world.gameobjects.add_component_factory(CharacterFactory())
+        self.world.gameobjects.add_component_factory(BusinessFactory())
+        self.world.gameobjects.add_component_factory(LocationFactory())
+        self.world.gameobjects.add_component_factory(LocationPreferencesFactory())
+        self.world.gameobjects.add_component_factory(FrequentedLocationsFactory())
+        self.world.gameobjects.add_component_factory(SettlementFactory())
+        self.world.gameobjects.add_component_factory(DistrictFactory())
+        self.world.gameobjects.add_component_factory(AgeFactory())
+        self.world.gameobjects.add_component_factory(SkillsFactory())
+        self.world.gameobjects.add_component_factory(TraitsFactory())
+        self.world.gameobjects.add_component_factory(StatsFactory())
+        self.world.gameobjects.add_component_factory(CharacterSpawnTableFactory())
+        self.world.gameobjects.add_component_factory(BusinessSpawnTableFactory())
+        self.world.gameobjects.add_component_factory(DistrictSpawnTableFactory())
+        self.world.gameobjects.add_component_factory(RelationshipsFactory())
+        self.world.gameobjects.add_component_factory(PersonalEventHistoryFactory())
+        self.world.gameobjects.add_component_factory(LifespanFactory())
+        self.world.gameobjects.add_component_factory(FertilityFactory())
+        self.world.gameobjects.add_component_factory(KindnessFactory())
+        self.world.gameobjects.add_component_factory(CourageFactory())
+        self.world.gameobjects.add_component_factory(StewardshipFactory())
+        self.world.gameobjects.add_component_factory(SociabilityFactory())
+        self.world.gameobjects.add_component_factory(IntelligenceFactory())
+        self.world.gameobjects.add_component_factory(DisciplineFactory())
+        self.world.gameobjects.add_component_factory(CharmFactory())
+        self.world.gameobjects.add_component_factory(AgentBeliefsFactory())
+        self.world.gameobjects.add_component_factory(AppliedBeliefsFactory())
+        self.world.gameobjects.add_component_factory(SpeciesFactory())
+
+    def _init_effect_precondition_factories(self) -> None:
+        """Add effect factories to the library."""
+
+        effect_library = self.world.resources.get_resource(EffectLibrary)
+
+        effect_library.add_effect_type(AddStatBuff)
+        effect_library.add_effect_type(AddStatDebuff)
+        effect_library.add_effect_type(IncreaseBaseStat)
+        effect_library.add_effect_type(DecreaseBaseStat)
+        effect_library.add_effect_type(AddSkillBuff)
+        effect_library.add_effect_type(AddSkillDebuff)
+        effect_library.add_effect_type(DecreaseBaseSkill)
+        effect_library.add_effect_type(IncreaseBaseSkill)
+        effect_library.add_effect_type(AddBelief)
+        effect_library.add_effect_type(AddLocationPreference)
+
+        precondition_library = self.world.resources.get_resource(PreconditionLibrary)
+
+        precondition_library.add_precondition_type(HasTrait)
+        precondition_library.add_precondition_type(SkillRequirement)
+        precondition_library.add_precondition_type(StatRequirement)
+        precondition_library.add_precondition_type(LifeStageRequirement)
+        precondition_library.add_precondition_type(GenderRequirement)
 
     def _init_logging(self) -> None:
         """Initialize simulation logging."""
         if self.config.logging.logging_enabled:
             if self.config.logging.log_to_terminal is False:
                 # Output the logs to a file
                 log_path = pathlib.Path(self.config.logging.log_file_path)
 
                 logging.basicConfig(
                     filename=log_path,
                     encoding="utf-8",
                     level=self.config.logging.log_level,
                     format="%(message)s",
                     force=True,
+                    filemode="w",
                 )
             else:
                 logging.basicConfig(
                     level=self.config.logging.log_level,
                     format="%(message)s",
                     force=True,
                 )
@@ -509,14 +361,27 @@
         initialization_system_group.set_active(False)
 
     def step(self) -> None:
         """Advance the simulation one time step (month)."""
         self._world.step()
         self.date.increment_month()
 
+    def run_for(self, years: int) -> None:
+        """Run the simulation for a given number of years."""
+
+        total_time_steps: int = years * MONTHS_PER_YEAR
+
+        if self.config.logging.log_to_terminal:
+
+            for _ in range(total_time_steps):
+                self.step()
+        else:
+            for _ in tqdm.trange(total_time_steps):
+                self.step()
+
     def to_json(self, indent: Optional[int] = None) -> str:
         """Export the simulation as a JSON string.
 
         Parameters
         ----------
         indent
             An optional amount of spaces to indent lines in the string.
@@ -531,16 +396,13 @@
             "gameobjects": {
                 str(g.uid): g.to_dict()
                 for g in self.world.gameobject_manager.gameobjects
             },
             "events": self.world.resource_manager.get_resource(
                 GlobalEventHistory
             ).to_dict(),
-            "data_tables": self.world.resource_manager.get_resource(
-                DataTables
-            ).to_dict(),
         }
 
         return json.dumps(
             serialized_data,
             indent=indent,
         )
```

### Comparing `neighborly-2.5.0/src/neighborly/systems.py` & `neighborly-3.0.0.dev1/src/neighborly/systems.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,78 +5,93 @@
 """
 
 from __future__ import annotations
 
 import logging
 import random
 from collections import defaultdict
-from typing import ClassVar, Optional
 
-import polars as pl
-
-from neighborly.components.business import (
-    Business,
-    Occupation,
-    OpenToPublic,
-    PendingOpening,
+from neighborly.components.beliefs import Belief
+from neighborly.components.business import Business, BusinessStatus, JobRole, Occupation
+from neighborly.components.character import (
+    Character,
+    Household,
+    LifeStage,
+    MemberOfHousehold,
+    Pregnant,
+    ResidentOf,
+    Sex,
+    Species,
+    SpeciesType,
 )
-from neighborly.components.character import Character, LifeStage, Pregnant, Species
 from neighborly.components.location import (
-    FrequentedBy,
+    CurrentSettlement,
     FrequentedLocations,
+    Location,
+    LocationPreferenceRule,
     LocationPreferences,
 )
 from neighborly.components.relationship import Relationship
-from neighborly.components.residence import Resident, ResidentialUnit, Vacant
-from neighborly.components.settlement import District
-from neighborly.components.spawn_table import (
-    BusinessSpawnTable,
-    CharacterSpawnTable,
-    ResidenceSpawnTable,
-)
+from neighborly.components.settlement import District, Settlement
+from neighborly.components.shared import Age
+from neighborly.components.skills import Skill
+from neighborly.components.spawn_table import CharacterSpawnTable, DistrictSpawnTable
+from neighborly.components.stats import Fertility, Lifespan
+from neighborly.components.traits import Trait, Traits, TraitType
 from neighborly.config import SimulationConfig
 from neighborly.datetime import MONTHS_PER_YEAR, SimDate
-from neighborly.defs.base_types import CharacterGenOptions
+from neighborly.defs.base_types import DistrictDef
 from neighborly.defs.definition_compiler import compile_definitions
-from neighborly.ecs import Active, GameObject, System, SystemGroup, World
+from neighborly.ecs import Active, Event, GameObject, System, SystemGroup, World
 from neighborly.events.defaults import (
     BecomeAdolescentEvent,
     BecomeAdultEvent,
     BecomeSeniorEvent,
     BecomeYoungAdultEvent,
     BirthEvent,
-    ChangeResidenceEvent,
-    Death,
     HaveChildEvent,
     JoinSettlementEvent,
+    SettlementAddedEvent,
+)
+from neighborly.helpers.character import (
+    add_character_to_household,
+    create_character,
+    create_child,
+    create_household,
+    set_household_head,
 )
-from neighborly.helpers.business import create_business
-from neighborly.helpers.character import create_character
-from neighborly.helpers.relationship import (
-    add_relationship,
-    get_relationship,
+from neighborly.helpers.content_selection import get_with_tags
+from neighborly.helpers.location import score_location
+from neighborly.helpers.settlement import (
+    add_district_to_settlement,
+    create_district,
+    create_settlement,
+)
+from neighborly.helpers.traits import (
+    add_relationship_trait,
     get_relationships_with_traits,
-    has_relationship,
+    remove_relationship_trait,
+    remove_trait,
 )
-from neighborly.helpers.residence import create_residence
-from neighborly.helpers.settlement import create_settlement
-from neighborly.helpers.stats import get_stat
-from neighborly.helpers.traits import add_trait
 from neighborly.libraries import (
+    BeliefLibrary,
     BusinessLibrary,
     CharacterLibrary,
     DistrictLibrary,
+    EffectLibrary,
     JobRoleLibrary,
-    LifeEventLibrary,
-    ResidenceLibrary,
+    LocationPreferenceLibrary,
+    PreconditionLibrary,
     SettlementLibrary,
     SkillLibrary,
+    SpeciesLibrary,
     TraitLibrary,
 )
-from neighborly.life_event import LifeEvent
+from neighborly.life_event import dispatch_life_event
+from neighborly.plugins.actions import CloseBusiness, Die
 
 _logger = logging.getLogger(__name__)
 
 
 class InitializationSystems(SystemGroup):
     """A group of systems that run once at the beginning of the simulation.
 
@@ -104,384 +119,434 @@
 
 class InitializeSettlementSystem(System):
     """Creates one or more settlement instances using simulation config settings."""
 
     def on_update(self, world: World) -> None:
         config = world.resource_manager.get_resource(SimulationConfig)
 
-        definition_ids = config.settlement
-
         rng = world.resource_manager.get_resource(random.Random)
 
-        if isinstance(definition_ids, str):
-            if definition_ids:
-                create_settlement(world, definition_ids)
-        elif len(definition_ids) > 0:
-            choice = rng.choice(definition_ids)
-            create_settlement(world, choice)
-
-
-class SpawnResidentialBuildingsSystem(System):
-    """Attempt to build new residential buildings in all districts."""
-
-    @staticmethod
-    def get_random_single_family_building(
-        district: District, spawn_table: ResidenceSpawnTable
-    ) -> Optional[str]:
-        """Attempt to randomly select a single-family building from the spawn table.
+        settlement_library = world.resources.get_resource(SettlementLibrary)
+        district_library = world.resources.get_resource(DistrictLibrary)
 
-        Parameters
-        ----------
-        district
-            The district where the residential building will be built.
-        spawn_table
-            The spawn table where buildings are sampled from.
+        # Select a settlement from the library using the theme tags
+        selection_tags = [f"~{tag}" for tag in config.theme_tags]
 
-        Returns
-        -------
-        str or None
-            The definition ID of a selected residence, or None if no eligible entries.
-        """
-        eligible_entries: pl.DataFrame = spawn_table.table.filter(  # type: ignore
-            (pl.col("instances") < pl.col("max_instances"))
-            & (pl.col("required_population") <= district.population)
-            & (pl.col("is_multifamily") == False)  # pylint: disable=C0121
+        settlement_options = settlement_library.get_definition_with_tags(selection_tags)
+
+        if not settlement_options:
+            return
+
+        chosen_settlement_definition = rng.choice(settlement_options)
+
+        settlement = create_settlement(
+            world, chosen_settlement_definition.definition_id
+        ).get_component(Settlement)
+
+        world.events.dispatch_event(
+            Event("settlement-added", world=world, settlement=settlement.gameobject)
         )
 
-        if len(eligible_entries) == 0:
-            return None
+        # Now generate districts for the settlement using the spawn table. The table
+        # has a subset of all the districts in the district library. We need to perform
+        # tag-based selection on all the entries
+        spawn_table = settlement.gameobject.get_component(DistrictSpawnTable)
 
-        rng = district.gameobject.world.resource_manager.get_resource(random.Random)
+        districts_and_tags: list[tuple[DistrictDef, list[str]]] = []
 
-        return rng.choices(
-            population=eligible_entries["name"].to_list(),
-            weights=eligible_entries["spawn_frequency"].to_list(),
-            k=1,
-        )[0]
-
-    @staticmethod
-    def get_random_multifamily_building(
-        district: District, spawn_table: ResidenceSpawnTable
-    ) -> Optional[str]:
-        """Attempt to randomly select a multifamily building from the spawn table.
+        for entry in spawn_table.table.values():
+            definition = district_library.get_definition(entry.definition_id)
+            districts_and_tags.append((definition, [*definition.tags]))
 
-        Parameters
-        ----------
-        district
-            The district where the residential building will be built.
-        spawn_table
-            The spawn table where buildings are sampled from.
+        district_options = get_with_tags(districts_and_tags, selection_tags)
 
-        Returns
-        -------
-        str or None
-            The definition ID of a selected residence, or None if no eligible entries.
-        """
-        eligible_entries: pl.DataFrame = spawn_table.table.filter(  # type: ignore
-            (pl.col("instances") < pl.col("max_instances"))
-            & (pl.col("required_population") <= district.population)
-            & (pl.col("is_multifamily") == True)  # pylint: disable=C0121
-        )
+        n_districts_remaining = config.num_districts
 
-        if len(eligible_entries) == 0:
-            return None
+        district_instance_counts: defaultdict[str, int] = defaultdict(lambda: 0)
 
-        rng = district.gameobject.world.resource_manager.get_resource(random.Random)
+        while n_districts_remaining > 0:
 
-        return rng.choices(
-            population=eligible_entries["name"].to_list(),
-            weights=eligible_entries["spawn_frequency"].to_list(),
-            k=1,
-        )[0]
+            if not district_options:
+                raise RuntimeError(
+                    "Ran out of eligible districts when constructing settlement. "
+                    "Please adjust settings or add more content."
+                )
 
-    def on_update(self, world: World) -> None:
-        for _, (_, district, spawn_table) in world.get_components(
-            (Active, District, ResidenceSpawnTable)
-        ):
-            # We can't build if there is no space
-            if district.residential_slots <= 0:
+            district_def = rng.choice(district_options)
+
+            # If there are too many instances of this district remove it from the list
+            # and try again
+            if (
+                district_instance_counts[district_def.definition_id]
+                > district_def.max_instances
+            ):
+                district_options.remove(district_def)
                 continue
 
-            # Try to build a multifamily residential building
-            multifamily_building = (
-                SpawnResidentialBuildingsSystem.get_random_multifamily_building(
-                    district=district, spawn_table=spawn_table
-                )
+            # Create an instance of the district and add it to the settlement
+            district = create_district(world, district_def.definition_id).get_component(
+                District
             )
 
-            if multifamily_building is not None:
-                residence = create_residence(
-                    world,
-                    district.gameobject,
-                    multifamily_building,
-                )
-                district.add_residence(residence)
-                district.gameobject.add_child(residence)
-                spawn_table.increment_count(multifamily_building)
-                continue
+            add_district_to_settlement(settlement, district)
 
-            # Try to build a single-family residential building
-            single_family_building = (
-                SpawnResidentialBuildingsSystem.get_random_single_family_building(
-                    district=district, spawn_table=spawn_table
-                )
+            world.events.dispatch_event(
+                Event("district-added", world=world, district=district)
             )
 
-            if single_family_building is not None:
-                residence = create_residence(
-                    world,
-                    district.gameobject,
-                    single_family_building,
-                )
-                district.add_residence(residence)
-                district.gameobject.add_child(residence)
-                spawn_table.increment_count(single_family_building)
+            n_districts_remaining -= 1
+
+        event = SettlementAddedEvent(settlement.gameobject)
+        dispatch_life_event(event, [settlement.gameobject])
 
 
 class SpawnNewResidentSystem(System):
     """Spawns new characters as residents within vacant residences."""
 
-    CHANCE_NEW_RESIDENT: ClassVar[float] = 0.5
-
     def on_update(self, world: World) -> None:
         rng = world.resource_manager.get_resource(random.Random)
+        config = world.resources.get_resource(SimulationConfig)
 
         # Find vacant residences
-        for _, (_, residence, _) in world.get_components(
-            (Active, ResidentialUnit, Vacant)
+        for _, (_, current_settlement, spawn_table, _) in world.get_components(
+            (District, CurrentSettlement, CharacterSpawnTable, Active)
         ):
-            # Get the spawn table of district the residence belongs to
-            spawn_table = residence.district.get_component(CharacterSpawnTable)
-
-            if len(spawn_table) == 0:
+            if len(spawn_table.table) == 0:
                 continue
 
-            if rng.random() > SpawnNewResidentSystem.CHANCE_NEW_RESIDENT:
+            if rng.random() > config.growth_factor:
                 continue
 
             # Weighted random selection on the characters in the table
-            characters = spawn_table.table["name"].to_list()
-            weights = spawn_table.table["spawn_frequency"].to_list()
+            eligible_entries: list[str] = []
+            weights: list[float] = []
 
-            character_definition_id: str = rng.choices(
-                population=characters, weights=weights, k=1
-            )[0]
+            for entry in spawn_table.table.values():
+                eligible_entries.append(entry.definition_id)
+                weights.append(entry.spawn_frequency)
+
+            if not eligible_entries:
+                continue
 
-            character_life_stage = rng.choices(
-                population=(LifeStage.YOUNG_ADULT, LifeStage.ADULT, LifeStage.SENIOR),
-                weights=(5, 2, 1),
+            character_definition_id = rng.choices(
+                population=eligible_entries,
+                weights=weights,
                 k=1,
             )[0]
 
-            character = create_character(
-                world,
-                character_definition_id,
-                CharacterGenOptions(
-                    life_stage=character_life_stage.name,
-                ),
-            )
-
-            JoinSettlementEvent(
-                subject=character,
-                settlement=residence.district.get_component(District).settlement,
-            ).dispatch()
-
-            # Add the character as the owner of the home and a resident
-            ChangeResidenceEvent(
-                subject=character, new_residence=residence.gameobject, is_owner=True
-            ).dispatch()
-
-
-class SpawnNewBusinessesSystem(System):
-    """Spawns new businesses for characters to open."""
-
-    @staticmethod
-    def get_random_business(
-        district: District, spawn_table: BusinessSpawnTable
-    ) -> Optional[str]:
-        """Attempt to randomly select a business from the spawn table.
-
-        Parameters
-        ----------
-        district
-            The district where the business will be built.
-        spawn_table
-            The spawn table where businesses are sampled from.
-
-        Returns
-        -------
-        str or None
-            The definition ID of a selected business, or None if no eligible entries.
-        """
-        eligible_entries: pl.DataFrame = spawn_table.table.filter(  # type: ignore
-            (pl.col("instances") < pl.col("max_instances"))
-            & (pl.col("min_population") <= district.population)
-        )
+            character = create_character(world, character_definition_id)
 
-        if len(eligible_entries) == 0:
-            return None
+            household = create_household(world).get_component(Household)
 
-        rng = district.gameobject.world.resource_manager.get_resource(random.Random)
+            set_household_head(household, character.get_component(Character))
+            add_character_to_household(household, character.get_component(Character))
 
-        return rng.choices(
-            population=eligible_entries["name"].to_list(),
-            weights=eligible_entries["spawn_frequency"].to_list(),
-            k=1,
-        )[0]
+            character.add_component(
+                ResidentOf(settlement=current_settlement.settlement)
+            )
 
-    def on_update(self, world: World) -> None:
-        for _, (_, district, spawn_table) in world.get_components(
-            (Active, District, BusinessSpawnTable)
-        ):
-            # We can't build if there is no space
-            if district.business_slots <= 0:
-                continue
+            current_settlement.settlement.get_component(Settlement).population += 1
 
-            business_id = SpawnNewBusinessesSystem.get_random_business(
-                district=district, spawn_table=spawn_table
+            world.events.dispatch_event(
+                Event("character-added", world=world, character=character)
             )
 
-            if business_id is not None:
-                business = create_business(
-                    world,
-                    district.gameobject,
-                    business_id,
-                )
-                district.add_business(business)
-                district.gameobject.add_child(business)
-                spawn_table.increment_count(business_id)
+            event = JoinSettlementEvent(
+                character,
+                current_settlement.settlement,
+            )
 
-                business.add_component(PendingOpening())
+            dispatch_life_event(event, [character])
 
 
-class InstantiateTraitsSystem(System):
+class CompileTraitDefsSystem(System):
     """Instantiates all the trait definitions within the TraitLibrary."""
 
     def on_update(self, world: World) -> None:
         trait_library = world.resource_manager.get_resource(TraitLibrary)
+        effect_library = world.resource_manager.get_resource(EffectLibrary)
 
         # Compile the loaded definitions
         compiled_defs = compile_definitions(trait_library.definitions.values())
 
         # Clear out the unprocessed ones
         trait_library.definitions.clear()
 
         # Add the new definitions and instances to the library.
         for trait_def in compiled_defs:
-            trait_library.add_definition(trait_def)
-            trait = trait_def.instantiate(world)
-            trait_library.add_trait(trait)
+            if not trait_def.is_template:
+                trait_library.add_definition(trait_def)
+
+                trait_library.add_trait(
+                    Trait(
+                        definition_id=trait_def.definition_id,
+                        name=trait_def.name,
+                        trait_type=TraitType[trait_def.trait_type.upper()],
+                        inheritance_chance_both=trait_def.inheritance_chance_both,
+                        inheritance_chance_single=trait_def.inheritance_chance_single,
+                        is_inheritable=(
+                            trait_def.inheritance_chance_single > 0
+                            or trait_def.inheritance_chance_both > 0
+                        ),
+                        description=trait_def.description,
+                        effects=[
+                            effect_library.create_from_obj(world, entry)
+                            for entry in trait_def.effects
+                        ],
+                        conflicting_traits=trait_def.conflicts_with,
+                        target_effects=[
+                            effect_library.create_from_obj(world, entry)
+                            for entry in trait_def.target_effects
+                        ],
+                        owner_effects=[
+                            effect_library.create_from_obj(world, entry)
+                            for entry in trait_def.owner_effects
+                        ],
+                        outgoing_relationship_effects=[
+                            effect_library.create_from_obj(world, entry)
+                            for entry in trait_def.outgoing_relationship_effects
+                        ],
+                        incoming_relationship_effects=[
+                            effect_library.create_from_obj(world, entry)
+                            for entry in trait_def.incoming_relationship_effects
+                        ],
+                    )
+                )
+
+
+class CompileSpeciesDefsSystem(System):
+    """Instantiates all the species definitions within the SpeciesLibrary."""
+
+    def on_update(self, world: World) -> None:
+        library = world.resource_manager.get_resource(SpeciesLibrary)
+
+        compiled_defs = compile_definitions(library.definitions.values())
+
+        library.definitions.clear()
+
+        for definition in compiled_defs:
+            if not definition.is_template:
+                library.add_definition(definition)
+
+                min_lifespan, max_lifespan = tuple(
+                    int(x.strip()) for x in definition.lifespan.split("-")
+                )
+
+                library.add_species(
+                    SpeciesType(
+                        definition_id=definition.definition_id,
+                        name=definition.name,
+                        description=definition.description,
+                        adolescent_age=definition.adolescent_age,
+                        young_adult_age=definition.young_adult_age,
+                        adult_age=definition.adult_age,
+                        senior_age=definition.senior_age,
+                        lifespan=(min_lifespan, max_lifespan),
+                        can_physically_age=definition.can_physically_age,
+                        traits=[*definition.traits],
+                        adolescent_female_fertility=definition.adolescent_female_fertility,
+                        young_adult_female_fertility=definition.young_adult_female_fertility,
+                        adult_female_fertility=definition.adult_female_fertility,
+                        senior_female_fertility=definition.senior_female_fertility,
+                        adolescent_male_fertility=definition.adolescent_male_fertility,
+                        young_adult_male_fertility=definition.young_adult_male_fertility,
+                        adult_male_fertility=definition.adult_male_fertility,
+                        senior_male_fertility=definition.senior_male_fertility,
+                        fertility_cost_per_child=definition.fertility_cost_per_child,
+                    )
+                )
 
 
-class InstantiateSkillsSystem(System):
+class CompileSkillDefsSystem(System):
     """Instantiates all the skill definitions within the SkillLibrary."""
 
     def on_update(self, world: World) -> None:
         skill_library = world.resource_manager.get_resource(SkillLibrary)
 
         # Compile the loaded definitions
         compiled_defs = compile_definitions(skill_library.definitions.values())
 
         # Clear out the unprocessed ones
         skill_library.definitions.clear()
 
         # Add the new definitions and instances to the library.
         for skill_def in compiled_defs:
-            skill_library.add_definition(skill_def)
-            skill = skill_def.instantiate(world)
-            skill_library.add_skill(skill)
+            if not skill_def.is_template:
+                skill_library.add_definition(skill_def)
 
+                skill_library.add_skill(
+                    Skill(
+                        definition_id=skill_def.definition_id,
+                        name=skill_def.name,
+                        description=skill_def.description,
+                        tags=set(*skill_def.tags),
+                    )
+                )
 
-class InstantiateJobRolesSystem(System):
+
+class CompileJobRoleDefsSystem(System):
     """Instantiates all the job role definitions within the TraitLibrary."""
 
     def on_update(self, world: World) -> None:
         job_role_library = world.resource_manager.get_resource(JobRoleLibrary)
+        effect_library = world.resource_manager.get_resource(EffectLibrary)
+        precondition_library = world.resource_manager.get_resource(PreconditionLibrary)
 
         # Compile the loaded definitions
         compiled_defs = compile_definitions(job_role_library.definitions.values())
 
         # Clear out the unprocessed ones
         job_role_library.definitions.clear()
 
         # Add the new definitions and instances to the library.
         for role_def in compiled_defs:
-            job_role_library.add_definition(role_def)
-            job_role = role_def.instantiate(world)
-            job_role_library.add_role(job_role)
+            if not role_def.is_template:
+                job_role_library.add_definition(role_def)
+
+                job_role_library.add_role(
+                    JobRole(
+                        definition_id=role_def.definition_id,
+                        name=role_def.name,
+                        job_level=role_def.job_level,
+                        description=role_def.description,
+                        requirements=[
+                            precondition_library.create_from_obj(world, entry)
+                            for entry in role_def.requirements
+                        ],
+                        effects=[
+                            effect_library.create_from_obj(world, entry)
+                            for entry in role_def.effects
+                        ],
+                        recurring_effects=[
+                            effect_library.create_from_obj(world, entry)
+                            for entry in role_def.recurring_effects
+                        ],
+                    )
+                )
 
 
 class CompileDistrictDefsSystem(System):
     """Compile district definitions."""
 
     def on_update(self, world: World) -> None:
         library = world.resource_manager.get_resource(DistrictLibrary)
 
         compiled_defs = compile_definitions(library.definitions.values())
 
         library.definitions.clear()
 
         for definition in compiled_defs:
-            library.add_definition(definition)
+            if not definition.is_template:
+                library.add_definition(definition)
 
 
-class CompileSettlementDefsSystem(System):
-    """Compile settlement definitions."""
+class CompileLocationPreferenceDefsSystem(System):
+    """Compile location preference definitions."""
 
     def on_update(self, world: World) -> None:
-        library = world.resource_manager.get_resource(SettlementLibrary)
+        library = world.resource_manager.get_resource(LocationPreferenceLibrary)
+        precondition_library = world.resource_manager.get_resource(PreconditionLibrary)
 
         compiled_defs = compile_definitions(library.definitions.values())
 
         library.definitions.clear()
 
         for definition in compiled_defs:
-            library.add_definition(definition)
+            if not definition.is_template:
+                library.add_definition(definition)
+
+                library.add_rule(
+                    LocationPreferenceRule(
+                        rule_id=definition.definition_id,
+                        description=definition.description,
+                        preconditions=[
+                            precondition_library.create_from_obj(world, entry)
+                            for entry in definition.preconditions
+                        ],
+                        probability=definition.probability,
+                    )
+                )
 
 
-class CompileResidenceDefsSystem(System):
-    """Compile residence definitions."""
+class CompileBeliefDefsSystem(System):
+    """Compile belief definitions."""
 
     def on_update(self, world: World) -> None:
-        library = world.resource_manager.get_resource(ResidenceLibrary)
+        library = world.resource_manager.get_resource(BeliefLibrary)
+        effect_library = world.resource_manager.get_resource(EffectLibrary)
+        precondition_library = world.resource_manager.get_resource(PreconditionLibrary)
 
         compiled_defs = compile_definitions(library.definitions.values())
 
         library.definitions.clear()
 
         for definition in compiled_defs:
-            library.add_definition(definition)
+            if not definition.is_template:
+                library.add_definition(definition)
+
+                library.add_belief(
+                    Belief(
+                        belief_id=definition.definition_id,
+                        description=definition.description,
+                        preconditions=[
+                            precondition_library.create_from_obj(world, entry)
+                            for entry in definition.preconditions
+                        ],
+                        effects=[
+                            effect_library.create_from_obj(world, entry)
+                            for entry in definition.effects
+                        ],
+                        is_global=definition.is_global,
+                    )
+                )
+
+
+class CompileSettlementDefsSystem(System):
+    """Compile settlement definitions."""
+
+    def on_update(self, world: World) -> None:
+        library = world.resource_manager.get_resource(SettlementLibrary)
+
+        compiled_defs = compile_definitions(library.definitions.values())
+
+        library.definitions.clear()
+
+        for definition in compiled_defs:
+            if not definition.is_template:
+                library.add_definition(definition)
 
 
 class CompileCharacterDefsSystem(System):
     """Compile character definitions."""
 
     def on_update(self, world: World) -> None:
         library = world.resource_manager.get_resource(CharacterLibrary)
 
         compiled_defs = compile_definitions(library.definitions.values())
 
         library.definitions.clear()
 
         for definition in compiled_defs:
-            library.add_definition(definition)
+            if not definition.is_template:
+                library.add_definition(definition)
 
 
 class CompileBusinessDefsSystem(System):
     """Compile business definitions."""
 
     def on_update(self, world: World) -> None:
         library = world.resource_manager.get_resource(BusinessLibrary)
 
         compiled_defs = compile_definitions(library.definitions.values())
 
         library.definitions.clear()
 
         for definition in compiled_defs:
-            library.add_definition(definition)
+            if not definition.is_template:
+                library.add_definition(definition)
 
 
 class UpdateFrequentedLocationSystem(System):
     """Characters update the locations that they frequent
 
     This system runs on a regular interval to allow characters to update the locations
     that they frequent to reflect their current status and the state of the settlement.
@@ -516,23 +581,28 @@
 
         Returns
         -------
         Tuple[list[float], list[GameObject]]
             A list of tuples containing location scores and the location, sorted in
             descending order
         """
-        location_prefs = character.get_component(LocationPreferences)
 
         scores: list[float] = []
         locations: list[GameObject] = []
 
-        for _, (business, _, _) in character.world.get_components(
-            (Business, OpenToPublic, Active)
+        for _, (business, location, _) in character.world.get_components(
+            (Business, Location, Active)
         ):
-            score = location_prefs.score_location(business.gameobject)
+            if business.status != BusinessStatus.OPEN:
+                continue
+
+            if location.is_private:
+                continue
+
+            score = score_location(character, business.gameobject)
             if score >= self.location_score_threshold:
                 scores.append(score)
                 locations.append(business.gameobject)
 
         return scores, locations
 
     def on_update(self, world: World) -> None:
@@ -572,335 +642,256 @@
 class AgingSystem(System):
     """Increases the age of all active GameObjects with Age components."""
 
     def on_update(self, world: World) -> None:
         # This system runs every simulated month
         elapsed_years: float = 1.0 / MONTHS_PER_YEAR
 
-        for _, (character, _) in world.get_components((Character, Active)):
-            character.age = character.age + elapsed_years
-            species = character.species.get_component(Species)
-
-            if species.can_physically_age:
-                if character.age >= species.senior_age:
-                    if character.life_stage != LifeStage.SENIOR:
-                        BecomeSeniorEvent(character.gameobject).dispatch()
-
-                elif character.age >= species.adult_age:
-                    if character.life_stage != LifeStage.ADULT:
-                        BecomeAdultEvent(character.gameobject).dispatch()
-
-                elif character.age >= species.young_adult_age:
-                    if character.life_stage != LifeStage.YOUNG_ADULT:
-                        BecomeYoungAdultEvent(character.gameobject).dispatch()
-
-                elif character.age >= species.adolescent_age:
-                    if character.life_stage != LifeStage.ADOLESCENT:
-                        BecomeAdolescentEvent(character.gameobject).dispatch()
-
-                else:
-                    if character.life_stage != LifeStage.CHILD:
-                        character.life_stage = LifeStage.CHILD
+        for _, (age, _) in world.get_components((Age, Active)):
+            age.value += elapsed_years
 
 
-class HealthDecaySystem(System):
-    """Decay the health points of characters as they get older."""
+class LifeStageSystem(System):
+    """Updates the life stage of all characters to reflect their current age."""
 
     def on_update(self, world: World) -> None:
-        # This system runs every simulated month
-        elapsed_time: float = 1.0 / MONTHS_PER_YEAR
 
-        for _, (
-            _,
-            character,
-        ) in world.get_components((Active, Character)):
-            get_stat(character.gameobject, "health").base_value -= (
-                get_stat(character.gameobject, "health_decay").value * elapsed_time
-            )
+        for _, (character, species, age, fertility, _) in world.get_components(
+            (Character, Species, Age, Fertility, Active)
+        ):
 
+            if species.species.can_physically_age:
+                if age.value >= species.species.senior_age:
+                    if character.life_stage != LifeStage.SENIOR:
+                        fertility_max = (
+                            species.species.senior_male_fertility
+                            if character.sex == Sex.MALE
+                            else species.species.senior_female_fertility
+                        )
+
+                        fertility.stat.base_value = min(
+                            fertility.stat.base_value, fertility_max
+                        )
+
+                        evt = BecomeSeniorEvent(character.gameobject)
+                        character.life_stage = LifeStage.SENIOR
+                        dispatch_life_event(evt, [character.gameobject])
 
-class PassiveReputationChange(System):
-    """Reputation stats have a probability of changing each time step."""
+                elif age.value >= species.species.adult_age:
+                    if character.life_stage != LifeStage.ADULT:
 
-    CHANCE_OF_CHANGE: ClassVar[float] = 0.05
+                        fertility_max = (
+                            species.species.adult_male_fertility
+                            if character.sex == Sex.MALE
+                            else species.species.adult_female_fertility
+                        )
+                        fertility.stat.base_value = min(
+                            fertility.stat.base_value, fertility_max
+                        )
+
+                        evt = BecomeAdultEvent(character.gameobject)
+                        character.life_stage = LifeStage.ADULT
+                        dispatch_life_event(evt, [character.gameobject])
 
-    def on_update(self, world: World) -> None:
-        rng = world.resource_manager.get_resource(random.Random)
+                elif age.value >= species.species.young_adult_age:
+                    if character.life_stage != LifeStage.YOUNG_ADULT:
 
-        for _, (
-            relationship,
-            _,
-        ) in world.get_components((Relationship, Active)):
-            interaction_boost = max(
-                1.0, get_stat(relationship.gameobject, "interaction_score").value / 10.0
-            )
+                        fertility_max = (
+                            species.species.young_adult_male_fertility
+                            if character.sex == Sex.MALE
+                            else species.species.young_adult_female_fertility
+                        )
+
+                        fertility.stat.base_value = min(
+                            fertility.stat.base_value, fertility_max
+                        )
+
+                        evt = BecomeYoungAdultEvent(character.gameobject)
+                        character.life_stage = LifeStage.YOUNG_ADULT
+                        dispatch_life_event(evt, [character.gameobject])
 
-            final_chance = PassiveReputationChange.CHANCE_OF_CHANGE * (
-                1.0 + interaction_boost
-            )
+                elif age.value >= species.species.adolescent_age:
+                    if character.life_stage != LifeStage.ADOLESCENT:
 
-            if rng.random() < final_chance:
-                get_stat(relationship.gameobject, "reputation").base_value = (
-                    get_stat(relationship.gameobject, "reputation").base_value
-                    + get_stat(relationship.gameobject, "compatibility").value
-                )
+                        fertility_max = (
+                            species.species.adolescent_male_fertility
+                            if character.sex == Sex.MALE
+                            else species.species.adolescent_female_fertility
+                        )
+
+                        fertility.stat.base_value = min(
+                            fertility.stat.base_value, fertility_max
+                        )
+
+                        evt = BecomeAdolescentEvent(character.gameobject)
+                        character.life_stage = LifeStage.ADOLESCENT
+                        dispatch_life_event(evt, [character.gameobject])
 
+                else:
+                    if character.life_stage != LifeStage.CHILD:
+                        character.life_stage = LifeStage.CHILD
 
-class PassiveRomanceChange(System):
-    """Romance stats have a probability of changing each time step."""
 
-    CHANCE_OF_CHANGE: ClassVar[float] = 0.05
+class CharacterLifespanSystem(System):
+    """Kills of characters who have reached their lifespan."""
 
     def on_update(self, world: World) -> None:
-        rng = world.resource_manager.get_resource(random.Random)
-
-        for _, (
-            relationship,
-            _,
-        ) in world.get_components((Relationship, Active)):
-            interaction_boost = max(
-                1.0, get_stat(relationship.gameobject, "interaction_score").value / 10.0
-            )
-
-            final_chance = PassiveRomanceChange.CHANCE_OF_CHANGE * (
-                1.0 + interaction_boost
-            )
+        for _, (character, age, life_span, _) in world.get_components(
+            (Character, Age, Lifespan, Active)
+        ):
 
-            if rng.random() < final_chance:
-                get_stat(relationship.gameobject, "romance").base_value = (
-                    get_stat(relationship.gameobject, "romance").base_value
-                    + get_stat(relationship.gameobject, "romantic_compatibility").value
-                )
+            if age.value >= life_span.stat.value:
+                Die(character.gameobject).execute()
 
 
-class DeathSystem(System):
-    """Characters die when their health hits zero."""
+class BusinessLifespanSystem(System):
+    """Kills of business that have reached their lifespan."""
 
     def on_update(self, world: World) -> None:
-        for _, (_, character) in world.get_components((Active, Character)):
-            if get_stat(character.gameobject, "health").value <= 0:
-                Death(character.gameobject).dispatch()
+        for _, (business, age, lifespan, _) in world.get_components(
+            (Business, Age, Lifespan, Active)
+        ):
+            if age.value >= lifespan.stat.value and business.owner:
+                CloseBusiness(business.gameobject).execute()
 
 
 class ChildBirthSystem(System):
     """Spawns new children when pregnant characters reach their due dates."""
 
     def on_update(self, world: World) -> None:
         current_date = world.resource_manager.get_resource(SimDate)
 
-        for _, (character, pregnancy, _) in world.get_components(
-            (Character, Pregnant, Active)
+        for _, (character, pregnancy, fertility, species, _) in world.get_components(
+            (Character, Pregnant, Fertility, Species, Active)
         ):
             if pregnancy.due_date > current_date:
                 continue
 
             other_parent = pregnancy.partner
 
-            baby = create_character(
-                character.gameobject.world,
-                character.gameobject.metadata["definition_id"],
-                CharacterGenOptions(
-                    last_name=character.last_name,
-                ),
+            baby = create_child(
+                birthing_parent=character.gameobject,
+                other_parent=other_parent,
             )
 
-            ChangeResidenceEvent(
-                baby,
-                new_residence=character.gameobject.get_component(Resident).residence,
-                is_owner=False,
-            ).dispatch()
+            baby.add_component(
+                ResidentOf(character.gameobject.get_component(ResidentOf).settlement)
+            )
+
+            household = character.gameobject.get_component(
+                MemberOfHousehold
+            ).household.get_component(Household)
+
+            add_character_to_household(household, baby.get_component(Character))
 
             # Birthing parent to child
-            add_trait(get_relationship(character.gameobject, baby), "child")
-            add_trait(get_relationship(baby, character.gameobject), "parent")
-            add_trait(get_relationship(baby, character.gameobject), "biological_parent")
+            add_relationship_trait(character.gameobject, baby, "child")
+            add_relationship_trait(baby, character.gameobject, "parent")
+            add_relationship_trait(baby, character.gameobject, "biological_parent")
 
             # Other parent to child
-            add_trait(get_relationship(other_parent, baby), "child")
-            add_trait(get_relationship(baby, other_parent), "parent")
-            add_trait(get_relationship(baby, other_parent), "biological_parent")
+            add_relationship_trait(other_parent, baby, "child")
+            add_relationship_trait(baby, other_parent, "parent")
+            add_relationship_trait(baby, other_parent, "biological_parent")
 
             # Create relationships with children of birthing parent
             for relationship in get_relationships_with_traits(
                 character.gameobject, "child"
             ):
                 rel = relationship.get_component(Relationship)
 
                 if rel.target == baby:
                     continue
 
                 sibling = rel.target
 
                 # Baby to sibling
-                add_trait(get_relationship(baby, sibling), "sibling")
-                add_trait(get_relationship(sibling, baby), "sibling")
+                add_relationship_trait(baby, sibling, "sibling")
+                add_relationship_trait(sibling, baby, "sibling")
 
             # Create relationships with children of the birthing parent's spouses
             for spousal_rel in get_relationships_with_traits(
                 character.gameobject, "spouse"
             ):
                 spouse = spousal_rel.get_component(Relationship).target
 
                 if spousal_rel.is_active:
-                    add_trait(get_relationship(spouse, baby), "child")
-                    add_trait(get_relationship(baby, spouse), "parent")
+                    add_relationship_trait(spouse, baby, "child")
+                    add_relationship_trait(baby, spouse, "parent")
 
                 for child_rel in get_relationships_with_traits(spouse, "child"):
                     rel = child_rel.get_component(Relationship)
                     if rel.target == baby:
                         continue
 
                     sibling = rel.target
 
                     # Baby to sibling
-                    add_trait(get_relationship(baby, sibling), "sibling")
-                    add_trait(get_relationship(sibling, baby), "sibling")
+                    add_relationship_trait(baby, sibling, "sibling")
+                    add_relationship_trait(sibling, baby, "sibling")
 
             # Create relationships with children of other parent
             for relationship in get_relationships_with_traits(other_parent, "child"):
                 rel = relationship.get_component(Relationship)
                 if rel.target == baby:
                     continue
 
                 sibling = rel.target
 
                 # Baby to sibling
-                add_trait(get_relationship(baby, sibling), "sibling")
-                add_trait(get_relationship(sibling, baby), "sibling")
+                add_relationship_trait(baby, sibling, "sibling")
+                add_relationship_trait(sibling, baby, "sibling")
 
             character.gameobject.remove_component(Pregnant)
-            get_stat(character.gameobject, "fertility").base_value -= 0.2
 
-            HaveChildEvent(
-                parent_0=character.gameobject,
-                parent_1=other_parent,
-                child=baby,
-            ).dispatch()
+            # Reduce the character's fertility according to their species
+            fertility.stat.base_value -= species.species.fertility_cost_per_child
 
-            BirthEvent(baby).dispatch()
+            have_child_evt = HaveChildEvent(
+                character.gameobject,
+                other_parent,
+                baby,
+            )
+            dispatch_life_event(have_child_evt, [character.gameobject, other_parent])
 
+            birth_evt = BirthEvent(baby)
+            dispatch_life_event(birth_evt, [baby])
 
-class LifeEventSystem(System):
-    """Simulate life events/character behavior.
 
-    This system is the core of character behavior for the Simulation. Each time step,
-    characters probabilistically select a life event to execute from a shared collection
-    of LifeEvent types. Life events are how we represent character behaviors and track
-    the various narrative-relevant events that happen in the simulation. Every life
-    event has a 'subject' (the character who the event happens to).
+class JobRoleMonthlyEffectsSystem(System):
+    """This system applies monthly effects associated with character's job roles.
 
-    To add a new life event to this system, create a new LifeEvent subclass and add it
-    to the LifeEventLibrary instance within the simulation world's resource manager.
+    Unlike the normal effects, monthly effects are not reversed when the character
+    leaves the role. The changes are permanent. This system is meant to give characters
+    a way of increasing specific skill points the longer they work at a job. This way
+    higher level jobs can require characters to meet skill thresholds.
     """
 
-    EVENT_PROBABILITY_THRESHOLD: ClassVar[float] = 0.5
-    """The minimum required probability for an event to be considered for execution."""
-
     def on_update(self, world: World) -> None:
-        life_event_library = world.resource_manager.get_resource(LifeEventLibrary)
-        rng = world.resource_manager.get_resource(random.Random)
+        for _, (occupation, _) in world.get_components((Occupation, Active)):
+            for effect in occupation.job_role.recurring_effects:
+                effect.apply(occupation.gameobject)
 
-        for _, (character, _) in world.get_components((Character, Active)):
-            life_event_choices: list[LifeEvent] = []
-            life_event_probabilities: list[float] = []
-
-            for event_type in life_event_library:
-                # Skip event types that with base probability zero
-                # these are most likely events that require more than one
-                # role and are triggered by other events/systems.
-                # if event_type.base_probability == 0.0:
-                #     continue
-
-                event_instance = event_type.instantiate(character.gameobject)
-                if event_instance is not None:
-                    event_probability = event_instance.get_probability()
-                    if event_probability >= self.EVENT_PROBABILITY_THRESHOLD:
-                        life_event_choices.append(event_instance)
-                        life_event_probabilities.append(event_probability)
-
-            # _logger.debug(
-            #     list(
-            #         zip(
-            #             [f.__class__.__name__ for f in life_event_choices],
-            #             life_event_probabilities,
-            #         )
-            #     )
-            # )
-
-            if life_event_choices:
-                chosen_event = rng.choices(
-                    population=life_event_choices, weights=life_event_probabilities, k=1
-                )[0]
-
-                # if rng.random() < chosen_event.get_probability():
-                chosen_event.dispatch()
-
-
-class MeetNewPeopleSystem(System):
-    """Characters introduce themselves to new people that frequent the same places.
-
-    Notes
-    -----
-    This system uses a character's sociability stat score to determine the probability
-    of them introducing themselves to someone else. The goal is for characters with
-    higher sociability scores to form more relationships over the course of their lives.
-    """
+
+class TickTraitsSystem(System):
+    """Update trait durations."""
 
     def on_update(self, world: World) -> None:
-        rng = world.resource_manager.get_resource(random.Random)
+        for _, (traits,) in world.get_components((Traits,)):
+            traits_to_remove: list[Trait] = []
 
-        for _, (character, _, frequented_locs) in world.get_components(
-            (Character, Active, FrequentedLocations)
-        ):
-            probability_meet_someone = get_stat(
-                character.gameobject, "sociability"
-            ).normalized
-
-            if rng.random() < probability_meet_someone:
-                candidate_scores: defaultdict[GameObject, int] = defaultdict(int)
-
-                for loc in frequented_locs:
-                    for other in loc.get_component(FrequentedBy):
-                        if other != character.gameobject and not has_relationship(
-                            character.gameobject, other
-                        ):
-                            candidate_scores[other] += 1
-
-                if candidate_scores:
-                    rng = world.resource_manager.get_resource(random.Random)
-
-                    acquaintance = rng.choices(
-                        list(candidate_scores.keys()),
-                        weights=list(candidate_scores.values()),
-                        k=1,
-                    )[0]
-
-                    add_relationship(character.gameobject, acquaintance)
-                    add_relationship(acquaintance, character.gameobject)
-
-                    # Calculate interaction scores
-                    get_stat(
-                        get_relationship(character.gameobject, acquaintance),
-                        "interaction_score",
-                    ).base_value += candidate_scores[acquaintance]
-
-                    get_stat(
-                        get_relationship(acquaintance, character.gameobject),
-                        "interaction_score",
-                    ).base_value += candidate_scores[acquaintance]
+            for trait_instance in traits.traits.values():
+                if not trait_instance.has_duration:
+                    continue
 
+                trait_instance.duration -= 1
 
-class JobRoleMonthlyEffectsSystem(System):
-    """This system applies monthly effects associated with character's job roles.
+                if trait_instance.duration <= 0:
+                    traits_to_remove.append(trait_instance.trait)
 
-    Unlike the normal effects, monthly effects are not reversed when the character
-    leaves the role. The changes are permanent. This system is meant to give characters
-    a way of increasing specific skill points the longer they work at a job. This way
-    higher level jobs can require characters to meet skill thresholds.
-    """
-
-    def on_update(self, world: World) -> None:
-        for _, (character, occupation, _) in world.get_components(
-            (Character, Occupation, Active)
-        ):
-            for effect in occupation.job_role.monthly_effects:
-                effect.apply(character.gameobject)
+            for trait_id in traits_to_remove:
+                if relationship := traits.gameobject.try_component(Relationship):
+                    remove_relationship_trait(
+                        relationship.owner, relationship.target, trait_id
+                    )
+                else:
+                    remove_trait(traits.gameobject, trait_id)
```

### Comparing `neighborly-2.5.0/src/neighborly.egg-info/PKG-INFO` & `neighborly-3.0.0.dev1/src/neighborly.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,664 +1,777 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e65 6967  : 2.1.Name: neig
 00000020: 6862 6f72 6c79 0a56 6572 7369 6f6e 3a20  hborly.Version: 
-00000030: 322e 352e 300a 5375 6d6d 6172 793a 2041  2.5.0.Summary: A
-00000040: 206e 6172 7261 7469 7665 2d66 6f63 7573   narrative-focus
-00000050: 6564 2061 6765 6e74 2d62 6173 6564 2073  ed agent-based s
-00000060: 6574 746c 656d 656e 7420 7369 6d75 6c61  ettlement simula
-00000070: 7469 6f6e 2066 7261 6d65 776f 726b 2e0a  tion framework..
-00000080: 4175 7468 6f72 2d65 6d61 696c 3a20 5368  Author-email: Sh
-00000090: 6920 4a6f 686e 736f 6e2d 4265 7920 3c73  i Johnson-Bey <s
-000000a0: 6869 6a62 6579 4067 6d61 696c 2e63 6f6d  hijbey@gmail.com
-000000b0: 3e0a 5072 6f6a 6563 742d 5552 4c3a 2048  >.Project-URL: H
-000000c0: 6f6d 6570 6167 652c 2068 7474 7073 3a2f  omepage, https:/
-000000d0: 2f67 6974 6875 622e 636f 6d2f 5368 694a  /github.com/ShiJ
-000000e0: 6265 792f 6e65 6967 6862 6f72 6c79 0a50  bey/neighborly.P
-000000f0: 726f 6a65 6374 2d55 524c 3a20 4275 6720  roject-URL: Bug 
-00000100: 5472 6163 6b65 722c 2068 7474 7073 3a2f  Tracker, https:/
-00000110: 2f67 6974 6875 622e 636f 6d2f 5368 694a  /github.com/ShiJ
-00000120: 6265 792f 6e65 6967 6862 6f72 6c79 2f69  bey/neighborly/i
-00000130: 7373 7565 730a 5072 6f6a 6563 742d 5552  ssues.Project-UR
-00000140: 4c3a 2052 6570 6f73 6974 6f72 792c 2068  L: Repository, h
-00000150: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000160: 6d2f 5368 694a 4265 792f 6e65 6967 6862  m/ShiJBey/neighb
-00000170: 6f72 6c79 2e67 6974 0a50 726f 6a65 6374  orly.git.Project
-00000180: 2d55 524c 3a20 4368 616e 6765 6c6f 672c  -URL: Changelog,
-00000190: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000001a0: 636f 6d2f 5368 694a 6265 792f 6e65 6967  com/ShiJbey/neig
-000001b0: 6862 6f72 6c79 2f62 6c6f 622f 6d61 696e  hborly/blob/main
-000001c0: 2f43 4841 4e47 454c 4f47 2e6d 640a 5072  /CHANGELOG.md.Pr
-000001d0: 6f6a 6563 742d 5552 4c3a 2044 6f63 756d  oject-URL: Docum
-000001e0: 656e 7461 7469 6f6e 2c20 6874 7470 733a  entation, https:
-000001f0: 2f2f 6e65 6967 6862 6f72 6c79 2e72 6561  //neighborly.rea
-00000200: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00000210: 6174 6573 742f 0a4b 6579 776f 7264 733a  atest/.Keywords:
-00000220: 2073 6f63 6961 6c20 7369 6d75 6c61 7469   social simulati
-00000230: 6f6e 2c67 616d 6573 2c73 696d 756c 6174  on,games,simulat
-00000240: 696f 6e2c 6172 7469 6669 6369 616c 2069  ion,artificial i
-00000250: 6e74 656c 6c69 6765 6e63 652c 6167 656e  ntelligence,agen
-00000260: 742d 6261 7365 6420 6d6f 6465 6c69 6e67  t-based modeling
-00000270: 2c6d 756c 7469 6167 656e 7420 7379 7374  ,multiagent syst
-00000280: 656d 732c 656d 6572 6765 6e74 206e 6172  ems,emergent nar
-00000290: 7261 7469 7665 2c6e 6172 7261 7469 7665  rative,narrative
-000002a0: 2067 656e 6572 6174 696f 6e2c 696e 7465   generation,inte
-000002b0: 7261 6374 6976 6520 7374 6f72 7974 656c  ractive storytel
-000002c0: 6c69 6e67 2c73 6574 746c 656d 656e 7420  ling,settlement 
-000002d0: 7369 6d75 6c61 7469 6f6e 0a43 6c61 7373  simulation.Class
-000002e0: 6966 6965 723a 2049 6e74 656e 6465 6420  ifier: Intended 
-000002f0: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
-00000300: 6c6f 7065 7273 0a43 6c61 7373 6966 6965  lopers.Classifie
-00000310: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
-00000320: 656e 6365 203a 3a20 5363 6965 6e63 652f  ence :: Science/
-00000330: 5265 7365 6172 6368 0a43 6c61 7373 6966  Research.Classif
-00000340: 6965 723a 204c 6963 656e 7365 203a 3a20  ier: License :: 
-00000350: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-00000360: 4d49 5420 4c69 6365 6e73 650a 436c 6173  MIT License.Clas
-00000370: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
-00000380: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-00000390: 6e64 6570 656e 6465 6e74 0a43 6c61 7373  ndependent.Class
-000003a0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-000003b0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000003c0: 7974 686f 6e20 3a3a 2033 203a 3a20 4f6e  ython :: 3 :: On
-000003d0: 6c79 0a43 6c61 7373 6966 6965 723a 2050  ly.Classifier: P
-000003e0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000003f0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000400: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
-00000410: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000420: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000430: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
-00000440: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000450: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000460: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
-00000470: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000480: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000490: 7468 6f6e 203a 3a20 332e 3131 0a43 6c61  thon :: 3.11.Cla
-000004a0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-000004b0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000004c0: 2050 7974 686f 6e20 3a3a 2033 2e31 320a   Python :: 3.12.
-000004d0: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
-000004e0: 6320 3a3a 2047 616d 6573 2f45 6e74 6572  c :: Games/Enter
-000004f0: 7461 696e 6d65 6e74 203a 3a20 5369 6d75  tainment :: Simu
-00000500: 6c61 7469 6f6e 0a43 6c61 7373 6966 6965  lation.Classifie
-00000510: 723a 2054 6f70 6963 203a 3a20 5363 6965  r: Topic :: Scie
-00000520: 6e74 6966 6963 2f45 6e67 696e 6565 7269  ntific/Engineeri
-00000530: 6e67 0a43 6c61 7373 6966 6965 723a 2054  ng.Classifier: T
-00000540: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
-00000550: 6963 2f45 6e67 696e 6565 7269 6e67 203a  ic/Engineering :
-00000560: 3a20 4172 7469 6669 6369 616c 2049 6e74  : Artificial Int
-00000570: 656c 6c69 6765 6e63 650a 436c 6173 7369  elligence.Classi
-00000580: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
-00000590: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
-000005a0: 6572 696e 6720 3a3a 2041 7274 6966 6963  ering :: Artific
-000005b0: 6961 6c20 4c69 6665 0a43 6c61 7373 6966  ial Life.Classif
-000005c0: 6965 723a 2054 6f70 6963 203a 3a20 536f  ier: Topic :: So
-000005d0: 6369 6f6c 6f67 790a 436c 6173 7369 6669  ciology.Classifi
-000005e0: 6572 3a20 546f 7069 6320 3a3a 2053 6f66  er: Topic :: Sof
-000005f0: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
-00000600: 7420 3a3a 204c 6962 7261 7269 6573 0a43  t :: Libraries.C
-00000610: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-00000620: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
-00000630: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
-00000640: 6172 6965 7320 3a3a 2041 7070 6c69 6361  aries :: Applica
-00000650: 7469 6f6e 2046 7261 6d65 776f 726b 730a  tion Frameworks.
-00000660: 436c 6173 7369 6669 6572 3a20 5479 7069  Classifier: Typi
-00000670: 6e67 203a 3a20 5479 7065 640a 5265 7175  ng :: Typed.Requ
-00000680: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
-00000690: 2e38 0a44 6573 6372 6970 7469 6f6e 2d43  .8.Description-C
-000006a0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-000006b0: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
-000006c0: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-000006d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000006e0: 6573 7065 723d 3d32 2e2a 0a52 6571 7569  esper==2.*.Requi
-000006f0: 7265 732d 4469 7374 3a20 6f72 6465 7265  res-Dist: ordere
-00000700: 642d 7365 743d 3d34 2e2a 0a52 6571 7569  d-set==4.*.Requi
-00000710: 7265 732d 4469 7374 3a20 7472 6163 6572  res-Dist: tracer
-00000720: 7933 3d3d 312e 2a0a 5265 7175 6972 6573  y3==1.*.Requires
-00000730: 2d44 6973 743a 2070 6f6c 6172 733d 3d30  -Dist: polars==0
-00000740: 2e31 392e 2a0a 5265 7175 6972 6573 2d44  .19.*.Requires-D
-00000750: 6973 743a 2074 6162 756c 6174 653d 3d30  ist: tabulate==0
-00000760: 2e39 2e2a 0a52 6571 7569 7265 732d 4469  .9.*.Requires-Di
-00000770: 7374 3a20 5079 5941 4d4c 3d3d 362e 302e  st: PyYAML==6.0.
-00000780: 2a0a 5265 7175 6972 6573 2d44 6973 743a  *.Requires-Dist:
-00000790: 2074 7164 6d3d 3d34 2e2a 0a52 6571 7569   tqdm==4.*.Requi
-000007a0: 7265 732d 4469 7374 3a20 7079 6461 6e74  res-Dist: pydant
-000007b0: 6963 3d3d 322e 2a0a 5072 6f76 6964 6573  ic==2.*.Provides
-000007c0: 2d45 7874 7261 3a20 7361 6d70 6c65 730a  -Extra: samples.
-000007d0: 5265 7175 6972 6573 2d44 6973 743a 206a  Requires-Dist: j
-000007e0: 7570 7974 6572 6c61 623b 2065 7874 7261  upyterlab; extra
-000007f0: 203d 3d20 2273 616d 706c 6573 220a 5265   == "samples".Re
-00000800: 7175 6972 6573 2d44 6973 743a 206d 6174  quires-Dist: mat
-00000810: 706c 6f74 6c69 623b 2065 7874 7261 203d  plotlib; extra =
-00000820: 3d20 2273 616d 706c 6573 220a 5265 7175  = "samples".Requ
-00000830: 6972 6573 2d44 6973 743a 2069 7079 7769  ires-Dist: ipywi
-00000840: 6467 6574 733b 2065 7874 7261 203d 3d20  dgets; extra == 
-00000850: 2273 616d 706c 6573 220a 5072 6f76 6964  "samples".Provid
-00000860: 6573 2d45 7874 7261 3a20 6465 7665 6c6f  es-Extra: develo
-00000870: 706d 656e 740a 5265 7175 6972 6573 2d44  pment.Requires-D
-00000880: 6973 743a 2069 736f 7274 3b20 6578 7472  ist: isort; extr
-00000890: 6120 3d3d 2022 6465 7665 6c6f 706d 656e  a == "developmen
-000008a0: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
-000008b0: 3a20 626c 6163 6b3b 2065 7874 7261 203d  : black; extra =
-000008c0: 3d20 2264 6576 656c 6f70 6d65 6e74 220a  = "development".
-000008d0: 5265 7175 6972 6573 2d44 6973 743a 2062  Requires-Dist: b
-000008e0: 6c61 636b 5b64 5d3b 2065 7874 7261 203d  lack[d]; extra =
-000008f0: 3d20 2264 6576 656c 6f70 6d65 6e74 220a  = "development".
-00000900: 5265 7175 6972 6573 2d44 6973 743a 2062  Requires-Dist: b
-00000910: 6c61 636b 5b6a 7570 7974 6572 5d3b 2065  lack[jupyter]; e
-00000920: 7874 7261 203d 3d20 2264 6576 656c 6f70  xtra == "develop
-00000930: 6d65 6e74 220a 5265 7175 6972 6573 2d44  ment".Requires-D
-00000940: 6973 743a 2062 7569 6c64 3b20 6578 7472  ist: build; extr
-00000950: 6120 3d3d 2022 6465 7665 6c6f 706d 656e  a == "developmen
-00000960: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
-00000970: 3a20 7079 7465 7374 3b20 6578 7472 6120  : pytest; extra 
-00000980: 3d3d 2022 6465 7665 6c6f 706d 656e 7422  == "development"
-00000990: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000009a0: 7079 7465 7374 2d63 6f76 3b20 6578 7472  pytest-cov; extr
-000009b0: 6120 3d3d 2022 6465 7665 6c6f 706d 656e  a == "developmen
-000009c0: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
-000009d0: 3a20 7370 6869 6e78 3b20 6578 7472 6120  : sphinx; extra 
-000009e0: 3d3d 2022 6465 7665 6c6f 706d 656e 7422  == "development"
-000009f0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000a00: 7370 6869 6e78 5f72 7464 5f74 6865 6d65  sphinx_rtd_theme
-00000a10: 3b20 6578 7472 6120 3d3d 2022 6465 7665  ; extra == "deve
-00000a20: 6c6f 706d 656e 7422 0a0a 3c68 3120 616c  lopment"..<h1 al
-00000a30: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
-00000a40: 3c69 6d67 0a20 2020 2077 6964 7468 3d22  <img.    width="
-00000a50: 3135 3022 0a20 2020 2068 6569 6768 743d  150".    height=
-00000a60: 2231 3530 220a 2020 2020 7372 633d 2268  "150".    src="h
-00000a70: 7474 7073 3a2f 2f75 7365 722d 696d 6167  ttps://user-imag
-00000a80: 6573 2e67 6974 6875 6275 7365 7263 6f6e  es.githubusercon
-00000a90: 7465 6e74 2e63 6f6d 2f31 3130 3736 3532  tent.com/1107652
-00000aa0: 352f 3136 3538 3336 3137 312d 3966 6664  5/165836171-9ffd
-00000ab0: 6561 3665 2d31 3633 332d 3434 3063 2d62  ea6e-1633-440c-b
-00000ac0: 6530 362d 6234 3665 3165 3365 3465 3034  e06-b46e1e3e4e04
-00000ad0: 2e70 6e67 220a 2020 3e0a 2020 3c62 723e  .png".  >.  <br>
-00000ae0: 0a20 204e 6569 6768 626f 726c 790a 3c2f  .  Neighborly.</
-00000af0: 6831 3e0a 0a3c 7020 616c 6967 6e3d 2263  h1>..<p align="c
-00000b00: 656e 7465 7222 3e0a 2020 3c69 6d67 2073  enter">.  <img s
-00000b10: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000b20: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000b30: 762f 6e65 6967 6862 6f72 6c79 223e 0a20  v/neighborly">. 
-00000b40: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000b50: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000b60: 6f2f 7079 7069 2f70 7976 6572 7369 6f6e  o/pypi/pyversion
-00000b70: 732f 6e65 6967 6862 6f72 6c79 223e 0a20  s/neighborly">. 
-00000b80: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000b90: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000ba0: 6f2f 7079 7069 2f6c 2f6e 6569 6768 626f  o/pypi/l/neighbo
-00000bb0: 726c 7922 3e0a 2020 3c69 6d67 2073 7263  rly">.  <img src
-00000bc0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00000bd0: 6965 6c64 732e 696f 2f70 7970 692f 646d  ields.io/pypi/dm
-00000be0: 2f6e 6569 6768 626f 726c 7922 3e0a 2020  /neighborly">.  
-00000bf0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000c00: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000c10: 2f62 6164 6765 2f63 6f64 6525 3230 7374  /badge/code%20st
-00000c20: 796c 652d 626c 6163 6b2d 626c 6163 6b22  yle-black-black"
-00000c30: 3e0a 2020 3c69 6d67 2073 7263 3d22 6874  >.  <img src="ht
-00000c40: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000c50: 732e 696f 2f62 6164 6765 2f25 3230 696d  s.io/badge/%20im
-00000c60: 706f 7274 732d 6973 6f72 742d 2532 3331  ports-isort-%231
-00000c70: 3637 3462 313f 7374 796c 653d 666c 6174  674b1?style=flat
-00000c80: 266c 6162 656c 436f 6c6f 723d 6566 3833  &labelColor=ef83
-00000c90: 3336 223e 0a3c 2f70 3e0a 0a4e 6569 6768  36">.</p>..Neigh
-00000ca0: 626f 726c 7920 6973 2061 6e20 6578 7465  borly is an exte
-00000cb0: 6e73 6962 6c65 2061 6765 6e74 2d62 6173  nsible agent-bas
-00000cc0: 6564 2073 6574 746c 656d 656e 7420 7369  ed settlement si
-00000cd0: 6d75 6c61 7469 6f6e 2e20 4974 2077 6173  mulation. It was
-00000ce0: 2062 7569 6c74 2074 6f20 6265 2061 2074   built to be a t
-00000cf0: 6f6f 6c20 666f 7220 656d 6572 6765 6e74  ool for emergent
-00000d00: 206e 6172 7261 7469 7665 2073 746f 7279   narrative story
-00000d10: 7465 6c6c 696e 6720 7265 7365 6172 6368  telling research
-00000d20: 2e20 4e65 6967 6862 6f72 6c79 2067 656e  . Neighborly gen
-00000d30: 6572 6174 6573 2061 2076 6972 7475 616c  erates a virtual
-00000d40: 2073 6574 746c 656d 656e 7420 616e 6420   settlement and 
-00000d50: 7369 6d75 6c61 7465 7320 7468 6520 696e  simulates the in
-00000d60: 6469 7669 6475 616c 206c 6976 6573 206f  dividual lives o
-00000d70: 6620 6974 7320 7265 7369 6465 6e74 7320  f its residents 
-00000d80: 6f76 6572 206d 756c 7469 706c 6520 6765  over multiple ge
-00000d90: 6e65 7261 7469 6f6e 732e 2049 7420 6d6f  nerations. It mo
-00000da0: 6465 6c73 2074 6865 2063 6861 7261 6374  dels the charact
-00000db0: 6572 7327 2074 7261 6974 732c 2073 7461  ers' traits, sta
-00000dc0: 7475 7365 732c 2072 656c 6174 696f 6e73  tuses, relations
-00000dd0: 6869 7073 2c20 6f63 6375 7061 7469 6f6e  hips, occupation
-00000de0: 732c 206c 6966 6520 6576 656e 7473 2c20  s, life events, 
-00000df0: 616e 6420 6d6f 7265 2e20 4e65 6967 6862  and more. Neighb
-00000e00: 6f72 6c79 2074 7261 636b 7320 616c 6c20  orly tracks all 
-00000e10: 7468 6520 6c69 6665 2065 7665 6e74 7320  the life events 
-00000e20: 2873 7461 7274 696e 6720 6120 6e65 7720  (starting a new 
-00000e30: 6a6f 622c 2066 616c 6c69 6e67 2069 6e20  job, falling in 
-00000e40: 6c6f 7665 2c20 7475 726e 696e 6720 696e  love, turning in
-00000e50: 746f 2061 2064 656d 6f6e 2c20 6574 632e  to a demon, etc.
-00000e60: 292c 2061 6e64 2074 6865 7365 2062 6563  ), and these bec
-00000e70: 6f6d 6520 7468 6520 6275 696c 6469 6e67  ome the building
-00000e80: 2062 6c6f 636b 7320 666f 7220 6372 6561   blocks for crea
-00000e90: 7469 6e67 2065 6d65 7267 656e 7420 7374  ting emergent st
-00000ea0: 6f72 6965 7320 6162 6f75 7420 6368 6172  ories about char
-00000eb0: 6163 7465 7273 2061 6e64 2074 6865 6972  acters and their
-00000ec0: 206c 6567 6163 6965 732e 2054 6865 2065   legacies. The e
-00000ed0: 6e74 6972 6520 6869 7374 6f72 7920 6f66  ntire history of
-00000ee0: 2074 6865 2073 6574 746c 656d 656e 7420   the settlement 
-00000ef0: 616e 6420 6974 7320 6765 6e65 7261 7469  and its generati
-00000f00: 6f6e 7320 6f66 2063 6861 7261 6374 6572  ons of character
-00000f10: 7320 6973 2074 6865 6e20 6d61 6465 2061  s is then made a
-00000f20: 7661 696c 6162 6c65 2066 6f72 2064 6174  vailable for dat
-00000f30: 6120 616e 616c 7973 6973 206f 7220 6173  a analysis or as
-00000f40: 2063 6f6e 7465 6e74 2066 6f72 206f 7468   content for oth
-00000f50: 6572 2061 7070 6c69 6361 7469 6f6e 7320  er applications 
-00000f60: 7375 6368 2061 7320 6761 6d65 732e 0a0a  such as games...
-00000f70: 4e65 6967 6862 6f72 6c79 2773 2077 6173  Neighborly's was
-00000f80: 2069 6e73 7069 7265 6420 5b5f 5461 6c6b   inspired [_Talk
-00000f90: 206f 6620 7468 6520 546f 776e 5f5d 2868   of the Town_](h
-00000fa0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000fb0: 6d2f 6a61 6d65 732d 6f77 656e 2d72 7961  m/james-owen-rya
-00000fc0: 6e2f 7461 6c6b 746f 776e 292c 2061 6e6f  n/talktown), ano
-00000fd0: 7468 6572 2073 6574 746c 656d 656e 7420  ther settlement 
-00000fe0: 7369 6d75 6c61 7469 6f6e 2066 6f72 2065  simulation for e
-00000ff0: 6d65 7267 656e 7420 6e61 7272 6174 6976  mergent narrativ
-00001000: 6520 7374 6f72 7974 656c 6c69 6e67 2072  e storytelling r
-00001010: 6573 6561 7263 682e 2049 7420 616c 736f  esearch. It also
-00001020: 2064 7261 7773 2069 6e73 7069 7261 7469   draws inspirati
-00001030: 6f6e 2066 726f 6d20 636f 6d6d 6572 6369  on from commerci
-00001040: 616c 2077 6f72 6c64 2d73 696d 756c 6174  al world-simulat
-00001050: 696f 6e20 6761 6d65 7320 6c69 6b65 205f  ion games like _
-00001060: 4361 7665 7320 6f66 2051 7564 5f2c 205f  Caves of Qud_, _
-00001070: 4477 6172 6620 466f 7274 7265 7373 5f2c  Dwarf Fortress_,
-00001080: 205f 4372 7573 6164 6572 204b 696e 6773   _Crusader Kings
-00001090: 5f2c 205f 5269 6d57 6f72 6c64 5f2c 2061  _, _RimWorld_, a
-000010a0: 6e64 205f 576f 726c 6442 6f78 5f2e 2049  nd _WorldBox_. I
-000010b0: 7420 6169 6d73 2074 6f20 6265 2061 6e20  t aims to be an 
-000010c0: 6561 7369 6c79 2063 7573 746f 6d69 7a61  easily customiza
-000010d0: 626c 6520 7369 6d75 6c61 7469 6f6e 2074  ble simulation t
-000010e0: 6861 7420 6361 6e20 6164 6170 7420 746f  hat can adapt to
-000010f0: 2076 6172 696f 7573 206e 6172 7261 7469   various narrati
-00001100: 7665 2073 6574 7469 6e67 7320 616e 6420  ve settings and 
-00001110: 7375 7070 6f72 7420 7265 7365 6172 6368  support research
-00001120: 206f 7220 656e 7465 7274 6169 6e6d 656e   or entertainmen
-00001130: 7420 7072 6f6a 6563 7473 2e0a 0a49 6620  t projects...If 
-00001140: 796f 7520 7573 6520 4e65 6967 6862 6f72  you use Neighbor
-00001150: 6c79 2069 6e20 6120 7072 6f6a 6563 742c  ly in a project,
-00001160: 2070 6c65 6173 6520 5b63 6974 6520 7468   please [cite th
-00001170: 6973 2072 6570 6f73 6974 6f72 795d 282e  is repository](.
-00001180: 2f43 4954 4154 494f 4e2e 6269 6229 2e20  /CITATION.bib). 
-00001190: 596f 7520 6361 6e20 7265 6164 2061 2063  You can read a c
-000011a0: 6f70 7920 6f66 0a4e 6569 6768 626f 726c  opy of.Neighborl
-000011b0: 7927 7320 6173 736f 6369 6174 6564 205b  y's associated [
-000011c0: 7061 7065 725d 2868 7474 7073 3a2f 2f73  paper](https://s
-000011d0: 6869 6a62 6579 2e67 6974 6875 622e 696f  hijbey.github.io
-000011e0: 2f70 7562 6c69 6361 7469 6f6e 732f 4e65  /publications/Ne
-000011f0: 6967 6862 6f72 6c79 2e70 6466 2920 7468  ighborly.pdf) th
-00001200: 6174 2077 6173 2070 7562 6c69 7368 6564  at was published
-00001210: 2069 6e20 7468 650a 7072 6f63 6565 6469   in the.proceedi
-00001220: 6e67 7320 6f66 2074 6865 2032 3032 3220  ngs of the 2022 
-00001230: 4945 4545 2043 6f6e 6665 7265 6e63 6520  IEEE Conference 
-00001240: 4f6e 2047 616d 6573 2e20 e29a a0ef b88f  On Games. ......
-00001250: 202a 2a57 6172 6e69 6e67 2a2a 3a20 506c   **Warning**: Pl
-00001260: 6561 7365 206e 6f74 6520 7468 6174 204e  ease note that N
-00001270: 6569 6768 626f 726c 7927 7320 6375 7272  eighborly's curr
-00001280: 656e 7420 7374 7275 6374 7572 650a 6469  ent structure.di
-00001290: 6666 6572 7320 6772 6561 746c 7920 6672  ffers greatly fr
-000012a0: 6f6d 2074 6865 2076 6572 7369 6f6e 2074  om the version t
-000012b0: 6865 2070 6170 6572 2064 6573 6372 6962  he paper describ
-000012c0: 6573 2e0a 0a23 2043 6f72 6520 4665 6174  es...# Core Feat
-000012d0: 7572 6573 0a0a 2d20 f09f 8f99 efb8 8f20  ures..- ....... 
-000012e0: 5072 6f63 6564 7572 616c 6c79 2067 656e  Procedurally gen
-000012f0: 6572 6174 6573 2061 2073 6574 746c 656d  erates a settlem
-00001300: 656e 7420 616e 6420 7468 6520 6869 7374  ent and the hist
-00001310: 6f72 7920 6f66 2069 7473 2072 6573 6964  ory of its resid
-00001320: 656e 7473 2e0a 2d20 f09f 9a80 2055 7469  ents..- .... Uti
-00001330: 6c69 7a65 2061 206c 6f77 2d66 6964 656c  lize a low-fidel
-00001340: 6974 7920 736f 6369 616c 2073 696d 756c  ity social simul
-00001350: 6174 696f 6e20 746f 2073 696d 756c 6174  ation to simulat
-00001360: 6520 6875 6e64 7265 6473 206f 6620 7965  e hundreds of ye
-00001370: 6172 7320 6f66 2077 6f72 6c64 2068 6973  ars of world his
-00001380: 746f 7279 2077 6974 6869 6e20 6d69 6e75  tory within minu
-00001390: 7465 732e 0a2d 20e2 9a99 efb8 8f20 4275  tes..- ...... Bu
-000013a0: 696c 7420 7573 696e 6720 616e 2065 6e74  ilt using an ent
-000013b0: 6974 792d 636f 6d70 6f6e 656e 7420 7379  ity-component sy
-000013c0: 7374 656d 2028 4543 5329 2061 7263 6869  stem (ECS) archi
-000013d0: 7465 6374 7572 650a 2d20 f09f 93a6 2050  tecture.- .... P
-000013e0: 6c75 6769 6e20 7379 7374 656d 2074 6f20  lugin system to 
-000013f0: 6c6f 6164 2061 6e64 2073 6861 7265 206e  load and share n
-00001400: 6577 2063 6f6e 7465 6e74 2e0a 2d20 f09f  ew content..- ..
-00001410: 9194 2043 6861 7261 6374 6572 7320 6361  .. Characters ca
-00001420: 6e20 7374 6172 7420 6275 7369 6e65 7373  n start business
-00001430: 6573 2061 6e64 2068 6f6c 6420 6a6f 6273  es and hold jobs
-00001440: 2e0a 2d20 efb8 8ff0 9fa7 ac20 4368 6172  ..- ....... Char
-00001450: 6163 7465 7273 2068 6176 6520 7472 6169  acters have trai
-00001460: 7473 2074 6861 7420 6d6f 6469 6679 2074  ts that modify t
-00001470: 6865 6972 2073 7461 7473 2061 6e64 2072  heir stats and r
-00001480: 656c 6174 696f 6e73 6869 7073 2e0a 2d20  elationships..- 
-00001490: e29d a4ef b88f 2043 6861 7261 6374 6572  ...... Character
-000014a0: 7320 666f 726d 2061 6e64 2063 756c 7469  s form and culti
-000014b0: 7661 7465 2072 656c 6174 696f 6e73 6869  vate relationshi
-000014c0: 7073 2062 6173 6564 206f 6e20 726f 6d61  ps based on roma
-000014d0: 6e63 6520 616e 6420 7265 7075 7461 7469  nce and reputati
-000014e0: 6f6e 2e0a 2d20 f09f 92a5 2053 696d 756c  on..- .... Simul
-000014f0: 6174 6520 7261 6e64 6f6d 206c 6966 6520  ate random life 
-00001500: 6576 656e 7473 2074 6861 7420 7370 6963  events that spic
-00001510: 6520 7570 2063 6861 7261 6374 6572 7327  e up characters'
-00001520: 206c 6976 6573 2e0a 2d20 e29a 96ef b88f   lives..- ......
-00001530: 2044 6566 696e 6520 536f 6369 616c 2052   Define Social R
-00001540: 756c 6573 2066 6f72 2068 6f77 2063 6861  ules for how cha
-00001550: 7261 6374 6572 7320 7368 6f75 6c64 2066  racters should f
-00001560: 6565 6c20 6162 6f75 7420 6561 6368 206f  eel about each o
-00001570: 7468 6572 2e0a 2d20 f09f 8fac 2044 6566  ther..- .... Def
-00001580: 696e 6520 6c6f 6361 7469 6f6e 2070 7265  ine location pre
-00001590: 6665 7265 6e63 6520 7275 6c65 7320 666f  ference rules fo
-000015a0: 7220 7768 6174 206c 6f63 6174 696f 6e73  r what locations
-000015b0: 2063 6861 7261 6374 6572 7320 6672 6571   characters freq
-000015c0: 7565 6e74 2e0a 2d20 f09f 9388 2055 7365  uent..- .... Use
-000015d0: 7320 5b50 6f6c 6172 735d 2868 7474 7073  s [Polars](https
-000015e0: 3a2f 2f77 7777 2e70 6f6c 612e 7273 2920  ://www.pola.rs) 
-000015f0: 666f 7220 6661 7374 2064 6174 6120 616e  for fast data an
-00001600: 616c 7973 6973 2e0a 2d20 f09f 939c 2045  alysis..- .... E
-00001610: 7870 6f72 7420 7369 6d75 6c61 7469 6f6e  xport simulation
-00001620: 2064 6174 6120 746f 204a 534f 4e2e 0a0a   data to JSON...
-00001630: 2320 5379 7374 656d 2063 6176 6561 7473  # System caveats
-00001640: 0a0a 2d20 4f6e 6c79 2073 696d 756c 6174  ..- Only simulat
-00001650: 6573 2061 2073 696e 676c 6520 7365 7474  es a single sett
-00001660: 6c65 6d65 6e74 0a2d 2043 6861 7261 6374  lement.- Charact
-00001670: 6572 7320 6361 6e20 6f6e 6c79 2068 6f6c  ers can only hol
-00001680: 6420 6f6e 6520 6f63 6375 7061 7469 6f6e  d one occupation
-00001690: 2061 7420 6120 7469 6d65 2e0a 2d20 446f   at a time..- Do
-000016a0: 6573 206e 6f74 206d 6f64 656c 2074 6865  es not model the
-000016b0: 2065 7861 6374 2070 6f73 6974 696f 6e20   exact position 
-000016c0: 6f66 2065 6e74 6974 6965 732e 0a0a 2320  of entities...# 
-000016d0: 5472 7920 4e65 6967 6862 6f72 6c79 2077  Try Neighborly w
-000016e0: 6974 686f 7574 2069 6e73 7461 6c6c 696e  ithout installin
-000016f0: 670a 0a4e 6569 6768 626f 726c 7920 6973  g..Neighborly is
-00001700: 2061 7661 696c 6162 6c65 2074 6f20 7573   available to us
-00001710: 6520 7769 7468 696e 2074 6869 7320 5b73  e within this [s
-00001720: 616d 706c 6520 476f 6f67 6c65 2043 6f6c  ample Google Col
-00001730: 6162 206e 6f74 6562 6f6f 6b5d 2868 7474  ab notebook](htt
-00001740: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
-00001750: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f64  rch.google.com/d
-00001760: 7269 7665 2f31 5778 5a6e 4352 3861 6665  rive/1WxZnCR8afe
-00001770: 6b66 426c 2d76 4936 5763 4963 5336 4f68  kfBl-vI6WcIcS6Oh
-00001780: 5247 646b 616d 3f75 7370 3d73 6861 7269  RGdkam?usp=shari
-00001790: 6e67 292e 2049 7420 636f 6e74 6169 6e73  ng). It contains
-000017a0: 2061 2062 6173 6963 2077 616c 6b74 6872   a basic walkthr
-000017b0: 6f75 6768 206f 6620 686f 7720 746f 2064  ough of how to d
-000017c0: 6566 696e 6520 636f 6e74 656e 7420 666f  efine content fo
-000017d0: 7220 7468 6520 7369 6d75 6c61 7469 6f6e  r the simulation
-000017e0: 2061 6e64 2069 6e73 7065 6374 2074 6865   and inspect the
-000017f0: 2067 656e 6572 6174 6564 2064 6174 612e   generated data.
-00001800: 0a0a 2320 496e 7374 616c 6c61 7469 6f6e  ..# Installation
-00001810: 0a0a 5468 6520 6c61 7465 7374 206f 6666  ..The latest off
-00001820: 6963 6961 6c20 7265 6c65 6173 6520 6f66  icial release of
-00001830: 204e 6569 6768 626f 726c 7920 6973 2061   Neighborly is a
-00001840: 7661 696c 6162 6c65 2074 6f20 696e 7374  vailable to inst
-00001850: 616c 6c20 6672 6f6d 205b 5079 5049 5d28  all from [PyPI](
-00001860: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00001870: 2f70 726f 6a65 6374 2f6e 6569 6768 626f  /project/neighbo
-00001880: 726c 792f 292e 0a0a 6060 6062 6173 680a  rly/)...```bash.
-00001890: 7069 7020 696e 7374 616c 6c20 6e65 6967  pip install neig
-000018a0: 6862 6f72 6c79 0a60 6060 0a0a 2323 2049  hborly.```..## I
-000018b0: 6e73 7461 6c6c 696e 6720 666f 7220 6c6f  nstalling for lo
-000018c0: 6361 6c20 6465 7665 6c6f 706d 656e 740a  cal development.
-000018d0: 0a49 6620 796f 7520 7769 7368 2074 6f20  .If you wish to 
-000018e0: 646f 776e 6c6f 6164 2061 204e 6569 6768  download a Neigh
-000018f0: 626f 726c 7920 666f 7220 6c6f 6361 6c20  borly for local 
-00001900: 6465 7665 6c6f 706d 656e 7420 6f72 2077  development or w
-00001910: 616e 7420 746f 2070 6c61 7920 6172 6f75  ant to play arou
-00001920: 6e64 2077 6974 680a 616e 7920 6f66 2074  nd with.any of t
-00001930: 6865 2073 616d 706c 6573 2c20 796f 7520  he samples, you 
-00001940: 6e65 6564 2074 6f20 636c 6f6e 6520 6f72  need to clone or
-00001950: 2064 6f77 6e6c 6f61 6420 7468 6973 2072   download this r
-00001960: 6570 6f73 6974 6f72 7920 616e 6420 696e  epository and in
-00001970: 7374 616c 6c0a 7573 696e 6720 7468 6520  stall.using the 
-00001980: 5f65 6469 7461 626c 655f 2066 6c61 6720  _editable_ flag 
-00001990: 282d 6529 2e20 506c 6561 7365 2073 6565  (-e). Please see
-000019a0: 2074 6865 2069 6e73 7472 7563 7469 6f6e   the instruction
-000019b0: 7320 6265 6c6f 772e 2054 6869 7320 636f  s below. This co
-000019c0: 6d6d 616e 6420 7769 6c6c 2069 6e73 7461  mmand will insta
-000019d0: 6c6c 0a61 204e 6569 6768 626f 726c 7920  ll.a Neighborly 
-000019e0: 696e 746f 2074 6865 2076 6972 7475 616c  into the virtual
-000019f0: 2065 6e76 6972 6f6e 6d65 6e74 2061 6c6f   environment alo
-00001a00: 6e67 2077 6974 6820 616c 6c20 6974 7320  ng with all its 
-00001a10: 6465 7065 6e64 656e 6369 6573 2061 6e64  dependencies and
-00001a20: 2061 2066 6577 0a61 6464 6974 696f 6e61   a few.additiona
-00001a30: 6c20 6465 7665 6c6f 706d 656e 7420 616e  l development an
-00001a40: 6420 7465 7374 696e 6720 6465 7065 6e64  d testing depend
-00001a50: 656e 6369 6573 2073 7563 6820 6173 205f  encies such as _
-00001a60: 626c 6163 6b5f 2c20 5f69 736f 7274 5f2c  black_, _isort_,
-00001a70: 2061 6e64 205f 7079 7465 7374 5f2e 0a0a   and _pytest_...
-00001a80: 6060 6062 6173 680a 2320 5374 6570 2031  ```bash.# Step 1
-00001a90: 3a20 436c 6f6e 6520 5265 706f 7369 746f  : Clone Reposito
-00001aa0: 7279 2061 6e64 2063 6861 6e67 6520 696e  ry and change in
-00001ab0: 746f 2070 726f 6a65 6374 2064 6972 6563  to project direc
-00001ac0: 746f 7279 0a67 6974 2063 6c6f 6e65 2068  tory.git clone h
-00001ad0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001ae0: 6d2f 5368 694a 6265 792f 6e65 6967 6862  m/ShiJbey/neighb
-00001af0: 6f72 6c79 2e67 6974 0a63 6420 6e65 6967  orly.git.cd neig
-00001b00: 6862 6f72 6c79 0a0a 2320 5374 6570 2032  hborly..# Step 2
-00001b10: 2028 4d61 634f 532f 4c69 6e75 7829 3a20   (MacOS/Linux): 
-00001b20: 4372 6561 7465 2061 6e64 2061 6374 6976  Create and activ
-00001b30: 6174 6520 6120 5079 7468 6f6e 2076 6972  ate a Python vir
-00001b40: 7475 616c 2065 6e76 6972 6f6e 6d65 6e74  tual environment
-00001b50: 0a70 7974 686f 6e33 202d 6d20 7665 6e76  .python3 -m venv
-00001b60: 2076 656e 760a 736f 7572 6365 202e 2f76   venv.source ./v
-00001b70: 656e 762f 6269 6e2f 6163 7469 7661 7465  env/bin/activate
-00001b80: 0a0a 2320 5374 6570 2032 2028 5769 6e64  ..# Step 2 (Wind
-00001b90: 6f77 7329 3a20 4372 6561 7465 2061 6e64  ows): Create and
-00001ba0: 2061 6374 6976 6174 6520 6120 5079 7468   activate a Pyth
-00001bb0: 6f6e 2076 6972 7475 616c 2065 6e76 6972  on virtual envir
-00001bc0: 6f6e 6d65 6e74 0a70 7974 686f 6e20 2d6d  onment.python -m
-00001bd0: 2076 656e 7620 7665 6e76 0a2e 5c76 656e   venv venv..\ven
-00001be0: 765c 5363 7269 7074 735c 4163 7469 7661  v\Scripts\Activa
-00001bf0: 7465 0a0a 2320 5374 6570 2033 3a20 496e  te..# Step 3: In
-00001c00: 7374 616c 6c20 6c6f 6361 6c20 6275 696c  stall local buil
-00001c10: 6420 616e 6420 6465 7065 6e64 656e 6369  d and dependenci
-00001c20: 6573 0a70 7974 686f 6e20 2d6d 2070 6970  es.python -m pip
-00001c30: 2069 6e73 7461 6c6c 202d 6520 222e 5b64   install -e ".[d
-00001c40: 6576 656c 6f70 6d65 6e74 5d22 0a60 6060  evelopment]".```
-00001c50: 0a0a 2320 5573 6167 650a 0a54 6865 2062  ..# Usage..The b
-00001c60: 6573 7420 7761 7920 746f 206c 6561 726e  est way to learn
-00001c70: 2068 6f77 2074 6f20 7573 6520 4e65 6967   how to use Neig
-00001c80: 6862 6f72 6c79 2069 7320 746f 2065 7870  hborly is to exp
-00001c90: 6c6f 7265 2074 6865 2076 6172 696f 7573  lore the various
-00001ca0: 2073 616d 706c 6573 2069 6e20 7468 6520   samples in the 
-00001cb0: 6073 616d 706c 6573 6020 6469 7265 6374  `samples` direct
-00001cc0: 6f72 790a 7468 6174 2064 656d 6f6e 7374  ory.that demonst
-00001cd0: 7261 7465 2068 6f77 2074 6f20 6372 6561  rate how to crea
-00001ce0: 7465 2063 7573 746f 6d20 7369 6d75 6c61  te custom simula
-00001cf0: 7469 6f6e 7320 616e 6420 636f 6c6c 6563  tions and collec
-00001d00: 7420 616e 6420 7669 7375 616c 697a 6520  t and visualize 
-00001d10: 6461 7461 2e20 496e 7465 7261 6374 6976  data. Interactiv
-00001d20: 6520 7361 6d70 6c65 7320 7769 7468 2074  e samples with t
-00001d30: 6865 2060 2e69 7079 6e62 600a 6578 7465  he `.ipynb`.exte
-00001d40: 6e73 696f 6e20 6172 6520 6d65 616e 7420  nsion are meant 
-00001d50: 746f 2062 6520 7275 6e20 7573 696e 6720  to be run using 
-00001d60: 5b4a 7570 7974 6572 204c 6162 5d28 6874  [Jupyter Lab](ht
-00001d70: 7470 733a 2f2f 6a75 7079 7465 722e 6f72  tps://jupyter.or
-00001d80: 672f 292e 2050 6c65 6173 6520 7275 6e20  g/). Please run 
-00001d90: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
-00001da0: 6d6d 616e 640a 746f 2065 6e73 7572 6520  mmand.to ensure 
-00001db0: 616c 6c20 6465 7065 6e64 656e 6369 6573  all dependencies
-00001dc0: 2061 7265 2069 6e73 7461 6c6c 6564 2066   are installed f
-00001dd0: 6f72 2074 6865 2073 616d 706c 6573 2e20  or the samples. 
-00001de0: 4d61 6b65 2073 7572 6520 7468 6174 2079  Make sure that y
-00001df0: 6f75 2776 6520 6163 7469 7661 7465 6420  ou've activated 
-00001e00: 796f 7572 2050 7974 686f 6e20 7669 7274  your Python virt
-00001e10: 7561 6c0a 656e 7669 726f 6e6d 656e 7420  ual.environment 
-00001e20: 6265 666f 7265 6861 6e64 2e0a 0a60 6060  beforehand...```
-00001e30: 6261 7368 0a70 7974 686f 6e20 2d6d 2070  bash.python -m p
-00001e40: 6970 2069 6e73 7461 6c6c 202d 6520 222e  ip install -e ".
-00001e50: 5b73 616d 706c 6573 5d22 0a60 6060 0a0a  [samples]".```..
-00001e60: 5468 656e 2c20 7275 6e20 7468 6520 666f  Then, run the fo
-00001e70: 6c6c 6f77 696e 6720 636f 6d6d 616e 6473  llowing commands
-00001e80: 2074 6f20 7275 6e20 7468 6520 7361 6d70   to run the samp
-00001e90: 6c65 2073 6372 6970 7473 206f 7220 6e6f  le scripts or no
-00001ea0: 7465 626f 6f6b 732e 0a0a 6060 6062 6173  tebooks...```bas
-00001eb0: 680a 2320 546f 2072 756e 2073 616d 706c  h.# To run sampl
-00001ec0: 6520 7363 7269 7074 732c 2075 7365 3a0a  e scripts, use:.
-00001ed0: 7079 7468 6f6e 202e 2f73 616d 706c 6573  python ./samples
-00001ee0: 2f3c 6e61 6d65 5f6f 665f 7361 6d70 6c65  /<name_of_sample
-00001ef0: 3e2e 7079 0a0a 2320 4578 706c 6f72 6520  >.py..# Explore 
-00001f00: 4950 7974 686f 6e20 6e6f 7465 626f 6f6b  IPython notebook
-00001f10: 7320 7573 696e 6720 4a75 7079 7465 7220  s using Jupyter 
-00001f20: 4c61 623a 0a6a 7570 7974 6572 2d6c 6162  Lab:.jupyter-lab
-00001f30: 0a60 6060 0a0a 2320 506c 7567 696e 730a  .```..# Plugins.
-00001f40: 0a50 6c75 6769 6e73 2061 7265 2069 6d70  .Plugins are imp
-00001f50: 6f72 7461 626c 6520 5079 7468 6f6e 206d  ortable Python m
-00001f60: 6f64 756c 6573 206f 7220 7061 636b 6167  odules or packag
-00001f70: 6573 2074 6861 7420 6164 6420 6e65 7720  es that add new 
-00001f80: 636f 6e74 656e 7420 746f 2061 2073 696d  content to a sim
-00001f90: 756c 6174 696f 6e2e 2054 6865 7920 616c  ulation. They al
-00001fa0: 6c6f 7720 7573 6572 7320 746f 2063 6861  low users to cha
-00001fb0: 6e67 650a 6120 7369 6d75 6c61 7469 6f6e  nge.a simulation
-00001fc0: 2773 2062 6568 6176 696f 7220 7769 7468  's behavior with
-00001fd0: 6f75 7420 6564 6974 696e 6720 7468 6520  out editing the 
-00001fe0: 636f 7265 206c 6962 7261 7279 2063 6f64  core library cod
-00001ff0: 652e 2041 6c6c 2070 6c75 6769 6e73 2073  e. All plugins s
-00002000: 686f 756c 6420 6861 7665 2061 2074 6f70  hould have a top
-00002010: 2d6c 6576 656c 0a60 6c6f 6164 5f70 6c75  -level.`load_plu
-00002020: 6769 6e28 7369 6d29 6020 6675 6e63 7469  gin(sim)` functi
-00002030: 6f6e 2074 6861 7420 6765 7473 2063 616c  on that gets cal
-00002040: 6c65 6420 746f 206c 6f61 6420 696e 2074  led to load in t
-00002050: 6865 2070 6c75 6769 6e20 636f 6e74 656e  he plugin conten
-00002060: 742e 0a0a 4173 2077 6974 6820 616e 7920  t...As with any 
-00002070: 7069 6563 6520 6f66 2073 6f66 7477 6172  piece of softwar
-00002080: 652c 2061 6c77 6179 7320 6578 7072 6573  e, always expres
-00002090: 7320 6361 7574 696f 6e20 7768 656e 2064  s caution when d
-000020a0: 6f77 6e6c 6f61 6469 6e67 2074 6869 7264  ownloading third
-000020b0: 2d70 6172 7479 2070 6c75 6769 6e73 2e20  -party plugins. 
-000020c0: 456e 7375 7265 2074 6865 7920 636f 6d65  Ensure they come
-000020d0: 2066 726f 6d20 610a 736f 7572 6365 2074   from a.source t
-000020e0: 6861 7420 796f 7520 7472 7573 742e 0a0a  hat you trust...
-000020f0: 546f 2072 6561 6420 6d6f 7265 2061 626f  To read more abo
-00002100: 7574 2070 6c75 6769 6e73 2c20 7669 7369  ut plugins, visi
-00002110: 7420 7468 6520 5b50 6c75 6769 6e73 5d28  t the [Plugins](
-00002120: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002130: 6f6d 2f53 6869 4a62 6579 2f6e 6569 6768  om/ShiJbey/neigh
-00002140: 626f 726c 792f 7769 6b69 2f70 6c75 6769  borly/wiki/plugi
-00002150: 6e73 2920 7365 6374 696f 6e20 6f66 2074  ns) section of t
-00002160: 6865 0a77 696b 692e 0a0a 2320 5465 7374  he.wiki...# Test
-00002170: 730a 0a4e 6569 6768 626f 726c 7920 7573  s..Neighborly us
-00002180: 6573 205b 5079 5465 7374 5d28 6874 7470  es [PyTest](http
-00002190: 733a 2f2f 646f 6373 2e70 7974 6573 742e  s://docs.pytest.
-000021a0: 6f72 672f 2920 666f 7220 756e 6974 2074  org/) for unit t
-000021b0: 6573 7469 6e67 2e20 416c 6c20 7465 7374  esting. All test
-000021c0: 7320 6172 6520 6c6f 6361 7465 6420 696e  s are located in
-000021d0: 2074 6865 2060 7465 7374 732f 6020 6469   the `tests/` di
-000021e0: 7265 6374 6f72 792e 2049 0a64 6f20 6d79  rectory. I.do my
-000021f0: 2062 6573 7420 746f 206b 6565 7020 7465   best to keep te
-00002200: 7374 7320 7570 6461 7465 642e 2048 6f77  sts updated. How
-00002210: 6576 6572 2c20 736f 6d65 2074 6573 7473  ever, some tests
-00002220: 206d 6179 206e 6565 6420 746f 2062 650a   may need to be.
-00002230: 6164 6465 6420 6f72 2075 7064 6174 6564  added or updated
-00002240: 2064 7565 2074 6f20 636f 6e73 7461 6e74   due to constant
-00002250: 2062 7265 616b 696e 6720 6368 616e 6765   breaking change
-00002260: 7320 6265 7477 6565 6e20 7265 6c65 6173  s between releas
-00002270: 6573 2e20 4966 2079 6f75 2077 616e 7420  es. If you want 
-00002280: 746f 2063 6f6e 7472 6962 7574 6520 756e  to contribute un
-00002290: 6974 2074 6573 7473 2c20 706c 6561 7365  it tests, please
-000022a0: 2072 6566 6572 0a74 6f20 5b43 4f4e 5452   refer.to [CONTR
-000022b0: 4942 5554 494e 472e 6d64 5d28 2e2f 434f  IBUTING.md](./CO
-000022c0: 4e54 5249 4255 5449 4e47 2e6d 6429 2e0a  NTRIBUTING.md)..
-000022d0: 0a60 6060 6261 7368 0a23 2053 7465 7020  .```bash.# Step 
-000022e0: 313a 2049 6e73 7461 6c6c 2061 6464 6974  1: Install addit
-000022f0: 696f 6e61 6c20 6465 7065 6e64 656e 6369  ional dependenci
-00002300: 6573 2066 6f72 2074 6573 7473 0a70 7974  es for tests.pyt
-00002310: 686f 6e20 2d6d 2070 6970 2069 6e73 7461  hon -m pip insta
-00002320: 6c6c 202d 6520 222e 5b64 6576 656c 6f70  ll -e ".[develop
-00002330: 6d65 6e74 5d22 0a0a 2320 5374 6570 2032  ment]"..# Step 2
-00002340: 3a20 5275 6e20 5079 7465 7374 0a70 7974  : Run Pytest.pyt
-00002350: 6573 740a 0a23 2053 7465 7033 203a 2028  est..# Step3 : (
-00002360: 4f70 7469 6f6e 616c 2920 4765 6e65 7261  Optional) Genera
-00002370: 7465 2061 2074 6573 7420 636f 7665 7261  te a test covera
-00002380: 6765 2072 6570 6f72 740a 7079 7465 7374  ge report.pytest
-00002390: 202d 2d63 6f76 3d6e 6569 6768 626f 726c   --cov=neighborl
-000023a0: 7920 7465 7374 732f 0a60 6060 0a0a 2320  y tests/.```..# 
-000023b0: 446f 6375 6d65 6e74 6174 696f 6e0a 0a54  Documentation..T
-000023c0: 6865 2062 6573 7420 706c 6163 6520 746f  he best place to
-000023d0: 2066 696e 6420 6578 616d 706c 6573 206f   find examples o
-000023e0: 6620 686f 7720 746f 2075 7365 204e 6569  f how to use Nei
-000023f0: 6768 626f 726c 7920 6973 2061 6374 7561  ghborly is actua
-00002400: 6c6c 7920 696e 2074 6865 2060 2e2f 7465  lly in the `./te
-00002410: 7374 7360 2064 6972 6563 746f 7279 2e20  sts` directory. 
-00002420: 5468 6572 6520 796f 7520 7769 6c6c 2066  There you will f
-00002430: 696e 6420 6578 616d 706c 6573 206f 6620  ind examples of 
-00002440: 6c6f 6164 696e 6720 636f 6e74 656e 7420  loading content 
-00002450: 6672 6f6d 2066 696c 6573 2c20 7275 6e6e  from files, runn
-00002460: 696e 6720 6120 7369 6d75 6c61 7469 6f6e  ing a simulation
-00002470: 2c20 616e 6420 7361 7669 6e67 2074 6865  , and saving the
-00002480: 206f 7574 7075 7420 746f 204a 534f 4e2e   output to JSON.
-00002490: 2054 6865 7265 2069 7320 616c 736f 2074   There is also t
-000024a0: 6865 205b 5265 6164 2074 6865 2044 6f63  he [Read the Doc
-000024b0: 735d 2868 7474 7073 3a2f 2f6e 6569 6768  s](https://neigh
-000024c0: 626f 726c 792e 7265 6164 7468 6564 6f63  borly.readthedoc
-000024d0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f69  s.io/en/latest/i
-000024e0: 6e64 6578 2e68 746d 6c29 2e20 486f 7765  ndex.html). Howe
-000024f0: 7665 722c 2074 6865 2064 6f63 7320 6861  ver, the docs ha
-00002500: 7320 6120 7465 6e64 656e 6379 2074 6f20  s a tendency to 
-00002510: 6265 206f 7574 206f 6620 6461 7465 2077  be out of date w
-00002520: 6865 6e20 6e65 772c 2070 6f74 656e 7469  hen new, potenti
-00002530: 616c 6c79 2062 7265 616b 696e 6720 6368  ally breaking ch
-00002540: 616e 6765 7320 6172 6520 6d61 6465 2074  anges are made t
-00002550: 6f20 7468 6520 6672 616d 6577 6f72 6b2e  o the framework.
-00002560: 2048 6f77 6576 6572 2c20 756e 6974 2074   However, unit t
-00002570: 6573 7473 2061 7265 2075 7064 6174 6564  ests are updated
-00002580: 2061 6c6d 6f73 7420 6576 6572 7920 7469   almost every ti
-00002590: 6d65 2061 206e 6577 2066 6561 7475 7265  me a new feature
-000025a0: 2069 7320 6164 6465 642e 0a0a 2320 4765   is added...# Ge
-000025b0: 7474 696e 6720 6865 6c70 2061 6e64 2073  tting help and s
-000025c0: 7562 6d69 7474 696e 6720 6275 6720 7265  ubmitting bug re
-000025d0: 706f 7274 730a 0a49 6620 796f 7520 6861  ports..If you ha
-000025e0: 7665 2061 6e79 2071 7565 7374 696f 6e73  ve any questions
-000025f0: 2c20 6665 6564 6261 636b 2c20 6f72 2070  , feedback, or p
-00002600: 726f 626c 656d 732c 2070 6c65 6173 6520  roblems, please 
-00002610: 6372 6561 7465 2061 206e 6577 2049 7373  create a new Iss
-00002620: 7565 2e20 4920 7769 6c6c 2064 6f20 6d79  ue. I will do my
-00002630: 2062 6573 7420 746f 2061 6e73 7765 7220   best to answer 
-00002640: 6173 2073 6f6f 6e20 6173 2049 0a63 616e  as soon as I.can
-00002650: 2e20 506c 6561 7365 2062 6520 7265 7370  . Please be resp
-00002660: 6563 7466 756c 2c20 616e 6420 4920 6170  ectful, and I ap
-00002670: 7072 6563 6961 7465 2079 6f75 7220 7061  preciate your pa
-00002680: 7469 656e 6365 2e0a 0a23 2043 6f6e 7472  tience...# Contr
-00002690: 6962 7574 696e 670a 0a43 6f6e 7472 6962  ibuting..Contrib
-000026a0: 7574 696f 6e73 2061 7265 2077 656c 636f  utions are welco
-000026b0: 6d65 2e20 506c 6561 7365 2072 6566 6572  me. Please refer
-000026c0: 2074 6f20 5b43 4f4e 5452 4942 5554 494e   to [CONTRIBUTIN
-000026d0: 472e 6d64 5d28 2e2f 434f 4e54 5249 4255  G.md](./CONTRIBU
-000026e0: 5449 4e47 2e6d 6429 2066 6f72 206d 6f72  TING.md) for mor
-000026f0: 6520 696e 666f 726d 6174 696f 6e20 6162  e information ab
-00002700: 6f75 7420 686f 7720 746f 2067 6574 0a69  out how to get.i
-00002710: 6e76 6f6c 7665 642e 0a0a 2320 4c69 6365  nvolved...# Lice
-00002720: 6e73 650a 0a54 6869 7320 7072 6f6a 6563  nse..This projec
-00002730: 7420 6973 206c 6963 656e 7365 6420 756e  t is licensed un
-00002740: 6465 7220 7468 6520 5b4d 4954 204c 6963  der the [MIT Lic
-00002750: 656e 7365 5d28 2e2f 4c49 4345 4e53 4529  ense](./LICENSE)
-00002760: 2e0a 0a23 2044 4d43 4120 5374 6174 656d  ...# DMCA Statem
-00002770: 656e 740a 0a55 706f 6e20 7265 6365 6970  ent..Upon receip
-00002780: 7420 6f66 2061 206e 6f74 6963 6520 616c  t of a notice al
-00002790: 6c65 6769 6e67 2063 6f70 7972 6967 6874  leging copyright
-000027a0: 2069 6e66 7269 6e67 656d 656e 742c 2049   infringement, I
-000027b0: 2077 696c 6c20 7461 6b65 2077 6861 7465   will take whate
-000027c0: 7665 7220 6163 7469 6f6e 2069 7420 6465  ver action it de
-000027d0: 656d 7320 6170 7072 6f70 7269 6174 6520  ems appropriate 
-000027e0: 7769 7468 696e 2069 7473 0a73 6f6c 6520  within its.sole 
-000027f0: 6469 7363 7265 7469 6f6e 2c20 696e 636c  discretion, incl
-00002800: 7564 696e 6720 7265 6d6f 7661 6c20 6f66  uding removal of
-00002810: 2074 6865 2061 6c6c 6567 6564 6c79 2069   the allegedly i
-00002820: 6e66 7269 6e67 696e 6720 6d61 7465 7269  nfringing materi
-00002830: 616c 732e 0a0a 5468 6520 7265 706f 2069  als...The repo i
-00002840: 6d61 6765 2069 7320 736f 6d65 7468 696e  mage is somethin
-00002850: 6720 6675 6e20 7468 6174 2049 206d 6164  g fun that I mad
-00002860: 652e 2049 206c 6f76 6520 5f54 6865 2053  e. I love _The S
-00002870: 696d 7073 6f6e 735f 2c20 616e 6420 4920  impsons_, and I 
-00002880: 636f 756c 646e 2774 2074 6869 6e6b 206f  couldn't think o
-00002890: 6620 616e 796f 6e65 206d 6f72 6520 6e65  f anyone more ne
-000028a0: 6967 6862 6f72 6c79 2074 6861 6e0a 4e65  ighborly than.Ne
-000028b0: 6420 466c 616e 6465 7273 2e20 4966 2074  d Flanders. If t
-000028c0: 6865 2063 6f70 7972 6967 6874 206f 776e  he copyright own
-000028d0: 6572 2066 6f72 205f 5468 6520 5369 6d70  er for _The Simp
-000028e0: 736f 6e73 5f20 776f 756c 6420 6c69 6b65  sons_ would like
-000028f0: 206d 6520 746f 2074 616b 6520 6974 2064   me to take it d
-00002900: 6f77 6e2c 2070 6c65 6173 6520 636f 6e74  own, please cont
-00002910: 6163 7420 6d65 2e20 5468 6520 7361 6d65  act me. The same
-00002920: 0a74 616b 6564 6f77 6e20 706f 6c69 6379  .takedown policy
-00002930: 2061 7070 6c69 6573 2074 6f20 636f 6465   applies to code
-00002940: 2073 616d 706c 6573 2069 6e73 7069 7265   samples inspire
-00002950: 6420 6279 2054 5620 7368 6f77 732c 206d  d by TV shows, m
-00002960: 6f76 6965 732c 2061 6e64 2067 616d 6573  ovies, and games
-00002970: 2e0a                                     ..
+00000030: 332e 302e 302e 6465 7631 0a53 756d 6d61  3.0.0.dev1.Summa
+00000040: 7279 3a20 4120 6368 6172 6163 7465 722d  ry: A character-
+00000050: 666f 6375 7365 6420 7365 7474 6c65 6d65  focused settleme
+00000060: 6e74 2067 656e 6572 6174 6f72 2075 7469  nt generator uti
+00000070: 6c69 7a69 6e67 2061 6765 6e74 2d62 6173  lizing agent-bas
+00000080: 6564 2073 6f63 6961 6c20 7369 6d75 6c61  ed social simula
+00000090: 7469 6f6e 2e0a 4175 7468 6f72 2d65 6d61  tion..Author-ema
+000000a0: 696c 3a20 5368 6920 4a6f 686e 736f 6e2d  il: Shi Johnson-
+000000b0: 4265 7920 3c73 6869 6a62 6579 4067 6d61  Bey <shijbey@gma
+000000c0: 696c 2e63 6f6d 3e0a 4c69 6365 6e73 653a  il.com>.License:
+000000d0: 2023 204d 4954 204c 4943 454e 5345 0a20   # MIT LICENSE. 
+000000e0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000000f0: 436f 7079 7269 6768 7420 3230 3232 2d32  Copyright 2022-2
+00000100: 3032 3420 5368 6920 4a6f 686e 736f 6e2d  024 Shi Johnson-
+00000110: 4265 7920 3c73 6869 6a62 6579 4067 6d61  Bey <shijbey@gma
+00000120: 696c 2e63 6f6d 3e0a 2020 2020 2020 2020  il.com>.        
+00000130: 0a20 2020 2020 2020 2050 6572 6d69 7373  .        Permiss
+00000140: 696f 6e20 6973 2068 6572 6562 7920 6772  ion is hereby gr
+00000150: 616e 7465 642c 2066 7265 6520 6f66 2063  anted, free of c
+00000160: 6861 7267 652c 2074 6f20 616e 7920 7065  harge, to any pe
+00000170: 7273 6f6e 206f 6274 6169 6e69 6e67 2061  rson obtaining a
+00000180: 2063 6f70 7920 6f66 2074 6869 730a 2020   copy of this.  
+00000190: 2020 2020 2020 736f 6674 7761 7265 2061        software a
+000001a0: 6e64 2061 7373 6f63 6961 7465 6420 646f  nd associated do
+000001b0: 6375 6d65 6e74 6174 696f 6e20 6669 6c65  cumentation file
+000001c0: 7320 2874 6865 2022 536f 6674 7761 7265  s (the "Software
+000001d0: 2229 2c20 746f 2064 6561 6c20 696e 2074  "), to deal in t
+000001e0: 6865 2053 6f66 7477 6172 650a 2020 2020  he Software.    
+000001f0: 2020 2020 7769 7468 6f75 7420 7265 7374      without rest
+00000200: 7269 6374 696f 6e2c 2069 6e63 6c75 6469  riction, includi
+00000210: 6e67 2077 6974 686f 7574 206c 696d 6974  ng without limit
+00000220: 6174 696f 6e20 7468 6520 7269 6768 7473  ation the rights
+00000230: 2074 6f20 7573 652c 2063 6f70 792c 206d   to use, copy, m
+00000240: 6f64 6966 792c 0a20 2020 2020 2020 206d  odify,.        m
+00000250: 6572 6765 2c20 7075 626c 6973 682c 2064  erge, publish, d
+00000260: 6973 7472 6962 7574 652c 2073 7562 6c69  istribute, subli
+00000270: 6365 6e73 652c 2061 6e64 2f6f 7220 7365  cense, and/or se
+00000280: 6c6c 2063 6f70 6965 7320 6f66 2074 6865  ll copies of the
+00000290: 2053 6f66 7477 6172 652c 2061 6e64 2074   Software, and t
+000002a0: 6f0a 2020 2020 2020 2020 7065 726d 6974  o.        permit
+000002b0: 2070 6572 736f 6e73 2074 6f20 7768 6f6d   persons to whom
+000002c0: 2074 6865 2053 6f66 7477 6172 6520 6973   the Software is
+000002d0: 2066 7572 6e69 7368 6564 2074 6f20 646f   furnished to do
+000002e0: 2073 6f2c 2073 7562 6a65 6374 2074 6f20   so, subject to 
+000002f0: 7468 6520 666f 6c6c 6f77 696e 670a 2020  the following.  
+00000300: 2020 2020 2020 636f 6e64 6974 696f 6e73        conditions
+00000310: 3a0a 2020 2020 2020 2020 0a20 2020 2020  :.        .     
+00000320: 2020 2054 6865 2061 626f 7665 2063 6f70     The above cop
+00000330: 7972 6967 6874 206e 6f74 6963 6520 616e  yright notice an
+00000340: 6420 7468 6973 2070 6572 6d69 7373 696f  d this permissio
+00000350: 6e20 6e6f 7469 6365 2073 6861 6c6c 2062  n notice shall b
+00000360: 6520 696e 636c 7564 6564 2069 6e20 616c  e included in al
+00000370: 6c20 636f 7069 6573 0a20 2020 2020 2020  l copies.       
+00000380: 206f 7220 7375 6273 7461 6e74 6961 6c20   or substantial 
+00000390: 706f 7274 696f 6e73 206f 6620 7468 6520  portions of the 
+000003a0: 536f 6674 7761 7265 2e0a 2020 2020 2020  Software..      
+000003b0: 2020 0a20 2020 2020 2020 2054 4845 2053    .        THE S
+000003c0: 4f46 5457 4152 4520 4953 2050 524f 5649  OFTWARE IS PROVI
+000003d0: 4445 4420 2241 5320 4953 222c 2057 4954  DED "AS IS", WIT
+000003e0: 484f 5554 2057 4152 5241 4e54 5920 4f46  HOUT WARRANTY OF
+000003f0: 2041 4e59 204b 494e 442c 2045 5850 5245   ANY KIND, EXPRE
+00000400: 5353 204f 5220 494d 504c 4945 442c 0a20  SS OR IMPLIED,. 
+00000410: 2020 2020 2020 2049 4e43 4c55 4449 4e47         INCLUDING
+00000420: 2042 5554 204e 4f54 204c 494d 4954 4544   BUT NOT LIMITED
+00000430: 2054 4f20 5448 4520 5741 5252 414e 5449   TO THE WARRANTI
+00000440: 4553 204f 4620 4d45 5243 4841 4e54 4142  ES OF MERCHANTAB
+00000450: 494c 4954 592c 2046 4954 4e45 5353 2046  ILITY, FITNESS F
+00000460: 4f52 2041 0a20 2020 2020 2020 2050 4152  OR A.        PAR
+00000470: 5449 4355 4c41 5220 5055 5250 4f53 4520  TICULAR PURPOSE 
+00000480: 414e 4420 4e4f 4e49 4e46 5249 4e47 454d  AND NONINFRINGEM
+00000490: 454e 542e 2049 4e20 4e4f 2045 5645 4e54  ENT. IN NO EVENT
+000004a0: 2053 4841 4c4c 2054 4845 2041 5554 484f   SHALL THE AUTHO
+000004b0: 5253 204f 5220 434f 5059 5249 4748 540a  RS OR COPYRIGHT.
+000004c0: 2020 2020 2020 2020 484f 4c44 4552 5320          HOLDERS 
+000004d0: 4245 204c 4941 424c 4520 464f 5220 414e  BE LIABLE FOR AN
+000004e0: 5920 434c 4149 4d2c 2044 414d 4147 4553  Y CLAIM, DAMAGES
+000004f0: 204f 5220 4f54 4845 5220 4c49 4142 494c   OR OTHER LIABIL
+00000500: 4954 592c 2057 4845 5448 4552 2049 4e20  ITY, WHETHER IN 
+00000510: 414e 2041 4354 494f 4e20 4f46 0a20 2020  AN ACTION OF.   
+00000520: 2020 2020 2043 4f4e 5452 4143 542c 2054       CONTRACT, T
+00000530: 4f52 5420 4f52 204f 5448 4552 5749 5345  ORT OR OTHERWISE
+00000540: 2c20 4152 4953 494e 4720 4652 4f4d 2c20  , ARISING FROM, 
+00000550: 4f55 5420 4f46 204f 5220 494e 2043 4f4e  OUT OF OR IN CON
+00000560: 4e45 4354 494f 4e20 5749 5448 2054 4845  NECTION WITH THE
+00000570: 2053 4f46 5457 4152 450a 2020 2020 2020   SOFTWARE.      
+00000580: 2020 4f52 2054 4845 2055 5345 204f 5220    OR THE USE OR 
+00000590: 4f54 4845 5220 4445 414c 494e 4753 2049  OTHER DEALINGS I
+000005a0: 4e20 5448 4520 534f 4654 5741 5245 2e0a  N THE SOFTWARE..
+000005b0: 2020 2020 2020 2020 0a50 726f 6a65 6374          .Project
+000005c0: 2d55 524c 3a20 486f 6d65 7061 6765 2c20  -URL: Homepage, 
+000005d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000005e0: 6f6d 2f53 6869 4a62 6579 2f6e 6569 6768  om/ShiJbey/neigh
+000005f0: 626f 726c 790a 5072 6f6a 6563 742d 5552  borly.Project-UR
+00000600: 4c3a 2042 7567 2054 7261 636b 6572 2c20  L: Bug Tracker, 
+00000610: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000620: 6f6d 2f53 6869 4a62 6579 2f6e 6569 6768  om/ShiJbey/neigh
+00000630: 626f 726c 792f 6973 7375 6573 0a50 726f  borly/issues.Pro
+00000640: 6a65 6374 2d55 524c 3a20 5265 706f 7369  ject-URL: Reposi
+00000650: 746f 7279 2c20 6874 7470 733a 2f2f 6769  tory, https://gi
+00000660: 7468 7562 2e63 6f6d 2f53 6869 4a42 6579  thub.com/ShiJBey
+00000670: 2f6e 6569 6768 626f 726c 792e 6769 740a  /neighborly.git.
+00000680: 5072 6f6a 6563 742d 5552 4c3a 2043 6861  Project-URL: Cha
+00000690: 6e67 656c 6f67 2c20 6874 7470 733a 2f2f  ngelog, https://
+000006a0: 6769 7468 7562 2e63 6f6d 2f53 6869 4a62  github.com/ShiJb
+000006b0: 6579 2f6e 6569 6768 626f 726c 792f 626c  ey/neighborly/bl
+000006c0: 6f62 2f6d 6169 6e2f 4348 414e 4745 4c4f  ob/main/CHANGELO
+000006d0: 472e 6d64 0a50 726f 6a65 6374 2d55 524c  G.md.Project-URL
+000006e0: 3a20 446f 6375 6d65 6e74 6174 696f 6e2c  : Documentation,
+000006f0: 2068 7474 7073 3a2f 2f6e 6569 6768 626f   https://neighbo
+00000700: 726c 792e 7265 6164 7468 6564 6f63 732e  rly.readthedocs.
+00000710: 696f 2f65 6e2f 6c61 7465 7374 2f0a 4b65  io/en/latest/.Ke
+00000720: 7977 6f72 6473 3a20 736f 6369 616c 2073  ywords: social s
+00000730: 696d 756c 6174 696f 6e2c 6761 6d65 732c  imulation,games,
+00000740: 7369 6d75 6c61 7469 6f6e 2c61 7274 6966  simulation,artif
+00000750: 6963 6961 6c20 696e 7465 6c6c 6967 656e  icial intelligen
+00000760: 6365 2c61 6765 6e74 2d62 6173 6564 206d  ce,agent-based m
+00000770: 6f64 656c 696e 672c 6d75 6c74 6961 6765  odeling,multiage
+00000780: 6e74 2073 7973 7465 6d73 2c65 6d65 7267  nt systems,emerg
+00000790: 656e 7420 6e61 7272 6174 6976 652c 6e61  ent narrative,na
+000007a0: 7272 6174 6976 6520 6765 6e65 7261 7469  rrative generati
+000007b0: 6f6e 2c69 6e74 6572 6163 7469 7665 2073  on,interactive s
+000007c0: 746f 7279 7465 6c6c 696e 672c 7365 7474  torytelling,sett
+000007d0: 6c65 6d65 6e74 2073 696d 756c 6174 696f  lement simulatio
+000007e0: 6e0a 436c 6173 7369 6669 6572 3a20 496e  n.Classifier: In
+000007f0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000800: 3a3a 2044 6576 656c 6f70 6572 730a 436c  :: Developers.Cl
+00000810: 6173 7369 6669 6572 3a20 496e 7465 6e64  assifier: Intend
+00000820: 6564 2041 7564 6965 6e63 6520 3a3a 2053  ed Audience :: S
+00000830: 6369 656e 6365 2f52 6573 6561 7263 680a  cience/Research.
+00000840: 436c 6173 7369 6669 6572 3a20 4c69 6365  Classifier: Lice
+00000850: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000860: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+00000870: 7365 0a43 6c61 7373 6966 6965 723a 204f  se.Classifier: O
+00000880: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000890: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+000008a0: 740a 436c 6173 7369 6669 6572 3a20 5072  t.Classifier: Pr
+000008b0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000008c0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000008d0: 3320 3a3a 204f 6e6c 790a 436c 6173 7369  3 :: Only.Classi
+000008e0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000008f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000900: 7468 6f6e 203a 3a20 332e 380a 436c 6173  thon :: 3.8.Clas
+00000910: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000920: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000930: 5079 7468 6f6e 203a 3a20 332e 390a 436c  Python :: 3.9.Cl
+00000940: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000950: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000960: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+00000970: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000980: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000990: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000009a0: 2e31 310a 436c 6173 7369 6669 6572 3a20  .11.Classifier: 
+000009b0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000009c0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000009d0: 3a20 332e 3132 0a43 6c61 7373 6966 6965  : 3.12.Classifie
+000009e0: 723a 2054 6f70 6963 203a 3a20 4761 6d65  r: Topic :: Game
+000009f0: 732f 456e 7465 7274 6169 6e6d 656e 7420  s/Entertainment 
+00000a00: 3a3a 2053 696d 756c 6174 696f 6e0a 436c  :: Simulation.Cl
+00000a10: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
+00000a20: 3a3a 2053 6369 656e 7469 6669 632f 456e  :: Scientific/En
+00000a30: 6769 6e65 6572 696e 670a 436c 6173 7369  gineering.Classi
+00000a40: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
+00000a50: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
+00000a60: 6572 696e 6720 3a3a 2041 7274 6966 6963  ering :: Artific
+00000a70: 6961 6c20 496e 7465 6c6c 6967 656e 6365  ial Intelligence
+00000a80: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+00000a90: 6963 203a 3a20 5363 6965 6e74 6966 6963  ic :: Scientific
+00000aa0: 2f45 6e67 696e 6565 7269 6e67 203a 3a20  /Engineering :: 
+00000ab0: 4172 7469 6669 6369 616c 204c 6966 650a  Artificial Life.
+00000ac0: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+00000ad0: 6320 3a3a 2053 6f63 696f 6c6f 6779 0a43  c :: Sociology.C
+00000ae0: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
+00000af0: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
+00000b00: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
+00000b10: 6172 6965 730a 436c 6173 7369 6669 6572  aries.Classifier
+00000b20: 3a20 546f 7069 6320 3a3a 2053 6f66 7477  : Topic :: Softw
+00000b30: 6172 6520 4465 7665 6c6f 706d 656e 7420  are Development 
+00000b40: 3a3a 204c 6962 7261 7269 6573 203a 3a20  :: Libraries :: 
+00000b50: 4170 706c 6963 6174 696f 6e20 4672 616d  Application Fram
+00000b60: 6577 6f72 6b73 0a43 6c61 7373 6966 6965  eworks.Classifie
+00000b70: 723a 2054 7970 696e 6720 3a3a 2054 7970  r: Typing :: Typ
+00000b80: 6564 0a52 6571 7569 7265 732d 5079 7468  ed.Requires-Pyth
+00000b90: 6f6e 3a20 3e3d 332e 380a 4465 7363 7269  on: >=3.8.Descri
+00000ba0: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
+00000bb0: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
+00000bc0: 6e0a 4c69 6365 6e73 652d 4669 6c65 3a20  n.License-File: 
+00000bd0: 4c49 4345 4e53 452e 6d64 0a52 6571 7569  LICENSE.md.Requi
+00000be0: 7265 732d 4469 7374 3a20 6573 7065 723d  res-Dist: esper=
+00000bf0: 3d32 2e2a 0a52 6571 7569 7265 732d 4469  =2.*.Requires-Di
+00000c00: 7374 3a20 6f72 6465 7265 642d 7365 743d  st: ordered-set=
+00000c10: 3d34 2e2a 0a52 6571 7569 7265 732d 4469  =4.*.Requires-Di
+00000c20: 7374 3a20 7461 6275 6c61 7465 3d3d 302e  st: tabulate==0.
+00000c30: 392e 2a0a 5265 7175 6972 6573 2d44 6973  9.*.Requires-Dis
+00000c40: 743a 2050 7959 414d 4c3d 3d36 2e30 2e2a  t: PyYAML==6.0.*
+00000c50: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000c60: 7471 646d 3d3d 342e 2a0a 5265 7175 6972  tqdm==4.*.Requir
+00000c70: 6573 2d44 6973 743a 2070 7964 616e 7469  es-Dist: pydanti
+00000c80: 633d 3d32 2e2a 0a52 6571 7569 7265 732d  c==2.*.Requires-
+00000c90: 4469 7374 3a20 7061 6e64 6173 3d3d 322e  Dist: pandas==2.
+00000ca0: 2a0a 5072 6f76 6964 6573 2d45 7874 7261  *.Provides-Extra
+00000cb0: 3a20 6465 7665 6c6f 706d 656e 740a 5265  : development.Re
+00000cc0: 7175 6972 6573 2d44 6973 743a 2069 736f  quires-Dist: iso
+00000cd0: 7274 3b20 6578 7472 6120 3d3d 2022 6465  rt; extra == "de
+00000ce0: 7665 6c6f 706d 656e 7422 0a52 6571 7569  velopment".Requi
+00000cf0: 7265 732d 4469 7374 3a20 626c 6163 6b3b  res-Dist: black;
+00000d00: 2065 7874 7261 203d 3d20 2264 6576 656c   extra == "devel
+00000d10: 6f70 6d65 6e74 220a 5265 7175 6972 6573  opment".Requires
+00000d20: 2d44 6973 743a 2062 6c61 636b 5b64 5d3b  -Dist: black[d];
+00000d30: 2065 7874 7261 203d 3d20 2264 6576 656c   extra == "devel
+00000d40: 6f70 6d65 6e74 220a 5265 7175 6972 6573  opment".Requires
+00000d50: 2d44 6973 743a 2062 7569 6c64 3b20 6578  -Dist: build; ex
+00000d60: 7472 6120 3d3d 2022 6465 7665 6c6f 706d  tra == "developm
+00000d70: 656e 7422 0a52 6571 7569 7265 732d 4469  ent".Requires-Di
+00000d80: 7374 3a20 7079 7465 7374 3b20 6578 7472  st: pytest; extr
+00000d90: 6120 3d3d 2022 6465 7665 6c6f 706d 656e  a == "developmen
+00000da0: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
+00000db0: 3a20 7079 7465 7374 2d63 6f76 3b20 6578  : pytest-cov; ex
+00000dc0: 7472 6120 3d3d 2022 6465 7665 6c6f 706d  tra == "developm
+00000dd0: 656e 7422 0a52 6571 7569 7265 732d 4469  ent".Requires-Di
+00000de0: 7374 3a20 7370 6869 6e78 3b20 6578 7472  st: sphinx; extr
+00000df0: 6120 3d3d 2022 6465 7665 6c6f 706d 656e  a == "developmen
+00000e00: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
+00000e10: 3a20 7370 6869 6e78 5f72 7464 5f74 6865  : sphinx_rtd_the
+00000e20: 6d65 3b20 6578 7472 6120 3d3d 2022 6465  me; extra == "de
+00000e30: 7665 6c6f 706d 656e 7422 0a0a 3c68 3120  velopment"..<h1 
+00000e40: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00000e50: 2020 3c69 6d67 0a20 2020 2077 6964 7468    <img.    width
+00000e60: 3d22 3135 3022 0a20 2020 2068 6569 6768  ="150".    heigh
+00000e70: 743d 2231 3530 220a 2020 2020 7372 633d  t="150".    src=
+00000e80: 2268 7474 7073 3a2f 2f75 7365 722d 696d  "https://user-im
+00000e90: 6167 6573 2e67 6974 6875 6275 7365 7263  ages.githubuserc
+00000ea0: 6f6e 7465 6e74 2e63 6f6d 2f31 3130 3736  ontent.com/11076
+00000eb0: 3532 352f 3136 3538 3336 3137 312d 3966  525/165836171-9f
+00000ec0: 6664 6561 3665 2d31 3633 332d 3434 3063  fdea6e-1633-440c
+00000ed0: 2d62 6530 362d 6234 3665 3165 3365 3465  -be06-b46e1e3e4e
+00000ee0: 3034 2e70 6e67 220a 2020 3e0a 2020 3c62  04.png".  >.  <b
+00000ef0: 723e 0a20 204e 6569 6768 626f 726c 790a  r>.  Neighborly.
+00000f00: 3c2f 6831 3e0a 0a3c 7020 616c 6967 6e3d  </h1>..<p align=
+00000f10: 2263 656e 7465 7222 3e0a 2020 3c61 2068  "center">.  <a h
+00000f20: 7265 663d 2268 7474 7073 3a2f 2f6e 6569  ref="https://nei
+00000f30: 6768 626f 726c 792e 7265 6164 7468 6564  ghborly.readthed
+00000f40: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00000f50: 2f69 6e64 6578 2e68 746d 6c22 3e44 6f63  /index.html">Doc
+00000f60: 756d 656e 7461 7469 6f6e 3c2f 613e 207c  umentation</a> |
+00000f70: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000f80: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000f90: 6a65 6374 2f6e 6569 6768 626f 726c 7922  ject/neighborly"
+00000fa0: 3e50 7950 493c 2f61 3e20 7c20 3c61 2068  >PyPI</a> | <a h
+00000fb0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000fc0: 6875 622e 636f 6d2f 5368 694a 6265 792f  hub.com/ShiJbey/
+00000fd0: 6e65 6967 6862 6f72 6c79 223e 4769 7448  neighborly">GitH
+00000fe0: 7562 3c2f 613e 0a3c 2f70 3e0a 0a3c 7020  ub</a>.</p>..<p 
+00000ff0: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00001000: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00001010: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00001020: 696f 2f70 7970 692f 762f 6e65 6967 6862  io/pypi/v/neighb
+00001030: 6f72 6c79 2220 616c 743d 2250 7950 4920  orly" alt="PyPI 
+00001040: 7665 7273 696f 6e20 6261 6467 6522 3e0a  version badge">.
+00001050: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00001060: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00001070: 696f 2f70 7970 692f 7079 7665 7273 696f  io/pypi/pyversio
+00001080: 6e73 2f6e 6569 6768 626f 726c 7922 2061  ns/neighborly" a
+00001090: 6c74 3d22 5375 7070 6f72 7465 6420 5079  lt="Supported Py
+000010a0: 7468 6f6e 2056 6572 7369 6f6e 7320 6261  thon Versions ba
+000010b0: 6467 6522 3e0a 2020 3c69 6d67 2073 7263  dge">.  <img src
+000010c0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000010d0: 6965 6c64 732e 696f 2f70 7970 692f 6c2f  ields.io/pypi/l/
+000010e0: 6e65 6967 6862 6f72 6c79 2220 616c 743d  neighborly" alt=
+000010f0: 224d 4954 204c 6963 656e 7365 2062 6164  "MIT License bad
+00001100: 6765 223e 0a20 203c 696d 6720 7372 633d  ge">.  <img src=
+00001110: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00001120: 656c 6473 2e69 6f2f 7079 7069 2f64 6d2f  elds.io/pypi/dm/
+00001130: 6e65 6967 6862 6f72 6c79 2220 616c 743d  neighborly" alt=
+00001140: 2250 7950 4920 646f 776e 6c6f 6164 7320  "PyPI downloads 
+00001150: 6261 6467 6522 3e0a 2020 3c69 6d67 2073  badge">.  <img s
+00001160: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00001170: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00001180: 2f63 6f64 6525 3230 7374 796c 652d 626c  /code%20style-bl
+00001190: 6163 6b2d 626c 6163 6b22 2061 6c74 3d22  ack-black" alt="
+000011a0: 426c 6163 6b20 666f 726d 6174 7465 7220  Black formatter 
+000011b0: 6261 6467 6522 3e0a 2020 3c69 6d67 2073  badge">.  <img s
+000011c0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+000011d0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+000011e0: 2f25 3230 696d 706f 7274 732d 6973 6f72  /%20imports-isor
+000011f0: 742d 2532 3331 3637 3462 313f 7374 796c  t-%231674b1?styl
+00001200: 653d 666c 6174 266c 6162 656c 436f 6c6f  e=flat&labelColo
+00001210: 723d 6566 3833 3336 2220 616c 743d 2249  r=ef8336" alt="I
+00001220: 536f 7274 2062 6164 6765 223e 0a3c 2f70  Sort badge">.</p
+00001230: 3e0a 0a4e 6569 6768 626f 726c 7920 6973  >..Neighborly is
+00001240: 2061 6e20 6167 656e 742d 6261 7365 6420   an agent-based 
+00001250: 7365 7474 6c65 6d65 6e74 2073 696d 756c  settlement simul
+00001260: 6174 696f 6e20 7468 6174 2067 656e 6572  ation that gener
+00001270: 6174 6573 2062 6163 6b73 746f 7279 2064  ates backstory d
+00001280: 6174 6120 666f 7220 6368 6172 6163 7465  ata for characte
+00001290: 7273 206c 6976 696e 6720 696e 2061 2070  rs living in a p
+000012a0: 726f 6365 6475 7261 6c6c 7920 6765 6e65  rocedurally gene
+000012b0: 7261 7465 6420 7365 7474 6c65 6d65 6e74  rated settlement
+000012c0: 2e20 4974 2077 6173 2062 7569 6c74 2074  . It was built t
+000012d0: 6f20 6265 2061 2074 6f6f 6c20 666f 7220  o be a tool for 
+000012e0: 656d 6572 6765 6e74 206e 6172 7261 7469  emergent narrati
+000012f0: 7665 2073 746f 7279 7465 6c6c 696e 6720  ve storytelling 
+00001300: 7265 7365 6172 6368 2e20 4e65 6967 6862  research. Neighb
+00001310: 6f72 6c79 206d 6f64 656c 7320 7468 6520  orly models the 
+00001320: 6368 6172 6163 7465 7273 2720 7472 6169  characters' trai
+00001330: 7473 2c20 7374 6174 7573 6573 2c20 7265  ts, statuses, re
+00001340: 6c61 7469 6f6e 7368 6970 732c 206f 6363  lationships, occ
+00001350: 7570 6174 696f 6e73 2c20 6c69 6665 2065  upations, life e
+00001360: 7665 6e74 732c 2065 7463 2e20 6f76 6572  vents, etc. over
+00001370: 2064 6563 6164 6573 206f 6620 7369 6d75   decades of simu
+00001380: 6c61 7465 6420 7469 6d65 2e20 5468 6520  lated time. The 
+00001390: 656e 7469 7265 2068 6973 746f 7279 206f  entire history o
+000013a0: 6620 7468 6520 7365 7474 6c65 6d65 6e74  f the settlement
+000013b0: 2061 6e64 2069 7473 2067 656e 6572 6174   and its generat
+000013c0: 696f 6e73 206f 6620 6368 6172 6163 7465  ions of characte
+000013d0: 7273 2069 7320 6d61 6465 2061 7661 696c  rs is made avail
+000013e0: 6162 6c65 2066 6f72 2064 6174 6120 616e  able for data an
+000013f0: 616c 7973 6973 2061 6e64 2065 7870 6f72  alysis and expor
+00001400: 7469 6e67 2e20 4e65 6967 6862 6f72 6c79  ting. Neighborly
+00001410: 2061 696d 7320 746f 2062 6520 616e 2065   aims to be an e
+00001420: 6173 696c 7920 6375 7374 6f6d 697a 6162  asily customizab
+00001430: 6c65 2073 696d 756c 6174 696f 6e20 7468  le simulation th
+00001440: 6174 2063 616e 2061 6461 7074 2074 6f20  at can adapt to 
+00001450: 7661 7269 6f75 7320 6e61 7272 6174 6976  various narrativ
+00001460: 6520 7365 7474 696e 6773 2061 6e64 2073  e settings and s
+00001470: 7570 706f 7274 2072 6573 6561 7263 6820  upport research 
+00001480: 6f72 2065 6e74 6572 7461 696e 6d65 6e74  or entertainment
+00001490: 2070 726f 6a65 6374 732e 0a0a 4e65 6967   projects...Neig
+000014a0: 6862 6f72 6c79 2773 2077 6173 2069 6e73  hborly's was ins
+000014b0: 7069 7265 6420 5b5f 5461 6c6b 206f 6620  pired [_Talk of 
+000014c0: 7468 6520 546f 776e 5f5d 2868 7474 7073  the Town_](https
+000014d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a61  ://github.com/ja
+000014e0: 6d65 732d 6f77 656e 2d72 7961 6e2f 7461  mes-owen-ryan/ta
+000014f0: 6c6b 746f 776e 292c 2061 6e6f 7468 6572  lktown), another
+00001500: 2073 6574 746c 656d 656e 7420 7369 6d75   settlement simu
+00001510: 6c61 7469 6f6e 2066 6f72 2065 6d65 7267  lation for emerg
+00001520: 656e 7420 6e61 7272 6174 6976 6520 7374  ent narrative st
+00001530: 6f72 7974 656c 6c69 6e67 2072 6573 6561  orytelling resea
+00001540: 7263 682e 2049 7420 616c 736f 2064 7261  rch. It also dra
+00001550: 7773 2069 6e73 7069 7261 7469 6f6e 2066  ws inspiration f
+00001560: 726f 6d20 636f 6d6d 6572 6369 616c 2077  rom commercial w
+00001570: 6f72 6c64 2d73 696d 756c 6174 696f 6e20  orld-simulation 
+00001580: 6761 6d65 7320 6c69 6b65 205f 4361 7665  games like _Cave
+00001590: 7320 6f66 2051 7564 5f2c 205f 4477 6172  s of Qud_, _Dwar
+000015a0: 6620 466f 7274 7265 7373 5f2c 205f 4372  f Fortress_, _Cr
+000015b0: 7573 6164 6572 204b 696e 6773 5f2c 205f  usader Kings_, _
+000015c0: 5269 6d57 6f72 6c64 5f2c 2061 6e64 205f  RimWorld_, and _
+000015d0: 576f 726c 6442 6f78 5f2e 0a0a 4966 2079  WorldBox_...If y
+000015e0: 6f75 2075 7365 204e 6569 6768 626f 726c  ou use Neighborl
+000015f0: 7920 696e 2061 2070 726f 6a65 6374 2c20  y in a project, 
+00001600: 706c 6561 7365 2063 6974 6520 7468 6973  please cite this
+00001610: 2072 6570 6f73 6974 6f72 792e 2059 6f75   repository. You
+00001620: 2063 616e 2072 6561 640a 4e65 6967 6862   can read.Neighb
+00001630: 6f72 6c79 2773 2061 7373 6f63 6961 7465  orly's associate
+00001640: 6420 5b70 6170 6572 5d28 6874 7470 733a  d [paper](https:
+00001650: 2f2f 7368 696a 6265 792e 6769 7468 7562  //shijbey.github
+00001660: 2e69 6f2f 7075 626c 6963 6174 696f 6e73  .io/publications
+00001670: 2f4e 6569 6768 626f 726c 792e 7064 6629  /Neighborly.pdf)
+00001680: 2074 6861 7420 7761 7320 7075 626c 6973   that was publis
+00001690: 6865 6420 696e 2074 6865 0a70 726f 6365  hed in the.proce
+000016a0: 6564 696e 6773 206f 6620 7468 6520 3230  edings of the 20
+000016b0: 3232 2049 4545 4520 436f 6e66 6572 656e  22 IEEE Conferen
+000016c0: 6365 204f 6e20 4761 6d65 732e 0a0a 6060  ce On Games...``
+000016d0: 6074 6578 740a 4069 6e70 726f 6365 6564  `text.@inproceed
+000016e0: 696e 6773 7b6a 6f68 6e73 6f6e 6265 7932  ings{johnsonbey2
+000016f0: 3032 326e 6569 6768 626f 726c 792c 0a20  022neighborly,. 
+00001700: 2020 2074 6974 6c65 203d 207b 4e65 6967     title = {Neig
+00001710: 6862 6f72 6c79 3a20 4120 5361 6e64 626f  hborly: A Sandbo
+00001720: 7820 666f 7220 5369 6d75 6c61 7469 6f6e  x for Simulation
+00001730: 2d62 6173 6564 2045 6d65 7267 656e 7420  -based Emergent 
+00001740: 4e61 7272 6174 6976 657d 2c0a 2020 2020  Narrative},.    
+00001750: 6175 7468 6f72 203d 207b 4a6f 686e 736f  author = {Johnso
+00001760: 6e2d 4265 792c 2053 6869 2061 6e64 204e  n-Bey, Shi and N
+00001770: 656c 736f 6e2c 204d 6172 6b20 4a20 616e  elson, Mark J an
+00001780: 6420 4d61 7465 6173 2c20 4d69 6368 6165  d Mateas, Michae
+00001790: 6c7d 2c0a 2020 2020 626f 6f6b 7469 746c  l},.    booktitl
+000017a0: 6520 3d20 7b32 3032 3220 4945 4545 2043  e = {2022 IEEE C
+000017b0: 6f6e 6665 7265 6e63 6520 6f6e 2047 616d  onference on Gam
+000017c0: 6573 2028 436f 4729 7d2c 0a20 2020 2070  es (CoG)},.    p
+000017d0: 6167 6573 203d 207b 3432 352d 2d34 3332  ages = {425--432
+000017e0: 7d2c 0a20 2020 2079 6561 7220 3d20 7b32  },.    year = {2
+000017f0: 3032 327d 2c0a 2020 2020 6f72 6761 6e69  022},.    organi
+00001800: 7a61 7469 6f6e 203d 207b 4945 4545 7d0a  zation = {IEEE}.
+00001810: 7d0a 6060 600a 0a3e 205b 2149 4d50 4f52  }.```..> [!IMPOR
+00001820: 5441 4e54 5d0a 3e20 4e65 6967 6862 6f72  TANT].> Neighbor
+00001830: 6c79 2773 2063 7572 7265 6e74 2061 7263  ly's current arc
+00001840: 6869 7465 6374 7572 6520 6469 6666 6572  hitecture differ
+00001850: 7320 6672 6f6d 2077 6861 7420 6973 2064  s from what is d
+00001860: 6573 6372 6962 6564 2069 6e20 7468 6520  escribed in the 
+00001870: 7061 7065 722e 2050 6c65 6173 6520 7365  paper. Please se
+00001880: 6520 7468 6520 5b44 6966 6665 7265 6e63  e the [Differenc
+00001890: 6573 2066 726f 6d20 7468 6520 5061 7065  es from the Pape
+000018a0: 725d 2823 e284 b9ef b88f 2d64 6966 6665  r](#......-diffe
+000018b0: 7265 6e63 6573 2d66 726f 6d2d 7468 652d  rences-from-the-
+000018c0: 7061 7065 7229 2073 6563 7469 6f6e 2062  paper) section b
+000018d0: 656c 6f77 2e0a 0a23 2320 f09f 8eaf 2043  elow...## .... C
+000018e0: 6f72 6520 4665 6174 7572 6573 0a0a 2d20  ore Features..- 
+000018f0: f09f 92be 202a 2a44 6174 612d 6472 6976  .... **Data-driv
+00001900: 656e 2a2a 2e20 4375 7374 6f6d 697a 6520  en**. Customize 
+00001910: 7468 6520 7369 6d75 6c61 7469 6f6e 2066  the simulation f
+00001920: 6f72 2064 6966 6665 7265 6e74 206e 6172  or different nar
+00001930: 7261 7469 7665 2073 6574 7469 6e67 730a  rative settings.
+00001940: 2d20 f09f a496 202a 2a41 6765 6e74 2d62  - .... **Agent-b
+00001950: 6173 6564 2a2a 2e20 5365 7474 6c65 6d65  ased**. Settleme
+00001960: 6e74 2061 6e64 2063 6861 7261 6374 6572  nt and character
+00001970: 2068 6973 746f 7269 6573 2061 7265 2067   histories are g
+00001980: 656e 6572 6174 6564 2062 6f74 746f 6d2d  enerated bottom-
+00001990: 7570 2066 726f 6d20 6368 6172 6163 7465  up from characte
+000019a0: 7220 6265 6861 7669 6f72 2e0a 2d20 f09f  r behavior..- ..
+000019b0: 93a6 202a 2a45 6e74 6974 792d 436f 6d70  .. **Entity-Comp
+000019c0: 6f6e 656e 7420 5379 7374 656d 2a2a 2e20  onent System**. 
+000019d0: 4167 656e 7473 2061 7265 2063 6f6d 706f  Agents are compo
+000019e0: 7365 6420 6f66 206d 6f64 756c 6172 2063  sed of modular c
+000019f0: 6f6d 706f 6e65 6e74 732e 0a2d 20f0 9f91  omponents..- ...
+00001a00: 9420 2a2a 5374 6174 2026 2053 6b69 6c6c  . **Stat & Skill
+00001a10: 2053 7973 7465 6d73 2a2a 2e20 5472 6163   Systems**. Trac
+00001a20: 6b20 6368 6172 6163 7465 7220 7072 6f66  k character prof
+00001a30: 6963 6965 6e63 6965 7320 616e 6420 5250  iciencies and RP
+00001a40: 472d 6c69 6b65 2073 7461 7473 2e0a 2d20  G-like stats..- 
+00001a50: efb8 8ff0 9f8f b7ef b88f 202a 2a54 7261  .......... **Tra
+00001a60: 6974 2053 7973 7465 6d2a 2a2e 2054 6167  it System**. Tag
+00001a70: 2047 616d 654f 626a 6563 7473 2077 6974   GameObjects wit
+00001a80: 6820 7472 6169 7473 2074 6861 7420 6d6f  h traits that mo
+00001a90: 6469 6679 2074 6865 6972 2073 7461 7473  dify their stats
+00001aa0: 2061 6e64 2072 656c 6174 696f 6e73 6869   and relationshi
+00001ab0: 7073 2e0a 2d20 e29d a4ef b88f 202a 2a52  ps..- ...... **R
+00001ac0: 656c 6174 696f 6e73 6869 7020 5379 7374  elationship Syst
+00001ad0: 656d 2a2a 2e20 4368 6172 6163 7465 7273  em**. Characters
+00001ae0: 2063 756c 7469 7661 7465 2072 656c 6174   cultivate relat
+00001af0: 696f 6e73 6869 7073 2062 6173 6564 206f  ionships based o
+00001b00: 6e20 726f 6d61 6e63 6520 616e 6420 7265  n romance and re
+00001b10: 7075 7461 7469 6f6e 2e0a 2d20 f09f 92a5  putation..- ....
+00001b20: 202a 2a41 6374 696f 6e20 2620 4576 656e   **Action & Even
+00001b30: 7420 5379 7374 656d 2a2a 2e20 4167 656e  t System**. Agen
+00001b40: 7473 2074 616b 6520 6163 7469 6f6e 7320  ts take actions 
+00001b50: 7468 6174 2062 7569 6c64 2075 7020 6869  that build up hi
+00001b60: 7374 6f72 6965 7320 6f66 206c 6966 6520  stories of life 
+00001b70: 6576 656e 7473 2e0a 2d20 e29a 96ef b88f  events..- ......
+00001b80: 202a 2a42 656c 6965 6620 5379 7374 656d   **Belief System
+00001b90: 2a2a 2e20 4368 6172 6163 7465 7227 7320  **. Character's 
+00001ba0: 6265 6c69 6566 7320 696e 666c 7565 6e63  beliefs influenc
+00001bb0: 6520 686f 7720 7468 6579 2066 6565 6c20  e how they feel 
+00001bc0: 6162 6f75 7420 6f74 6865 7273 2e0a 2d20  about others..- 
+00001bd0: f09f 8fac 202a 2a4c 6f63 6174 696f 6e20  .... **Location 
+00001be0: 5072 6566 6572 656e 6365 2053 7973 7465  Preference Syste
+00001bf0: 6d2a 2a2e 204d 6f64 656c 2077 6861 7420  m**. Model what 
+00001c00: 6c6f 6361 7469 6f6e 7320 6120 6368 6172  locations a char
+00001c10: 6163 7465 7220 6d69 6768 7420 6672 6571  acter might freq
+00001c20: 7565 6e74 2067 6976 656e 2074 6865 6972  uent given their
+00001c30: 2074 7261 6974 732e 0a2d 20f0 9f93 8820   traits..- .... 
+00001c40: 2a2a 5265 6164 7920 666f 7220 6461 7461  **Ready for data
+00001c50: 2073 6369 656e 6365 2a2a 2e20 4578 7472   science**. Extr
+00001c60: 6163 7420 616e 6420 616e 616c 797a 6520  act and analyze 
+00001c70: 6461 7461 2077 6974 6820 5b50 616e 6461  data with [Panda
+00001c80: 735d 2868 7474 7073 3a2f 2f70 616e 6461  s](https://panda
+00001c90: 732e 7079 6461 7461 2e6f 7267 2f29 2e0a  s.pydata.org/)..
+00001ca0: 0a23 2320 f09f 9a80 2048 6f77 2074 6f20  .## .... How to 
+00001cb0: 496e 7374 616c 6c0a 0a54 6865 206c 6174  Install..The lat
+00001cc0: 6573 7420 6f66 6669 6369 616c 2072 656c  est official rel
+00001cd0: 6561 7365 206f 6620 4e65 6967 6862 6f72  ease of Neighbor
+00001ce0: 6c79 2069 7320 6176 6169 6c61 626c 6520  ly is available 
+00001cf0: 746f 2069 6e73 7461 6c6c 2066 726f 6d20  to install from 
+00001d00: 5b50 7950 495d 2868 7474 7073 3a2f 2f70  [PyPI](https://p
+00001d10: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+00001d20: 6e65 6967 6862 6f72 6c79 2f29 2e0a 0a60  neighborly/)...`
+00001d30: 6060 6261 7368 0a70 6970 2069 6e73 7461  ``bash.pip insta
+00001d40: 6c6c 206e 6569 6768 626f 726c 790a 6060  ll neighborly.``
+00001d50: 600a 0a23 2323 2054 7279 204e 6569 6768  `..### Try Neigh
+00001d60: 626f 726c 7920 5769 7468 6f75 7420 496e  borly Without In
+00001d70: 7374 616c 6c69 6e67 0a0a 4e65 6967 6862  stalling..Neighb
+00001d80: 6f72 6c79 2069 7320 6176 6169 6c61 626c  orly is availabl
+00001d90: 6520 746f 2075 7365 2077 6974 6869 6e20  e to use within 
+00001da0: 7468 6973 205b 7361 6d70 6c65 2047 6f6f  this [sample Goo
+00001db0: 676c 6520 436f 6c61 6220 6e6f 7465 626f  gle Colab notebo
+00001dc0: 6f6b 5d28 6874 7470 733a 2f2f 636f 6c61  ok](https://cola
+00001dd0: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
+00001de0: 652e 636f 6d2f 6472 6976 652f 3157 785a  e.com/drive/1WxZ
+00001df0: 6e43 5238 6166 656b 6642 6c2d 7649 3657  nCR8afekfBl-vI6W
+00001e00: 6349 6353 364f 6852 4764 6b61 6d3f 7573  cIcS6OhRGdkam?us
+00001e10: 703d 7368 6172 696e 6729 2e20 4974 2063  p=sharing). It c
+00001e20: 6f6e 7461 696e 7320 6120 6261 7369 6320  ontains a basic 
+00001e30: 7761 6c6b 7468 726f 7567 6820 6f66 2068  walkthrough of h
+00001e40: 6f77 2074 6f20 6465 6669 6e65 2063 6f6e  ow to define con
+00001e50: 7465 6e74 2066 6f72 2074 6865 2073 696d  tent for the sim
+00001e60: 756c 6174 696f 6e20 616e 6420 696e 7370  ulation and insp
+00001e70: 6563 7420 7468 6520 6765 6e65 7261 7465  ect the generate
+00001e80: 6420 6461 7461 2e0a 0a23 2323 2049 6e73  d data...### Ins
+00001e90: 7461 6c6c 696e 6720 666f 7220 4c6f 6361  talling for Loca
+00001ea0: 6c20 4465 7665 6c6f 706d 656e 740a 0a54  l Development..T
+00001eb0: 6f20 646f 776e 6c6f 6164 2061 204e 6569  o download a Nei
+00001ec0: 6768 626f 726c 7920 666f 7220 6c6f 6361  ghborly for loca
+00001ed0: 6c20 6465 7665 6c6f 706d 656e 7420 6f72  l development or
+00001ee0: 2070 6c61 7920 6172 6f75 6e64 2077 6974   play around wit
+00001ef0: 6820 616e 7920 6f66 2074 6865 2073 616d  h any of the sam
+00001f00: 706c 6573 2c20 796f 7520 6e65 6564 2074  ples, you need t
+00001f10: 6f20 636c 6f6e 6520 6f72 2064 6f77 6e6c  o clone or downl
+00001f20: 6f61 6420 7468 6973 2072 6570 6f73 6974  oad this reposit
+00001f30: 6f72 7920 616e 6420 696e 7374 616c 6c20  ory and install 
+00001f40: 6974 2075 7369 6e67 2074 6865 205f 6564  it using the _ed
+00001f50: 6974 6162 6c65 5f20 666c 6167 2028 2d65  itable_ flag (-e
+00001f60: 292e 2050 6c65 6173 6520 7365 6520 7468  ). Please see th
+00001f70: 6520 696e 7374 7275 6374 696f 6e73 2062  e instructions b
+00001f80: 656c 6f77 2e20 5468 6973 2063 6f6d 6d61  elow. This comma
+00001f90: 6e64 2077 696c 6c20 696e 7374 616c 6c20  nd will install 
+00001fa0: 6120 4e65 6967 6862 6f72 6c79 2069 6e74  a Neighborly int
+00001fb0: 6f20 7468 6520 7669 7274 7561 6c20 656e  o the virtual en
+00001fc0: 7669 726f 6e6d 656e 7420 616c 6f6e 6720  vironment along 
+00001fd0: 7769 7468 2061 6c6c 2069 7473 2064 6570  with all its dep
+00001fe0: 656e 6465 6e63 6965 7320 616e 6420 6120  endencies and a 
+00001ff0: 6665 7720 6164 6469 7469 6f6e 616c 2064  few additional d
+00002000: 6576 656c 6f70 6d65 6e74 2061 6e64 2074  evelopment and t
+00002010: 6573 7469 6e67 2064 6570 656e 6465 6e63  esting dependenc
+00002020: 6965 7320 7375 6368 2061 7320 5f62 6c61  ies such as _bla
+00002030: 636b 5f2c 205f 6973 6f72 745f 2c20 616e  ck_, _isort_, an
+00002040: 6420 5f70 7974 6573 745f 2e0a 0a60 6060  d _pytest_...```
+00002050: 6261 7368 0a23 2053 7465 7020 313a 2043  bash.# Step 1: C
+00002060: 6c6f 6e65 2052 6570 6f73 6974 6f72 7920  lone Repository 
+00002070: 616e 6420 6368 616e 6765 2069 6e74 6f20  and change into 
+00002080: 7072 6f6a 6563 7420 6469 7265 6374 6f72  project director
+00002090: 790a 6769 7420 636c 6f6e 6520 6874 7470  y.git clone http
+000020a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
+000020b0: 6869 4a62 6579 2f6e 6569 6768 626f 726c  hiJbey/neighborl
+000020c0: 792e 6769 740a 6364 206e 6569 6768 626f  y.git.cd neighbo
+000020d0: 726c 790a 0a23 2053 7465 7020 3220 284d  rly..# Step 2 (M
+000020e0: 6163 4f53 2f4c 696e 7578 293a 2043 7265  acOS/Linux): Cre
+000020f0: 6174 6520 616e 6420 6163 7469 7661 7465  ate and activate
+00002100: 2061 2050 7974 686f 6e20 7669 7274 7561   a Python virtua
+00002110: 6c20 656e 7669 726f 6e6d 656e 740a 7079  l environment.py
+00002120: 7468 6f6e 3320 2d6d 2076 656e 7620 7665  thon3 -m venv ve
+00002130: 6e76 0a73 6f75 7263 6520 2e2f 7665 6e76  nv.source ./venv
+00002140: 2f62 696e 2f61 6374 6976 6174 650a 0a23  /bin/activate..#
+00002150: 2053 7465 7020 3220 2857 696e 646f 7773   Step 2 (Windows
+00002160: 293a 2043 7265 6174 6520 616e 6420 6163  ): Create and ac
+00002170: 7469 7661 7465 2061 2050 7974 686f 6e20  tivate a Python 
+00002180: 7669 7274 7561 6c20 656e 7669 726f 6e6d  virtual environm
+00002190: 656e 740a 7079 7468 6f6e 202d 6d20 7665  ent.python -m ve
+000021a0: 6e76 2076 656e 760a 2e5c 7665 6e76 5c53  nv venv..\venv\S
+000021b0: 6372 6970 7473 5c41 6374 6976 6174 650a  cripts\Activate.
+000021c0: 0a23 2053 7465 7020 333a 2049 6e73 7461  .# Step 3: Insta
+000021d0: 6c6c 206e 6569 6768 626f 726c 7920 616e  ll neighborly an
+000021e0: 6420 6465 7065 6e64 656e 6369 6573 0a70  d dependencies.p
+000021f0: 7974 686f 6e20 2d6d 2070 6970 2069 6e73  ython -m pip ins
+00002200: 7461 6c6c 202d 6520 222e 5b64 6576 656c  tall -e ".[devel
+00002210: 6f70 6d65 6e74 5d22 0a60 6060 0a0a 2323  opment]".```..##
+00002220: 20f0 9f8d aa20 5275 6e6e 696e 6720 7468   .... Running th
+00002230: 6520 5361 6d70 6c65 730a 0a45 7861 6d70  e Samples..Examp
+00002240: 6c65 2073 696d 756c 6174 696f 6e73 2063  le simulations c
+00002250: 616e 2062 6520 666f 756e 6420 696e 2074  an be found in t
+00002260: 6865 2060 7361 6d70 6c65 7360 2064 6972  he `samples` dir
+00002270: 6563 746f 7279 2e20 5468 656e 2074 6865  ectory. Then the
+00002280: 2063 6f6d 6d61 6e64 7320 6265 6c6f 7720   commands below 
+00002290: 7769 6c6c 2067 6574 2079 6f75 2073 7461  will get you sta
+000022a0: 7274 6564 2077 6974 6820 7275 6e6e 696e  rted with runnin
+000022b0: 6720 7468 6520 7361 6d70 6c65 2073 696d  g the sample sim
+000022c0: 756c 6174 696f 6e73 2e0a 0a60 6060 6261  ulations...```ba
+000022d0: 7368 0a23 2053 7465 7020 313a 2049 6e73  sh.# Step 1: Ins
+000022e0: 7461 6c6c 206e 6569 6768 626f 726c 7920  tall neighborly 
+000022f0: 6c6f 6361 6c6c 7920 616e 6420 616c 6c20  locally and all 
+00002300: 7468 6520 6465 7065 6e64 656e 6369 6573  the dependencies
+00002310: 206e 6565 6465 6420 746f 2072 756e 2074   needed to run t
+00002320: 6865 2073 616d 706c 6520 636f 6e74 656e  he sample conten
+00002330: 742e 0a70 7974 686f 6e20 2d6d 2070 6970  t..python -m pip
+00002340: 2069 6e73 7461 6c6c 2022 2e22 0a0a 2320   install "."..# 
+00002350: 5374 6570 2032 3a20 5275 6e20 6120 7361  Step 2: Run a sa
+00002360: 6d70 6c65 2073 6372 6970 740a 7079 7468  mple script.pyth
+00002370: 6f6e 202e 2f73 616d 706c 6573 2f4e 414d  on ./samples/NAM
+00002380: 455f 4f46 5f53 414d 504c 455f 4649 4c45  E_OF_SAMPLE_FILE
+00002390: 2e70 790a 6060 600a 0a23 2320 f09f a7aa  .py.```..## ....
+000023a0: 2052 756e 6e69 6e67 2074 6865 2054 6573   Running the Tes
+000023b0: 7473 0a0a 4e65 6967 6862 6f72 6c79 2075  ts..Neighborly u
+000023c0: 7365 7320 5b50 7954 6573 745d 2868 7474  ses [PyTest](htt
+000023d0: 7073 3a2f 2f64 6f63 732e 7079 7465 7374  ps://docs.pytest
+000023e0: 2e6f 7267 2f29 2066 6f72 2075 6e69 7420  .org/) for unit 
+000023f0: 7465 7374 696e 672e 2041 6c6c 2074 6573  testing. All tes
+00002400: 7473 2061 7265 206c 6f63 6174 6564 2069  ts are located i
+00002410: 6e20 7468 6520 6074 6573 7473 2f60 2064  n the `tests/` d
+00002420: 6972 6563 746f 7279 2e0a 0a60 6060 6261  irectory...```ba
+00002430: 7368 0a23 2053 7465 7020 313a 2049 6e73  sh.# Step 1: Ins
+00002440: 7461 6c6c 2061 6464 6974 696f 6e61 6c20  tall additional 
+00002450: 6465 7065 6e64 656e 6369 6573 2066 6f72  dependencies for
+00002460: 2074 6573 7469 6e67 2061 6e64 2064 6576   testing and dev
+00002470: 656c 6f70 6d65 6e74 0a70 7974 686f 6e20  elopment.python 
+00002480: 2d6d 2070 6970 2069 6e73 7461 6c6c 202d  -m pip install -
+00002490: 6520 222e 5b64 6576 656c 6f70 6d65 6e74  e ".[development
+000024a0: 5d22 0a0a 2320 5374 6570 2032 3a20 5275  ]"..# Step 2: Ru
+000024b0: 6e20 5079 7465 7374 0a70 7974 6573 740a  n Pytest.pytest.
+000024c0: 0a23 2053 7465 7020 333a 2028 4f70 7469  .# Step 3: (Opti
+000024d0: 6f6e 616c 2920 4765 6e65 7261 7465 2061  onal) Generate a
+000024e0: 2074 6573 7420 636f 7665 7261 6765 2072   test coverage r
+000024f0: 6570 6f72 740a 7079 7465 7374 202d 2d63  eport.pytest --c
+00002500: 6f76 3d6e 6569 6768 626f 726c 7920 7465  ov=neighborly te
+00002510: 7374 732f 0a60 6060 0a0a 2323 20f0 9f93  sts/.```..## ...
+00002520: 9a20 446f 6375 6d65 6e74 6174 696f 6e0a  . Documentation.
+00002530: 0a4e 6569 6768 626f 726c 7927 7320 646f  .Neighborly's do
+00002540: 6375 6d65 6e74 6174 696f 6e20 6361 6e20  cumentation can 
+00002550: 6265 2066 6f75 6e64 2061 7420 5b52 6561  be found at [Rea
+00002560: 6420 7468 6520 446f 6373 5d28 6874 7470  d the Docs](http
+00002570: 733a 2f2f 6e65 6967 6862 6f72 6c79 2e72  s://neighborly.r
+00002580: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00002590: 2f6c 6174 6573 742f 696e 6465 782e 6874  /latest/index.ht
+000025a0: 6d6c 292e 0a0a 2323 20f0 9fa4 9d20 436f  ml)...## .... Co
+000025b0: 6e74 7269 6275 7469 6e67 0a0a 436f 6e74  ntributing..Cont
+000025c0: 7269 6275 7469 6f6e 7320 6172 6520 7765  ributions are we
+000025d0: 6c63 6f6d 652e 2050 6c65 6173 6520 7265  lcome. Please re
+000025e0: 6665 7220 746f 205b 434f 4e54 5249 4255  fer to [CONTRIBU
+000025f0: 5449 4e47 2e6d 645d 282e 2f43 4f4e 5452  TING.md](./CONTR
+00002600: 4942 5554 494e 472e 6d64 2920 666f 7220  IBUTING.md) for 
+00002610: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+00002620: 2061 626f 7574 2068 6f77 2074 6f20 6765   about how to ge
+00002630: 7420 696e 766f 6c76 6564 2e0a 0a23 2320  t involved...## 
+00002640: f09f 9384 204c 6963 656e 7365 0a0a 5468  .... License..Th
+00002650: 6973 2070 726f 6a65 6374 2069 7320 6c69  is project is li
+00002660: 6365 6e73 6564 2075 6e64 6572 2074 6865  censed under the
+00002670: 205b 4d49 5420 4c69 6365 6e73 655d 282e   [MIT License](.
+00002680: 2f4c 4943 454e 5345 292e 0a0a 2323 20e2  /LICENSE)...## .
+00002690: 84b9 efb8 8f20 4469 6666 6572 656e 6365  ..... Difference
+000026a0: 7320 6672 6f6d 2074 6865 2050 6170 6572  s from the Paper
+000026b0: 0a0a 2d20 2a2a 4469 7265 6374 6564 2072  ..- **Directed r
+000026c0: 656c 6174 696f 6e73 6869 7073 206f 6e6c  elationships onl
+000026d0: 792a 2a20 2d20 204e 6569 6768 626f 726c  y** -  Neighborl
+000026e0: 7920 6f6e 6c79 2073 7570 706f 7274 7320  y only supports 
+000026f0: 6469 7265 6374 6564 2072 656c 6174 696f  directed relatio
+00002700: 6e73 6869 7073 2074 6861 7420 7472 6163  nships that trac
+00002710: 6b20 686f 7720 6f6e 6520 6368 6172 6163  k how one charac
+00002720: 7465 7220 6665 656c 7320 6162 6f75 7420  ter feels about 
+00002730: 616e 6f74 6865 722e 2053 7570 706f 7274  another. Support
+00002740: 2066 6f72 2072 6563 6970 726f 6361 6c20   for reciprocal 
+00002750: 7265 6c61 7469 6f6e 7368 6970 7320 7761  relationships wa
+00002760: 7320 7265 6d6f 7665 6420 6265 6361 7573  s removed becaus
+00002770: 6520 6974 2063 6f6d 706c 6963 6174 6564  e it complicated
+00002780: 2074 6865 2073 696d 756c 6174 696f 6e20   the simulation 
+00002790: 6279 2066 6f72 6369 6e67 2075 7365 7273  by forcing users
+000027a0: 2074 6f20 6368 6563 6b20 6d75 6c74 6970   to check multip
+000027b0: 6c65 206c 6f63 6174 696f 6e73 2066 6f72  le locations for
+000027c0: 2072 656c 6174 696f 6e73 6869 7020 6461   relationship da
+000027d0: 7461 2e0a 2d20 2a2a 4e6f 2061 6374 6976  ta..- **No activ
+000027e0: 6974 792f 7365 7276 6963 6520 7379 7374  ity/service syst
+000027f0: 656d 2a2a 202d 2054 6865 2061 6374 6976  em** - The activ
+00002800: 6974 7920 7379 7374 656d 2077 6173 2069  ity system was i
+00002810: 6e74 726f 6475 6365 6420 746f 2068 656c  ntroduced to hel
+00002820: 7020 6368 6172 6163 7465 7273 2064 6563  p characters dec
+00002830: 6964 6520 7768 6572 6520 746f 2066 7265  ide where to fre
+00002840: 7175 656e 7420 6f75 7473 6964 6520 6f66  quent outside of
+00002850: 2077 6f72 6b2f 686f 6d65 2e20 5468 6973   work/home. This
+00002860: 2073 7973 7465 6d20 7761 7320 7265 706c   system was repl
+00002870: 6163 6564 2077 6974 6820 5f6c 6f63 6174  aced with _locat
+00002880: 696f 6e20 7072 6566 6572 656e 6365 735f  ion preferences_
+00002890: 2c20 7768 6963 6820 6172 6520 6d6f 7265  , which are more
+000028a0: 2066 6c65 7869 626c 652e 2054 6865 2061   flexible. The a
+000028b0: 6374 6976 6974 7920 7379 7374 656d 2063  ctivity system c
+000028c0: 616e 2062 6520 656d 756c 6174 6564 2062  an be emulated b
+000028d0: 7920 6173 736f 6369 6174 696e 6720 6365  y associating ce
+000028e0: 7274 6169 6e20 7472 6169 7473 2077 6974  rtain traits wit
+000028f0: 6820 6c6f 6361 7469 6f6e 732e 0a2d 202a  h locations..- *
+00002900: 2a4e 6f20 372d 6461 7920 7765 656b 6c79  *No 7-day weekly
+00002910: 2072 6f75 7469 6e65 732a 2a20 2d20 526f   routines** - Ro
+00002920: 7574 696e 6573 2077 6572 6520 7465 6469  utines were tedi
+00002930: 6f75 7320 746f 2063 7265 6174 6520 616e  ous to create an
+00002940: 6420 6265 6361 6d65 2069 7272 656c 6576  d became irrelev
+00002950: 616e 7420 7768 656e 204e 6569 6768 626f  ant when Neighbo
+00002960: 726c 7927 7320 7469 6d65 2073 7465 7020  rly's time step 
+00002970: 7363 616c 6520 6368 616e 6765 6420 6672  scale changed fr
+00002980: 6f6d 2069 6e63 7265 6d65 6e74 696e 6720  om incrementing 
+00002990: 7468 6520 6461 7465 2062 7920 6120 6665  the date by a fe
+000029a0: 7720 686f 7572 7320 746f 2069 6e63 7265  w hours to incre
+000029b0: 6d65 6e74 696e 6720 6279 2061 2073 696e  menting by a sin
+000029c0: 676c 6520 6d6f 6e74 682e 0a2d 202a 2a4e  gle month..- **N
+000029d0: 6f20 6469 7265 6374 2073 7570 706f 7274  o direct support
+000029e0: 2066 6f72 2064 6966 6665 7269 6e67 2041   for differing A
+000029f0: 4920 7374 7261 7465 6769 6573 2a2a 202d  I strategies** -
+00002a00: 2057 6520 696e 7465 6e64 6564 2074 6f20   We intended to 
+00002a10: 7375 7070 6f72 7420 7661 7269 6f75 7320  support various 
+00002a20: 6368 6172 6163 7465 7220 6465 6369 7369  character decisi
+00002a30: 6f6e 2d6d 616b 696e 6720 616c 676f 7269  on-making algori
+00002a40: 7468 6d73 2062 7574 206d 6164 6520 6265  thms but made be
+00002a50: 6861 7669 6f72 2061 7574 686f 7269 6e67  havior authoring
+00002a60: 2074 6f6f 2074 6564 696f 7573 2061 6e64   too tedious and
+00002a70: 2074 6f6f 6b20 656d 7068 6173 6973 2061   took emphasis a
+00002a80: 7761 7920 6672 6f6d 2074 6865 2063 6f6e  way from the con
+00002a90: 7465 6e74 2061 7574 686f 7269 6e67 2061  tent authoring a
+00002aa0: 6e64 2064 6174 6120 6765 6e65 7261 7469  nd data generati
+00002ab0: 6f6e 2061 7370 6563 7473 206f 6620 4e65  on aspects of Ne
+00002ac0: 6967 6862 6f72 6c79 2e0a 2d20 2a2a 4576  ighborly..- **Ev
+00002ad0: 656e 7420 7379 7374 656d 2072 6570 6c61  ent system repla
+00002ae0: 6365 6420 7769 7468 2061 6374 696f 6e20  ced with action 
+00002af0: 6f62 6a65 6374 7320 616e 6420 7574 696c  objects and util
+00002b00: 6974 7920 7363 6f72 6573 2a2a 202d 2053  ity scores** - S
+00002b10: 696e 6365 204e 6569 6768 626f 726c 7920  ince Neighborly 
+00002b20: 646f 6573 206e 6f74 206e 6565 6420 746f  does not need to
+00002b30: 2073 7570 706f 7274 2075 7365 722d 7375   support user-su
+00002b40: 7070 6c69 6564 2063 6861 7261 6374 6572  pplied character
+00002b50: 2064 6563 6973 696f 6e2d 6d61 6b69 6e67   decision-making
+00002b60: 206c 6f67 6963 2c20 6974 206d 6164 6520   logic, it made 
+00002b70: 6265 6861 7669 6f72 206d 6f64 656c 696e  behavior modelin
+00002b80: 6720 6d75 6368 2073 696d 706c 6572 2e20  g much simpler. 
+00002b90: 5468 6520 6f6c 6420 6c69 6665 2065 7665  The old life eve
+00002ba0: 6e74 2073 7973 7465 6d20 7265 7175 6972  nt system requir
+00002bb0: 6564 2075 7365 7273 2074 6f20 7370 6563  ed users to spec
+00002bc0: 6966 7920 6576 656e 7420 6566 6665 6374  ify event effect
+00002bd0: 7320 666f 7220 6561 6368 2064 6966 6665  s for each diffe
+00002be0: 7265 6e74 2074 7970 6520 6f66 2061 6765  rent type of age
+00002bf0: 6e74 2c20 616e 6420 7468 6973 206e 6174  nt, and this nat
+00002c00: 7572 616c 6c79 2063 6f6d 706c 6963 6174  urally complicat
+00002c10: 6564 2074 6869 6e67 732e 2043 7572 7265  ed things. Curre
+00002c20: 6e74 6c79 2c20 6167 656e 7420 6265 6861  ntly, agent beha
+00002c30: 7669 6f72 2069 7320 696d 706c 656d 656e  vior is implemen
+00002c40: 7465 6420 7573 696e 6720 6120 636f 6d62  ted using a comb
+00002c50: 696e 6174 696f 6e20 6f66 2053 7973 7465  ination of Syste
+00002c60: 6d73 2c20 6163 7469 6f6e 732c 2061 6e64  ms, actions, and
+00002c70: 206c 6966 6520 6576 656e 7473 2e0a 2d20   life events..- 
+00002c80: 2a2a 4e6f 2062 6568 6176 696f 7220 7472  **No behavior tr
+00002c90: 6565 732a 2a20 2d20 4265 6861 7669 6f72  ees** - Behavior
+00002ca0: 2074 7265 6573 2061 6464 6564 2063 6f6d   trees added com
+00002cb0: 706c 6578 6974 7920 746f 2074 6865 2073  plexity to the s
+00002cc0: 7973 7465 6d2e 2049 7420 7761 7320 7265  ystem. It was re
+00002cd0: 6d6f 7665 6420 746f 2073 696d 706c 6966  moved to simplif
+00002ce0: 7920 7468 696e 6773 2e0a 2d20 2a2a 4e6f  y things..- **No
+00002cf0: 2063 6861 7261 6374 6572 2076 616c 7565   character value
+00002d00: 732a 2a20 2d20 4f76 6572 2074 696d 652c  s** - Over time,
+00002d10: 2074 6865 2063 6861 7261 6374 6572 2076   the character v
+00002d20: 616c 7565 2073 7973 7465 6d20 616e 6420  alue system and 
+00002d30: 7065 7273 6f6e 616c 6974 7920 6d6f 6465  personality mode
+00002d40: 6c73 2077 6572 6520 636f 6d62 696e 6564  ls were combined
+00002d50: 2069 6e74 6f20 6120 7369 6e67 6c65 2073   into a single s
+00002d60: 7461 7420 7379 7374 656d 2e20 5265 6d6f  tat system. Remo
+00002d70: 7669 6e67 2074 6865 6d20 7369 6d70 6c69  ving them simpli
+00002d80: 6669 6564 206d 7563 6820 6f66 2074 6865  fied much of the
+00002d90: 2061 6765 6e74 206d 6f64 656c 696e 6720   agent modeling 
+00002da0: 616e 6420 616c 6c6f 7765 6420 666f 7220  and allowed for 
+00002db0: 7468 6520 6d6f 7374 2066 6c65 7869 6269  the most flexibi
+00002dc0: 6c69 7479 2e0a 2d20 2a2a 4e6f 2063 6861  lity..- **No cha
+00002dd0: 7261 6374 6572 206d 6f76 656d 656e 742a  racter movement*
+00002de0: 2a20 2d20 4368 6172 6163 7465 7273 2064  * - Characters d
+00002df0: 6f20 6e6f 7420 6d6f 7665 2062 6574 7765  o not move betwe
+00002e00: 656e 206c 6f63 6174 696f 6e73 2e20 5468  en locations. Th
+00002e10: 6973 2061 6464 6564 2061 6464 6974 696f  is added additio
+00002e20: 6e61 6c20 7072 6f63 6573 7369 6e67 206f  nal processing o
+00002e30: 7665 7268 6561 6420 616e 6420 6265 6361  verhead and beca
+00002e40: 6d65 2075 6e6e 6563 6573 7361 7279 2077  me unnecessary w
+00002e50: 6865 6e20 6d6f 7669 6e67 2074 6f20 6120  hen moving to a 
+00002e60: 6f6e 652d 6d6f 6e74 6820 7469 6d65 2073  one-month time s
+00002e70: 7465 7073 2e0a 0a23 2320 c2a9 efb8 8f20  teps...## ..... 
+00002e80: 444d 4341 2053 7461 7465 6d65 6e74 0a0a  DMCA Statement..
+00002e90: 5570 6f6e 2072 6563 6569 7074 206f 6620  Upon receipt of 
+00002ea0: 6120 6e6f 7469 6365 2061 6c6c 6567 696e  a notice allegin
+00002eb0: 6720 636f 7079 7269 6768 7420 696e 6672  g copyright infr
+00002ec0: 696e 6765 6d65 6e74 2c20 4920 7769 6c6c  ingement, I will
+00002ed0: 2074 616b 6520 7768 6174 6576 6572 2061   take whatever a
+00002ee0: 6374 696f 6e20 6974 2064 6565 6d73 2061  ction it deems a
+00002ef0: 7070 726f 7072 6961 7465 2077 6974 6869  ppropriate withi
+00002f00: 6e20 6974 7320 736f 6c65 2064 6973 6372  n its sole discr
+00002f10: 6574 696f 6e2c 2069 6e63 6c75 6469 6e67  etion, including
+00002f20: 2072 656d 6f76 616c 206f 6620 7468 6520   removal of the 
+00002f30: 616c 6c65 6765 646c 7920 696e 6672 696e  allegedly infrin
+00002f40: 6769 6e67 206d 6174 6572 6961 6c73 2e0a  ging materials..
+00002f50: 0a54 6865 2072 6570 6f20 696d 6167 6520  .The repo image 
+00002f60: 6973 2073 6f6d 6574 6869 6e67 2066 756e  is something fun
+00002f70: 2074 6861 7420 4920 6d61 6465 2e20 4920   that I made. I 
+00002f80: 6c6f 7665 205f 5468 6520 5369 6d70 736f  love _The Simpso
+00002f90: 6e73 5f2c 2061 6e64 2049 2063 6f75 6c64  ns_, and I could
+00002fa0: 6e27 7420 7468 696e 6b20 6f66 2061 6e79  n't think of any
+00002fb0: 6f6e 6520 6d6f 7265 206e 6569 6768 626f  one more neighbo
+00002fc0: 726c 7920 7468 616e 204e 6564 2046 6c61  rly than Ned Fla
+00002fd0: 6e64 6572 732e 2049 6620 7468 6520 636f  nders. If the co
+00002fe0: 7079 7269 6768 7420 6f77 6e65 7220 666f  pyright owner fo
+00002ff0: 7220 5f54 6865 2053 696d 7073 6f6e 735f  r _The Simpsons_
+00003000: 2077 6f75 6c64 206c 696b 6520 6d65 2074   would like me t
+00003010: 6f20 7461 6b65 2069 7420 646f 776e 2c20  o take it down, 
+00003020: 706c 6561 7365 2063 6f6e 7461 6374 206d  please contact m
+00003030: 652e 2054 6865 2073 616d 6520 7461 6b65  e. The same take
+00003040: 646f 776e 2070 6f6c 6963 7920 6170 706c  down policy appl
+00003050: 6965 7320 746f 2063 6f64 6520 7361 6d70  ies to code samp
+00003060: 6c65 7320 696e 7370 6972 6564 2062 7920  les inspired by 
+00003070: 5456 2073 686f 7773 2c20 6d6f 7669 6573  TV shows, movies
+00003080: 2c20 616e 6420 6761 6d65 732e 0a         , and games..
```

### Comparing `neighborly-2.5.0/tests/test_character.py` & `neighborly-3.0.0.dev1/tests/test_character.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,36 @@
+"""Test character-related functionality.
+
+"""
+
 import pathlib
 
 from neighborly.helpers.character import create_character
-from neighborly.loaders import load_characters, load_skills
-from neighborly.plugins import default_traits
+from neighborly.loaders import load_characters, load_skills, load_species
+from neighborly.plugins import default_character_names, default_traits
 from neighborly.simulation import Simulation
 from neighborly.systems import InitializeSettlementSystem
 
-_TEST_DATA_DIR = pathlib.Path(__file__).parent / "data"
+_DATA_DIR = (
+    pathlib.Path(__file__).parent.parent / "src" / "neighborly" / "plugins" / "data"
+)
 
 
 def test_create_character() -> None:
+    """Test character creation."""
+
     sim = Simulation()
 
-    load_characters(sim, _TEST_DATA_DIR / "characters.json")
-    load_skills(sim, _TEST_DATA_DIR / "skills.json")
+    load_characters(sim, _DATA_DIR / "characters.json")
+    load_skills(sim, _DATA_DIR / "skills.json")
+    load_species(sim, _DATA_DIR / "species.json")
 
     default_traits.load_plugin(sim)
+    default_character_names.load_plugin(sim)
 
     sim.world.system_manager.get_system(InitializeSettlementSystem).set_active(False)
 
     sim.initialize()
 
-    character = create_character(sim.world, "farmer")
+    character = create_character(sim.world, "farmer.female")
 
     assert character is not None
```

### Comparing `neighborly-2.5.0/tests/test_datetime.py` & `neighborly-3.0.0.dev1/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `neighborly-2.5.0/tests/test_loaders.py` & `neighborly-3.0.0.dev1/tests/test_loaders.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,121 +5,97 @@
 import pathlib
 
 from neighborly.libraries import (
     BusinessLibrary,
     CharacterLibrary,
     DistrictLibrary,
     JobRoleLibrary,
-    ResidenceLibrary,
     SettlementLibrary,
     SkillLibrary,
     TraitLibrary,
 )
 from neighborly.loaders import (
     load_businesses,
     load_characters,
     load_districts,
     load_job_roles,
-    load_residences,
     load_settlements,
     load_skills,
-    load_tracery,
     load_traits,
 )
 from neighborly.simulation import Simulation
-from neighborly.tracery import Tracery
 
-_TEST_DATA_DIR = pathlib.Path(__file__).parent / "data"
-
-
-def test_load_residences() -> None:
-    sim = Simulation()
-    load_residences(sim, _TEST_DATA_DIR / "residences.json")
-    library = sim.world.resource_manager.get_resource(ResidenceLibrary)
-
-    residence_def = library.get_definition("house")
-
-    assert residence_def.definition_id == "house"
+_DATA_DIR = (
+    pathlib.Path(__file__).parent.parent / "src" / "neighborly" / "plugins" / "data"
+)
 
 
 def test_load_settlements() -> None:
     sim = Simulation()
-    load_settlements(sim, _TEST_DATA_DIR / "settlements.json")
+    load_settlements(sim, _DATA_DIR / "settlements.json")
     library = sim.world.resource_manager.get_resource(SettlementLibrary)
 
     settlement_def = library.get_definition("basic_settlement")
 
     assert settlement_def.definition_id == "basic_settlement"
 
 
 def test_load_business() -> None:
     sim = Simulation()
-    load_businesses(sim, _TEST_DATA_DIR / "businesses.json")
+    load_businesses(sim, _DATA_DIR / "businesses.json")
     library = sim.world.resource_manager.get_resource(BusinessLibrary)
 
     business_def = library.get_definition("cafe")
 
     assert business_def.definition_id == "cafe"
 
 
 def test_load_characters() -> None:
     sim = Simulation()
-    load_characters(sim, _TEST_DATA_DIR / "characters.json")
+    load_characters(sim, _DATA_DIR / "characters.json")
     library = sim.world.resource_manager.get_resource(CharacterLibrary)
 
-    character_def = library.get_definition("person")
+    character_def = library.get_definition("base_character")
 
-    assert character_def.definition_id == "person"
+    assert character_def.definition_id == "base_character"
 
 
 def test_load_districts() -> None:
     sim = Simulation()
-    load_districts(sim, _TEST_DATA_DIR / "districts.json")
+    load_districts(sim, _DATA_DIR / "districts.json")
     library = sim.world.resource_manager.get_resource(DistrictLibrary)
 
     district_def = library.get_definition("market_district")
 
     assert district_def.definition_id == "market_district"
 
 
 def test_load_traits() -> None:
     sim = Simulation()
-    load_traits(sim, _TEST_DATA_DIR / "traits.json")
+    load_traits(sim, _DATA_DIR / "traits.json")
     library = sim.world.resource_manager.get_resource(TraitLibrary)
 
     trait_def = library.get_definition("flirtatious")
 
     assert trait_def.definition_id == "flirtatious"
 
 
 def test_load_job_roles() -> None:
     sim = Simulation()
-    load_job_roles(sim, _TEST_DATA_DIR / "job_roles.json")
+    load_job_roles(sim, _DATA_DIR / "job_roles.json")
     library = sim.world.resource_manager.get_resource(JobRoleLibrary)
 
     trait_def = library.get_definition("blacksmith")
 
     assert trait_def.definition_id == "blacksmith"
 
 
-def test_load_names() -> None:
-    sim = Simulation()
-
-    load_tracery(sim, _TEST_DATA_DIR / "sample.tracery.json")
-
-    tracery = sim.world.resource_manager.get_resource(Tracery)
-
-    generated_name = tracery.generate("#simpsons_name#")
-
-    assert generated_name in {"Homer", "Marge", "Maggie", "Lisa", "Bart"}
-
-
 def test_load_skills() -> None:
     """Test loading skill definitions from a data file."""
 
     sim = Simulation()
-    load_skills(sim, _TEST_DATA_DIR / "skills.json")
+    load_skills(sim, _DATA_DIR / "skills.json")
     library = sim.world.resource_manager.get_resource(SkillLibrary)
 
     definition = library.get_definition("blacksmithing")
 
     assert definition.definition_id == "blacksmithing"
```

### Comparing `neighborly-2.5.0/tests/test_location_preferences.py` & `neighborly-3.0.0.dev1/tests/test_location_preferences.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,68 @@
+# pylint: disable=#C0104
 """Test Location Preference Functionality.
 
 """
 
 import pathlib
 
 import pytest
 
-from neighborly.components.location import LocationPreferences
 from neighborly.helpers.business import create_business
 from neighborly.helpers.character import create_character
-from neighborly.helpers.settlement import create_district, create_settlement
+from neighborly.helpers.location import score_location
 from neighborly.helpers.traits import add_trait, remove_trait
 from neighborly.loaders import (
     load_businesses,
     load_characters,
     load_districts,
     load_job_roles,
-    load_residences,
     load_settlements,
     load_skills,
+    load_species,
+)
+from neighborly.plugins import (
+    default_character_names,
+    default_settlement_names,
+    default_traits,
 )
-from neighborly.plugins import default_traits
 from neighborly.simulation import Simulation
 
-_TEST_DATA_DIR = pathlib.Path(__file__).parent / "data"
+_DATA_DIR = (
+    pathlib.Path(__file__).parent.parent / "src" / "neighborly" / "plugins" / "data"
+)
 
 
 def test_trait_with_location_preferences() -> None:
     """Test traits that apply social rules"""
     sim = Simulation()
 
-    load_districts(sim, _TEST_DATA_DIR / "districts.json")
-    load_settlements(sim, _TEST_DATA_DIR / "settlements.json")
-    load_businesses(sim, _TEST_DATA_DIR / "businesses.json")
-    load_characters(sim, _TEST_DATA_DIR / "characters.json")
-    load_residences(sim, _TEST_DATA_DIR / "residences.json")
-    load_job_roles(sim, _TEST_DATA_DIR / "job_roles.json")
-    load_skills(sim, _TEST_DATA_DIR / "skills.json")
+    load_districts(sim, _DATA_DIR / "districts.json")
+    load_settlements(sim, _DATA_DIR / "settlements.json")
+    load_businesses(sim, _DATA_DIR / "businesses.json")
+    load_characters(sim, _DATA_DIR / "characters.json")
+    load_job_roles(sim, _DATA_DIR / "job_roles.json")
+    load_skills(sim, _DATA_DIR / "skills.json")
+    load_species(sim, _DATA_DIR / "species.json")
 
     default_traits.load_plugin(sim)
+    default_settlement_names.load_plugin(sim)
+    default_character_names.load_plugin(sim)
 
     sim.initialize()
 
-    settlement = create_settlement(sim.world, "basic_settlement")
-
-    district = create_district(sim.world, settlement, "entertainment_district")
-
-    cafe = create_business(sim.world, district, "cafe")
-    bar = create_business(sim.world, district, "bar")
-
-    farmer = create_character(sim.world, "farmer")
+    cafe = create_business(sim.world, "cafe")
+    bar = create_business(sim.world, "bar")
 
-    farmer_preferences = farmer.get_component(LocationPreferences)
+    farmer = create_character(sim.world, "farmer.female")
 
-    assert farmer_preferences.score_location(cafe) == 0.5
-    assert farmer_preferences.score_location(bar) == 0.5
+    assert score_location(farmer, cafe) == 0.5
+    assert score_location(farmer, bar) == 0.5
 
     add_trait(farmer, "drinks_too_much")
 
-    assert farmer_preferences.score_location(cafe) == 0.5
-    assert farmer_preferences.score_location(bar) == pytest.approx(0.65, 0.001)  # type: ignore
+    assert score_location(farmer, cafe) == 0.5
+    assert score_location(farmer, bar) == pytest.approx(0.65, 0.001)  # type: ignore
 
     remove_trait(farmer, "drinks_too_much")
 
-    assert farmer_preferences.score_location(bar) == 0.5
+    assert score_location(farmer, bar) == 0.5
```

### Comparing `neighborly-2.5.0/tests/test_relationship.py` & `neighborly-3.0.0.dev1/tests/test_relationship.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=redefined-outer-name
+# pylint: disable=redefined-outer-name, disable=W0621
 """Test Relationship Components, Systems, and Helper Functions.
 
 """
 
 import pathlib
 
 import pytest
@@ -11,53 +11,68 @@
 from neighborly.helpers.relationship import (
     add_relationship,
     get_relationship,
     has_relationship,
 )
 from neighborly.helpers.stats import get_stat
 from neighborly.helpers.traits import add_trait, remove_trait
+from neighborly.libraries import CharacterLibrary
 from neighborly.loaders import (
     load_businesses,
     load_characters,
     load_districts,
     load_job_roles,
-    load_residences,
     load_settlements,
     load_skills,
+    load_species,
+)
+from neighborly.plugins import (
+    default_character_names,
+    default_settlement_names,
+    default_traits,
 )
-from neighborly.plugins import default_traits
 from neighborly.simulation import Simulation
 
-_TEST_DATA_DIR = pathlib.Path(__file__).parent / "data"
+_DATA_DIR = (
+    pathlib.Path(__file__).parent.parent / "src" / "neighborly" / "plugins" / "data"
+)
 
 
 @pytest.fixture
 def sim() -> Simulation:
     """Create sample simulation to use for test cases"""
     simulation = Simulation()
 
-    load_districts(simulation, _TEST_DATA_DIR / "districts.json")
-    load_settlements(simulation, _TEST_DATA_DIR / "settlements.json")
-    load_businesses(simulation, _TEST_DATA_DIR / "businesses.json")
-    load_characters(simulation, _TEST_DATA_DIR / "characters.json")
-    load_residences(simulation, _TEST_DATA_DIR / "residences.json")
-    load_job_roles(simulation, _TEST_DATA_DIR / "job_roles.json")
-    load_skills(simulation, _TEST_DATA_DIR / "skills.json")
+    load_districts(simulation, _DATA_DIR / "districts.json")
+    load_settlements(simulation, _DATA_DIR / "settlements.json")
+    load_businesses(simulation, _DATA_DIR / "businesses.json")
+    load_characters(simulation, _DATA_DIR / "characters.json")
+    load_job_roles(simulation, _DATA_DIR / "job_roles.json")
+    load_skills(simulation, _DATA_DIR / "skills.json")
+    load_species(simulation, _DATA_DIR / "species.json")
+
     default_traits.load_plugin(simulation)
+    default_character_names.load_plugin(simulation)
+    default_settlement_names.load_plugin(simulation)
+
+    # IMPORTANT: Stop character from generating with traits
+    simulation.world.resources.get_resource(CharacterLibrary).get_definition(
+        "base_character"
+    ).traits.clear()
 
     simulation.initialize()
 
     return simulation
 
 
 def test_get_relationship(sim: Simulation) -> None:
     """Test that get_relationship creates new relationship if one does not exist."""
 
-    a = create_character(sim.world, "person")
-    b = create_character(sim.world, "person")
+    a = create_character(sim.world, "base_character.female")
+    b = create_character(sim.world, "base_character.male")
 
     assert has_relationship(a, b) is False
     assert has_relationship(b, a) is False
 
     a_to_b = get_relationship(a, b)
 
     assert has_relationship(a, b) is True
@@ -74,42 +89,42 @@
 
     assert id(a_to_b) == id(a_to_b_again)
 
 
 def test_add_relationship(sim: Simulation) -> None:
     """Test that adding a relationship create a new relationship or returns the old"""
 
-    a = create_character(sim.world, "person")
-    b = create_character(sim.world, "person")
+    a = create_character(sim.world, "base_character.male")
+    b = create_character(sim.world, "base_character.female")
 
     assert has_relationship(a, b) is False
     assert has_relationship(b, a) is False
 
     add_relationship(a, b)
 
     assert has_relationship(a, b) is True
     assert has_relationship(b, a) is False
 
 
 def test_trait_with_social_rules(sim: Simulation) -> None:
     """Test traits that apply social rules"""
 
-    farmer = create_character(sim.world, "farmer")
-    merchant = create_character(sim.world, "merchant")
-    noble = create_character(sim.world, "nobility")
+    farmer = create_character(sim.world, "farmer.female")
+    merchant = create_character(sim.world, "merchant.male")
+    noble = create_character(sim.world, "nobility.female")
 
     rel_to_noble = add_relationship(farmer, noble)
 
     assert get_stat(rel_to_noble, "reputation").value == 0
 
     add_trait(farmer, "gullible")
 
-    assert get_stat(rel_to_noble, "reputation").value == 5
+    assert get_stat(rel_to_noble, "reputation").value == 10
 
     rel = add_relationship(farmer, merchant)
 
-    assert get_stat(rel, "reputation").value == 5
+    assert get_stat(rel, "reputation").value == 10
 
     remove_trait(farmer, "gullible")
 
     assert get_stat(rel, "reputation").value == 0
     assert get_stat(rel_to_noble, "reputation").value == 0
```

### Comparing `neighborly-2.5.0/tests/test_stats.py` & `neighborly-3.0.0.dev1/tests/test_traits.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,108 @@
-"""Stat System Unit Tests.
+# pylint: disable=W0621
+"""Test for Neighborly's Trait System.
 
 """
 
-from __future__ import annotations
-
 import pathlib
 
-from neighborly.components.stats import Stat
+import pytest
+
 from neighborly.helpers.character import create_character
-from neighborly.helpers.stats import add_stat, get_stat, has_stat, remove_stat
-from neighborly.loaders import load_characters, load_skills
-from neighborly.plugins import default_traits
+from neighborly.helpers.stats import get_stat
+from neighborly.helpers.traits import add_trait, has_trait, remove_trait
+from neighborly.libraries import CharacterLibrary
+from neighborly.loaders import load_characters, load_skills, load_species, load_traits
+from neighborly.plugins import default_character_names, default_traits
 from neighborly.simulation import Simulation
 
-_TEST_DATA_DIR = pathlib.Path(__file__).parent / "data"
+_DATA_DIR = (
+    pathlib.Path(__file__).parent.parent / "src" / "neighborly" / "plugins" / "data"
+)
 
 
-def test_has_stat() -> None:
-    """Test checking for stats."""
-    sim = Simulation()
+@pytest.fixture
+def test_sim() -> Simulation:
+    """Create a simulation instance for tests."""
 
-    load_characters(sim, _TEST_DATA_DIR / "characters.json")
-    load_skills(sim, _TEST_DATA_DIR / "skills.json")
+    sim = Simulation()
 
     default_traits.load_plugin(sim)
+    default_character_names.load_plugin(sim)
+
+    load_characters(sim, _DATA_DIR / "characters.json")
+    load_skills(sim, _DATA_DIR / "skills.json")
+    load_species(sim, _DATA_DIR / "species.json")
+    load_traits(sim, _DATA_DIR / "traits.json")
+
+    # IMPORTANT: Stop character from generating with traits
+    sim.world.resources.get_resource(CharacterLibrary).get_definition(
+        "base_character"
+    ).traits.clear()
 
     sim.initialize()
 
-    character = create_character(sim.world, "farmer")
+    return sim
 
-    assert has_stat(character, "hunger") is False
 
-    assert has_stat(character, "health") is True
+def test_add_trait(test_sim: Simulation) -> None:
+    """Test that adding a trait makes it visible with has_trait."""
 
+    character = create_character(test_sim.world, "farmer.female")
 
-def test_get_stat() -> None:
-    """Test stat retrieval."""
-    sim = Simulation()
+    assert has_trait(character, "flirtatious") is False
 
-    load_characters(sim, _TEST_DATA_DIR / "characters.json")
-    load_skills(sim, _TEST_DATA_DIR / "skills.json")
+    success = add_trait(character, "flirtatious")
 
-    default_traits.load_plugin(sim)
+    assert success is True
 
-    sim.initialize()
 
-    character = create_character(sim.world, "farmer")
+def test_remove_trait(test_sim: Simulation) -> None:
+    """Test that removing a trait makes it not available to has_trait."""
 
-    health = get_stat(character, "health")
-    health.base_value = 10
+    character = create_character(test_sim.world, "farmer.female")
 
-    assert health.base_value == 10
+    assert has_trait(character, "flirtatious") is False
 
-    health.base_value += 100
+    add_trait(character, "flirtatious")
 
-    assert health.base_value == 110
-    assert health.value == 110
+    assert has_trait(character, "flirtatious") is True
 
+    success = remove_trait(character, "flirtatious")
 
-def test_add_stat() -> None:
-    """Test stat addition."""
+    assert success is True
 
-    sim = Simulation()
 
-    load_characters(sim, _TEST_DATA_DIR / "characters.json")
-    load_skills(sim, _TEST_DATA_DIR / "skills.json")
+def test_add_remove_trait_effects(test_sim: Simulation) -> None:
+    """Test that trait effects are added and removed with the trait."""
 
-    default_traits.load_plugin(sim)
+    farmer = create_character(test_sim.world, "farmer.female")
 
-    sim.initialize()
+    get_stat(farmer, "sociability").base_value = 0
 
-    character = create_character(sim.world, "farmer")
+    success = add_trait(farmer, "gullible")
 
-    hunger = add_stat(character, "hunger", Stat(base_value=100, bounds=(0, 255)))
+    assert success is True
+    assert get_stat(farmer, "sociability").value == 3
 
-    assert hunger.base_value == 100
+    success = remove_trait(farmer, "gullible")
 
+    assert success is True
+    assert get_stat(farmer, "sociability").value == 0
 
-def test_remove_stat() -> None:
-    """Test removing stats."""
 
-    sim = Simulation()
+def test_try_add_conflicting_trait(test_sim: Simulation) -> None:
+    """Test that adding a conflicting trait to a character fails"""
 
-    load_characters(sim, _TEST_DATA_DIR / "characters.json")
-    load_skills(sim, _TEST_DATA_DIR / "skills.json")
+    character = create_character(test_sim.world, "farmer.female")
 
-    default_traits.load_plugin(sim)
-
-    sim.initialize()
+    success = add_trait(character, "skeptical")
 
-    character = create_character(sim.world, "farmer")
+    assert success is True
 
-    add_stat(character, "hunger", Stat(base_value=0, bounds=(0, 255)))
+    success = add_trait(character, "gullible")
 
-    assert has_stat(character, "hunger")
+    assert success is False
 
-    remove_stat(character, "hunger")
+    success = add_trait(character, "skeptical")
 
-    assert has_stat(character, "hunger") is False
+    assert success is False
```

### Comparing `neighborly-2.5.0/tests/test_tag_selection.py` & `neighborly-3.0.0.dev1/tests/test_tag_selection.py`

 * *Files identical despite different names*

