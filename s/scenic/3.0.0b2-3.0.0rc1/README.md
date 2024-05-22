# Comparing `tmp/scenic-3.0.0b2.tar.gz` & `tmp/scenic-3.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenic-3.0.0b2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "scenic-3.0.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `scenic-3.0.0b2.tar` & `scenic-3.0.0rc1.tar`

### file list

```diff
@@ -1,115 +1,121 @@
--rw-r--r--   0        0        0     1622 2019-02-12 18:33:34.000000 scenic-3.0.0b2/LICENSE
--rw-r--r--   0        0        0     1844 2023-05-09 15:10:50.278771 scenic-3.0.0b2/README.md
--rw-r--r--   0        0        0     2735 2023-06-30 22:49:11.376668 scenic-3.0.0b2/pyproject.toml
--rw-r--r--   0        0        0    10244 2023-02-12 21:53:28.063140 scenic-3.0.0b2/src/scenic/.DS_Store
--rw-r--r--   0        0        0      329 2023-06-30 22:40:23.467525 scenic-3.0.0b2/src/scenic/__init__.py
--rw-r--r--   0        0        0    10383 2023-06-30 22:40:23.468246 scenic-3.0.0b2/src/scenic/__main__.py
--rw-r--r--   0        0        0     6148 2023-04-20 16:43:54.709970 scenic-3.0.0b2/src/scenic/core/.DS_Store
--rw-r--r--   0        0        0       55 2023-06-30 22:40:23.468901 scenic-3.0.0b2/src/scenic/core/__init__.py
--rw-r--r--   0        0        0    51195 2023-06-30 22:40:23.469944 scenic-3.0.0b2/src/scenic/core/distributions.py
--rw-r--r--   0        0        0    32997 2023-06-30 22:40:23.471175 scenic-3.0.0b2/src/scenic/core/dynamics.py
--rw-r--r--   0        0        0    11090 2023-06-30 22:40:23.472296 scenic-3.0.0b2/src/scenic/core/errors.py
--rw-r--r--   0        0        0    15140 2023-06-30 22:40:23.473237 scenic-3.0.0b2/src/scenic/core/external_params.py
--rw-r--r--   0        0        0    10400 2023-06-30 22:40:23.474054 scenic-3.0.0b2/src/scenic/core/geometry.py
--rw-r--r--   0        0        0     9536 2023-06-30 22:40:23.474969 scenic-3.0.0b2/src/scenic/core/lazy_eval.py
--rw-r--r--   0        0        0    66305 2023-06-30 22:40:23.476364 scenic-3.0.0b2/src/scenic/core/object_types.py
--rw-r--r--   0        0        0     6559 2023-06-30 22:40:23.477046 scenic-3.0.0b2/src/scenic/core/propositions.py
--rw-r--r--   0        0        0    15990 2023-06-30 22:40:23.479989 scenic-3.0.0b2/src/scenic/core/pruning.py
--rw-r--r--   0        0        0   138471 2023-06-30 22:40:23.482098 scenic-3.0.0b2/src/scenic/core/regions.py
--rw-r--r--   0        0        0    13568 2023-06-30 22:40:23.482913 scenic-3.0.0b2/src/scenic/core/requirements.py
--rw-r--r--   0        0        0     4393 2023-06-30 22:40:23.483637 scenic-3.0.0b2/src/scenic/core/sample_checking.py
--rw-r--r--   0        0        0    28991 2023-06-30 22:40:23.484395 scenic-3.0.0b2/src/scenic/core/scenarios.py
--rw-r--r--   0        0        0    11484 2023-06-30 22:40:23.485118 scenic-3.0.0b2/src/scenic/core/serialization.py
--rw-r--r--   0        0        0     7264 2023-06-30 22:40:23.485675 scenic-3.0.0b2/src/scenic/core/shapes.py
--rw-r--r--   0        0        0    39129 2023-06-30 22:40:23.486547 scenic-3.0.0b2/src/scenic/core/simulators.py
--rw-r--r--   0        0        0     4445 2023-06-30 22:40:23.487268 scenic-3.0.0b2/src/scenic/core/specifiers.py
--rw-r--r--   0        0        0    15751 2023-06-30 22:40:23.488150 scenic-3.0.0b2/src/scenic/core/type_support.py
--rw-r--r--   0        0        0     6148 2023-04-20 16:43:54.707226 scenic-3.0.0b2/src/scenic/core/type_support/.DS_Store
--rw-r--r--   0        0        0     5022 2023-06-30 22:40:23.488952 scenic-3.0.0b2/src/scenic/core/utils.py
--rw-r--r--   0        0        0    27741 2023-06-30 22:40:23.489783 scenic-3.0.0b2/src/scenic/core/vectors.py
--rw-r--r--   0        0        0    25874 2023-06-30 22:40:23.490355 scenic-3.0.0b2/src/scenic/core/visibility.py
--rw-r--r--   0        0        0     4555 2023-06-30 22:40:23.491019 scenic-3.0.0b2/src/scenic/core/workspaces.py
--rw-r--r--   0        0        0     6148 2022-09-29 05:01:12.946087 scenic-3.0.0b2/src/scenic/domains/.DS_Store
--rw-r--r--   0        0        0       55 2023-05-09 15:10:50.304640 scenic-3.0.0b2/src/scenic/domains/__init__.py
--rw-r--r--   0        0        0     2146 2023-05-09 15:10:50.304928 scenic-3.0.0b2/src/scenic/domains/driving/__init__.py
--rw-r--r--   0        0        0     7626 2023-06-30 22:40:23.491706 scenic-3.0.0b2/src/scenic/domains/driving/actions.py
--rw-r--r--   0        0        0    12962 2023-06-29 20:07:50.086992 scenic-3.0.0b2/src/scenic/domains/driving/behaviors.scenic
--rw-r--r--   0        0        0     3000 2023-06-30 22:40:23.492538 scenic-3.0.0b2/src/scenic/domains/driving/controllers.py
--rw-r--r--   0        0        0    12663 2023-06-30 22:40:23.493317 scenic-3.0.0b2/src/scenic/domains/driving/model.scenic
--rw-r--r--   0        0        0    50790 2023-06-30 22:40:23.494161 scenic-3.0.0b2/src/scenic/domains/driving/roads.py
--rw-r--r--   0        0        0     3017 2023-06-30 22:40:23.494785 scenic-3.0.0b2/src/scenic/domains/driving/simulators.py
--rw-r--r--   0        0        0      387 2023-06-30 22:40:23.495478 scenic-3.0.0b2/src/scenic/domains/driving/workspace.py
--rw-r--r--   0        0        0     6148 2020-09-15 22:57:40.000000 scenic-3.0.0b2/src/scenic/formats/.DS_Store
--rw-r--r--   0        0        0       70 2023-05-09 15:10:50.306678 scenic-3.0.0b2/src/scenic/formats/__init__.py
--rw-r--r--   0        0        0      127 2023-05-09 15:10:50.307038 scenic-3.0.0b2/src/scenic/formats/opendrive/__init__.py
--rw-r--r--   0        0        0     1881 2023-06-30 22:40:23.497272 scenic-3.0.0b2/src/scenic/formats/opendrive/workspace.py
--rw-r--r--   0        0        0    80566 2023-06-30 22:40:23.498250 scenic-3.0.0b2/src/scenic/formats/opendrive/xodr_parser.py
--rw-r--r--   0        0        0     8196 2023-02-12 21:53:34.597183 scenic-3.0.0b2/src/scenic/simulators/.DS_Store
--rw-r--r--   0        0        0       61 2023-05-09 15:10:50.308928 scenic-3.0.0b2/src/scenic/simulators/__init__.py
--rw-r--r--   0        0        0     6148 2020-04-13 10:57:15.000000 scenic-3.0.0b2/src/scenic/simulators/carla/.DS_Store
--rw-r--r--   0        0        0      750 2023-06-30 22:40:23.498929 scenic-3.0.0b2/src/scenic/simulators/carla/__init__.py
--rw-r--r--   0        0        0     8255 2023-06-30 22:40:23.499712 scenic-3.0.0b2/src/scenic/simulators/carla/actions.py
--rw-r--r--   0        0        0     2386 2023-06-30 22:40:23.500644 scenic-3.0.0b2/src/scenic/simulators/carla/behaviors.scenic
--rw-r--r--   0        0        0     5292 2023-06-21 22:25:24.345822 scenic-3.0.0b2/src/scenic/simulators/carla/blueprints.scenic
--rw-r--r--   0        0        0     6010 2023-06-30 22:40:23.501275 scenic-3.0.0b2/src/scenic/simulators/carla/misc.py
--rw-r--r--   0        0        0    12784 2023-06-30 22:40:23.502215 scenic-3.0.0b2/src/scenic/simulators/carla/model.scenic
--rw-r--r--   0        0        0    11780 2023-06-30 22:40:23.503028 scenic-3.0.0b2/src/scenic/simulators/carla/simulator.py
--rw-r--r--   0        0        0     2536 2023-06-30 22:40:23.503894 scenic-3.0.0b2/src/scenic/simulators/carla/utils/utils.py
--rw-r--r--   0        0        0    15118 2023-06-30 22:40:23.505021 scenic-3.0.0b2/src/scenic/simulators/carla/utils/visuals.py
--rw-r--r--   0        0        0     6148 2020-04-13 07:04:31.000000 scenic-3.0.0b2/src/scenic/simulators/gta/.DS_Store
--rw-r--r--   0        0        0      205 2023-06-30 22:40:23.505977 scenic-3.0.0b2/src/scenic/simulators/gta/__init__.py
--rw-r--r--   0        0        0     8700 2023-06-30 22:40:23.506724 scenic-3.0.0b2/src/scenic/simulators/gta/center_detection.py
--rw-r--r--   0        0        0     1496 2023-06-30 22:40:23.507436 scenic-3.0.0b2/src/scenic/simulators/gta/img_modf.py
--rw-r--r--   0        0        0     8665 2023-06-30 22:40:23.508247 scenic-3.0.0b2/src/scenic/simulators/gta/interface.py
--rw-r--r--   0        0        0      234 2023-06-30 22:40:23.508695 scenic-3.0.0b2/src/scenic/simulators/gta/map.py
--rw-r--r--   0        0        0     4010 2023-06-30 22:40:23.509552 scenic-3.0.0b2/src/scenic/simulators/gta/messages.py
--rw-r--r--   0        0        0     2747 2023-06-30 22:40:23.509911 scenic-3.0.0b2/src/scenic/simulators/gta/model.scenic
--rw-r--r--   0        0        0      622 2023-06-30 22:40:23.510668 scenic-3.0.0b2/src/scenic/simulators/lgsvl/__init__.py
--rw-r--r--   0        0        0     5130 2023-06-30 22:40:23.512361 scenic-3.0.0b2/src/scenic/simulators/lgsvl/actions.py
--rw-r--r--   0        0        0      601 2023-06-30 22:40:23.512813 scenic-3.0.0b2/src/scenic/simulators/lgsvl/behaviors.scenic
--rw-r--r--   0        0        0     4124 2023-06-30 22:40:23.513528 scenic-3.0.0b2/src/scenic/simulators/lgsvl/model.scenic
--rw-r--r--   0        0        0     6114 2023-06-30 22:40:23.514263 scenic-3.0.0b2/src/scenic/simulators/lgsvl/simulator.py
--rw-r--r--   0        0        0      979 2023-06-30 22:40:23.514816 scenic-3.0.0b2/src/scenic/simulators/lgsvl/utils.py
--rw-r--r--   0        0        0      418 2023-05-09 15:10:50.313101 scenic-3.0.0b2/src/scenic/simulators/newtonian/__init__.py
--rw-r--r--   0        0        0    73799 2022-04-24 16:36:45.983622 scenic-3.0.0b2/src/scenic/simulators/newtonian/car.png
--rw-r--r--   0        0        0     1759 2023-06-30 22:40:23.515069 scenic-3.0.0b2/src/scenic/simulators/newtonian/driving_model.scenic
--rw-r--r--   0        0        0      454 2023-06-29 20:07:50.091051 scenic-3.0.0b2/src/scenic/simulators/newtonian/model.scenic
--rw-r--r--   0        0        0    10438 2023-06-30 22:40:23.515786 scenic-3.0.0b2/src/scenic/simulators/newtonian/simulator.py
--rw-r--r--   0        0        0       59 2023-05-09 15:10:50.313974 scenic-3.0.0b2/src/scenic/simulators/utils/__init__.py
--rw-r--r--   0        0        0     4389 2023-06-30 22:40:23.516386 scenic-3.0.0b2/src/scenic/simulators/utils/colors.py
--rw-r--r--   0        0        0    10244 2023-02-13 14:29:52.230267 scenic-3.0.0b2/src/scenic/simulators/webots/.DS_Store
--rw-r--r--   0        0        0     1609 2022-04-24 16:33:57.804475 scenic-3.0.0b2/src/scenic/simulators/webots/WBT.g4
--rw-r--r--   0        0        0     5416 2023-06-30 22:40:23.517077 scenic-3.0.0b2/src/scenic/simulators/webots/WBTLexer.py
--rw-r--r--   0        0        0    26753 2023-06-30 22:40:23.517884 scenic-3.0.0b2/src/scenic/simulators/webots/WBTParser.py
--rw-r--r--   0        0        0     2032 2023-06-30 22:40:23.518740 scenic-3.0.0b2/src/scenic/simulators/webots/WBTVisitor.py
--rw-r--r--   0        0        0      375 2023-06-30 22:40:23.519420 scenic-3.0.0b2/src/scenic/simulators/webots/__init__.py
--rw-r--r--   0        0        0     1468 2023-06-30 22:40:23.520099 scenic-3.0.0b2/src/scenic/simulators/webots/actions.py
--rw-r--r--   0        0        0     6148 2019-02-12 18:47:25.000000 scenic-3.0.0b2/src/scenic/simulators/webots/guideways/.DS_Store
--rw-r--r--   0        0        0      291 2023-06-30 22:40:23.521027 scenic-3.0.0b2/src/scenic/simulators/webots/guideways/__init__.py
--rw-r--r--   0        0        0     6049 2023-06-30 22:40:23.521974 scenic-3.0.0b2/src/scenic/simulators/webots/guideways/interface.py
--rw-r--r--   0        0        0      311 2023-06-30 22:40:23.522290 scenic-3.0.0b2/src/scenic/simulators/webots/guideways/intersection.py
--rw-r--r--   0        0        0     1270 2023-06-30 22:40:23.522879 scenic-3.0.0b2/src/scenic/simulators/webots/guideways/model.scenic
--rw-r--r--   0        0        0     6148 2019-02-12 18:47:20.000000 scenic-3.0.0b2/src/scenic/simulators/webots/mars/.DS_Store
--rw-r--r--   0        0        0    13755 2023-06-30 22:40:23.523654 scenic-3.0.0b2/src/scenic/simulators/webots/model.scenic
--rw-r--r--   0        0        0     6148 2019-02-12 18:47:15.000000 scenic-3.0.0b2/src/scenic/simulators/webots/road/.DS_Store
--rw-r--r--   0        0        0      178 2023-06-30 22:40:23.524575 scenic-3.0.0b2/src/scenic/simulators/webots/road/__init__.py
--rw-r--r--   0        0        0      796 2023-06-30 22:40:23.525283 scenic-3.0.0b2/src/scenic/simulators/webots/road/car_models.py
--rw-r--r--   0        0        0    16983 2023-06-30 22:40:23.526112 scenic-3.0.0b2/src/scenic/simulators/webots/road/interface.py
--rw-r--r--   0        0        0     2949 2023-06-30 22:40:23.526921 scenic-3.0.0b2/src/scenic/simulators/webots/road/model.scenic
--rw-r--r--   0        0        0      440 2023-06-30 22:40:23.527267 scenic-3.0.0b2/src/scenic/simulators/webots/road/world.py
--rw-r--r--   0        0        0    11074 2023-06-30 22:40:23.528010 scenic-3.0.0b2/src/scenic/simulators/webots/simulator.py
--rw-r--r--   0        0        0     3370 2023-06-30 22:40:23.528740 scenic-3.0.0b2/src/scenic/simulators/webots/utils.py
--rw-r--r--   0        0        0     3429 2023-06-30 22:40:23.529388 scenic-3.0.0b2/src/scenic/simulators/webots/world_parser.py
--rw-r--r--   0        0        0      215 2023-05-09 15:10:50.317105 scenic-3.0.0b2/src/scenic/simulators/xplane/__init__.py
--rw-r--r--   0        0        0      262 2022-04-24 16:33:57.813980 scenic-3.0.0b2/src/scenic/simulators/xplane/model.scenic
--rw-r--r--   0        0        0     6148 2022-09-27 14:43:55.355940 scenic-3.0.0b2/src/scenic/syntax/.DS_Store
--rw-r--r--   0        0        0     1141 2023-06-30 22:40:23.530061 scenic-3.0.0b2/src/scenic/syntax/__init__.py
--rw-r--r--   0        0        0    32133 2023-06-30 22:40:23.530497 scenic-3.0.0b2/src/scenic/syntax/ast.py
--rw-r--r--   0        0        0    60871 2023-06-30 22:40:23.531247 scenic-3.0.0b2/src/scenic/syntax/compiler.py
--rw-r--r--   0        0        0   468409 2023-06-30 18:16:53.130193 scenic-3.0.0b2/src/scenic/syntax/parser.py
--rw-r--r--   0        0        0    33410 2023-06-30 22:40:23.532150 scenic-3.0.0b2/src/scenic/syntax/pygment.py
--rw-r--r--   0        0        0     9042 2023-06-30 22:40:23.532913 scenic-3.0.0b2/src/scenic/syntax/relations.py
--rw-r--r--   0        0        0    96273 2023-06-30 22:40:23.534325 scenic-3.0.0b2/src/scenic/syntax/scenic.gram
--rw-r--r--   0        0        0    26355 2023-06-30 22:40:23.535315 scenic-3.0.0b2/src/scenic/syntax/translator.py
--rw-r--r--   0        0        0    64003 2023-06-30 22:40:23.536531 scenic-3.0.0b2/src/scenic/syntax/veneer.py
--rw-r--r--   0        0        0     4193 1970-01-01 00:00:00.000000 scenic-3.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1622 2023-07-01 17:43:04.664026 scenic-3.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     2306 2024-05-22 17:32:52.794578 scenic-3.0.0rc1/README.md
+-rw-r--r--   0        0        0     3138 2024-05-22 17:32:52.811342 scenic-3.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    10244 2024-04-03 17:13:41.465395 scenic-3.0.0rc1/src/scenic/.DS_Store
+-rw-r--r--   0        0        0      329 2024-05-04 20:37:36.900623 scenic-3.0.0rc1/src/scenic/__init__.py
+-rw-r--r--   0        0        0    10450 2024-05-22 17:32:52.811636 scenic-3.0.0rc1/src/scenic/__main__.py
+-rw-r--r--   0        0        0     6148 2023-04-20 16:43:54.709970 scenic-3.0.0rc1/src/scenic/core/.DS_Store
+-rw-r--r--   0        0        0       55 2024-05-04 20:37:36.902161 scenic-3.0.0rc1/src/scenic/core/__init__.py
+-rw-r--r--   0        0        0    51825 2024-05-22 17:32:52.812872 scenic-3.0.0rc1/src/scenic/core/distributions.py
+-rw-r--r--   0        0        0      655 2024-05-22 17:32:52.817948 scenic-3.0.0rc1/src/scenic/core/dynamics/__init__.py
+-rw-r--r--   0        0        0     2236 2024-05-22 17:32:52.820018 scenic-3.0.0rc1/src/scenic/core/dynamics/actions.py
+-rw-r--r--   0        0        0     5320 2024-05-22 17:32:52.820975 scenic-3.0.0rc1/src/scenic/core/dynamics/behaviors.py
+-rw-r--r--   0        0        0     1291 2024-05-22 17:32:52.821432 scenic-3.0.0rc1/src/scenic/core/dynamics/guards.py
+-rw-r--r--   0        0        0     7914 2024-05-22 17:32:52.822208 scenic-3.0.0rc1/src/scenic/core/dynamics/invocables.py
+-rw-r--r--   0        0        0    19627 2024-05-22 17:32:52.823547 scenic-3.0.0rc1/src/scenic/core/dynamics/scenarios.py
+-rw-r--r--   0        0        0      791 2024-05-22 17:32:52.823999 scenic-3.0.0rc1/src/scenic/core/dynamics/utils.py
+-rw-r--r--   0        0        0    11090 2024-05-04 23:59:29.370823 scenic-3.0.0rc1/src/scenic/core/errors.py
+-rw-r--r--   0        0        0    15239 2024-05-22 17:32:52.825138 scenic-3.0.0rc1/src/scenic/core/external_params.py
+-rw-r--r--   0        0        0    10400 2024-05-04 20:37:36.913832 scenic-3.0.0rc1/src/scenic/core/geometry.py
+-rw-r--r--   0        0        0     9568 2024-05-22 17:32:52.825629 scenic-3.0.0rc1/src/scenic/core/lazy_eval.py
+-rw-r--r--   0        0        0    72097 2024-05-22 17:32:52.826305 scenic-3.0.0rc1/src/scenic/core/object_types.py
+-rw-r--r--   0        0        0     6559 2024-05-04 20:37:36.917154 scenic-3.0.0rc1/src/scenic/core/propositions.py
+-rw-r--r--   0        0        0    24232 2024-05-22 17:32:52.826737 scenic-3.0.0rc1/src/scenic/core/pruning.py
+-rw-r--r--   0        0        0   150145 2024-05-22 17:32:52.829248 scenic-3.0.0rc1/src/scenic/core/regions.py
+-rw-r--r--   0        0        0    13568 2024-05-04 20:37:36.920967 scenic-3.0.0rc1/src/scenic/core/requirements.py
+-rw-r--r--   0        0        0     4393 2024-05-04 20:37:36.921602 scenic-3.0.0rc1/src/scenic/core/sample_checking.py
+-rw-r--r--   0        0        0    29983 2024-05-22 17:32:52.829826 scenic-3.0.0rc1/src/scenic/core/scenarios.py
+-rw-r--r--   0        0        0    12238 2024-05-22 17:32:52.830273 scenic-3.0.0rc1/src/scenic/core/serialization.py
+-rw-r--r--   0        0        0     7663 2024-05-22 17:32:52.831025 scenic-3.0.0rc1/src/scenic/core/shapes.py
+-rw-r--r--   0        0        0    38071 2024-05-22 17:32:52.831534 scenic-3.0.0rc1/src/scenic/core/simulators.py
+-rw-r--r--   0        0        0     4572 2024-05-22 17:32:52.832281 scenic-3.0.0rc1/src/scenic/core/specifiers.py
+-rw-r--r--   0        0        0    15807 2024-05-22 17:32:52.833290 scenic-3.0.0rc1/src/scenic/core/type_support.py
+-rw-r--r--   0        0        0     6148 2023-04-20 16:43:54.707226 scenic-3.0.0rc1/src/scenic/core/type_support/.DS_Store
+-rw-r--r--   0        0        0    11532 2024-05-22 17:32:52.834065 scenic-3.0.0rc1/src/scenic/core/utils.py
+-rw-r--r--   0        0        0    28638 2024-05-22 17:32:52.834898 scenic-3.0.0rc1/src/scenic/core/vectors.py
+-rw-r--r--   0        0        0    25874 2024-05-04 20:37:36.933728 scenic-3.0.0rc1/src/scenic/core/visibility.py
+-rw-r--r--   0        0        0     4555 2024-05-04 20:37:36.934475 scenic-3.0.0rc1/src/scenic/core/workspaces.py
+-rw-r--r--   0        0        0     6148 2022-09-29 05:01:12.946087 scenic-3.0.0rc1/src/scenic/domains/.DS_Store
+-rw-r--r--   0        0        0       55 2023-07-01 18:11:06.432308 scenic-3.0.0rc1/src/scenic/domains/__init__.py
+-rw-r--r--   0        0        0     2210 2024-05-22 17:32:52.835751 scenic-3.0.0rc1/src/scenic/domains/driving/__init__.py
+-rw-r--r--   0        0        0     7626 2024-05-04 20:37:36.936049 scenic-3.0.0rc1/src/scenic/domains/driving/actions.py
+-rw-r--r--   0        0        0    12962 2024-05-04 23:59:29.378592 scenic-3.0.0rc1/src/scenic/domains/driving/behaviors.scenic
+-rw-r--r--   0        0        0     3000 2024-05-04 20:37:36.937815 scenic-3.0.0rc1/src/scenic/domains/driving/controllers.py
+-rw-r--r--   0        0        0    13649 2024-05-22 17:32:52.836156 scenic-3.0.0rc1/src/scenic/domains/driving/model.scenic
+-rw-r--r--   0        0        0    51507 2024-05-22 17:32:52.837001 scenic-3.0.0rc1/src/scenic/domains/driving/roads.py
+-rw-r--r--   0        0        0     3017 2024-05-04 20:37:36.940133 scenic-3.0.0rc1/src/scenic/domains/driving/simulators.py
+-rw-r--r--   0        0        0      387 2024-05-04 20:37:36.941265 scenic-3.0.0rc1/src/scenic/domains/driving/workspace.py
+-rw-r--r--   0        0        0     6148 2020-09-15 22:57:40.000000 scenic-3.0.0rc1/src/scenic/formats/.DS_Store
+-rw-r--r--   0        0        0       70 2023-07-01 18:11:06.437266 scenic-3.0.0rc1/src/scenic/formats/__init__.py
+-rw-r--r--   0        0        0      127 2023-07-01 18:11:06.437496 scenic-3.0.0rc1/src/scenic/formats/opendrive/__init__.py
+-rw-r--r--   0        0        0     1881 2024-05-04 20:37:36.941846 scenic-3.0.0rc1/src/scenic/formats/opendrive/workspace.py
+-rw-r--r--   0        0        0    81879 2024-05-22 17:32:52.838582 scenic-3.0.0rc1/src/scenic/formats/opendrive/xodr_parser.py
+-rw-r--r--   0        0        0     8196 2023-02-12 21:53:34.597183 scenic-3.0.0rc1/src/scenic/simulators/.DS_Store
+-rw-r--r--   0        0        0       61 2023-07-01 18:11:06.439388 scenic-3.0.0rc1/src/scenic/simulators/__init__.py
+-rw-r--r--   0        0        0     6148 2020-04-13 10:57:15.000000 scenic-3.0.0rc1/src/scenic/simulators/carla/.DS_Store
+-rw-r--r--   0        0        0      817 2024-05-22 17:32:52.839238 scenic-3.0.0rc1/src/scenic/simulators/carla/__init__.py
+-rw-r--r--   0        0        0     8490 2024-05-22 17:32:52.839820 scenic-3.0.0rc1/src/scenic/simulators/carla/actions.py
+-rw-r--r--   0        0        0     2386 2024-05-04 20:37:36.945225 scenic-3.0.0rc1/src/scenic/simulators/carla/behaviors.scenic
+-rw-r--r--   0        0        0     5100 2024-05-22 17:32:52.840394 scenic-3.0.0rc1/src/scenic/simulators/carla/blueprints.py
+-rw-r--r--   0        0        0     6010 2024-05-04 20:37:36.946287 scenic-3.0.0rc1/src/scenic/simulators/carla/misc.py
+-rw-r--r--   0        0        0    13527 2024-05-22 17:32:52.840659 scenic-3.0.0rc1/src/scenic/simulators/carla/model.scenic
+-rw-r--r--   0        0        0    11975 2024-05-22 17:32:52.840933 scenic-3.0.0rc1/src/scenic/simulators/carla/simulator.py
+-rw-r--r--   0        0        0     2490 2024-05-22 17:32:52.841152 scenic-3.0.0rc1/src/scenic/simulators/carla/utils/utils.py
+-rw-r--r--   0        0        0    15118 2024-05-04 20:37:36.948041 scenic-3.0.0rc1/src/scenic/simulators/carla/utils/visuals.py
+-rw-r--r--   0        0        0     6148 2020-04-13 07:04:31.000000 scenic-3.0.0rc1/src/scenic/simulators/gta/.DS_Store
+-rw-r--r--   0        0        0      262 2024-05-22 17:32:52.841821 scenic-3.0.0rc1/src/scenic/simulators/gta/__init__.py
+-rw-r--r--   0        0        0     8700 2024-05-04 20:37:36.949215 scenic-3.0.0rc1/src/scenic/simulators/gta/center_detection.py
+-rw-r--r--   0        0        0     1496 2024-05-15 22:24:13.008500 scenic-3.0.0rc1/src/scenic/simulators/gta/img_modf.py
+-rw-r--r--   0        0        0     8666 2024-05-22 17:32:52.842530 scenic-3.0.0rc1/src/scenic/simulators/gta/interface.py
+-rw-r--r--   0        0        0      234 2024-05-04 20:37:36.950472 scenic-3.0.0rc1/src/scenic/simulators/gta/map.py
+-rw-r--r--   0        0        0     4010 2024-05-04 20:37:36.951046 scenic-3.0.0rc1/src/scenic/simulators/gta/messages.py
+-rw-r--r--   0        0        0     2747 2024-05-04 20:37:36.951246 scenic-3.0.0rc1/src/scenic/simulators/gta/model.scenic
+-rw-r--r--   0        0        0      403 2024-05-22 17:32:52.843193 scenic-3.0.0rc1/src/scenic/simulators/lgsvl/__init__.py
+-rw-r--r--   0        0        0     5130 2024-05-04 20:37:36.952383 scenic-3.0.0rc1/src/scenic/simulators/lgsvl/actions.py
+-rw-r--r--   0        0        0      601 2024-05-04 20:37:36.952624 scenic-3.0.0rc1/src/scenic/simulators/lgsvl/behaviors.scenic
+-rw-r--r--   0        0        0     4441 2024-05-22 17:32:52.843856 scenic-3.0.0rc1/src/scenic/simulators/lgsvl/model.scenic
+-rw-r--r--   0        0        0     6114 2024-05-04 20:37:36.953869 scenic-3.0.0rc1/src/scenic/simulators/lgsvl/simulator.py
+-rw-r--r--   0        0        0      979 2024-05-04 20:37:36.954531 scenic-3.0.0rc1/src/scenic/simulators/lgsvl/utils.py
+-rw-r--r--   0        0        0      475 2024-05-22 17:32:52.844510 scenic-3.0.0rc1/src/scenic/simulators/newtonian/__init__.py
+-rw-r--r--   0        0        0    73799 2023-07-01 17:49:37.066496 scenic-3.0.0rc1/src/scenic/simulators/newtonian/car.png
+-rw-r--r--   0        0        0     1763 2024-05-22 17:32:52.845139 scenic-3.0.0rc1/src/scenic/simulators/newtonian/driving_model.scenic
+-rw-r--r--   0        0        0      454 2023-07-01 17:49:37.066908 scenic-3.0.0rc1/src/scenic/simulators/newtonian/model.scenic
+-rw-r--r--   0        0        0    10438 2024-05-04 20:37:36.956061 scenic-3.0.0rc1/src/scenic/simulators/newtonian/simulator.py
+-rw-r--r--   0        0        0       59 2023-07-01 18:11:06.452903 scenic-3.0.0rc1/src/scenic/simulators/utils/__init__.py
+-rw-r--r--   0        0        0     4480 2024-05-22 17:32:52.846030 scenic-3.0.0rc1/src/scenic/simulators/utils/colors.py
+-rw-r--r--   0        0        0    10244 2023-02-13 14:29:52.230267 scenic-3.0.0rc1/src/scenic/simulators/webots/.DS_Store
+-rw-r--r--   0        0        0     1609 2023-07-01 17:44:04.908336 scenic-3.0.0rc1/src/scenic/simulators/webots/WBT.g4
+-rw-r--r--   0        0        0     5416 2024-05-04 20:37:36.957297 scenic-3.0.0rc1/src/scenic/simulators/webots/WBTLexer.py
+-rw-r--r--   0        0        0    26753 2024-05-04 20:37:36.958228 scenic-3.0.0rc1/src/scenic/simulators/webots/WBTParser.py
+-rw-r--r--   0        0        0     2032 2024-05-04 20:37:36.958807 scenic-3.0.0rc1/src/scenic/simulators/webots/WBTVisitor.py
+-rw-r--r--   0        0        0      375 2024-05-04 20:37:36.959298 scenic-3.0.0rc1/src/scenic/simulators/webots/__init__.py
+-rw-r--r--   0        0        0     1468 2024-05-04 20:37:36.959878 scenic-3.0.0rc1/src/scenic/simulators/webots/actions.py
+-rw-r--r--   0        0        0     6148 2019-02-12 18:47:25.000000 scenic-3.0.0rc1/src/scenic/simulators/webots/guideways/.DS_Store
+-rw-r--r--   0        0        0      291 2024-05-04 20:37:36.960371 scenic-3.0.0rc1/src/scenic/simulators/webots/guideways/__init__.py
+-rw-r--r--   0        0        0     6049 2024-05-04 20:37:36.961009 scenic-3.0.0rc1/src/scenic/simulators/webots/guideways/interface.py
+-rw-r--r--   0        0        0      311 2024-05-04 20:37:36.961231 scenic-3.0.0rc1/src/scenic/simulators/webots/guideways/intersection.py
+-rw-r--r--   0        0        0     1270 2024-05-04 20:37:36.961603 scenic-3.0.0rc1/src/scenic/simulators/webots/guideways/model.scenic
+-rw-r--r--   0        0        0     6148 2019-02-12 18:47:20.000000 scenic-3.0.0rc1/src/scenic/simulators/webots/mars/.DS_Store
+-rw-r--r--   0        0        0    13755 2024-05-04 20:37:36.962308 scenic-3.0.0rc1/src/scenic/simulators/webots/model.scenic
+-rw-r--r--   0        0        0     6148 2019-02-12 18:47:15.000000 scenic-3.0.0rc1/src/scenic/simulators/webots/road/.DS_Store
+-rw-r--r--   0        0        0      178 2024-05-04 20:37:36.962926 scenic-3.0.0rc1/src/scenic/simulators/webots/road/__init__.py
+-rw-r--r--   0        0        0      796 2024-05-04 20:37:36.963410 scenic-3.0.0rc1/src/scenic/simulators/webots/road/car_models.py
+-rw-r--r--   0        0        0    16983 2024-05-04 20:37:36.964016 scenic-3.0.0rc1/src/scenic/simulators/webots/road/interface.py
+-rw-r--r--   0        0        0     2949 2024-05-04 20:37:36.964636 scenic-3.0.0rc1/src/scenic/simulators/webots/road/model.scenic
+-rw-r--r--   0        0        0      440 2024-05-04 20:37:36.964832 scenic-3.0.0rc1/src/scenic/simulators/webots/road/world.py
+-rw-r--r--   0        0        0    11074 2024-05-04 20:37:36.965412 scenic-3.0.0rc1/src/scenic/simulators/webots/simulator.py
+-rw-r--r--   0        0        0     3370 2024-05-04 20:37:36.965994 scenic-3.0.0rc1/src/scenic/simulators/webots/utils.py
+-rw-r--r--   0        0        0     3429 2024-05-04 20:37:36.966727 scenic-3.0.0rc1/src/scenic/simulators/webots/world_parser.py
+-rw-r--r--   0        0        0      215 2023-07-01 18:11:06.464416 scenic-3.0.0rc1/src/scenic/simulators/xplane/__init__.py
+-rw-r--r--   0        0        0      262 2023-08-28 02:49:08.905157 scenic-3.0.0rc1/src/scenic/simulators/xplane/model.scenic
+-rw-r--r--   0        0        0     6148 2022-09-27 14:43:55.355940 scenic-3.0.0rc1/src/scenic/syntax/.DS_Store
+-rw-r--r--   0        0        0     1141 2024-05-04 20:37:36.967233 scenic-3.0.0rc1/src/scenic/syntax/__init__.py
+-rw-r--r--   0        0        0    32806 2024-05-22 17:32:52.847122 scenic-3.0.0rc1/src/scenic/syntax/ast.py
+-rw-r--r--   0        0        0    61638 2024-05-22 17:32:52.848276 scenic-3.0.0rc1/src/scenic/syntax/compiler.py
+-rw-r--r--   0        0        0   515661 2024-05-10 17:25:21.614883 scenic-3.0.0rc1/src/scenic/syntax/parser.py
+-rw-r--r--   0        0        0    33410 2024-05-04 20:37:36.970371 scenic-3.0.0rc1/src/scenic/syntax/pygment.py
+-rw-r--r--   0        0        0     9042 2024-05-04 20:37:36.971183 scenic-3.0.0rc1/src/scenic/syntax/relations.py
+-rw-r--r--   0        0        0   109784 2024-05-22 17:32:52.849744 scenic-3.0.0rc1/src/scenic/syntax/scenic.gram
+-rw-r--r--   0        0        0    26414 2024-05-22 17:32:52.850361 scenic-3.0.0rc1/src/scenic/syntax/translator.py
+-rw-r--r--   0        0        0    65603 2024-05-22 17:32:52.850978 scenic-3.0.0rc1/src/scenic/syntax/veneer.py
+-rw-r--r--   0        0        0     5221 1970-01-01 00:00:00.000000 scenic-3.0.0rc1/PKG-INFO
```

### Comparing `scenic-3.0.0b2/LICENSE` & `scenic-3.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/README.md` & `scenic-3.0.0rc1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # Scenic
 
 [![Documentation Status](https://readthedocs.org/projects/scenic-lang/badge/?version=latest)](https://scenic-lang.readthedocs.io/en/latest/?badge=latest)
 [![Tests Status](https://github.com/BerkeleyLearnVerify/Scenic/actions/workflows/run-tests.yml/badge.svg)](https://github.com/BerkeleyLearnVerify/Scenic/actions/workflows/run-tests.yml)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
-A compiler and scenario generator for the Scenic scenario description language.
+A compiler and scenario generator for Scenic, a domain-specific probabilistic programming language for modeling the environments of cyber-physical systems.
 Please see the [documentation](https://scenic-lang.readthedocs.io/) for installation instructions, as well as tutorials and other information about the Scenic language, its implementation, and its interfaces to various simulators.
 
-For a description of the language and some of its applications, see [our journal paper](https://link.springer.com/article/10.1007/s10994-021-06120-5), which extends our [PLDI 2019 paper](https://arxiv.org/abs/1809.09310) (*note:* the syntax of Scenic has changed slightly since the PLDI paper, and many features such as support for dynamic scenarios have been added; these are described in the journal paper).
-Scenic was designed and implemented by Daniel J. Fremont, Edward Kim, Tommaso Dreossi, Shromona Ghosh, Xiangyu Yue, Alberto L. Sangiovanni-Vincentelli, and Sanjit A. Seshia.
+For an overview of the language and some of its applications, see our [2022 journal paper](https://link.springer.com/article/10.1007/s10994-021-06120-5) on Scenic 2, which extends our [PLDI 2019 paper](https://arxiv.org/abs/1809.09310) on Scenic 1.
+The new syntax and features of Scenic 3 are described in our [CAV 2023 paper](https://arxiv.org/abs/2307.03325).
+Our [Publications](https://scenic-lang.readthedocs.io/en/latest/publications.html) page lists additional relevant publications.
+
+Scenic was initially designed and implemented by Daniel J. Fremont, Tommaso Dreossi, Shromona Ghosh, Xiangyu Yue, Alberto L. Sangiovanni-Vincentelli, and Sanjit A. Seshia.
+Additionally, Edward Kim made major contributions to Scenic 2, and Eric Vin, Shun Kashiwa, Matthew Rhea, and Ellen Kalvan to Scenic 3.
+Please see our [Credits](https://scenic-lang.readthedocs.io/en/latest/credits.html) page for details and more contributors.
 
-If you have any problems using Scenic, please submit an issue to [our GitHub repository](https://github.com/BerkeleyLearnVerify/Scenic) or contact Daniel at <dfremont@ucsc.edu>.
+If you have any problems using Scenic, please submit an issue to [our GitHub repository](https://github.com/BerkeleyLearnVerify/Scenic).
 
 The repository is organized as follows:
 
 * the _src/scenic_ directory contains the package proper;
 * the _examples_ directory has many examples of Scenic programs;
+* the _assets_ directory contains meshes and other resources used by the examples and tests;
 * the _docs_ directory contains the sources for the documentation;
-* the _tests_ directory contains tests for the Scenic compiler.
+* the _tests_ directory contains tests for the Scenic tool.
```

### Comparing `scenic-3.0.0b2/pyproject.toml` & `scenic-3.0.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [project]
 name = "scenic"
-version = "3.0.0b2"
+version = "3.0.0rc1"
 description = "The Scenic scenario description language."
 authors = [
 	{ name = "Daniel Fremont" },
 	{ name = "Eric Vin" },
+	{ name = "Shun Kashiwa" },
 	{ name = "Edward Kim" },
 	{ name = "Tommaso Dreossi" },
 	{ name = "Shromona Ghosh" },
 	{ name = "Xiangyu Yue" },
 	{ name = "Alberto L. Sangiovanni-Vincentelli" },
 	{ name = "Sanjit A. Seshia" },
 ]
@@ -27,53 +28,63 @@
 
 dependencies = [
 	"antlr4-python3-runtime ~= 4.11",
 	"attrs >= 19.3.0",
 	"dotmap ~= 1.3",
 	"mapbox_earcut >= 0.12.10",
 	"matplotlib ~= 3.2",
+	"manifold3d == 2.3.0",
 	"networkx >= 2.6",
 	"numpy ~= 1.24",
 	"opencv-python ~= 4.5",
-	"pegen >= 0.2",
-	"pillow ~= 9.1",
+	"pegen >= 0.3.0",
+	"pillow >= 9.1",
 	'pygame >= 2.1.3.dev8, <3; python_version >= "3.11"',
 	'pygame ~= 2.0; python_version < "3.11"',
 	"pyglet ~= 1.5",
 	"python-fcl >= 0.7",
 	"Rtree ~= 1.0",
 	"rv-ltl ~= 0.1",
+	"scikit-image ~= 0.21",
 	"scipy ~= 1.7",
 	"shapely ~= 2.0",
-	"trimesh >=3.22.2, <4",
+	"trimesh >=4.0.9, <5",
 ]
 
 [project.optional-dependencies]
 guideways = [
 	'pyproj ~= 3.0; python_version < "3.10"',
 	'pyproj ~= 3.3; python_version >= "3.10"',
 ]
 test = [	# minimum dependencies for running tests (used for tox virtualenvs)
 	"pytest >= 7.0.0, <8",
+	"pytest-cov >= 3.0.0",
 	"pytest-randomly ~= 3.2",
 ]
-dev = [
-	"scenic[test]",		# all dependencies from 'test' extra above
-	"scenic[guideways]", # for running guideways modules
+test-full = [  # like 'test' but adds dependencies for optional features
+	"scenic[test]",       # all dependencies from 'test' extra above
+	"scenic[guideways]",  # for running guideways modules
 	"astor >= 0.8.1",
-	"black ~= 23.0",
+	'carla >= 0.9.12; python_version <= "3.8" and (platform_system == "Linux" or platform_system == "Windows")',
+	"dill",
+	"exceptiongroup",
 	"inflect ~= 5.5",
-	"isort ~= 5.11",
-	"pre-commit ~= 3.0",
 	"pygments ~= 2.11",
-	"pytest-cov >= 3.0.0",
 	"sphinx >= 5.0.0, <6",
 	"sphinx_rtd_theme >= 0.5.2",
 	"sphinx-tabs ~= 3.4.1",
-	"tox ~= 3.14",
+	"verifai >= 2.1.0b1",
+]
+dev = [
+	"scenic[test-full]",
+	"black ~= 24.0",
+	"isort ~= 5.11",
+	"pre-commit ~= 3.0",
+	"pytest-cov >= 3.0.0",
+	"tox ~= 4.0",
 ]
 
 [project.urls]
 Repository = "https://github.com/BerkeleyLearnVerify/Scenic"
 Documentation = "https://scenic-lang.readthedocs.io"
 
 [project.scripts]
@@ -107,7 +118,10 @@
 extend_skip_glob = [
 	"src/scenic/simulators/webots/WBT.*",
 	"tests/syntax/polychrome.*",
 ]
 
 [tool.pytest.ini_options]
 norecursedirs = ["examples"]
+
+[tool.coverage.run]
+source = ["src"]
```

### Comparing `scenic-3.0.0b2/src/scenic/.DS_Store` & `scenic-3.0.0rc1/src/scenic/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -389,28 +389,28 @@
 00001840: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
 00001850: 6d6e 6f87 0000 0000 0000 0101 0000 0000  mno.............
 00001860: 0000 000d 0000 0000 0000 0000 0000 0000  ................
 00001870: 0000 0088 0000 000a 0073 0069 006d 0075  .........s.i.m.u
 00001880: 006c 0061 0074 006f 0072 0073 7653 726e  .l.a.t.o.r.svSrn
 00001890: 6c6f 6e67 0000 0001 0000 0006 0073 0079  long.........s.y
 000018a0: 006e 0074 0061 0078 6277 7370 626c 6f62  .n.t.a.xbwspblob
-000018b0: 0000 00b7 6270 6c69 7374 3030 d601 0203  ....bplist00....
+000018b0: 0000 00b6 6270 6c69 7374 3030 d601 0203  ....bplist00....
 000018c0: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
 000018d0: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
 000018e0: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 000018f0: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 00001900: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
 00001910: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00001920: 0908 095f 1017 7b7b 3233 322c 2036 397d  ..._..{{232, 69}
-00001930: 2c20 7b39 3230 2c20 3433 367d 7d09 0815  , {920, 436}}...
-00001940: 232f 3b52 5f6b 6c6d 6e6f 8900 0000 0000  #/;R_klmno......
-00001950: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
-00001960: 0000 0000 0000 0000 0000 8a00 0000 0600  ................
-00001970: 7300 7900 6e00 7400 6100 7876 5372 6e6c  s.y.n.t.a.xvSrnl
-00001980: 6f6e 6700 0000 0100 0000 0000 0000 0000  ong.............
+00001920: 0908 095f 1016 7b7b 322c 2034 3136 7d2c  ..._..{{2, 416},
+00001930: 207b 3932 302c 2034 3336 7d7d 0908 1523   {920, 436}}...#
+00001940: 2f3b 525f 6b6c 6d6e 6f88 0000 0000 0000  /;R_klmno.......
+00001950: 0101 0000 0000 0000 000d 0000 0000 0000  ................
+00001960: 0000 0000 0000 0000 0089 0000 0006 0073  ...............s
+00001970: 0079 006e 0074 0061 0078 7653 726e 6c6f  .y.n.t.a.xvSrnlo
+00001980: 6e67 0000 0001 0000 0000 0000 0000 0000  ng..............
 00001990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `scenic-3.0.0b2/src/scenic/__main__.py` & `scenic-3.0.0rc1/src/scenic/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,34 +47,35 @@
     help="override a global parameter",
     nargs=2,
     default=[],
     action="append",
     metavar=("PARAM", "VALUE"),
 )
 mainOptions.add_argument(
+    "--count",
+    help="number of successful scenes to generate or simulations to run (default infinity)",
+    type=int,
+    default=0,
+)
+mainOptions.add_argument(
     "-m", "--model", help="specify a Scenic world model", default=None
 )
 mainOptions.add_argument(
     "--scenario", default=None, help="name of scenario to run (if file contains multiple)"
 )
 mainOptions.add_argument(
     "--2d", action="store_true", help="run Scenic in 2D compatibility mode"
 )
 
 # Simulation options
 simOpts = parser.add_argument_group("dynamic simulation options")
 simOpts.add_argument(
     "--time", help="time bound for simulations (default none)", type=int, default=None
 )
-simOpts.add_argument(
-    "--count",
-    help="number of successful simulations to run (default infinity)",
-    type=int,
-    default=0,
-)
+
 simOpts.add_argument(
     "--max-sims-per-scene",
     type=int,
     default=1,
     metavar="N",
     help="max # of rejected simulations before sampling a new scene (default 1)",
 )
@@ -250,15 +251,16 @@
                     print(f"      {step:4d}: {subval}")
             else:
                 print(f'    Record "{name}": {value}')
     return simulation is not None
 
 
 try:
-    if args.gather_stats is None:  # Generate scenes interactively until killed
+    if args.gather_stats is None:
+        # Generate scenes interactively until killed/count reached
         if not args.simulate:  # will need matplotlib to draw scene schematic
             import matplotlib
             import matplotlib.pyplot as plt
 
             if matplotlib.get_backend().lower() == "agg":
                 raise RuntimeError(
                     "need an interactive matplotlib backend to display scenes\n"
@@ -268,27 +270,29 @@
         successCount = 0
         while True:
             scene, _ = generateScene()
             if args.simulate:
                 success = runSimulation(scene)
                 if success:
                     successCount += 1
-                    if 0 < args.count <= successCount:
-                        break
             else:
+                successCount += 1
                 if mode2D:
                     if delay is None:
                         scene.show2D(zoom=args.zoom)
                     else:
                         scene.show2D(zoom=args.zoom, block=False)
                         plt.pause(delay)
                         plt.clf()
                 else:
                     scene.show(axes=args.axes)
 
+            if 0 < args.count <= successCount:
+                break
+
     else:  # Gather statistics over the specified number of scenes/iterations
         its = []
         maxIterations = 2000
         iterations = 0
         totalIterations = 0
         if args.gather_stats >= 0:  # scenes
```

### Comparing `scenic-3.0.0b2/src/scenic/core/.DS_Store` & `scenic-3.0.0rc1/src/scenic/core/.DS_Store`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/core/distributions.py` & `scenic-3.0.0rc1/src/scenic/core/distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,16 +326,16 @@
         return None, None
 
     def __getattr__(self, name):
         if name.startswith("__") and name.endswith("__"):  # ignore special attributes
             return object.__getattribute__(self, name)
         return AttributeDistribution(name, self)
 
-    def __call__(self, *args):
-        return OperatorDistribution("__call__", self, args)
+    def __call__(self, *args, **kwargs):
+        return OperatorDistribution("__call__", self, args, kwargs)
 
     def __iter__(self):
         raise RandomControlFlowError(f"cannot iterate through a random value")
 
     def _comparisonError(self, other):
         raise RandomControlFlowError(
             "random values cannot be compared " "(and control flow cannot depend on them)"
@@ -680,54 +680,57 @@
     def supportInterval(self):
         obj = self.object
         if isinstance(obj, MultiplexerDistribution):
             attrs = (getattr(opt, self.attribute) for opt in obj.options)
             return unionOfSupports(supportInterval(attr) for attr in attrs)
         return None, None
 
-    def __call__(self, *args):
+    def __call__(self, *args, **kwargs):
         vty = self.object._valueType
         retTy = None
         if vty is not object:
             func = getattr(vty, self.attribute, None)
             if func:
                 if isinstance(func, property):
                     func = func.fget
                 retTy = get_type_hints(func).get("return")
-        return OperatorDistribution("__call__", self, args, valueType=retTy)
+        return OperatorDistribution("__call__", self, args, kwargs, valueType=retTy)
 
     def __repr__(self):
         return f"{self.object!r}.{self.attribute}"
 
 
 class OperatorDistribution(Distribution):
     """Distribution resulting from applying an operator to one or more distributions"""
 
     _deterministic = True
 
-    def __init__(self, operator, obj, operands, valueType=None):
+    def __init__(self, operator, obj, operands, kwoperands, valueType=None):
         operands = tuple(toDistribution(arg) for arg in operands)
+        kwoperands = {key: toDistribution(kwarg) for key, kwarg in kwoperands.items()}
+        dependencies = operands + tuple(kwoperands.values())
         if valueType is None:
             ty = type_support.underlyingType(obj)
-            valueType = self.inferType(ty, operator, operands)
-        super().__init__(obj, *operands, valueType=valueType)
+            valueType = self.inferType(ty, operator, operands, kwoperands)
+        super().__init__(obj, *dependencies, valueType=valueType)
         self.operator = operator
         self.object = obj
         self.operands = operands
+        self.kwoperands = kwoperands
         self.symbol = allowedReversibleOperators.get(operator)
         if self.symbol:
             if operator[:3] == "__r":
                 self.reverse = "__" + operator[3:]
             else:
                 self.reverse = "__r" + operator[2:]
         else:
             self.reverse = None
 
     @staticmethod
-    def inferType(ty, operator, operands):
+    def inferType(ty, operator, operands, kwoperands):
         """Attempt to infer the result type of the given operator application."""
         # If the object's type is known, see if we have a return type annotation.
         origin = type_support.get_type_origin(ty)
         op = getattr(origin if origin else ty, operator, None)
         if op:
             retTy = get_type_hints(op).get("return")
             if retTy:
@@ -737,15 +740,17 @@
         if origin == typing.Union:
             types = []
             for option in type_support.get_type_args(ty):
                 if option is type(None) and not hasattr(None, operator):
                     # None does not support this operator; using it will raise an
                     # exception, so we can ignore this case for type inference.
                     continue
-                res = OperatorDistribution.inferType(option, operator, operands)
+                res = OperatorDistribution.inferType(
+                    option, operator, operands, kwoperands
+                )
                 types.append(res)
             return type_support.unifierOfTypes(types) if types else object
 
         # The supported arithmetic operations on scalars all return scalars.
         def scalar(thing):
             ty = type_support.underlyingType(thing)
             return type_support.canCoerceType(ty, float)
@@ -792,44 +797,48 @@
 
         # We can't tell what the result type is.
         return object
 
     def sampleGiven(self, value):
         first = value[self.object]
         rest = [value[child] for child in self.operands]
+        kwargs = {key: value[child] for key, child in self.kwoperands.items()}
         op = getattr(first, self.operator)
-        result = op(*rest)
+        result = op(*rest, **kwargs)
         if result is NotImplemented and self.reverse:
-            assert len(rest) == 1
+            assert len(rest) == 1 and len(kwargs) == 0
             rop = getattr(rest[0], self.reverse)
             result = rop(first)
         if result is NotImplemented and self.symbol:
             raise TypeError(
                 f"unsupported operand type(s) for {self.symbol}: "
                 f"'{type(first).__name__}' and '{type(rest[0]).__name__}'"
             )
         return result
 
     def evaluateInner(self, context):
         obj = valueInContext(self.object, context)
         operands = tuple(valueInContext(arg, context) for arg in self.operands)
-        return OperatorDistribution(self.operator, obj, operands)
+        kwoperands = {
+            key: valueInContext(arg, context) for key, kwarg in self.kwoperands.items()
+        }
+        return OperatorDistribution(self.operator, obj, operands, kwoperands)
 
     def supportInterval(self):
         if self.operator in (
             "__add__",
             "__radd__",
             "__sub__",
             "__rsub__",
             "__mul__",
             "__rmul__",
             "__truediv__",
             "__rtruediv__",
         ):
-            assert len(self.operands) == 1
+            assert len(self.operands) == 1 and len(self.kwoperands) == 0
             l1, r1 = supportInterval(self.object)
             l2, r2 = supportInterval(self.operands[0])
             if l1 is None or l2 is None or r1 is None or r2 is None:
                 return None, None
             if self.operator == "__add__" or self.operator == "__radd__":
                 l = l1 + l2
                 r = r1 + r2
@@ -855,15 +864,15 @@
                     r = r2 / l1 if r2 >= 0 else r2 / r1
                 else:
                     l, r = None, None
             else:
                 raise AssertionError(f"unexpected operator {self.operator}")
             return l, r
         elif self.operator in ("__neg__", "__abs__"):
-            assert len(self.operands) == 0
+            assert len(self.operands) == 0 and len(self.kwoperands) == 0
             l, r = supportInterval(self.object)
             if self.operator == "__neg__":
                 return -r, -l
             elif self.operator == "__abs__":
                 if r < 0:
                     return -r, -l
                 elif l < 0:
@@ -917,43 +926,43 @@
         def handler(self, arg):
             if (
                 not isLazy(arg)
                 and issubclass(self._valueType, numbers.Number)
                 and arg == 0
             ):
                 return self
-            return OperatorDistribution(op, self, (arg,), valueType=ty)
+            return OperatorDistribution(op, self, (arg,), {}, valueType=ty)
 
     elif op in ("__mul__", "__rmul__"):
 
         def handler(self, arg):
             if not isLazy(arg):
                 if issubclass(self._valueType, numbers.Number) and arg == 1:
                     return self
                 from scenic.core.vectors import Orientation, globalOrientation
 
                 if issubclass(self._valueType, Orientation) and arg == globalOrientation:
                     return self
-            return OperatorDistribution(op, self, (arg,), valueType=ty)
+            return OperatorDistribution(op, self, (arg,), {}, valueType=ty)
 
     elif op in ("__truediv__", "__floordiv__", "__pow__"):
 
         def handler(self, arg):
             if (
                 not isLazy(arg)
                 and issubclass(self._valueType, numbers.Number)
                 and arg == 1
             ):
                 return self
-            return OperatorDistribution(op, self, (arg,), valueType=ty)
+            return OperatorDistribution(op, self, (arg,), {}, valueType=ty)
 
     else:
         # The general case.
         def handler(self, *args):
-            return OperatorDistribution(op, self, args, valueType=ty)
+            return OperatorDistribution(op, self, args, {}, valueType=ty)
 
     return handler
 
 
 for data in allowedOperators:
     if isinstance(data, tuple):
         op, ty = data
```

### Comparing `scenic-3.0.0b2/src/scenic/core/errors.py` & `scenic-3.0.0rc1/src/scenic/core/errors.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/core/external_params.py` & `scenic-3.0.0rc1/src/scenic/core/external_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,18 +202,20 @@
 
         # set up VerifAI sampler
         samplerType = globalParams.get("verifaiSamplerType", "halton")
         samplerParams = globalParams.get("verifaiSamplerParams", None)
         if usingProbs and samplerType == "ce":
             if samplerParams is None:
                 samplerParams = DotMap()
+            else:
+                samplerParams = samplerParams.copy()  # avoid mutating original
             if "cont" in samplerParams or "disc" in samplerParams:
                 raise RuntimeError(
                     "CE distributions specified in both VerifaiParameters"
-                    "and verifaiSamplerParams"
+                    " and verifaiSamplerParams"
                 )
             cont_buckets = []
             cont_dists = []
             disc_dists = []
             for param in self.params:
                 if isinstance(param, VerifaiRange):
                     if param.probs is None:
```

### Comparing `scenic-3.0.0b2/src/scenic/core/geometry.py` & `scenic-3.0.0rc1/src/scenic/core/geometry.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/core/lazy_eval.py` & `scenic-3.0.0rc1/src/scenic/core/lazy_eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,15 @@
 def needsLazyEvaluation(thing):
     """Whether the given value requires lazy evaluation."""
     return getattr(thing, "_needsLazyEval", False)
 
 
 def dependencies(thing):
     """Dependencies which must be sampled before this value."""
-    return getattr(thing, "_dependencies", ())
+    return getattr(getattr(thing, "_conditioned", thing), "_dependencies", ())
 
 
 def needsSampling(thing):
     """Whether this value requires sampling."""
     return getattr(thing, "_needsSampling", False)
```

### Comparing `scenic-3.0.0b2/src/scenic/core/object_types.py` & `scenic-3.0.0rc1/src/scenic/core/object_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 import numpy as np
 import shapely
 import shapely.affinity
 import trimesh
 
 from scenic.core.distributions import (
+    FunctionDistribution,
     MultiplexerDistribution,
     RandomControlFlowError,
     Samplable,
     distributionFunction,
     distributionMethod,
     needsSampling,
     supportInterval,
@@ -41,15 +42,20 @@
     averageVectors,
     hypot,
     max,
     min,
     normalizeAngle,
     pointIsInCone,
 )
-from scenic.core.lazy_eval import LazilyEvaluable, isLazy, needsLazyEvaluation
+from scenic.core.lazy_eval import (
+    LazilyEvaluable,
+    isLazy,
+    needsLazyEvaluation,
+    valueInContext,
+)
 from scenic.core.regions import (
     BoxRegion,
     CircularRegion,
     EmptyRegion,
     IntersectionRegion,
     MeshSurfaceRegion,
     MeshVolumeRegion,
@@ -110,57 +116,91 @@
         super().__init_subclass__()
 
         if "_defaults" in cls.__dict__:
             # This class is being unpickled by value; the pickled class already was
             # transformed by __init_subclass__, so we skip it now.
             return
 
+        # Identify cached properties/methods which will need to be cleared
+        # each time step during dynamic simulations.
+        clearers = {}
+        for attr, value in cls.__dict__.items():
+            if isinstance(value, property):
+                value = value.fget
+            if clearer := getattr(value, "_scenic_cache_clearer", None):
+                clearers[attr] = clearer
+        for sc in cls.__mro__:
+            if sclearers := getattr(sc, "_cache_clearers", None):
+                for attr, clearer in sclearers.items():
+                    if attr not in clearers:
+                        clearers[attr] = clearer
+        cls._cache_clearers = clearers
+
         # Find all defaults provided by the class or its superclasses
         allDefs = collections.defaultdict(list)
 
         for sc in cls.__mro__:
             if issubclass(sc, Constructible) and hasattr(sc, "_scenic_properties"):
                 for prop, value in sc._scenic_properties.items():
                     allDefs[prop].append(PropertyDefault.forValue(value))
 
         # Resolve conflicting defaults and gather dynamic properties
         resolvedDefs = {}
         dyns = []
         finals = []
+        dynFinals = {}
         for prop, defs in allDefs.items():
             primary, rest = defs[0], defs[1:]
             spec = primary.resolveFor(prop, rest)
             resolvedDefs[prop] = spec
 
-            if any(defn.isDynamic for defn in defs):
+            if isDynamic := any(defn.isDynamic for defn in defs):
                 dyns.append(prop)
             if primary.isFinal:
                 finals.append(prop)
+                if isDynamic:
+                    dynFinals[prop] = primary.value
         cls._defaults = resolvedDefs
-        cls._finalProperties = tuple(finals)
+        cls._finalProperties = frozenset(finals)
 
         # Determine types of dynamic properties
         dynTypes = {}
-        inst = None
+        defaultValues = None  # compute only if necessary
         for prop in dyns:
             ty = super(cls, cls)._dynamicProperties.get(prop)
             if not ty:
-                # First time this property has been defined; create a dummy object to
-                # run specifier resolution and determine the property's default value
-                if not inst:
-                    inst = cls._withSpecifiers((), register=False)
-                ty = underlyingType(getattr(inst, prop))
+                # First time this property has been defined; get the type of
+                # its default value.
+                if not defaultValues:
+                    # N.B. Here we evaluate the default value expressions, which is
+                    # risky since global state like the workspace may not have been set
+                    # up yet. For this reason we only compute default values when they
+                    # are actually needed; a better solution would be to have syntax for
+                    # annotating the types of dynamic properties.
+                    defaultValues, _ = cls._resolveSpecifiers(())
+                ty = underlyingType(defaultValues[prop])
             dynTypes[prop] = ty
         cls._dynamicProperties = dynTypes
         cls._simulatorProvidedProperties = {
             prop: val
             for prop, val in cls._dynamicProperties.items()
             if prop not in cls._finalProperties
         }
 
+        # Extract order in which to recompute dynamic final properties each time step
+        if defaultValues:
+            recomputers = {}
+            for prop in defaultValues:  # order is that from specifier resolution
+                if prop in dynFinals:
+                    recomputers[prop] = dynFinals[prop]
+            cls._dynamicFinalProperties = recomputers
+        else:
+            # No new dynamic properties: just inherit the order from the superclass
+            pass
+
     def __new__(cls, *args, _internal=False, **kwargs):
         if not _internal:
             # Catch users trying to instantiate a Scenic class like a Python class
             raise InvalidScenarioError('Scenic classes must be instantiated with "new"')
         return super().__new__(cls)
 
     def __getnewargs_ex__(self):
@@ -404,14 +444,22 @@
         properties = LazilyEvaluable.getContextValues(context)
 
         constProps = frozenset(
             {prop for prop in _defaultedProperties if not needsSampling(properties[prop])}
         )
         return properties, constProps
 
+    def _recomputeDynamicFinals(self):
+        # Evaluate default value expression for each dynamic final property
+        # and assign the obtained value
+        for prop, recomputer in self._dynamicFinalProperties.items():
+            rawVal = recomputer(self)
+            value = valueInContext(rawVal, self)
+            self._specify(self, prop, value)
+
     @classmethod
     def _specify(cls, context, prop, value):
         # Normalize types of some built-in properties
         if prop in (
             "position",
             "velocity",
             "cameraOffset",
@@ -445,14 +493,17 @@
 
         if prop == "color" and value is not None and not isLazy(value):
             if any(not (0 <= v <= 1) for v in value):
                 raise ValueError(
                     "Color property contains value not between 0 and 1 (inclusive)."
                 )
 
+            if not 3 <= len(value) <= 4:
+                raise ValueError(f"Color property has incorrect length {len(value)}.")
+
         object.__setattr__(context, prop, value)
 
     def _register(self):
         import scenic.syntax.veneer as veneer  # TODO improve?
 
         veneer.registerInstance(self)
 
@@ -500,20 +551,24 @@
 
     def _copyWith(self, **overrides):
         """Copy this object, possibly overriding some of its properties."""
         # Copy all properties except for final values, which will retain their default values
         props = {
             prop: val
             for prop, val in self._allProperties().items()
-            if prop not in set(self._finalProperties)
+            if prop not in self._finalProperties
         }
         props.update(overrides)
         constProps = self._constProps.difference(overrides)
         return self._withProperties(props, constProps=constProps)
 
+    def _clearCaches(self):
+        for clearer in self._cache_clearers.values():
+            clearer(self)
+
     def dumpAsScenicCode(self, stream, skipConstProperties=True):
         stream.write(f"new {self.__class__.__name__}")
         first = True
         for prop in self.properties:
             if skipConstProperties and prop in self._constProps:
                 continue
             if prop in self._finalProperties:
@@ -554,23 +609,23 @@
     control the effect of the :keyword:`mutate` statement. When mutation is enabled
     for such an object using that statement, the mutator's `appliedTo` method
     is called to compute a mutated version. The `appliedTo` method can also decide
     whether to apply mutators inherited from superclasses.
     """
 
     def appliedTo(self, obj):
-        """Return a mutated copy of the given object. Implemented by subclasses.
+        """Return a mutated version of the given object. Implemented by subclasses.
 
         The mutator may inspect the ``mutationScale`` attribute of the given object
         to scale its effect according to the scale given in ``mutate O by S``.
 
         Returns:
-            A pair consisting of the mutated copy of the object (which is most easily
-            created using `_copyWith`) together with a Boolean indicating whether the
-            mutator inherited from the superclass (if any) should also be applied.
+            A pair consisting of the mutated version of the object together with a
+            Boolean indicating whether the mutator inherited from the superclass
+            (if any) should also be applied.
         """
         raise NotImplementedError
 
 
 class PositionMutator(Mutator):
     """Mutator adding Gaussian noise to ``position``. Used by `Point`.
 
@@ -583,16 +638,16 @@
 
     def appliedTo(self, obj):
         noise = Vector(
             random.gauss(0, self.stddevs[0] * obj.mutationScale),
             random.gauss(0, self.stddevs[1] * obj.mutationScale),
             random.gauss(0, self.stddevs[2] * obj.mutationScale),
         )
-        pos = obj.position + noise
-        return (obj._copyWith(position=pos), True)  # allow further mutation
+        obj.position += noise
+        return (obj, True)  # allow further mutation
 
     def __eq__(self, other):
         if type(other) is not type(self):
             return NotImplemented
         return other.stddevs == self.stddevs
 
     def __hash__(self):
@@ -606,21 +661,19 @@
         stddevs (tuple[float,float,float]): standard deviation of noise for each angle (yaw, pitch, roll).
     """
 
     def __init__(self, stddevs):
         self.stddevs = tuple(stddevs)
 
     def appliedTo(self, obj):
-        yaw = obj.yaw + random.gauss(0, self.stddevs[0] * obj.mutationScale)
-        pitch = obj.pitch + random.gauss(0, self.stddevs[1] * obj.mutationScale)
-        roll = obj.roll + random.gauss(0, self.stddevs[2] * obj.mutationScale)
+        obj.yaw += random.gauss(0, self.stddevs[0] * obj.mutationScale)
+        obj.pitch += random.gauss(0, self.stddevs[1] * obj.mutationScale)
+        obj.roll += random.gauss(0, self.stddevs[2] * obj.mutationScale)
 
-        new_obj = obj._copyWith(yaw=yaw, pitch=pitch, roll=roll)
-
-        return (new_obj, True)  # allow further mutation
+        return (obj, True)  # allow further mutation
 
     def __eq__(self, other):
         if type(other) is not type(self):
             return NotImplemented
         return other.stddevs == self.stddevs
 
     def __hash__(self):
@@ -744,40 +797,36 @@
         if value[self.mutationScale] != 0:
             for mutator in self.mutator:
                 if mutator is None:
                     continue
                 sample, proceed = mutator.appliedTo(sample)
                 if not proceed:
                     break
+            sample._recomputeDynamicFinals()
         return sample
 
     # Points automatically convert to Vectors when needed
     def __getattr__(self, attr):
         if hasattr(Vector, attr):
             return getattr(self.toVector(), attr)
         else:
-            raise AttributeError(
-                f"'{type(self).__name__}' object has no attribute '{attr}'"
-            )
+            self.__getattribute__(attr)
 
 
 ## OrientedPoint
 
 
 class OrientedPoint(Point):
     """The Scenic class ``OrientedPoint``.
 
-    The default mutator for `OrientedPoint` adds Gaussian noise to ``yaw`` while
-    leaving ``pitch`` and ``roll`` unchanged, using the three standard deviations
-    (for yaw/pitch/roll respectively) given by the  ``orientationStdDev`` property.
-    It then also applies the mutator for `Point`.
-
     The default mutator for `OrientedPoint` adds Gaussian noise to ``yaw``, ``pitch``
-    and ``roll`` according to ``orientationStdDev``. By default the standard deviations
-    for ``pitch`` and ``roll`` are zero so that, by default, only ``yaw`` is mutated.
+    and ``roll``, using the three standard deviations (for yaw/pitch/roll respectively)
+    given by the  ``orientationStdDev`` property. It then also applies the mutator for `Point`.
+    By default the standard deviations for ``pitch`` and ``roll`` are zero so that, by
+    default, only ``yaw`` is mutated.
 
     Properties:
         yaw (float; dynamic): Yaw of the `OrientedPoint` in radians in the local coordinate system
           provided by :prop:`parentOrientation`. Default value 0.
         pitch (float; dynamic): Pitch of the `OrientedPoint` in radians in the local coordinate system
           provided by :prop:`parentOrientation`. Default value 0.
         roll (float; dynamic): Roll of the `OrientedPoint` in radians in the local coordinate system
@@ -804,27 +853,29 @@
         "pitch": PropertyDefault((), {"dynamic"}, lambda self: 0),
         "roll": PropertyDefault((), {"dynamic"}, lambda self: 0),
         "parentOrientation": globalOrientation,
         "orientation": PropertyDefault(
             {"yaw", "pitch", "roll", "parentOrientation"},
             {"dynamic", "final"},
             lambda self: (
-                Orientation.fromEuler(self.yaw, self.pitch, self.roll)
-                * self.parentOrientation
+                self.parentOrientation
+                * Orientation.fromEuler(self.yaw, self.pitch, self.roll)
             ),
         ),
         # Heading is equal to orientation.yaw, which is equal to self.yaw if this OrientedPoint's
         # parentOrientation is the global orientation. Defined this way to simplify the value for pruning
         # purposes if possible.
         "heading": PropertyDefault(
             {"orientation"},
             {"dynamic", "final"},
-            lambda self: self.yaw
-            if alwaysGlobalOrientation(self.parentOrientation)
-            else self.orientation.yaw,
+            lambda self: (
+                self.yaw
+                if alwaysGlobalOrientation(self.parentOrientation)
+                else self.orientation.yaw
+            ),
         ),
         "viewAngle": math.tau,  # Primarily for backwards compatibility. Set viewAngles instead.
         "viewAngles": PropertyDefault(
             ("viewAngle",), set(), lambda self: (self.viewAngle, math.pi)
         ),
         "mutator": PropertyDefault(
             {"orientationStdDev"},
@@ -962,15 +1013,15 @@
         speed (float; dynamic): Speed in dynamic simulations. Default value 0.
         angularVelocity (`Vector`; *dynamic*):
         angularSpeed (float; dynamic): Angular speed in dynamic simulations. Default
           value 0.
         behavior: Behavior for dynamic agents, if any (see :ref:`dynamics`). Default
           value ``None``.
         lastActions: Tuple of :term:`actions` taken by this agent in the last time step
-          (or `None` if the object is not an agent or this is the first time step).
+          (an empty tuple if the object is not an agent or this is the first time step).
     """
 
     _scenic_properties = {
         "width": PropertyDefault(("shape",), {}, lambda self: self.shape.width),
         "length": PropertyDefault(("shape",), {}, lambda self: self.shape.length),
         "height": PropertyDefault(("shape",), {}, lambda self: self.shape.height),
         "shape": BoxShape(),
@@ -987,15 +1038,15 @@
         "showVisibleRegion": False,
         "color": None,
         "velocity": PropertyDefault((), {"dynamic"}, lambda self: Vector(0, 0, 0)),
         "speed": PropertyDefault((), {"dynamic"}, lambda self: 0),
         "angularVelocity": PropertyDefault((), {"dynamic"}, lambda self: Vector(0, 0, 0)),
         "angularSpeed": PropertyDefault((), {"dynamic"}, lambda self: 0),
         "behavior": None,
-        "lastActions": None,
+        "lastActions": tuple(),
         # weakref to scenario which created this object, for internal use
         "_parentScenario": None,
     }
 
     def __new__(cls, *args, **kwargs):
         obj = super().__new__(cls, *args, **kwargs)
         # The _dynamicProxy attribute stores a mutable copy of the object used during
@@ -1062,30 +1113,52 @@
     @cached_method
     def distanceTo(self, point):
         """The minimal distance from the space this object occupies to a given point"""
         return self.occupiedSpace.distanceTo(point)
 
     @cached_method
     def intersects(self, other):
-        """Whether or not this object intersects another object"""
-        # For objects that are boxes and flat, we can take a fast route
-        if self._isPlanarBox and other._isPlanarBox:
+        """Whether or not this object intersects another object or region"""
+        ## Type Checking ##
+        if not isinstance(other, (Object, Region)):
+            raise TypeError(
+                f"Cannot compute intersection of Scenic Object with {type(other)}."
+            )
+
+        ## Heuristic Fast Paths ##
+        # For two objects that are boxes and flat, we can take a fast route
+        if self._isPlanarBox and (isinstance(other, Object) and other._isPlanarBox):
             if abs(self.position.z - other.position.z) > (self.height + other.height) / 2:
                 return False
 
             self_poly = self._boundingPolygon
             other_poly = other._boundingPolygon
             return self_poly.intersects(other_poly)
 
-        if isLazy(self.occupiedSpace) or isLazy(other.occupiedSpace):
+        # For an object that is a box and flat with a polygonal region, we can
+        # also take a fast route.
+        if self._isPlanarBox and (
+            isinstance(other, PolygonalRegion)
+            and abs(self.position.z - other.z) <= self.height / 2
+        ):
+            return self._boundingPolygon.intersects(other.polygons)
+
+        ## Default Case
+        # Extract other's occupied space if it's an object
+        if isinstance(other, Object):
+            other_occupied_space = other.occupiedSpace
+        else:
+            other_occupied_space = other
+
+        if isLazy(self.occupiedSpace) or isLazy(other_occupied_space):
             raise RandomControlFlowError(
                 "Cannot compute intersection between Objects with non-fixed values."
             )
 
-        return self.occupiedSpace.intersects(other.occupiedSpace)
+        return self.occupiedSpace.intersects(other_occupied_space)
 
     @cached_property
     def left(self):
         return self.relativize(Vector(-self.hw, 0))
 
     @cached_property
     def right(self):
@@ -1219,19 +1292,23 @@
             self.relativePosition(Vector(-hw, -hl)),
             self.relativePosition(Vector(hw, -hl)),
         )
 
     @cached_property
     def occupiedSpace(self):
         """A region representing the space this object occupies"""
+        shape = self.shape
         return MeshVolumeRegion(
-            mesh=self.shape.mesh,
+            mesh=shape.mesh,
             dimensions=(self.width, self.length, self.height),
             position=self.position,
             rotation=self.orientation,
+            centerMesh=False,
+            _internal=True,
+            _isConvex=shape.isConvex,
         )
 
     @property
     def _isConvex(self):
         """Whether this object's shape is convex"""
         return self.shape.isConvex
 
@@ -1251,75 +1328,133 @@
     def boundingBox(self):
         """A region representing this object's bounding box"""
         return MeshVolumeRegion(self.occupiedSpace.mesh.bounding_box, centerMesh=False)
 
     @cached_property
     def inradius(self):
         """A lower bound on the inradius of this object"""
-        # First check if all needed variables are defined. If so, we can
-        # compute the inradius exactly.
-        width, length, height = self.width, self.length, self.height
-        shape = self.shape
-        if not any(needsSampling(val) for val in (width, length, height, shape)):
-            shapeRegion = MeshVolumeRegion(
+
+        # Define a helper function that computes the support of the inradius,
+        # given the sub supports.
+        def inradiusSupport(width_s, length_s, height_s, shape_s):
+            # Unpack the dimension supports (and ignore the shape support)
+            min_width, max_width = width_s
+            min_length, max_length = length_s
+            min_height, max_height = height_s
+
+            if None in [
+                min_width,
+                max_width,
+                min_length,
+                max_length,
+                min_height,
+                max_height,
+            ]:
+                # Can't get a bound on one or more dimensions, abort
+                return None, None
+
+            min_bounds = np.array([min_width, min_length, min_height])
+            max_bounds = np.array([max_width, max_length, max_height])
+
+            # Extract a list of possible shapes
+            if isinstance(self.shape, Shape):
+                shapes = [self.shape]
+            elif isinstance(self.shape, MultiplexerDistribution) and all(
+                isinstance(opt, Shape) for opt in self.shape.options
+            ):
+                shapes = self.shape.options
+            else:
+                # Something we don't recognize, abort
+                return None, None
+
+            # Get the inradius for each shape with the min and max bounds
+            min_distances = [
+                MeshVolumeRegion(mesh=shape.mesh, dimensions=min_bounds).inradius
+                for shape in shapes
+            ]
+            max_distances = [
+                MeshVolumeRegion(mesh=shape.mesh, dimensions=max_bounds).inradius
+                for shape in shapes
+            ]
+
+            distance_range = (min(min_distances), max(max_distances))
+
+            return distance_range
+
+        # Define a helper function that computes the actual inradius
+        @distributionFunction(support=inradiusSupport)
+        def inradiusActual(width, length, height, shape):
+            return MeshVolumeRegion(
                 mesh=shape.mesh, dimensions=(width, length, height)
-            )
-            return shapeRegion.inradius
+            ).inradius
+
+        # Return the inradius (possibly a distribution) with proper support information
+        return inradiusActual(self.width, self.length, self.height, self.shape)
+
+    @cached_property
+    def planarInradius(self):
+        """A lower bound on the planar inradius of this object.
 
-        # If we havea uniform distribution over shapes and a supportInterval for each dimension,
-        # we can compute a supportInterval for this object's inradius
+        This is defined as the inradius of the polygon of the occupiedSpace
+        of this object projected into the XY plane, assuming that pitch and
+        roll are both 0.
+        """
 
-        # Define helper class
-        class InradiusHelper:
-            def __init__(self, support):
-                self.support = support
-
-            def supportInterval(self):
-                return self.support
-
-        # Extract bounds on all dimensions
-        min_width, max_width = supportInterval(width)
-        min_length, max_length = supportInterval(length)
-        min_height, max_height = supportInterval(height)
-
-        if None in [min_width, max_width, min_length, max_length, min_height, max_height]:
-            # Can't get a bound on one or more dimensions, abort
-            return 0
-
-        min_bounds = np.array([min_width, min_length, min_height])
-        max_bounds = np.array([max_width, max_length, max_height])
-
-        # Extract a list of possible shapes
-        if isinstance(shape, Shape):
-            shapes = [shape]
-        elif isinstance(shape, MultiplexerDistribution):
-            if all(isinstance(opt, Shape) for opt in shape.options):
-                shapes = shape.options
+        # Define a helper function that computes the support of the inradius,
+        # given the sub supports.
+        def planarInradiusSupport(width_s, length_s, shape_s):
+            # Unpack the dimension supports (and ignore the shape support)
+            min_width, max_width = width_s
+            min_length, max_length = length_s
+
+            if None in [min_width, max_width, min_length, max_length]:
+                # Can't get a bound on one or more dimensions, abort
+                return None, None
+
+            min_bounds = np.array([min_width, min_length, 1])
+            max_bounds = np.array([max_width, max_length, 1])
+
+            # Extract a list of possible shapes
+            if isinstance(self.shape, Shape):
+                shapes = [self.shape]
+            elif isinstance(self.shape, MultiplexerDistribution) and all(
+                isinstance(opt, Shape) for opt in self.shape.options
+            ):
+                shapes = self.shape.options
             else:
                 # Something we don't recognize, abort
-                return 0
+                return None, None
 
-        # Check that all possible shapes contain the origin
-        if not all(shape.containsCenter for shape in shapes):
-            # One or more shapes has inradius 0
-            return 0
-
-        # Get the inradius for each shape with the min and max bounds
-        min_distances = [
-            MeshVolumeRegion(mesh=shape.mesh, dimensions=min_bounds).inradius
-            for shape in shapes
-        ]
-        max_distances = [
-            MeshVolumeRegion(mesh=shape.mesh, dimensions=max_bounds).inradius
-            for shape in shapes
-        ]
+            # Get the inradius of the projected for each shape with the min and max bounds
+            min_distances = [
+                MeshVolumeRegion(
+                    mesh=shape.mesh, dimensions=min_bounds
+                ).boundingPolygon.inradius
+                for shape in shapes
+            ]
+            max_distances = [
+                MeshVolumeRegion(
+                    mesh=shape.mesh, dimensions=max_bounds
+                ).boundingPolygon.inradius
+                for shape in shapes
+            ]
 
-        distance_range = (min(min_distances), max(max_distances))
+            distance_range = (min(min_distances), max(max_distances))
 
-        return InradiusHelper(support=distance_range)
+            return distance_range
+
+        # Define a helper function that computes the actual planarInradius
+        @distributionFunction(support=planarInradiusSupport)
+        def planarInradiusActual(width, length, shape):
+            return MeshVolumeRegion(
+                mesh=shape.mesh, dimensions=(width, length, 1)
+            ).boundingPolygon.inradius
+
+        # Return the planar inradius (possibly a distribution) with proper support information
+        return planarInradiusActual(self.width, self.length, self.shape)
 
     @cached_property
     def surface(self):
         """A region containing the entire surface of this object"""
         return self.occupiedSpace.getSurfaceRegion()
 
     @cached_property
@@ -1417,15 +1552,23 @@
 
         # Render the object
         object_mesh = self.occupiedSpace.mesh.copy()
 
         if highlight:
             object_mesh.visual.face_colors = [30, 179, 0, 255]
         elif self.color is not None:
-            object_mesh.visual.face_colors = self.color
+            if len(self.color) == 3:
+                r, g, b = self.color
+                a = 1
+            elif len(self.color) == 4:
+                r, g, b, a = self.color
+            else:
+                assert False
+
+            object_mesh.visual.face_colors = [255 * r, 255 * g, 255 * b, 255 * a]
 
         viewer.add_geometry(object_mesh)
 
         if self.showVisibleRegion:
             view_region_mesh = self.visibleRegion.mesh
 
             edges = view_region_mesh.face_adjacency_edges[
@@ -1617,21 +1760,24 @@
     _3DClass = OrientedPoint
 
     def __init_subclass__(cls):
         if cls.__dict__.get("_props_transformed", False):
             # Can get here when cls is unpickled (the transformed version was pickled)
             pass
         else:
-            cls._props_transformed = True
+            # Mark class as being transformed.
+            # To work around https://github.com/uqfoundation/dill/issues/612,
+            # use a different truthy value for each class.
+            cls._props_transformed = str(cls)
+
             props = cls._scenic_properties
-            # Raise error if parentOrientation already defined
-            if "parentOrientation" in props:
+            # Raise error if parentOrientation and heading already defined
+            if "parentOrientation" in props and "heading" in props:
                 raise RuntimeError(
-                    "this scenario cannot be run with the --2d flag (the "
-                    f'{cls.__name__} class defines "parentOrientation")'
+                    f'{cls.__name__} defines both "parentOrientation" and "heading"'
                 )
 
             # Map certain properties to their 3D analog
             if "heading" in props:
                 props["parentOrientation"] = props["heading"]
                 del props["heading"]
```

### Comparing `scenic-3.0.0b2/src/scenic/core/propositions.py` & `scenic-3.0.0rc1/src/scenic/core/propositions.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/core/pruning.py` & `scenic-3.0.0rc1/src/scenic/core/pruning.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,62 @@
 """Pruning parts of the sample space which violate requirements.
 
 The top-level function here, `prune`, is called as the very last step of scenario
 compilation (from `translator.constructScenarioFrom`).
 """
 
 import builtins
+import collections
 import math
 import time
 
+import numpy
 import shapely.geometry
 import shapely.geos
+from trimesh.transformations import translation_matrix
 
 from scenic.core.distributions import (
     AttributeDistribution,
     FunctionDistribution,
     MethodDistribution,
     OperatorDistribution,
     Samplable,
+    dependencies,
     needsSampling,
     supportInterval,
     underlyingFunction,
 )
 from scenic.core.errors import InvalidScenarioError
 from scenic.core.geometry import hypot, normalizeAngle, plotPolygon, polygonUnion
 from scenic.core.object_types import Object, Point
 import scenic.core.regions as regions
-from scenic.core.regions import EmptyRegion, MeshSurfaceRegion, MeshVolumeRegion
+from scenic.core.regions import (
+    EmptyRegion,
+    MeshSurfaceRegion,
+    MeshVolumeRegion,
+    PolygonalRegion,
+    Region,
+    VoxelRegion,
+)
 from scenic.core.type_support import TypecheckedDistribution
 from scenic.core.vectors import (
     PolygonalVectorField,
+    Vector,
     VectorField,
     VectorMethodDistribution,
     VectorOperatorDistribution,
 )
 from scenic.core.workspaces import Workspace
 from scenic.syntax.relations import DistanceRelation, RelativeHeadingRelation
 
-### Utilities
+### Constants
+PRUNING_PITCH = 0.15
 
 
+### Utilities
 def currentPropValue(obj, prop):
     """Get the current value of an object's property, taking into account prior pruning."""
     value = getattr(obj, prop)
     return value._conditioned if isinstance(value, Samplable) else value
 
 
 def isMethodCall(thing, method):
@@ -55,44 +69,45 @@
 def isFunctionCall(thing, function):
     """Match calls to a given function, taking into account distribution decorators."""
     if not isinstance(thing, FunctionDistribution):
         return False
     return thing.function is underlyingFunction(function)
 
 
+def unpackWorkspace(reg):
+    if isinstance(reg, Workspace):
+        return reg.region
+    else:
+        return reg
+
+
 def matchInRegion(position):
     """Match uniform samples from a `Region`
 
-    Returns the Region, if any, and a lower and upper bound
-    on the distance the object will be placed along with any
-    offset that should be added to the base.
+    Returns the Region, if any, the offset that should be added to the base, and
+    the PointInRegionDistribution itself.
     """
     # Case 1: Position is simply a point in a region
     if isinstance(position, regions.PointInRegionDistribution):
-        reg = position.region
-        if isinstance(reg, Workspace):
-            reg = reg.region
-        return reg, 0, 0, None
+        reg = unpackWorkspace(position.region)
+        return reg, None, position
 
     # Case 2: Position is a point in a region with a vector offset.
     if isinstance(position, VectorOperatorDistribution) and position.operator in (
         "__add__",
         "__radd__",
     ):
         if isinstance(position.object, regions.PointInRegionDistribution):
-            reg = position.object.region
+            reg = unpackWorkspace(position.object.region)
             assert len(position.operands) == 1
             offset = position.operands[0]
-            # TODO: Proper vector supportInterval calculations. Right now this gives us None
-            # if value is not exact
-            lower, upper = supportInterval(offset.norm())
 
-            return reg, lower, upper, offset
+            return reg, offset, position.object
 
-    return None, 0, 0, None
+    return None, None, None
 
 
 def matchPolygonalField(heading, position):
     """Match orientation yaw defined by a `PolygonalVectorField` at the given position.
 
     Matches the yaw attribute of orientations exactly equal to a `PolygonalVectorField`,
     or offset by a bounded disturbance. Returns a triple consisting of the matched field
@@ -151,34 +166,33 @@
     """
     if verbosity >= 1:
         print("  Pruning scenario...")
         startTime = time.time()
 
     pruneContainment(scenario, verbosity)
     pruneRelativeHeading(scenario, verbosity)
+    pruneVisibility(scenario, verbosity)
 
     if verbosity >= 1:
         totalTime = time.time() - startTime
         print(f"  Pruned scenario in {totalTime:.4g} seconds.")
 
 
 ## Pruning based on containment
-
-
 def pruneContainment(scenario, verbosity):
     """Prune based on the requirement that individual Objects fit within their container.
 
     Specifically, if O is positioned uniformly (with a possible offset) in region B and
     has container C, then we can instead pick a position uniformly in their intersection.
     If we can also lower bound the radius of O, then we can first erode C by that distance
     minus that maximum offset distance.
     """
     for obj in scenario.objects:
         # Extract the base region and container region, while doing minor checks.
-        base, _, maxDistance, offset = matchInRegion(obj.position)
+        base, offset, _ = matchInRegion(obj.position)
 
         if base is None or needsSampling(base):
             continue
 
         if isinstance(base, regions.EmptyRegion):
             raise InvalidScenarioError(f"Object {obj} placed in empty region")
 
@@ -186,74 +200,116 @@
 
         if container is None or needsSampling(container):
             continue
 
         if isinstance(container, regions.EmptyRegion):
             raise InvalidScenarioError(f"Object {obj} contained in empty region")
 
-        # Erode the container region if possible.
-        minRadius, _ = supportInterval(obj.inradius)
+        # Compute the maximum distance the object can be from the sampled point
+        if offset is not None:
+            # TODO: Support interval doesn't really work here for random values.
+            if isinstance(base, PolygonalRegion):
+                # Special handling for 2D regions that ignores vertical component of offset
+                offset_2d = Vector(offset.x, offset.y, 0)
+                _, maxDistance = supportInterval(offset_2d.norm())
+            else:
+                _, maxDistance = supportInterval(offset.norm())
+        else:
+            maxDistance = 0
 
+        # Compute the minimum radius of the object, with respect to the
+        # bounded dimensions of the container.
         if (
-            hasattr(container, "buffer")
-            and maxDistance is not None
+            isinstance(base, PolygonalRegion)
+            and supportInterval(obj.pitch) == (0, 0)
+            and supportInterval(obj.roll) == (0, 0)
+        ):
+            # Special handling for 2D regions with no pitch or roll,
+            # using planar inradius instead.
+            minRadius, _ = supportInterval(obj.planarInradius)
+        else:
+            # For most regions, use full object inradius.
+            minRadius, _ = supportInterval(obj.inradius)
+
+        # Erode the container if possible and productive
+        if (
+            maxDistance is not None
             and minRadius is not None
+            and (maxErosion := minRadius - maxDistance) > 0
         ):
-            maxErosion = minRadius - maxDistance
-            if maxErosion > 0:
+            if hasattr(container, "buffer"):
+                # We can do an exact erosion
                 container = container.buffer(-maxErosion)
+            elif isinstance(container, MeshVolumeRegion):
+                current_pitch = PRUNING_PITCH
+                eroded_container = None
+
+                while eroded_container is None:
+                    # We can attempt to erode a voxel approximation of the MeshVolumeRegion.
+                    eroded_container = container._erodeOverapproximate(
+                        maxErosion, PRUNING_PITCH
+                    )
+
+                    if isinstance(eroded_container, VoxelRegion):
+                        eroded_container = eroded_container.mesh
 
-        # Restrict the base region to the container, unless
+                    current_pitch = min(2 * current_pitch, 1)
+
+                # Now check if this erosion is valid and useful, i.e. do we have less volume
+                # to sample from. If so, replace the original container.
+                if (
+                    eroded_container is not None
+                    and eroded_container.size < container.size
+                ):
+                    container = eroded_container
+
+        # Restrict the base region to the possibly eroded container, unless
         # they're the same in which case we're done
         if base is container:
             continue
 
         newBase = base.intersect(container)
         newBase.orientation = base.orientation
 
         # Check if base was a volume and newBase is a surface,
         # in which case the mesh operation might be undefined and we abort.
         if isinstance(base, MeshVolumeRegion) and isinstance(newBase, MeshSurfaceRegion):
             continue
 
+        # Check newBase properties
         if isinstance(newBase, EmptyRegion):
             raise InvalidScenarioError(f"Object {obj} does not fit in container")
 
-        if verbosity >= 1:
-            if (
-                base.dimensionality is None
-                or newBase.dimensionality is None
-                or base.dimensionality != newBase.dimensionality
-            ):
+        percentage_pruned = percentagePruned(base, newBase)
+
+        if percentage_pruned is None:
+            if verbosity >= 1:
                 print(
                     f"    Region containment constraint pruning attempted but could not compute percentage for {base} and {newBase}."
                 )
-            elif base.dimensionality == newBase.dimensionality:
-                ratio = newBase.size / base.size
-                percent = max(0, 100 * (1.0 - ratio))
-
-                if percent <= 0.001:
-                    # We didn't really prune anything, don't bother setting new position
-                    continue
+        else:
+            if percentage_pruned <= 0.001:
+                # We didn't really prune anything, don't bother setting new position
+                continue
 
+            if verbosity >= 1:
                 print(
-                    f"    Region containment constraint pruned {percent:.1f}% of space."
+                    f"    Region containment constraint pruned {percentage_pruned:.1f}% of space."
                 )
 
+        # Condition object to pruned position
         newPos = regions.Region.uniformPointIn(newBase)
 
         if offset is not None:
             newPos += offset
 
         obj.position.conditionTo(newPos)
 
 
 ## Pruning based on orientation
-
-
 def pruneRelativeHeading(scenario, verbosity):
     """Prune based on requirements bounding the relative heading of an Object.
 
     Specifically, if an object O is:
 
         * positioned uniformly within a polygonal region B;
         * aligned to a polygonal vector field F (up to a bounded offset);
@@ -275,15 +331,15 @@
         field, offsetL, offsetR = matchPolygonalField(obj.heading, obj.position)
         if field is not None:
             fields[obj] = (field, offsetL, offsetR)
 
     # Check for relative heading relations among such objects
     for obj, (field, offsetL, offsetR) in fields.items():
         position = currentPropValue(obj, "position")
-        base, _, _, offset = matchInRegion(position)
+        base, offset, _ = matchInRegion(position)
 
         # obj must be positioned uniformly in a Region
         if base is None or needsSampling(base):
             continue
 
         if offset is not None:
             continue
@@ -329,14 +385,142 @@
             newBase = regions.PolygonalRegion(
                 polygon=newBasePoly, orientation=base.orientation
             )
             newPos = regions.Region.uniformPointIn(newBase)
             obj.position.conditionTo(newPos)
 
 
+# Pruning based on visibility
+def pruneVisibility(scenario, verbosity):
+    ego = scenario.egoObject
+
+    for obj in scenario.objects:
+        # Extract the base region if it exists
+        position = currentPropValue(obj, "position")
+        base, offset, pir_dist = matchInRegion(position)
+
+        # Compute the maximum distance the object can be from the sampled point
+        if offset is not None:
+            _, maxDistance = supportInterval(offset.norm())
+        else:
+            maxDistance = 0
+
+        if (
+            base is None
+            or needsSampling(base)
+            or needsSampling(obj.radius)
+            or maxDistance is None
+        ):
+            continue
+
+        currBase = base
+        currDist = pir_dist
+        currPos = position
+
+        # Define a helper function to attempt to buffer an observer's visibleRegion, resulting
+        # in a region that contains all points that could feasibly be the position
+        # of obj, if it is visible from the observer. If possible buffer exactly, otherwise
+        # try to buffer approximately, and if that is also not feasible just return the viewRegion.
+        def bufferHelper(viewRegion):
+            buffer_quantity = obj.radius + maxDistance
+            if hasattr(viewRegion, "buffer"):
+                return viewRegion.buffer(buffer_quantity)
+            elif hasattr(viewRegion, "_bufferOverapproximate"):
+                if needsSampling(viewRegion):
+                    return viewRegion._bufferOverapproximate(buffer_quantity, 1)
+                else:
+                    current_pitch = PRUNING_PITCH
+                    buffered_container = None
+
+                    while buffered_container is None:
+                        buffered_container = viewRegion._bufferOverapproximate(
+                            buffer_quantity, current_pitch
+                        )
+
+                        if isinstance(buffered_container, VoxelRegion):
+                            buffered_container = buffered_container.mesh
+
+                        current_pitch = min(2 * current_pitch, 1)
+
+                    assert buffered_container is not None
+
+                    return buffered_container
+            else:
+                assert False
+
+        # Prune based off visibility/non-visibility requirements
+        if obj.requireVisible and obj is not ego:
+            # We can restrict the base region to the buffered visible region
+            # of the ego.
+            if verbosity >= 1:
+                print(
+                    f"    Pruning restricted base region of {obj} to visible region of ego."
+                )
+            candidateBase = currBase.intersect(bufferHelper(ego.visibleRegion))
+            candidateDist = regions.Region.uniformPointIn(candidateBase)
+
+            # Condition object to pruned position
+            if offset is not None:
+                candidatePos = candidateDist + offset
+            else:
+                candidatePos = candidateDist
+
+            if not checkConditionedCycle(candidatePos, currPos):
+                currBase = candidateBase
+                currDist = candidateDist
+                if offset is not None:
+                    currPos = currDist + offset
+                else:
+                    currPos = currDist
+
+        if obj._observingEntity:
+            # We can restrict the base region to the buffered visible region
+            # of the observing entity.
+            if verbosity >= 1:
+                print(
+                    f"    Pruning restricted base region of {obj} to visible region of {obj._observingEntity}."
+                )
+            candidateBase = currBase.intersect(
+                bufferHelper(obj._observingEntity.visibleRegion)
+            )
+            candidateDist = regions.Region.uniformPointIn(candidateBase)
+
+            if not checkConditionedCycle(candidateDist, currDist):
+                currBase = candidateBase
+                currDist = candidateDist
+                if offset is not None:
+                    currPos = currDist + offset
+                else:
+                    currPos = currDist
+
+        # Check currBase properties
+        if isinstance(currBase, EmptyRegion):
+            raise InvalidScenarioError(
+                f"Object {obj} can not satisfy visibility/non-visibility constraints."
+            )
+
+        percentage_pruned = percentagePruned(base, currBase)
+
+        if percentage_pruned is None:
+            if verbosity >= 1:
+                print(
+                    f"    Visibility pruning attempted but could not compute percentage for {base} and {currBase}."
+                )
+        else:
+            if percentage_pruned <= 0.001:
+                # We didn't really prune anything, skip conditioning
+                continue
+
+            if verbosity >= 1:
+                print(f"    Visibility pruning pruned {percentage_pruned:.1f}% of space.")
+
+        # Condition position value to pruned position
+        obj.position.conditionTo(currPos)
+
+
 def maxDistanceBetween(scenario, obj, target):
     """Upper bound the distance between the given Objects."""
     # visDist is initialized to infinity. Then we can use
     # various visibility constraints to upper bound it,
     # keeping the tightest bound.
     ego = scenario.egoObject
     visDist = float("inf")
@@ -424,7 +608,55 @@
     tLower = normalizeAngle(targetHeading + tOffsetL)
     tUpper = normalizeAngle(targetHeading + tOffsetR)
     tPoints = [tLower, tUpper]
     if tUpper < tLower:
         tPoints.extend((math.pi, -math.pi))
     rhs = [tp - p for tp in tPoints for p in points]  # TODO improve
     return min(rhs), max(rhs)
+
+
+def percentagePruned(base, newBase):
+    if needsSampling(base) or needsSampling(newBase):
+        return None
+
+    if (
+        base.dimensionality
+        and newBase.dimensionality
+        and base.dimensionality == newBase.dimensionality
+    ):
+        ratio = newBase.size / base.size
+        percent = max(0, 100 * (1.0 - ratio))
+        return percent
+
+    return None
+
+
+def checkConditionedCycle(A, B):
+    """Returns true if A depends on B"""
+    if A is B:
+        return True
+
+    deps = set()
+    unseen_deps = conditionedDeps(A)
+
+    A = conditionedVal(A)
+    B = conditionedVal(B)
+
+    while unseen_deps:
+        target_dep = unseen_deps.pop()
+        new_deps = conditionedDeps(target_dep)
+
+        if target_dep is B or any(d is B for d in new_deps):
+            return True
+
+        unseen_deps += [d for d in new_deps if d not in deps]
+        deps.update(new_deps)
+
+    return False
+
+
+def conditionedDeps(samp):
+    return [conditionedVal(s) for s in dependencies(conditionedVal(samp))]
+
+
+def conditionedVal(samp):
+    return samp._conditioned if isinstance(samp, Samplable) else samp
```

### Comparing `scenic-3.0.0b2/src/scenic/core/regions.py` & `scenic-3.0.0rc1/src/scenic/core/regions.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 `trimesh <https://trimsh.org/>`_ package.
 """
 
 from abc import ABC, abstractmethod
 import itertools
 import math
 import random
-from subprocess import CalledProcessError
 import warnings
 
 import numpy
 import scipy
 import shapely
 import shapely.geometry
 from shapely.geometry import MultiPolygon
 import shapely.ops
 import trimesh
 from trimesh.transformations import (
-    concatenate_matrices,
+    compose_matrix,
+    identity_matrix,
     quaternion_matrix,
     translation_matrix,
 )
+import trimesh.voxel
 
 warnings.filterwarnings(
     "ignore", module="trimesh"
 )  # temporarily suppress annoying warnings
 
 from scenic.core.distributions import (
     RejectionException,
@@ -51,15 +52,15 @@
     pointIsInCone,
     polygonUnion,
     sin,
     triangulatePolygon,
 )
 from scenic.core.lazy_eval import isLazy, valueInContext
 from scenic.core.type_support import toOrientation, toScalar, toVector
-from scenic.core.utils import cached, cached_method, cached_property, loadMesh
+from scenic.core.utils import cached, cached_method, cached_property, unifyMesh
 from scenic.core.vectors import (
     Orientation,
     OrientedVector,
     Vector,
     VectorDistribution,
     VectorField,
 )
@@ -179,14 +180,22 @@
         elif isinstance(other, AllRegion):
             return nowhere
         return DifferenceRegion(self, other)
 
     def sampleGiven(self, value):
         return self
 
+    def _trueContainsPoint(self, point) -> bool:
+        """Whether or not this region could produce point when sampled.
+
+        By default this method calls `containsPoint`, but should be overwritten if
+        `containsPoint` does not properly represent the points that can be sampled.
+        """
+        return self.containsPoint(point)
+
     ## Generic Methods (not to be overriden by subclasses) ##
     @cached_method
     def containsRegion(self, reg, tolerance=0):
         # Default behavior for AllRegion and EmptyRegion
         if type(self) is AllRegion or type(reg) is EmptyRegion:
             return True
 
@@ -204,17 +213,17 @@
                 # same dimensionality.
                 if self.dimensionality == reg.dimensionality and self.size < reg.size:
                     return False
 
         return self.containsRegionInner(reg, tolerance)
 
     @staticmethod
-    def uniformPointIn(region):
+    def uniformPointIn(region, tag=None):
         """Get a uniform `Distribution` over points in a `Region`."""
-        return PointInRegionDistribution(region)
+        return PointInRegionDistribution(region, tag=tag)
 
     def __contains__(self, thing) -> bool:
         """Check if this `Region` contains an object or vector."""
         from scenic.core.object_types import Object
 
         if isinstance(thing, Object):
             return self.containsObject(thing)
@@ -240,17 +249,18 @@
             s += f" {self.name}"
         return s + f" at {hex(id(self))}>"
 
 
 class PointInRegionDistribution(VectorDistribution):
     """Uniform distribution over points in a Region"""
 
-    def __init__(self, region):
+    def __init__(self, region, tag=None):
         super().__init__(region)
         self.region = region
+        self.tag = tag
 
     def sampleGiven(self, value):
         return value[self.region].uniformPointInner()
 
     @property
     def heading(self):
         if self.region.orientation is not None:
@@ -459,40 +469,49 @@
         if not sampler:
             sampler = self.genericSampler
         return self.orient(sampler(self))
 
     @staticmethod
     def genericSampler(intersection):
         regs = intersection.regions
+        # Filter out all regions with known dimensionality greater than the minimum
+        known_dim_regions = [
+            r.dimensionality for r in regs if r.dimensionality is not None
+        ]
+        min_dim = min(known_dim_regions) if known_dim_regions else float("inf")
+        sampling_regions = [
+            r for r in regs if r.dimensionality is None or r.dimensionality <= min_dim
+        ]
 
-        # Get a candidate point from each region
-        points = []
-
+        # Try to sample a point from all sampling regions
         num_regs_undefined = 0
 
-        for reg in regs:
+        for reg in sampling_regions:
             try:
-                points.append(reg.uniformPointInner())
+                point = reg.uniformPointInner()
             except UndefinedSamplingException:
                 num_regs_undefined += 1
-                pass
+                continue
+            except RejectionException:
+                continue
 
-        if num_regs_undefined == len(regs):
+            if all(region._trueContainsPoint(point) for region in regs):
+                return point
+
+        # No points were successfully sampled.
+        # If all regions were undefined for sampling, raise the appropriate exception.
+        # Otherwise, reject.
+        if num_regs_undefined == len(sampling_regions):
             # All regions do not support sampling, so the
             # intersection doesn't either.
             raise UndefinedSamplingException(
-                f"All regions in {regs}"
+                f"All regions in {sampling_regions}"
                 " do not support sampling, so the intersection doesn't either."
             )
 
-        # Check each point for containment each region.
-        for point in points:
-            if all(region.containsPoint(point) for region in regs):
-                return point
-
         raise RejectionException(f"sampling intersection of Regions {regs}")
 
     def __repr__(self):
         return f"IntersectionRegion({self.regions!r})"
 
 
 class UnionRegion(Region):
@@ -562,15 +581,15 @@
         sampler = self.sampler
         if not sampler:
             sampler = self.genericSampler
         return self.orient(sampler(self))
 
     @staticmethod
     def genericSampler(union):
-        regs = intersection.regions
+        regs = union.regions
 
         # Check that all regions have well defined dimensionality
         if any(reg.dimensionality is None for reg in regs):
             raise UndefinedSamplingException(
                 f"cannot sample union of Regions {regs} with " "undefined dimensionality"
             )
 
@@ -586,15 +605,15 @@
 
         # Pick a sample, weighted by region size
         reg_sizes = tuple(reg.size for reg in large_regs)
         target_reg = random.choices(large_regs, weights=reg_sizes)[0]
         point = target_reg.uniformPointInner()
 
         # Potentially reject based on containment of the sample
-        containment_count = sum(int(reg.containsPoint(point)) for reg in regs)
+        containment_count = sum(int(reg._trueContainsPoint(point)) for reg in regs)
 
         if random.random() < 1 - 1 / containment_count:
             raise RejectionException("rejected sample from UnionRegion")
 
         return point
 
     def __repr__(self):
@@ -665,15 +684,15 @@
             sampler = self.genericSampler
         return self.orient(sampler(self))
 
     @staticmethod
     def genericSampler(difference):
         regionA, regionB = difference.regionA, difference.regionB
         point = regionA.uniformPointInner()
-        if regionB.containsPoint(point):
+        if regionB._trueContainsPoint(point):
             raise RejectionException(
                 f"sampling difference of Regions {regionA} and {regionB}"
             )
         return point
 
     def __repr__(self):
         return f"DifferenceRegion({self.regionA!r}, {self.regionB!r})"
@@ -764,42 +783,39 @@
         position: An optional position, which determines where the center of the region will be.
         rotation: An optional Orientation object which determines the rotation of the object in space.
         orientation: An optional vector field describing the preferred orientation at every point in
           the region.
         tolerance: Tolerance for internal computations.
         centerMesh: Whether or not to center the mesh after copying and before transformations.
         onDirection: The direction to use if an object being placed on this region doesn't specify one.
-        engine: Which engine to use for mesh operations. Either "blender" or "scad".
         additionalDeps: Any additional sampling dependencies this region relies on.
     """
 
     def __init__(
         self,
         mesh,
         dimensions=None,
         position=None,
         rotation=None,
         orientation=None,
         tolerance=1e-6,
         centerMesh=True,
         onDirection=None,
-        engine="blender",
         name=None,
         additionalDeps=[],
     ):
         # Copy parameters
         self._mesh = mesh
         self.dimensions = None if dimensions is None else toVector(dimensions)
         self.position = None if position is None else toVector(position)
         self.rotation = None if rotation is None else toOrientation(rotation)
         self.orientation = None if orientation is None else toDistribution(orientation)
         self.tolerance = tolerance
         self.centerMesh = centerMesh
         self.onDirection = onDirection
-        self.engine = engine
 
         # Initialize superclass with samplables
         super().__init__(
             name,
             self._mesh,
             self.dimensions,
             self.position,
@@ -809,68 +825,64 @@
         )
 
         # If our region isn't fixed yet, then compute other values later
         if isLazy(self):
             return
 
         # Convert extract mesh
-        if isinstance(mesh, trimesh.primitives._Primitive):
+        if isinstance(mesh, trimesh.primitives.Primitive):
             self._mesh = mesh.to_mesh()
         elif isinstance(mesh, trimesh.base.Trimesh):
             self._mesh = mesh.copy()
         else:
             raise TypeError(
                 f"Got unexpected mesh parameter of type {type(mesh).__name__}"
             )
 
         # Center mesh unless disabled
         if centerMesh:
             self.mesh.vertices -= self.mesh.bounding_box.center_mass
 
-        # If dimensions are provided, scale mesh to those dimension
+        # Apply scaling, rotation, and translation, if any
         if self.dimensions is not None:
-            scale = self.mesh.extents / numpy.array(self.dimensions)
-
-            scale_matrix = numpy.eye(4)
-            scale_matrix[:3, :3] /= scale
-
-            self.mesh.apply_transform(scale_matrix)
-
-        # If rotation is provided, apply rotation
+            scale = numpy.array(self.dimensions) / self.mesh.extents
+        else:
+            scale = None
         if self.rotation is not None:
-            rotation_matrix = quaternion_matrix(
-                (self.rotation.w, self.rotation.x, self.rotation.y, self.rotation.z)
-            )
-            self.mesh.apply_transform(rotation_matrix)
-
-        # If position is provided, translate mesh.
-        if self.position is not None:
-            position_matrix = translation_matrix(self.position)
-            self.mesh.apply_transform(position_matrix)
+            angles = self.rotation._trimeshEulerAngles()
+        else:
+            angles = None
+        matrix = compose_matrix(scale=scale, angles=angles, translate=self.position)
+        self.mesh.apply_transform(matrix)
 
         self.orientation = orientation
 
     @classmethod
-    def fromFile(cls, path, filetype=None, compressed=None, binary=False, **kwargs):
+    def fromFile(cls, path, unify=True, **kwargs):
         """Load a mesh region from a file, attempting to infer filetype and compression.
 
         For example: "foo.obj.bz2" is assumed to be a compressed .obj file.
         "foo.obj" is assumed to be an uncompressed .obj file. "foo" is an
         unknown filetype, so unless a filetype is provided an exception will be raised.
 
         Args:
             path (str): Path to the file to import.
             filetype (str): Filetype of file to be imported. This will be inferred if not provided.
                 The filetype must be one compatible with `trimesh.load`.
             compressed (bool): Whether or not this file is compressed (with bz2). This will be inferred
                 if not provided.
             binary (bool): Whether or not to open the file as a binary file.
+            unify (bool): Whether or not to attempt to unify this mesh.
             kwargs: Additional arguments to the MeshRegion initializer.
         """
-        mesh = loadMesh(path, filetype, compressed, binary)
+        mesh = trimesh.load(path, force="mesh")
+
+        if unify and issubclass(cls, MeshVolumeRegion):
+            mesh = unifyMesh(mesh, verbose=True)
+
         return cls(mesh=mesh, **kwargs)
 
     ## Lazy Construction Methods ##
     def sampleGiven(self, value):
         if isinstance(self, MeshVolumeRegion):
             cls = MeshVolumeRegion
         elif isinstance(self, MeshSurfaceRegion):
@@ -879,19 +891,22 @@
             assert False
 
         return cls(
             mesh=value[self._mesh],
             dimensions=value[self.dimensions],
             position=value[self.position],
             rotation=value[self.rotation],
-            orientation=value[self.orientation],
+            orientation=(
+                True
+                if self.__dict__.get("_usingDefaultOrientation", False)
+                else value[self.orientation]
+            ),
             tolerance=self.tolerance,
             centerMesh=self.centerMesh,
             onDirection=self.onDirection,
-            engine=self.engine,
             name=self.name,
         )
 
     def evaluateInner(self, context):
         if isinstance(self, MeshVolumeRegion):
             cls = MeshVolumeRegion
         elif isinstance(self, MeshSurfaceRegion):
@@ -899,26 +914,29 @@
         else:
             assert False
 
         mesh = valueInContext(self._mesh, context)
         dimensions = valueInContext(self.dimensions, context)
         position = valueInContext(self.position, context)
         rotation = valueInContext(self.rotation, context)
-        orientation = valueInContext(self.orientation, context)
+        orientation = (
+            True
+            if self.__dict__.get("_usingDefaultOrientation", False)
+            else valueInContext(self.orientation, context)
+        )
 
         return cls(
             mesh,
             dimensions,
             position,
             rotation,
             orientation,
             tolerance=self.tolerance,
             centerMesh=self.centerMesh,
             onDirection=self.onDirection,
-            engine=self.engine,
             name=self.name,
         )
 
     ## API Methods ##
     @property
     @distributionFunction
     def mesh(self):
@@ -977,26 +995,31 @@
     @cached_property
     def isConvex(self):
         return self.mesh.is_convex
 
     @property
     def AABB(self):
         return (
-            tuple(self.mesh.bounds[0]),
-            tuple(self.mesh.bounds[1]),
-            tuple(self.mesh.bounds[2]),
+            tuple(self.mesh.bounds[:, 0]),
+            tuple(self.mesh.bounds[:, 1]),
+            tuple(self.mesh.bounds[:, 2]),
         )
 
     @cached_property
+    def _boundingPolygonHull(self):
+        assert not isLazy(self)
+        return shapely.multipoints(self.mesh.vertices).convex_hull
+
+    @cached_property
     def _boundingPolygon(self):
         assert not isLazy(self)
 
         # Relatively fast case for convex regions
         if self.isConvex:
-            return shapely.geometry.MultiPoint(self.mesh.vertices).convex_hull
+            return self._boundingPolygonHull
 
         # Generic case for arbitrary shapes
         if self.mesh.is_watertight:
             projection = trimesh.path.polygons.projected(
                 self.mesh, normal=(0, 0, 1), rpad=1e-4
             )
         else:
@@ -1047,44 +1070,48 @@
         position: An optional position, which determines where the center of the region will be.
         rotation: An optional Orientation object which determines the rotation of the object in space.
         orientation: An optional vector field describing the preferred orientation at every point in
           the region.
         tolerance: Tolerance for internal computations.
         centerMesh: Whether or not to center the mesh after copying and before transformations.
         onDirection: The direction to use if an object being placed on this region doesn't specify one.
-        engine: Which engine to use for mesh operations. Either "blender" or "scad".
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, _internal=False, _isConvex=None, **kwargs):
         super().__init__(*args, **kwargs)
+        self._isConvex = _isConvex
 
         if isLazy(self):
             return
 
         # Validate dimensions
         if self.dimensions is not None:
             for dim, name in zip(self.dimensions, ("width", "length", "height")):
                 if dim <= 0:
                     raise ValueError(f"{name} of MeshVolumeRegion must be positive")
 
-        # Ensure the mesh is watertight so volume is well defined
-        if not self._mesh.is_volume:
+        # Ensure the mesh is a well defined volume
+        if not _internal and not self._mesh.is_volume:
             raise ValueError(
                 "A MeshVolumeRegion cannot be defined with a mesh that does not have a well defined volume."
+                " Consider using scenic.core.utils.repairMesh."
             )
 
         # Compute how many samples are necessary to achieve 99% probability
         # of success when rejection sampling volume.
         p_volume = self._mesh.volume / self._mesh.bounding_box.volume
 
         if p_volume > 0.99:
             self.num_samples = 1
         else:
             self.num_samples = min(1e6, max(1, math.ceil(math.log(0.01, 1 - p_volume))))
 
+        # Always try to take at least 8 samples to avoid surface point total rejections
+        self.num_samples = max(self.num_samples, 8)
+
     # Property testing methods #
     @distributionFunction
     def intersects(self, other, triedReversed=False):
         """Check if this region intersects another.
 
         This function handles intersect calculations for `MeshVolumeRegion` with:
         * `MeshVolumeRegion`
@@ -1092,19 +1119,21 @@
         * `PolygonalFootprintRegion`
         """
         if isinstance(other, MeshVolumeRegion):
             # PASS 1
             # Check if bounding boxes intersect. If not, volumes cannot intersect.
             # For bounding boxes to intersect there must be overlap of the bounds
             # in all 3 dimensions.
-            range_overlaps = [
-                (self.mesh.bounds[0, dim] <= other.mesh.bounds[1, dim])
-                and (other.mesh.bounds[0, dim] <= self.mesh.bounds[1, dim])
+            bounds = self._mesh.bounds
+            obounds = other._mesh.bounds
+            range_overlaps = (
+                (bounds[0, dim] <= obounds[1, dim])
+                and (obounds[0, dim] <= bounds[1, dim])
                 for dim in range(3)
-            ]
+            )
             bb_overlap = all(range_overlaps)
 
             if not bb_overlap:
                 return False
 
             # PASS 2
             # Compute inradius and circumradius for a candidate point in each region,
@@ -1181,14 +1210,28 @@
 
             if self.mesh.is_convex and other.mesh.is_convex:
                 # For convex shapes, the manager detects containment as well as
                 # surface intersections, so we can just return the result
                 return surface_collision
 
             # PASS 4
+            # If we have 2 candidate points and both regions have only one body,
+            # we can just check if either region contains the candidate point of the
+            # other. (This is because we previously ruled out surface intersections)
+            if (
+                s_candidate_point is not None
+                and o_candidate_point is not None
+                and self.mesh.body_count == 1
+                and other.mesh.body_count == 1
+            ):
+                return self.containsPoint(o_candidate_point) or other.containsPoint(
+                    s_candidate_point
+                )
+
+            # PASS 5
             # Compute intersection and check if it's empty. Expensive but guaranteed
             # to give the right answer.
             return not isinstance(self.intersect(other), EmptyRegion)
 
         if isinstance(other, MeshSurfaceRegion):
             # PASS 1
             # Check if bounding boxes intersect. If not, volumes cannot intersect.
@@ -1390,36 +1433,23 @@
             return super().intersect(other, triedReversed)
 
         if isinstance(other, MeshVolumeRegion):
             # Other region is a mesh volume. We can extract the mesh to perform boolean operations on it
             other_mesh = other.mesh
 
             # Compute intersection using Trimesh
-            try:
-                new_mesh = self.mesh.intersection(other_mesh, engine=self.engine)
-            except CalledProcessError as e:
-                # Check if scad is complaining about an empty top level geometry.
-                # If so, just return an empty Trimesh object.
-                if "Current top level object is empty." in e.output.decode():
-                    return nowhere
-                else:
-                    raise
-            except ValueError as exc:
-                raise ValueError(
-                    "Unable to compute mesh boolean operation. Do you have the Blender and OpenSCAD installed on your system?"
-                ) from exc
+            new_mesh = self.mesh.intersection(other_mesh)
 
             if new_mesh.is_empty:
                 return nowhere
             elif new_mesh.is_volume:
                 return MeshVolumeRegion(
                     new_mesh,
                     tolerance=min(self.tolerance, other.tolerance),
                     centerMesh=False,
-                    engine=self.engine,
                 )
             else:
                 # Something went wrong, abort
                 return super().intersect(other, triedReversed)
 
         if isinstance(other, PolygonalFootprintRegion):
             # Other region is a polygonal footprint region. We can bound it in the vertical dimension
@@ -1608,29 +1638,23 @@
 
         # If other region is represented by a mesh, we can extract the mesh to
         # perform boolean operations on it
         if isinstance(other, MeshVolumeRegion):
             other_mesh = other.mesh
 
             # Compute union using Trimesh
-            try:
-                new_mesh = self.mesh.union(other_mesh, engine=self.engine)
-            except ValueError as exc:
-                raise ValueError(
-                    "Unable to compute mesh boolean operation. Do you have the Blender and OpenSCAD installed on your system?"
-                ) from exc
+            new_mesh = self.mesh.union(other_mesh)
 
             if new_mesh.is_empty:
                 return nowhere
             elif new_mesh.is_volume:
                 return MeshVolumeRegion(
                     new_mesh,
                     tolerance=min(self.tolerance, other.tolerance),
                     centerMesh=False,
-                    engine=self.engine,
                 )
             else:
                 # Something went wrong, abort
                 return super().union(other, triedReversed)
 
         # Don't know how to compute this union, fall back to default behavior.
         return super().union(other, triedReversed)
@@ -1648,38 +1672,23 @@
 
         # If other region is represented by a mesh, we can extract the mesh to
         # perform boolean operations on it
         if isinstance(other, MeshVolumeRegion):
             other_mesh = other.mesh
 
             # Compute difference using Trimesh
-            try:
-                new_mesh = self.mesh.difference(
-                    other_mesh, engine=self.engine, debug=debug
-                )
-            except CalledProcessError as e:
-                # Check if scad is complaining about an empty top level geometry.
-                # If so, just return an empty Trimesh object.
-                if "Current top level object is empty." in e.output.decode():
-                    return nowhere
-                else:
-                    raise
-            except ValueError as exc:
-                raise ValueError(
-                    "Unable to compute mesh boolean operation. Do you have the Blender and OpenSCAD installed on your system?"
-                ) from exc
+            new_mesh = self.mesh.difference(other_mesh)
 
             if new_mesh.is_empty:
                 return nowhere
             elif new_mesh.is_volume:
                 return MeshVolumeRegion(
                     new_mesh,
                     tolerance=min(self.tolerance, other.tolerance),
                     centerMesh=False,
-                    engine=self.engine,
                 )
             else:
                 # Something went wrong, abort
                 return super().difference(other)
 
         if isinstance(other, PolygonalFootprintRegion):
             # Other region is a polygonal footprint region. We can bound it in the vertical dimension
@@ -1721,45 +1730,111 @@
         # Positive distance indicates being contained in the mesh.
         if dist > 0:
             dist = 0
 
         return abs(dist)
 
     @cached_property
+    @distributionFunction
     def inradius(self):
         center_point = self.mesh.bounding_box.center_mass
 
         pq = trimesh.proximity.ProximityQuery(self.mesh)
-        region_distance = abs(pq.signed_distance([center_point])[0])
+        region_distance = pq.signed_distance([center_point])[0]
 
         if region_distance < 0:
             return 0
         else:
             return region_distance
 
+    @cached_property
+    def isConvex(self):
+        return self.mesh.is_convex if self._isConvex is None else self._isConvex
+
     @property
     def dimensionality(self):
         return 3
 
     @cached_property
     def size(self):
         return self.mesh.mass / self.mesh.density
 
     ## Utility Methods ##
+    def voxelized(self, pitch, lazy=False):
+        """Returns a VoxelRegion representing a filled voxelization of this mesh"""
+        return VoxelRegion(voxelGrid=self.mesh.voxelized(pitch).fill(), lazy=lazy)
+
+    @distributionFunction
+    def _erodeOverapproximate(self, maxErosion, pitch):
+        """Compute an overapproximation of this region eroded.
+
+        Erode as much as possible, but no more than maxErosion, outputting
+        a VoxelRegion. Note that this can sometimes return a larger region
+        than the original mesh
+        """
+        # Compute a voxel overapproximation of the mesh. Technically this is not
+        # an overapproximation, but one dilation with a rank 3 structuring unit
+        # with connectivity 3 is. To simplify, we just erode one fewer time than
+        # needed.
+        target_pitch = pitch * max(self.mesh.extents)
+        voxelized_mesh = self.voxelized(target_pitch, lazy=True)
+
+        # Erode the voxel region. Erosion is done with a rank 3 structuring unit with
+        # connectivity 3 (a 3x3x3 cube of voxels). Each erosion pass can erode by at
+        # most math.hypot([pitch]*3). Therefore we can safely make at most
+        # floor(maxErosion/math.hypot([pitch]*3)) passes without eroding more
+        # than maxErosion. We also subtract 1 iteration for the reasons above.
+        iterations = math.floor(maxErosion / math.hypot(*([target_pitch] * 3))) - 1
+
+        eroded_mesh = voxelized_mesh.dilation(iterations=-iterations)
+
+        return eroded_mesh
+
+    @distributionFunction
+    def _bufferOverapproximate(self, minBuffer, pitch):
+        """Compute an overapproximation of this region buffered.
+
+        Buffer as little as possible, but at least minBuffer. If pitch is
+        less than 1, the output is a VoxelRegion. If pitch is 1, a fast
+        path is taken which returns a BoxRegion.
+        """
+        if pitch >= 1:
+            # First extract the bounding box of the mesh, and then extend each dimension
+            # by minBuffer.
+            bounds = self.mesh.bounds
+            midpoint = numpy.mean(bounds, axis=0)
+            extents = numpy.diff(bounds, axis=0)[0] + 2 * minBuffer
+            return BoxRegion(position=toVector(midpoint), dimensions=list(extents))
+        else:
+            # Compute a voxel overapproximation of the mesh. Technically this is not
+            # an overapproximation, but one dilation with a rank 3 structuring unit
+            # with connectivity 3 is. To simplify, we just dilate one additional time
+            # than needed.
+            target_pitch = pitch * max(self.mesh.extents)
+            voxelized_mesh = self.voxelized(target_pitch, lazy=True)
+
+            # Dilate the voxel region. Dilation is done with a rank 3 structuring unit with
+            # connectivity 3 (a 3x3x3 cube of voxels). Each dilation pass must dilate by at
+            # least pitch. Therefore we must make at least ceil(minBuffer/pitch) passes to
+            # guarantee dilating at least minBuffer. We also add 1 iteration for the reasons above.
+            iterations = math.ceil(minBuffer / pitch) + 1
+
+            dilated_mesh = voxelized_mesh.dilation(iterations=iterations)
+
+            return dilated_mesh
+
     @cached_method
     def getSurfaceRegion(self):
         """Return a region equivalent to this one, except as a MeshSurfaceRegion"""
         return MeshSurfaceRegion(
             self.mesh,
             self.name,
-            orientation=self.orientation,
             tolerance=self.tolerance,
             centerMesh=False,
             onDirection=self.onDirection,
-            engine=self.engine,
         )
 
     def getVolumeRegion(self):
         """Returns this object, as it is already a MeshVolumeRegion"""
         return self
 
 
@@ -1787,29 +1862,31 @@
         orientation: An optional vector field describing the preferred orientation at every point in
           the region.
         tolerance: Tolerance for internal computations.
         centerMesh: Whether or not to center the mesh after copying and before transformations.
         onDirection: The direction to use if an object being placed on this region doesn't specify one.
     """
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self, *args, orientation=True, **kwargs):
+        if orientation is True:
+            orientation = VectorField(
+                "DefaultSurfaceVectorField", self.getFlatOrientation
+            )
+            self._usingDefaultOrientation = True
+        else:
+            self._usingDefaultOrientation = False
+
+        super().__init__(*args, orientation=orientation, **kwargs)
 
         # Validate dimensions
         if self.dimensions is not None:
             for dim, name in zip(self.dimensions, ("width", "length", "height")):
                 if dim < 0:
                     raise ValueError(f"{name} of MeshSurfaceRegion must be nonnegative")
 
-        # Set default orientation to one inferred from face norms if none is provided.
-        if self.orientation is None:
-            self.orientation = VectorField(
-                "DefaultSurfaceVectorField", lambda pos: self.getFlatOrientation(pos)
-            )
-
     # Property testing methods #
     @distributionFunction
     def intersects(self, other, triedReversed=False):
         """Check if this region's surface intersects another.
 
         This function handles intersection computation for `MeshSurfaceRegion` with:
         * `MeshSurfaceRegion`
@@ -1939,19 +2016,17 @@
     ## Utility Methods ##
     @cached_method
     def getVolumeRegion(self):
         """Return a region equivalent to this one, except as a MeshVolumeRegion"""
         return MeshVolumeRegion(
             self.mesh,
             self.name,
-            orientation=self.orientation,
             tolerance=self.tolerance,
             centerMesh=False,
             onDirection=self.onDirection,
-            engine=self.engine,
         )
 
     def getSurfaceRegion(self):
         """Returns this object, as it is already a MeshSurfaceRegion"""
         return self
 
 
@@ -1975,15 +2050,14 @@
     def sampleGiven(self, value):
         return BoxRegion(
             dimensions=value[self.dimensions],
             position=value[self.position],
             rotation=value[self.rotation],
             orientation=value[self.orientation],
             tolerance=self.tolerance,
-            engine=self.engine,
             name=self.name,
         )
 
     def evaluateInner(self, context):
         dimensions = valueInContext(self.dimensions, context)
         position = valueInContext(self.position, context)
         rotation = valueInContext(self.rotation, context)
@@ -1991,15 +2065,14 @@
 
         return BoxRegion(
             dimensions=dimensions,
             position=position,
             rotation=rotation,
             orientation=orientation,
             tolerance=self.tolerance,
-            engine=self.engine,
             name=self.name,
         )
 
 
 class SpheroidRegion(MeshVolumeRegion):
     """Region in the shape of a spheroid.
 
@@ -2020,15 +2093,14 @@
     def sampleGiven(self, value):
         return SpheroidRegion(
             dimensions=value[self.dimensions],
             position=value[self.position],
             rotation=value[self.rotation],
             orientation=value[self.orientation],
             tolerance=self.tolerance,
-            engine=self.engine,
             name=self.name,
         )
 
     def evaluateInner(self, context):
         dimensions = valueInContext(self.dimensions, context)
         position = valueInContext(self.position, context)
         rotation = valueInContext(self.rotation, context)
@@ -2036,19 +2108,223 @@
 
         return SpheroidRegion(
             dimensions=dimensions,
             position=position,
             rotation=rotation,
             orientation=orientation,
             tolerance=self.tolerance,
-            engine=self.engine,
             name=self.name,
         )
 
 
+class VoxelRegion(Region):
+    """(WIP) Region represented by a voxel grid in 3D space.
+
+    NOTE: This region is a work in progress and is currently only recommended for internal use.
+
+    Args:
+        voxelGrid: The Trimesh voxelGrid to be used.
+        orientation: An optional vector field describing the preferred orientation at every point in
+          the region.
+        name: An optional name to help with debugging.
+        lazy: Whether or not to be lazy about pre-computing internal values. Set this to True if this
+          VoxelRegion is unlikely to be used outside of an intermediate step in compiling/pruning.
+    """
+
+    def __init__(self, voxelGrid, orientation=None, name=None, lazy=False):
+        # Initialize superclass
+        super().__init__(name, orientation=orientation)
+
+        # Check that the encoding isn't empty. In that case, raise an error.
+        if voxelGrid.encoding.is_empty:
+            raise ValueError("Tried to create an empty VoxelRegion.")
+
+        # Store voxel grid and extract points and scale
+        self.voxelGrid = voxelGrid
+        self.voxel_points = self.voxelGrid.points
+        self.scale = self.voxelGrid.scale
+
+    @cached_property
+    def kdTree(self):
+        return scipy.spatial.KDTree(self.voxel_points)
+
+    def containsPoint(self, point):
+        point = toVector(point)
+
+        # Find closest voxel point
+        _, index = self.kdTree.query(point)
+        closest_point = self.voxel_points[index]
+
+        # Check voxel containment
+        voxel_low = closest_point - self.scale / 2
+        voxel_high = closest_point + self.scale / 2
+
+        return numpy.all(voxel_low <= point) & numpy.all(point <= voxel_high)
+
+    def containsObject(self, obj):
+        raise NotImplementedError
+
+    def containsRegionInner(self, reg):
+        raise NotImplementedError
+
+    def distanceTo(self, point):
+        raise NotImplementedError
+
+    def projectVector(self, point, onDirection):
+        raise NotImplementedError
+
+    def uniformPointInner(self):
+        # First generate a point uniformly in a box with dimensions
+        # equal to scale, centered at the origin.
+        base_pt = numpy.random.random_sample(3) - 0.5
+        scaled_pt = base_pt * self.scale
+
+        # Pick a random voxel point and add it to base_pt.
+        voxel_base = self.voxel_points[random.randrange(len(self.voxel_points))]
+        offset_pt = voxel_base + scaled_pt
+
+        return Vector(*offset_pt)
+
+    def dilation(self, iterations, structure=None):
+        """Returns a dilated/eroded version of this VoxelRegion.
+
+        Args:
+            iterations: How many times repeat the dilation/erosion. A positive
+              number indicates a dilation and a negative number indicates an
+              erosion.
+            structure: The structure to use. If none is provided, a rank 3
+              structuring unit with connectivity 3 is used.
+        """
+        # Parse parameters
+        if iterations == 0:
+            return self
+
+        if iterations > 0:
+            morphology_func = scipy.ndimage.binary_dilation
+        else:
+            morphology_func = scipy.ndimage.binary_erosion
+
+        iterations = abs(iterations)
+
+        if structure == None:
+            structure = scipy.ndimage.generate_binary_structure(3, 3)
+
+        # Compute a dilated/eroded encoding
+        new_encoding = trimesh.voxel.encoding.DenseEncoding(
+            morphology_func(
+                trimesh.voxel.morphology._dense(self.voxelGrid.encoding, rank=3),
+                structure=structure,
+                iterations=iterations,
+            )
+        )
+
+        # Check if the encoding is empty, in which case we should return the empty region.
+        if new_encoding.is_empty:
+            return nowhere
+
+        # Otherwise, return a VoxelRegion representing the eroded region.
+        new_voxel_grid = trimesh.voxel.VoxelGrid(
+            new_encoding, transform=self.voxelGrid.transform
+        )
+        return VoxelRegion(voxelGrid=new_voxel_grid)
+
+    @cached_property
+    def mesh(self):
+        """(WIP) Return a MeshVolumeRegion representation of this region.
+
+        NOTE: This region is a WIP and will sometimes return None if the transformation
+        is not feasible.
+        """
+        # Extract values for original voxel grid and the surface of the voxel grid.
+        dense_encoding = self.voxelGrid.encoding.dense
+        hpitch = self.voxelGrid.pitch[0] / 2
+        hollow_vr = trimesh.voxel.VoxelGrid(
+            trimesh.voxel.morphology.surface(self.voxelGrid.encoding),
+            transform=self.voxelGrid.transform,
+        )
+
+        surface_indices = numpy.argwhere(hollow_vr.encoding.dense == True)
+        surface_centers = hollow_vr.indices_to_points(hollow_vr.sparse_indices)
+
+        # Determine which faces should be added for each voxel in our extracted surface.
+        point_face_mask_list = []
+
+        def index_in_bounds(index):
+            return all((0, 0, 0) <= index) and all(index < dense_encoding.shape)
+
+        def actual_face(index):
+            return not index_in_bounds(index) or not dense_encoding[tuple(index)]
+
+        offsets = (
+            [1, 0, 0],
+            [-1, 0, 0],
+            [0, 1, 0],
+            [0, -1, 0],
+            [0, 0, 1],
+            [0, 0, -1],
+        )
+
+        # fmt: off
+        pitch_signs = [
+            ([[1, 1, -1],  [1, 1, 1],    [1, -1, 1]],
+             [[1, 1, -1],  [1, -1, 1],   [1, -1, -1]]),
+            ([[-1, 1, -1], [-1, -1, 1],  [-1, 1, 1]],
+             [[-1, 1, -1], [-1, -1, -1], [-1, -1, 1]]),
+            ([[1, 1, -1],  [-1, 1, 1],   [1, 1, 1]],
+             [[1, 1, -1],  [-1, 1, -1],  [-1, 1, 1]]),
+            ([[1, -1, -1], [1, -1, 1],   [-1, -1, 1]],
+             [[1, -1, -1], [-1, -1, 1],  [-1, -1, -1]]),
+            ([[1, -1, 1],  [1, 1, 1],    [-1, 1, 1]],
+             [[1, -1, 1],  [-1, 1, 1],   [-1, -1, 1]]),
+            ([[1, -1, -1], [-1, 1, -1],  [1, 1, -1]],
+             [[1, -1, -1], [-1, -1, -1], [-1, 1, -1]]),
+        ]
+        # fmt: on
+
+        triangles = []
+
+        for i in range(len(surface_indices)):
+            base_index = surface_indices[i]
+            base_center = surface_centers[i]
+
+            for i, offset in enumerate(offsets):
+                if actual_face(base_index + offset):
+                    for t_num in range(2):
+                        triangles.append(
+                            [
+                                base_center + hpitch * numpy.array(signs)
+                                for signs in pitch_signs[i][t_num]
+                            ]
+                        )
+
+        out_mesh = trimesh.Trimesh(**trimesh.triangles.to_kwargs(triangles))
+
+        # TODO: Ensure the mesh is a proper volume
+        if not out_mesh.is_volume:
+            return None
+        else:
+            return MeshVolumeRegion(out_mesh, centerMesh=False)
+
+    @property
+    def AABB(self):
+        return (
+            tuple(self.voxelGrid.bounds[:, 0]),
+            tuple(self.voxelGrid.bounds[:, 1]),
+            tuple(self.voxelGrid.bounds[:, 2]),
+        )
+
+    @property
+    def size(self):
+        return self.voxelGrid.volume
+
+    @property
+    def dimensionality(self):
+        return 3
+
+
 class PolygonalFootprintRegion(Region):
     """Region that contains all points in a polygonal footprint, regardless of their z value.
 
     This region cannot be sampled from, as it has infinite height and therefore infinite volume.
 
     Args:
         polygon: A ``shapely`` ``Polygon`` or ``MultiPolygon``, that defines the footprint of this region.
@@ -2147,15 +2423,26 @@
 
     def containsObject(self, obj):
         """Checks if an object is contained in the polygonal footprint.
 
         Args:
             obj: An object to be checked for containment.
         """
-        # Check containment using the bounding polygon of the object.
+        # Fast path for convex objects, whose bounding polygons are relatively
+        # easy to compute.
+        if obj._isConvex:
+            return self.polygons.contains(obj._boundingPolygon)
+
+        # Quick check using the projected convex hull of the object, which
+        # overapproximates the actual bounding polygon.
+        hullPoly = obj.occupiedSpace._boundingPolygonHull
+        if self.polygons.contains(hullPoly):
+            return True
+
+        # Need to compute exact bounding polygon.
         return self.polygons.contains(obj._boundingPolygon)
 
     def containsRegionInner(self, reg, tolerance):
         buffered_polygons = self.polygons.buffer(tolerance)
 
         if isinstance(other, MeshRegion):
             return buffered_polygons.contains(reg._boundingPolygon)
@@ -2284,19 +2571,30 @@
     """A region composed of multiple polylines in 3D space.
 
     One of points or polylines should be provided.
 
     Args:
         points: A list of points defining a single polyline.
         polylines: A list of list of points, defining multiple polylines.
+        orientation (optional): :term:`preferred orientation` to use, or `True` to use an
+            orientation aligned with the direction of the path (the default).
         tolerance: Tolerance used internally.
     """
 
-    def __init__(self, points=None, polylines=None, tolerance=1e-8, name=None):
-        super().__init__(name)
+    def __init__(
+        self, points=None, polylines=None, tolerance=1e-8, orientation=True, name=None
+    ):
+        if orientation is True:
+            orientation = VectorField("Path", self.defaultOrientation)
+            self._usingDefaultOrientation = True
+        else:
+            self._usingDefaultOrientation = False
+
+        super().__init__(name, orientation=orientation)
+
         # Standardize inputs
         if points is not None and polylines is not None:
             raise ValueError("Both points and polylines passed to PathRegion initializer")
 
         if points is not None:
             polylines = [points]
         elif polylines is not None:
@@ -2360,14 +2658,24 @@
     def containsObject(self, obj):
         return False
 
     def containsRegionInner(self, reg, tolerance):
         raise NotImplementedError
 
     def distanceTo(self, point):
+        return self._segmentDistanceHelper(point).min()
+
+    def nearestSegmentTo(self, point):
+        nearest_segment = self._edgeVectorArray[
+            self._segmentDistanceHelper(point).argmin()
+        ]
+        return toVector(nearest_segment[0:3]), toVector(nearest_segment[3:6])
+
+    def _segmentDistanceHelper(self, point):
+        """Returns distance to point from each line segment"""
         p = numpy.asarray(toVector(point))
         a = self._edgeVectorArray[:, 0:3]
         b = self._edgeVectorArray[:, 3:6]
         a_min_p = a - p
 
         d = (b - a) / numpy.linalg.norm(b - a, axis=1).reshape(len(a), 1)
 
@@ -2377,15 +2685,19 @@
 
         # Actual parallel distance is 0 if on the line segment.
         parallel_dist = numpy.amax(
             [a_dist, b_dist, numpy.zeros(len(self._edgeVectorArray))], axis=0
         )
         perp_dist = numpy.linalg.norm(numpy.cross(a_min_p, d), axis=1)
 
-        return numpy.hypot(parallel_dist, perp_dist).min()
+        return numpy.hypot(parallel_dist, perp_dist)
+
+    def defaultOrientation(self, point):
+        start, end = self.nearestSegmentTo(point)
+        return Orientation.fromEuler(start.azimuthTo(end), start.altitudeTo(end), 0)
 
     def projectVector(self, point, onDirection):
         raise NotImplementedError
 
     @cached_property
     def AABB(self):
         return tuple(
@@ -2520,14 +2832,18 @@
         return PolygonalFootprintRegion(self.polygons)
 
     @distributionFunction
     def containsPoint(self, point):
         return self.footprint.containsPoint(point)
 
     @distributionFunction
+    def _trueContainsPoint(self, point):
+        return point.z == self.z and self.containsPoint(point)
+
+    @distributionFunction
     def containsObject(self, obj):
         return self.footprint.containsObject(obj)
 
     @cached_property
     def _samplingData(self):
         triangles = []
         for polygon in self.polygons.geoms:
@@ -2629,31 +2945,36 @@
             return regionFromShapelyObject(diff, orientation=self.orientation)
         return super().difference(other)
 
     @staticmethod
     @distributionFunction
     def unionAll(regions, buf=0):
         regions = tuple(regions)
-        if not all([r.z == regions[0].z for r in regions]):
-            raise ValueError(
-                "union of PolygonalRegions with different z values is undefined."
-            )
+        z = None
+        for reg in regions:
+            if z is not None and isinstance(reg, PolygonalRegion) and reg.z != z:
+                raise ValueError(
+                    "union of PolygonalRegions with different z values is undefined."
+                )
+            if isinstance(reg, PolygonalRegion) and z is None:
+                z = reg.z
 
         regs, polys = [], []
         for reg in regions:
             if reg != nowhere:
                 regs.append(reg)
                 polys.append(toPolygon(reg))
         if not polys:
             return nowhere
         if any(not poly for poly in polys):
             raise TypeError(f"cannot take union of regions {regions}")
         union = polygonUnion(polys, buf=buf)
         orientation = VectorField.forUnionOf(regs, tolerance=buf)
-        return PolygonalRegion(polygon=union, orientation=orientation)
+        z = 0 if z is None else z
+        return PolygonalRegion(polygon=union, orientation=orientation, z=z)
 
     @property
     @distributionFunction
     def boundary(self) -> "PolylineRegion":
         """Get the boundary of this region as a `PolylineRegion`."""
         return PolylineRegion(polyline=self.polygons.boundary)
 
@@ -2666,14 +2987,27 @@
 
     @distributionFunction
     def distanceTo(self, point):
         point = toVector(point)
         dist2D = shapely.distance(self.polygons, makeShapelyPoint(point))
         return math.hypot(dist2D, point[2] - self.z)
 
+    @cached_property
+    @distributionFunction
+    def inradius(self):
+        minx, miny, maxx, maxy = self.polygons.bounds
+        center = makeShapelyPoint(((minx + maxx) / 2, (maxy + miny) / 2))
+
+        # Check if center is contained
+        if not self.polygons.contains(center):
+            return 0
+
+        # Return the distance to the nearest boundary
+        return shapely.distance(self.polygons.boundary, center)
+
     def projectVector(self, point, onDirection):
         raise NotImplementedError(
             f'{type(self).__name__} does not yet support projection using "on"'
         )
 
     @property
     def AABB(self):
@@ -2973,15 +3307,15 @@
         length = valueInContext(self.length, context)
         return RectangularRegion(position, heading, width, length, name=self.name)
 
     def uniformPointInner(self):
         hw, hl = self.hw, self.hl
         rx = random.uniform(-hw, hw)
         ry = random.uniform(-hl, hl)
-        pt = self.position.offsetRotated(self.heading, Vector(rx, ry, self.position.z))
+        pt = self.position.offsetRotated(self.heading, Vector(rx, ry, 0))
         return self.orient(pt)
 
     @property
     def AABB(self):
         x, y, z = zip(*self.corners)
         minx, maxx = findMinMax(x)
         miny, maxy = findMinMax(y)
@@ -3009,17 +3343,17 @@
             orientation aligned with the direction of the polyline (the default).
         name (str; optional): name for debugging.
     """
 
     def __init__(self, points=None, polyline=None, orientation=True, name=None):
         if orientation is True:
             orientation = VectorField("Polyline", self.defaultOrientation)
-            self.usingDefaultOrientation = True
+            self._usingDefaultOrientation = True
         else:
-            self.usingDefaultOrientation = False
+            self._usingDefaultOrientation = False
         super().__init__(name, orientation=orientation)
 
         if points is not None:
             points = tuple(points)
 
             if any(len(point) > 2 and point[2] != 0 for point in points):
                 warnings.warn(
@@ -3101,15 +3435,15 @@
     def start(self):
         """Get an `OrientedPoint` at the start of the polyline.
 
         The OP's orientation will be aligned with the orientation of the region, if
         there is one (the default orientation pointing along the polyline).
         """
         pointA, pointB = self.segments[0]
-        if self.usingDefaultOrientation:
+        if self._usingDefaultOrientation:
             orientation = headingOfSegment(pointA, pointB)
         elif self.orientation is not None:
             orientation = self.orientation[Vector(*pointA)]
         else:
             orientation = 0
         orientation = toOrientation(orientation)
         from scenic.core.object_types import OrientedPoint
@@ -3125,15 +3459,15 @@
     def end(self):
         """Get an `OrientedPoint` at the end of the polyline.
 
         The OP's orientation will be aligned with the orientation of the region, if
         there is one (the default orientation pointing along the polyline).
         """
         pointA, pointB = self.segments[-1]
-        if self.usingDefaultOrientation:
+        if self._usingDefaultOrientation:
             orientation = headingOfSegment(pointA, pointB)
         elif self.orientation is not None:
             orientation = self.orientation[Vector(*pointB)].yaw
         else:
             orientation = 0
         from scenic.core.object_types import OrientedPoint
 
@@ -3153,15 +3487,15 @@
 
     def uniformPointInner(self):
         pointA, pointB = random.choices(
             self.segments, cum_weights=self.cumulativeLengths
         )[0]
         interpolation = random.random()
         x, y = averageVectors(pointA, pointB, weight=interpolation)
-        if self.usingDefaultOrientation:
+        if self._usingDefaultOrientation:
             return OrientedVector(x, y, 0, headingOfSegment(pointA, pointB))
         else:
             return self.orient(Vector(x, y, 0))
 
     def containsRegionInner(self, other, tolerance):
         poly = toPolygon(other)
         if poly is None:
@@ -3577,106 +3911,84 @@
 class ViewRegion(MeshVolumeRegion):
     """The viewing volume of a camera defined by a radius and horizontal/vertical view angles.
 
     The default view region can take several forms, depending on the viewAngles parameter:
 
     * Case 1:       viewAngles[1] = 180 degrees
 
-      * Case 2.a    viewAngles[0] = 360 degrees     => Sphere
-      * Case 2.b    viewAngles[0] < 360 degrees     => Sphere & CylinderSectionRegion
-
-    * Case 2:       viewAngles[1] < 180 degrees
+      * Case 1.a    viewAngles[0] = 360 degrees     => Sphere
+      * Case 1.b    viewAngles[0] < 360 degrees     => Sphere & CylinderSectionRegion
 
-      * Case 2.a    viewAngles[0] = 360 degrees     => Sphere - (Cone + Cone) (Cones on z axis expanding from origin)
-      * Case 2.b    viewAngles[0] < 360 degrees     => Sphere & ViewSectionRegion
+    * Case 2:       viewAngles[1] < 180 degrees     => Sphere & ViewSectionRegion
 
     When making changes to this class you should run ``pytest -k test_viewRegion --exhaustive``.
 
     Args:
         visibleDistance: The view distance for this region.
         viewAngles: The view angles for this region.
         name: An optional name to help with debugging.
         position: An optional position, which determines where the center of the region will be.
         rotation: An optional Orientation object which determines the rotation of the object in space.
-        orientation: An optional vector field describing the preferred orientation at every point in
-          the region.
         angleCutoff: How close to 180/360 degrees an angle has to be to be mapped to that value.
         tolerance: Tolerance for collision computations.
     """
 
     def __init__(
         self,
         visibleDistance,
         viewAngles,
         name=None,
         position=Vector(0, 0, 0),
         rotation=None,
-        orientation=None,
-        angleCutoff=0.01,
+        angleCutoff=0.017,
         tolerance=1e-8,
     ):
         # Bound viewAngles from either side.
         if min(viewAngles) <= 0:
             raise ValueError("viewAngles cannot have a component less than or equal to 0")
 
+        # TODO True surface representation
+        viewAngles = (max(viewAngles[0], angleCutoff), max(viewAngles[1], angleCutoff))
+
+        if math.tau - angleCutoff <= viewAngles[0]:
+            viewAngles = (math.tau, viewAngles[1])
+
+        if math.pi - angleCutoff <= viewAngles[1]:
+            viewAngles = (viewAngles[0], math.pi)
+
         view_region = None
         diameter = 2 * visibleDistance
-        base_sphere = SpheroidRegion(
-            dimensions=(diameter, diameter, diameter), engine="scad"
-        )
+        base_sphere = SpheroidRegion(dimensions=(diameter, diameter, diameter))
 
         if math.pi - angleCutoff <= viewAngles[1]:
             # Case 1
-            if math.tau - angleCutoff <= viewAngles[0]:
+            if viewAngles[0] == math.tau:
                 # Case 1.a
                 view_region = base_sphere
             else:
+                # Case 1.b
                 view_region = base_sphere.intersect(
                     CylinderSectionRegion(visibleDistance, viewAngles[0])
                 )
         else:
             # Case 2
-            if math.tau - angleCutoff <= viewAngles[0]:
-                # Case 2.a
-                # Create cone with yaw oriented around (0,0,-1)
-                padded_height = visibleDistance * 2
-                radius = padded_height * math.tan((math.pi - viewAngles[1]) / 2)
-
-                cone_mesh = trimesh.creation.cone(radius=radius, height=padded_height)
-
-                position_matrix = translation_matrix((0, 0, -1 * padded_height))
-                cone_mesh.apply_transform(position_matrix)
-
-                # Create two cones around the yaw axis
-                orientation_1 = Orientation._fromEuler(0, 0, 0)
-                orientation_2 = Orientation._fromEuler(0, 0, math.pi)
-
-                cone_1 = MeshVolumeRegion(
-                    mesh=cone_mesh, rotation=orientation_1, centerMesh=False
-                )
-                cone_2 = MeshVolumeRegion(
-                    mesh=cone_mesh, rotation=orientation_2, centerMesh=False
-                )
-
-                view_region = base_sphere.difference(cone_1).difference(cone_2)
-            else:
-                # Case 2.b
-                view_region = base_sphere.intersect(
-                    ViewSectionRegion(visibleDistance, viewAngles)
-                )
+            view_region = base_sphere.intersect(
+                ViewSectionRegion(visibleDistance, viewAngles)
+            )
 
         assert view_region is not None
+        assert isinstance(view_region, MeshVolumeRegion)
+        assert view_region.containsPoint(Vector(0, 0, 0))
 
         # Initialize volume region
         super().__init__(
             mesh=view_region.mesh,
             name=name,
             position=position,
             rotation=rotation,
-            orientation=orientation,
             tolerance=tolerance,
             centerMesh=False,
         )
 
 
 class ViewSectionRegion(MeshVolumeRegion):
     def __init__(self, visibleDistance, viewAngles, rotation=None, resolution=32):
@@ -3698,16 +4010,17 @@
 
         # Face triangles
         for li in range(len(top_line) - 1):
             triangles.append((top_line[li], bot_line[li], top_line[li + 1]))
             triangles.append((bot_line[li], bot_line[li + 1], top_line[li + 1]))
 
         # Side triangles
-        triangles.append((bot_line[0], top_line[0], (0, 0, 0)))
-        triangles.append((top_line[-1], bot_line[-1], (0, 0, 0)))
+        if viewAngles[0] < math.tau:
+            triangles.append((bot_line[0], top_line[0], (0, 0, 0)))
+            triangles.append((top_line[-1], bot_line[-1], (0, 0, 0)))
 
         # Top/Bottom triangles
         for li in range(len(top_line) - 1):
             triangles.append((top_line[li], top_line[li + 1], (0, 0, 0)))
             triangles.append((bot_line[li + 1], bot_line[li], (0, 0, 0)))
 
         vr_mesh = trimesh.Trimesh(**trimesh.triangles.to_kwargs(triangles))
```

### Comparing `scenic-3.0.0b2/src/scenic/core/requirements.py` & `scenic-3.0.0rc1/src/scenic/core/requirements.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/core/sample_checking.py` & `scenic-3.0.0rc1/src/scenic/core/sample_checking.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/core/scenarios.py` & `scenic-3.0.0rc1/src/scenic/core/scenarios.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,24 @@
 from scenic.core.distributions import (
     ConstantSamplable,
     RejectionException,
     Samplable,
     distributionFunction,
     needsSampling,
 )
-from scenic.core.dynamics import Behavior, Monitor
+from scenic.core.dynamics.behaviors import Behavior, Monitor
 from scenic.core.errors import InvalidScenarioError, optionallyDebugRejection
 from scenic.core.external_params import ExternalSampler
 from scenic.core.lazy_eval import needsLazyEvaluation
-from scenic.core.regions import AllRegion, EmptyRegion, convertToFootprint
+from scenic.core.regions import (
+    AllRegion,
+    EmptyRegion,
+    PointInRegionDistribution,
+    convertToFootprint,
+)
 from scenic.core.requirements import (
     BlanketCollisionRequirement,
     BoundRequirement,
     ContainmentRequirement,
     IntersectionRequirement,
     NonVisibilityRequirement,
     VisibilityRequirement,
@@ -194,15 +199,15 @@
             stream.write("\n")
         stream.write("ego = ")
         for obj in self.objects:
             dumpAsScenicCode(obj, stream)
             stream.write("\n")
 
     def show(self, axes=True):
-        self.show3D(axes=axes)
+        return self.show3D(axes=axes)
 
     def show3D(self, axes):
         """Render a 3D schematic of the scene for debugging."""
         import trimesh
 
         # Create a new trimesh scene to contain meshes
         render_scene = trimesh.scene.Scene()
@@ -222,15 +227,15 @@
                 )
             )
 
         flags = dict()
         if axes:
             flags["axis"] = "world"
 
-        render_scene.show(flags=flags)
+        return render_scene.show(flags=flags)
 
     def show2D(self, zoom=None, block=True):
         """Render a 2D schematic of the scene for debugging."""
         import matplotlib.pyplot as plt
 
         plt.gca().set_aspect("equal")
         # display map
@@ -307,16 +312,14 @@
             for value in namespace.values():
                 if isinstance(value, Samplable):
                     behaviorDeps.append(value)
         self.dependencies = (
             self._instances + paramDeps + tuple(requirementDeps) + tuple(behaviorDeps)
         )
 
-        self.validate()
-
         # Setup the default checker
         self.defaultRequirements = self.generateDefaultRequirements()
         self.setSampleChecker(WeightedAcceptanceChecker(bufferSize=100))
 
     def setSampleChecker(self, checker):
         self.checker = checker
         self.checker.setRequirements(self.defaultRequirements + self.userRequirements)
@@ -338,14 +341,27 @@
         staticBounds = [obj._hasStaticBounds for obj in objects]
         for i in range(len(objects)):
             oi = objects[i]
             container = self.containerOfObject(oi)
             # Trivial case where container is empty
             if isinstance(container, EmptyRegion):
                 raise InvalidScenarioError(f"Container region of {oi} is empty")
+            # Ensure we are not sampling position from AllRegion
+            if isinstance(
+                oi.position._conditioned, PointInRegionDistribution
+            ) and isinstance(oi.position._conditioned.region, AllRegion):
+                if oi.position.tag == "visible":
+                    raise InvalidScenarioError(
+                        f"Object {oi} uses the visible specifier to specify position, but it lacks enough information to do so."
+                        f" The simplest solution to this is to define a workspace or specify position in some other fashion."
+                    )
+                else:
+                    raise InvalidScenarioError(
+                        f"Object {oi} has position sampled from everywhere."
+                    )
             # skip objects with unknown positions or bounding boxes
             if not staticBounds[i]:
                 continue
             # Require object to be contained in the workspace/valid region
             if not needsSampling(container) and not container.containsObject(oi):
                 raise InvalidScenarioError(
                     f"Object at {oi.position} does not fit in container"
@@ -513,14 +529,18 @@
                 NonVisibilityRequirement(obj._nonObservingEntity, obj, possible_occluders)
             )
 
         # Visibility from the ego
         for obj in filter(
             lambda x: x.requireVisible and x is not self.egoObject, self.objects
         ):
+            if not self.egoObject:
+                raise InvalidScenarioError(
+                    "requireVisible set to true but no ego is defined"
+                )
             requirements.append(VisibilityRequirement(self.egoObject, obj, self.objects))
 
         return tuple(requirements)
 
     def _makeSceneFromSample(self, sample):
         sampledObjects = tuple(sample[obj] for obj in self.objects)
         ego = sample[self.egoObject]
```

### Comparing `scenic-3.0.0b2/src/scenic/core/serialization.py` & `scenic-3.0.0rc1/src/scenic/core/serialization.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 `Scenario.simulationToBytes`, and `Scene.dumpAsScenicCode`.
 """
 
 import io
 import math
 import pickle
 import struct
+import types
 
 from scenic.core.distributions import Samplable, needsSampling
 from scenic.core.utils import DefaultIdentityDict
 
 ## JSON
 
 
@@ -37,14 +38,38 @@
     """Utility function to help export Scenic objects as Scenic code."""
     if hasattr(value, "dumpAsScenicCode"):
         value.dumpAsScenicCode(stream)
     else:
         stream.write(repr(value))
 
 
+## Pickles
+
+# If dill is installed, register some custom handlers to improve the pickling
+# of Scene and Scenario objects.
+
+try:
+    import dill
+except Exception:
+    pass
+else:
+    _orig_save_module = dill.Pickler.dispatch[types.ModuleType]
+
+    @dill.register(types.ModuleType)
+    def patched_save_module(pickler, obj):
+        # Save Scenic's internal modules by reference to avoid inconsistent versions
+        # as well as some unpicklable objects (and shrink the size of pickles while
+        # we're at it).
+        name = obj.__name__
+        if name == "scenic" or name.startswith("scenic."):
+            pickler.save_reduce(dill._dill._import_module, (name,), obj=obj)
+            return
+        _orig_save_module(pickler, obj)
+
+
 ## Binary serialization format
 
 
 class SerializationError(Exception):
     """An error occurring during serialization/deserialization of Scenic objects."""
 
     pass
```

### Comparing `scenic-3.0.0b2/src/scenic/core/shapes.py` & `scenic-3.0.0rc1/src/scenic/core/shapes.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from trimesh.transformations import (
     concatenate_matrices,
     quaternion_matrix,
     translation_matrix,
 )
 
 from scenic.core.type_support import toOrientation
-from scenic.core.utils import cached_property, loadMesh
+from scenic.core.utils import cached_property, unifyMesh
 from scenic.core.vectors import Orientation
 
 ###################################################################################################
 # Abstract Classes and Utilities
 ###################################################################################################
 
 
@@ -90,14 +90,15 @@
     """
 
     def __init__(self, mesh, dimensions=None, scale=1, initial_rotation=None):
         # Ensure the mesh is watertight so volume is well defined
         if not mesh.is_volume:
             raise ValueError(
                 "A MeshShape cannot be defined with a mesh that does not have a well defined volume."
+                " Consider using scenic.core.utils.repairMesh."
             )
 
         # Copy mesh and center vertices around origin
         self._mesh = mesh.copy()
         self._mesh.vertices -= self._mesh.bounding_box.center_mass
 
         # If rotation is provided, apply rotation
@@ -117,31 +118,39 @@
         scale_matrix = numpy.eye(4)
         scale_matrix[:3, :3] /= scale_vals
         self._mesh.apply_transform(scale_matrix)
 
         super().__init__(dimensions, scale)
 
     @classmethod
-    def fromFile(cls, path, filetype=None, compressed=None, binary=False, **kwargs):
+    def fromFile(cls, path, unify=True, **kwargs):
         """Load a mesh shape from a file, attempting to infer filetype and compression.
 
         For example: "foo.obj.bz2" is assumed to be a compressed .obj file.
         "foo.obj" is assumed to be an uncompressed .obj file. "foo" is an
         unknown filetype, so unless a filetype is provided an exception will be raised.
 
         Args:
             path (str): Path to the file to import.
             filetype (str): Filetype of file to be imported. This will be inferred if not provided.
                 The filetype must be one compatible with `trimesh.load`.
             compressed (bool): Whether or not this file is compressed (with bz2). This will be inferred
                 if not provided.
             binary (bool): Whether or not to open the file as a binary file.
+            unify (bool): Whether or not to attempt to unify this mesh.
             kwargs: Additional arguments to the MeshShape initializer.
         """
-        mesh = loadMesh(path, filetype, compressed, binary)
+        mesh = trimesh.load(path, force="mesh")
+        if not mesh.is_volume:
+            raise ValueError(
+                "A MeshShape cannot be defined with a mesh that does not have a well defined volume."
+                " Consider using scenic.core.utils.repairMesh."
+            )
+        if unify:
+            mesh = unifyMesh(mesh, verbose=True)
         return cls(mesh, **kwargs)
 
     @property
     def mesh(self):
         return self._mesh
 
     @cached_property
```

### Comparing `scenic-3.0.0b2/src/scenic/core/simulators.py` & `scenic-3.0.0rc1/src/scenic/core/simulators.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 Ordinary Scenic users only need to know about the top-level simulation API
 `Simulator.simulate` and the attributes of the `Simulation` class (in particular
 the ``result`` attribute, which captures information about the result of the
 simulation as a `SimulationResult` object).
 """
 
 import abc
-from collections import OrderedDict, defaultdict
+from collections import defaultdict
 import enum
 import math
 import numbers
 import time
 import types
 
 from scenic.core.distributions import RejectionException
-import scenic.core.dynamics as dynamics
+from scenic.core.dynamics import GuardViolation, RejectSimulationException
+from scenic.core.dynamics.actions import Action, _EndScenarioAction, _EndSimulationAction
 import scenic.core.errors as errors
 from scenic.core.errors import InvalidScenarioError, optionallyDebugRejection
 from scenic.core.object_types import (
     Object2D,
     disableDynamicProxyFor,
     enableDynamicProxyFor,
     setDynamicProxyFor,
@@ -50,29 +51,23 @@
 
 class DivergenceError(Exception):
     """Exception indicating simulation replay failed due to simulator nondeterminism."""
 
     pass
 
 
-class RejectSimulationException(Exception):
-    """Exception indicating a requirement was violated at runtime."""
-
-    pass
-
-
 class Simulator(abc.ABC):
     """A simulator which can execute dynamic simulations from Scenic scenes.
 
     Simulator interfaces which support dynamic simulations should implement a
     subclass of `Simulator`. An instance of the class represents a connection to
     the simulator suitable for running multiple simulations (not necessarily of
-    the same Scenic program). For a simple example of how to implement this class,
+    the same Scenic program). For an example of how to implement this class,
     and its counterpart `Simulation` for individual simulations, see
-    :mod:`scenic.simulators.lgsvl.simulator`.
+    :mod:`scenic.simulators.webots.simulator`.
 
     Users who create an instance of `Simulator` should call its `destroy` method
     when they are finished running simulations to allow the interface to do any
     necessary cleanup.
     """
 
     def __init__(self):
@@ -215,25 +210,21 @@
             simulation = self.createSimulation(
                 scene,
                 maxSteps=maxSteps,
                 name=name,
                 verbosity=verbosity,
                 **kwargs,
             )
-        except (
-            RejectSimulationException,
-            RejectionException,
-            dynamics.GuardViolation,
-        ) as e:
+        except (RejectSimulationException, RejectionException, GuardViolation) as e:
             if verbosity >= 2:
                 print(
                     f"  Rejected simulation {name} at time step "
-                    f"{simulation.currentTime} because: {e}"
+                    f"{e.simulation.currentTime} because: {e}"
                 )
-            if raiseGuardViolations and isinstance(e, dynamics.GuardViolation):
+            if raiseGuardViolations and isinstance(e, GuardViolation):
                 raise
             else:
                 optionallyDebugRejection(e)
                 return None
 
         # Completed the simulation without violating a requirement
         if not isinstance(simulation, Simulation):
@@ -299,15 +290,18 @@
         that ``maxIterations`` is omitted.
 
     Attributes:
         currentTime (int): Number of time steps elapsed so far.
         timestep (float): Length of each time step in seconds.
         objects: List of Scenic objects (instances of `Object`) existing in the
             simulation. This list will change if objects are created dynamically.
-        agents: List of :term:`agents` in the simulation.
+        agents: List of :term:`agents` in the simulation. An agent is any object that has
+            or had a behavior at any point in the simulation. The agents list may have objects
+            appended to the end as the simulation progresses (if a non-agent object has its
+            behavior overridden), but once an object is in the agents list its position is fixed.
         result (`SimulationResult`): Result of the simulation, or `None` if it has not
             yet completed. This is the primary object which should be inspected to get
             data out of the simulation: the other undocumented attributes of this class
             are for internal use only.
 
     Raises:
         RejectSimulationException: if a requirement is violated.
@@ -336,15 +330,14 @@
         divergenceTolerance=0,
         continueAfterDivergence=False,
         verbosity=0,
     ):
         self.result = None
         self.scene = scene
         self.objects = []
-        self.agents = []
         self.trajectory = []
         self.records = defaultdict(list)
         self.currentTime = 0
         self.timestep = 1 if timestep is None else float(timestep)
         self.verbosity = verbosity
         self.name = name
         self.worker_num = 0
@@ -393,21 +386,25 @@
                 self.trajectory,
                 self.actionSequence,
                 terminationType,
                 terminationReason,
                 self.records,
             )
             self.result = result
-            return self
+        except (RejectSimulationException, RejectionException, GuardViolation) as e:
+            # This simulation will be thrown out, but attach it to the exception
+            # to aid in debugging.
+            e.simulation = self
+            raise
         finally:
             self.destroy()
             for obj in self.objects:
                 disableDynamicProxyFor(obj)
             for agent in self.agents:
-                if agent.behavior._isRunning:
+                if agent.behavior and agent.behavior._isRunning:
                     agent.behavior._stop()
             # If the simulation was terminated by an exception (including rejections),
             # some scenarios may still be running; we need to clean them up without
             # checking their requirements, which could raise rejection exceptions.
             for scenario in tuple(reversed(veneer.runningScenarios)):
                 scenario._stop("exception", quiet=True)
             veneer.endSimulation(self)
@@ -442,25 +439,40 @@
                 return terminationType, terminationReason
             terminationReason = dynamicScenario._checkSimulationTerminationConditions()
             if terminationReason is not None:
                 return TerminationType.simulationTerminationCondition, terminationReason
             if maxSteps and self.currentTime >= maxSteps:
                 return TerminationType.timeLimit, f"reached time limit ({maxSteps} steps)"
 
+            # Clear lastActions for all objects
+            for obj in self.objects:
+                obj.lastActions = tuple()
+
+            # Update agents with any objects that now have behaviors (and are not already agents)
+            self.agents += [
+                obj for obj in self.objects if obj.behavior and obj not in self.agents
+            ]
+
             # Compute the actions of the agents in this time step
-            allActions = OrderedDict()
+            allActions = defaultdict(tuple)
             schedule = self.scheduleForAgents()
+            if not set(self.agents) == set(schedule):
+                raise RuntimeError("Simulator schedule does not contain all agents")
             for agent in schedule:
+                # If agent doesn't have a behavior right now, continue
+                if not agent.behavior:
+                    continue
+
                 # Run the agent's behavior to get its actions
                 actions = agent.behavior._step()
 
                 # Handle pseudo-actions marking the end of a simulation/scenario
-                if isinstance(actions, EndSimulationAction):
+                if isinstance(actions, _EndSimulationAction):
                     return TerminationType.terminatedByBehavior, str(actions)
-                elif isinstance(actions, EndScenarioAction):
+                elif isinstance(actions, _EndScenarioAction):
                     scenario = actions.scenario
                     if scenario._isRunning:
                         scenario._stop(actions)
                     if scenario is dynamicScenario:
                         # Top-level scenario was terminated, so whole simulation will end.
                         return TerminationType.terminatedByBehavior, str(actions)
                     actions = ()
@@ -473,19 +485,21 @@
                     raise InvalidScenarioError(
                         f"agent {agent} tried incompatible action(s) {actions}"
                     )
 
                 # Save actions for execution below
                 allActions[agent] = actions
 
+                # Log lastActions
+                agent.lastActions = actions
+
             # Execute the actions
             if self.verbosity >= 3:
                 for agent, actions in allActions.items():
                     print(f"      Agent {agent} takes action(s) {actions}")
-                    agent.lastActions = actions
             self.actionSequence.append(allActions)
             self.executeActions(allActions)
 
             # Run the simulation for a single step and read its state back into Scenic
             self.step()
             self.currentTime += 1
             self.updateObjects()
@@ -493,14 +507,15 @@
     def setup(self):
         """Set up the simulation to run in the simulator.
 
         Subclasses may override this method to perform custom initialization,
         but should call the parent implementation to create the objects in the
         initial scene (through `createObjectInSimulator`).
         """
+        self.agents = []
         for obj in self.scene.objects:
             self._createObject(obj)
 
     def initializeReplay(self, replay, enableReplay, enableDivergenceCheck, allowPickle):
         if replay:
             self.replaying = True
             self._replayIn = Serializer(replay, allowPickle=allowPickle, detectEnd=True)
@@ -625,17 +640,17 @@
         The default implementation calls the `applyTo` method of each `Action` to apply
         it to the appropriate agent.
         Subclasses may override this method to make additional simulator API calls as
         needed, but should call this implementation too or otherwise emulate its
         functionality.
 
         Args:
-            allActions: an :obj:`~collections.OrderedDict` mapping each agent to a tuple
-                of actions. The order of agents in the dict should be respected in case
-                the order of actions matters.
+            allActions: a :obj:`~collections.defaultdict` mapping each agent to a tuple
+                of actions, with the default value being an empty tuple. The order of
+                agents in the dict should be respected in case the order of actions matters.
         """
         for agent, actions in allActions.items():
             for action in actions:
                 action.applyTo(agent, self)
 
     @abc.abstractmethod
     def step(self):
@@ -649,20 +664,21 @@
     def updateObjects(self):
         """Update the positions and other properties of objects from the simulation.
 
         Subclasses likely do not need to override this method: they should implement its
         subroutine `getProperties` below.
         """
         for obj in self.objects:
-            # Get latest values of dynamic properties from simulation
+            # Get latest values of dynamic properties from simulation and assign them
             dynTypes = obj._simulatorProvidedProperties
             properties = set(dynTypes)
             values = self.getProperties(obj, properties)
             assert properties == set(values), properties ^ set(values)
             for prop, value in values.items():
+                # Check new value has the expected type
                 ty = dynTypes[prop]
                 if ty is float and isinstance(value, numbers.Real):
                     # Special case for scalars so that we don't penalize simulator interfaces
                     # for returning ints, NumPy scalar types, etc.
                     value = float(value)
                 elif ty is type(None):
                     # Special case for properties with initial value None: the simulator sets
@@ -673,14 +689,17 @@
                     actual = type(value).__name__
                     expected = ty.__name__
                     raise RuntimeError(
                         f'simulator provided value for property "{prop}" '
                         f"with type {actual} instead of expected {expected}"
                     )
 
+                # Assign the new value
+                setattr(obj, prop, value)
+
             # If saving a replay with divergence-checking support, save all the new values;
             # if running a replay with such support, check for divergence.
             if self._replayOut and self._writeDivergenceData:
                 for prop, ty in dynTypes.items():
                     self._replayOut.writeValue(values[prop], ty)
             if self.replayCanContinue() and self._checkDivergence:
                 for prop, ty in dynTypes.items():
@@ -698,21 +717,20 @@
                                     f"{self.currentTime} ({msg})"
                                 )
                             self.replaying = False
                             break
                         else:
                             raise DivergenceError(msg)
 
-            # Preserve some other properties which are assigned internally by Scenic
-            for prop in self.mutableProperties(obj):
-                values[prop] = getattr(obj, prop)
-
-            # Make a new copy of the object to ensure that computed properties like
-            # visibleRegion, etc. are recomputed
-            setDynamicProxyFor(obj, obj._copyWith(**values))
+            # Recompute dynamic final properties
+            obj._recomputeDynamicFinals()
+
+            # Clear caches to ensure that cached properties like visibleRegion, etc.
+            # are recomputed
+            obj._clearCaches()
 
     def valuesHaveDiverged(self, obj, prop, expected, actual):
         """Decide whether the value of a dynamic property has diverged from the replay.
 
         The default implementation considers scalar and vector properties to have diverged
         if the distance between the actual and expected values is greater than
         ``self.divergenceTolerance`` (which is 0 by default); other types of properties
@@ -737,17 +755,14 @@
         elif isinstance(expected, Vector):
             diff = (actual - expected).norm()
         if diff:
             return diff > self.divergenceTolerance
         else:
             return actual != expected
 
-    def mutableProperties(self, obj):
-        return {"lastActions", "behavior"}
-
     @abc.abstractmethod
     def getProperties(self, obj, properties):
         """Read the values of the given properties of the object from the simulator.
 
         Implemented by subclasses.
 
         Args:
@@ -845,76 +860,14 @@
         )
         for prop in properties:
             if prop not in vals:
                 vals[prop] = None
         return vals
 
 
-class Action(abc.ABC):
-    """An :term:`action` which can be taken by an agent for one step of a simulation."""
-
-    def canBeTakenBy(self, agent):
-        """Whether this action is allowed to be taken by the given agent.
-
-        The default implementation always returns True.
-        """
-        return True
-
-    @abc.abstractmethod
-    def applyTo(self, agent, simulation):
-        """Apply this action to the given agent in the given simulation.
-
-        This method should call simulator APIs so that the agent will take this action
-        during the next simulated time step. Depending on the simulator API, it may be
-        necessary to batch each agent's actions into a single update: in that case you
-        can have this method set some state on the agent, then apply the actual update
-        in an overridden implementation of `Simulation.executeActions`. For examples,
-        see the CARLA interface: `scenic.simulators.carla.actions` has some CARLA-specific
-        actions which directly call CARLA APIs, while the generic steering and braking
-        actions from `scenic.domains.driving.actions` are implemented using the batching
-        approach (see for example the ``setThrottle`` method of the class
-        `scenic.simulators.carla.model.Vehicle`, which sets state later read by
-        ``CarlaSimulation.executeActions`` in `scenic.simulators.carla.simulator`).
-        """
-        raise NotImplementedError
-
-
-class EndSimulationAction(Action):
-    """Special action indicating it is time to end the simulation.
-
-    Only for internal use.
-    """
-
-    def __init__(self, line):
-        self.line = line
-
-    def __str__(self):
-        return f'"terminate simulation" executed on line {self.line}'
-
-    def applyTo(self, agent, simulation):
-        assert False
-
-
-class EndScenarioAction(Action):
-    """Special action indicating it is time to end the current scenario.
-
-    Only for internal use.
-    """
-
-    def __init__(self, scenario, line):
-        self.scenario = scenario
-        self.line = line
-
-    def __str__(self):
-        return f'"terminate" executed on line {self.line}'
-
-    def applyTo(self, agent, simulation):
-        assert False
-
-
 @enum.unique
 class TerminationType(enum.Enum):
     """Enum describing the possible ways a simulation can end."""
 
     #: Simulation reached the specified time limit.
     timeLimit = "reached simulation time limit"
```

### Comparing `scenic-3.0.0b2/src/scenic/core/specifiers.py` & `scenic-3.0.0rc1/src/scenic/core/specifiers.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,16 @@
                 return default
 
         self.isAdditive = enabled("additive", False)
         self.isDynamic = enabled("dynamic", False)
         self.isFinal = enabled("final", False)
         for attr in attributes:
             raise RuntimeError(f'unknown property attribute "{attr}"')
+        if self.isAdditive and self.isDynamic:
+            raise InvalidScenarioError("additive properties cannot be dynamic")
 
     @staticmethod
     def forValue(value):
         if isinstance(value, PropertyDefault):
             return value
         else:
             return PropertyDefault(set(), set(), lambda self: value)
```

### Comparing `scenic-3.0.0b2/src/scenic/core/type_support.py` & `scenic-3.0.0rc1/src/scenic/core/type_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,20 +150,20 @@
         )
     elif hasattr(typeB, "_canCoerceType"):
         return typeB._canCoerceType(typeA)
     else:
         return issubclass(typeA, typeB)
 
 
-def canCoerce(thing, ty):
+def canCoerce(thing, ty, exact=False):
     """Can this value be coerced into the given type?"""
     tt = underlyingType(thing)
     if canCoerceType(tt, ty):
         return True
-    elif isinstance(thing, Distribution):
+    elif (not exact) and isinstance(thing, Distribution):
         return True  # fall back on type-checking at runtime
     else:
         return False
 
 
 def coerce(thing, ty, error="wrong type"):
     """Coerce something into the given type.
@@ -255,14 +255,16 @@
     Only for internal use by the typechecking system; introduced by `coerce` when it is
     unable to guarantee that a random value will have the correct type after sampling.
     Note that the type check is not a purely passive operation, and may actually
     transform the sampled value according to the coercion rules above (e.g. a sampled
     `Point` will be converted to a `Vector` in a context which expects the latter).
     """
 
+    _deterministic = True
+
     def __init__(self, dist, ty, errorMessage, coercer=None):
         super().__init__(dist, valueType=ty)
         self._dist = dist
         self._errorMessage = errorMessage
         self._coercer = coercer
         if not coercer:
             # Erase any type parameters, which we don't attempt to check
```

### Comparing `scenic-3.0.0b2/src/scenic/core/type_support/.DS_Store` & `scenic-3.0.0rc1/src/scenic/core/type_support/.DS_Store`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/core/vectors.py` & `scenic-3.0.0rc1/src/scenic/core/vectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,27 +307,38 @@
         return canCoerceType(ty, float) or hasattr(ty, "toOrientation")
 
     @cached_property
     def eulerAngles(self) -> typing.Tuple[float, float, float]:
         """Global intrinsic Euler angles yaw, pitch, roll."""
         return self.r.as_euler("ZXY", degrees=False)
 
+    def _trimeshEulerAngles(self):
+        return self.r.as_euler("xyz", degrees=False)
+
     def getRotation(self):
         return self.r
 
     @cached_property
     def inverse(self) -> Orientation:
         return Orientation(self.r.inv())
 
     @cached_property
     def _inverseRotation(self):
         return self.r.inv()
 
     # will be converted to a distributionMethod after the class definition
     def __mul__(self, other) -> Orientation:
+        """Apply a rotation to this orientation, yielding a new orientation.
+
+        As we represent orientations as intrinsic rotations, rotation A followed by rotation B is
+        given by the quaternion product A*B, not B*A.
+
+        See https://en.wikipedia.org/wiki/Davenport_chained_rotations#Conversion_to_extrinsic_rotations
+        for more details.
+        """
         if type(other) is not Orientation:
             return NotImplemented
         # Preserve existing orientation objects when possible to help pruning.
         if self == globalOrientation:
             return other
         if other == globalOrientation:
             return self
@@ -335,38 +346,38 @@
 
     @distributionMethod
     def __add__(self, other) -> Orientation:
         if isinstance(other, (float, int)):
             other = Orientation._fromHeading(other)
         elif type(other) is not Orientation:
             return NotImplemented
-        return other * self
+        return self * other
 
     @distributionMethod
     def __radd__(self, other) -> Orientation:
         if isinstance(other, (float, int)):
             other = Orientation._fromHeading(other)
         elif type(other) is not Orientation:
             return NotImplemented
-        return self * other
+        return other * self
 
     def __repr__(self):
         return f"Orientation.fromEuler{tuple(self.eulerAngles)!r}"
 
     def __hash__(self):
         return hash(tuple(self.q)) + hash(tuple(-self.q))
 
     @distributionFunction
     def localAnglesFor(self, orientation) -> typing.Tuple[float, float, float]:
         """Get local Euler angles for an orientation w.r.t. this orientation.
 
         That is, considering ``self`` as the parent orientation, find the Euler angles
         expressing the given orientation.
         """
-        local = orientation * self.inverse
+        local = self.inverse * orientation
         return local.eulerAngles
 
     @distributionFunction
     def globalToLocalAngles(self, yaw, pitch, roll) -> typing.Tuple[float, float, float]:
         """Convert global Euler angles to local angles w.r.t. this orientation.
 
         Equivalent to `localAnglesFor` but takes Euler angles as input.
@@ -380,14 +391,26 @@
         return numpy.array_equal(self.q, other.q) or numpy.array_equal(self.q, -other.q)
 
     def approxEq(self, other, tol=1e-10):
         if not isinstance(other, Orientation):
             return NotImplemented
         return abs(numpy.dot(self.q, other.q)) > 1 - tol
 
+    @classmethod
+    def encodeTo(cls, orientation, stream):
+        stream.write(struct.pack("<dddd", *orientation.q))
+
+    @classmethod
+    def decodeFrom(cls, stream):
+        # Quaternion constructor does not roundtrip so we manually
+        # construct a rotation and pass that in.
+        quaternion = struct.unpack("<dddd", stream.read(32))
+        rotation = Rotation(quaternion, normalize=False)
+        return cls(rotation)
+
 
 globalOrientation = Orientation.fromEuler(0, 0, 0)
 
 Orientation.__mul__ = distributionMethod(Orientation.__mul__, identity=globalOrientation)
 
 
 def alwaysGlobalOrientation(orientation):
```

### Comparing `scenic-3.0.0b2/src/scenic/core/visibility.py` & `scenic-3.0.0rc1/src/scenic/core/visibility.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/core/workspaces.py` & `scenic-3.0.0rc1/src/scenic/core/workspaces.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/domains/.DS_Store` & `scenic-3.0.0rc1/src/scenic/domains/.DS_Store`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/domains/driving/__init__.py` & `scenic-3.0.0rc1/src/scenic/domains/driving/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Domain for driving scenarios.
 
+This domain must currently be used in `2D compatibility mode`.
+
 The :doc:`world model <scenic.domains.driving.model>` defines Scenic classes for cars,
 pedestrians, etc., actions for dynamic agents which walk or drive, as well as simple
 behaviors like lane-following. Scenarios for the driving domain should import the model
 as follows::
 
     model scenic.domains.driving.model
```

### Comparing `scenic-3.0.0b2/src/scenic/domains/driving/actions.py` & `scenic-3.0.0rc1/src/scenic/domains/driving/actions.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/domains/driving/behaviors.scenic` & `scenic-3.0.0rc1/src/scenic/domains/driving/behaviors.scenic`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/domains/driving/controllers.py` & `scenic-3.0.0rc1/src/scenic/domains/driving/controllers.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/domains/driving/model.scenic` & `scenic-3.0.0rc1/src/scenic/domains/driving/model.scenic`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,22 @@
     param map_options = { 'tolerance': 0.1 }
     model scenic.domains.driving.model
 
 If you are writing a generic scenario that supports multiple maps, you may leave the
 ``map`` parameter undefined; then running the scenario will produce an error unless the
 user uses the :option:`--param` command-line option to specify the map.
 
+The ``use2DMap`` global parameter determines whether or not maps are generated in 2D. Currently
+3D maps are not supported, but are under development. By default, this parameter is `False`
+(so that future versions of Scenic will automatically use 3D maps), unless
+:ref:`2D compatibility mode` is enabled, in which case the default is `True`. The parameter
+can be manually set to `True` to ensure 2D maps are used even if the scenario is not compiled
+in 2D compatibility mode.
+
+
 .. note::
 
     If you are using a simulator, you may have to also define simulator-specific global
     parameters to tell the simulator which world to load. For example, our LGSVL
     interface uses a parameter ``lgsvl_map`` to specify the name of the Unity scene.
     See the :doc:`documentation <scenic.simulators>` of the simulator interfaces for
     details.
@@ -34,14 +42,30 @@
                                           NetworkElement)
 from scenic.domains.driving.actions import *
 from scenic.domains.driving.behaviors import *
 
 from scenic.core.distributions import RejectionException
 from scenic.simulators.utils.colors import Color
 
+## 2D mode flag & checks
+
+def is2DMode():
+    from scenic.syntax.veneer import mode2D
+    return mode2D
+
+param use2DMap = True if is2DMode() else False
+
+if is2DMode() and not globalParameters.use2DMap:
+    raise RuntimeError('in 2D mode, global parameter "use2DMap" must be True')
+
+# Note: The following should be removed when 3D maps are supported
+if not globalParameters.use2DMap:
+    raise RuntimeError('3D maps not supported at this time.'
+        '(to use 2D maps set global parameter "use2DMap" to True)')
+
 ## Load map and set up workspace
 
 if 'map' not in globalParameters:
     raise RuntimeError('need to specify map before importing driving model '
                        '(set the global parameter "map")')
 param map_options = {}
 
@@ -76,18 +100,14 @@
 #: Inside intersections or anywhere else where there can be multiple nominal
 #: traffic directions, the choice is arbitrary. At such points, the function
 #: `Network.nominalDirectionsAt` can be used to get all nominal directions.
 roadDirection : VectorField = network.roadDirection
 
 ## Standard object types
 
-def is2DMode():
-    from scenic.syntax.veneer import mode2D
-    return mode2D
-
 class DrivingObject:
     """Abstract class for objects in a road network.
 
     Provides convenience properties for the lane, road, intersection, etc. at the
     object's current position (if any).
 
     Also defines the ``elevation`` property as a standard way to access the Z
@@ -246,29 +266,29 @@
         raise NotImplementedError
 
 class Vehicle(DrivingObject):
     """Vehicles which drive, such as cars.
 
     Properties:
         position: The default position is uniformly random over the `road`.
-        heading: The default heading is aligned with `roadDirection`, plus an offset
+        parentOrientation: The default parentOrientation is aligned with `roadDirection`, plus an offset
             given by **roadDeviation**.
         roadDeviation (float): Relative heading with respect to the road direction at
-            the `Vehicle`'s position. Used by the default value for **heading**.
+            the `Vehicle`'s position. Used by the default value for **parentOrientation**.
         regionContainedIn: The default container is :obj:`roadOrShoulder`.
         viewAngle: The default view angle is 90 degrees.
         width: The default width is 2 meters.
         length: The default length is 4.5 meters.
         color (:obj:`Color` or RGB tuple): Color of the vehicle. The default value is a
             distribution derived from car color popularity statistics; see
             :obj:`Color.defaultCarColor`.
     """
     regionContainedIn: roadOrShoulder
     position: new Point on road
-    heading: (roadDirection at self.position) + self.roadDeviation
+    parentOrientation: (roadDirection at self.position) + self.roadDeviation
     roadDeviation: 0
     viewAngle: 90 deg
     width: 2
     length: 4.5
     color: Color.defaultCarColor()
 
     @property
@@ -286,24 +306,24 @@
     pass
 
 class Pedestrian(DrivingObject):
     """A pedestrian.
 
     Properties:
         position: The default position is uniformly random over sidewalks and crosswalks.
-        heading: The default heading is uniformly random.
+        parentOrientation: The default parentOrientation has uniformly random yaw.
         viewAngle: The default view angle is 90 degrees.
         width: The default width is 0.75 m.
         length: The default length is 0.75 m.
         color: The default color is turquoise. Pedestrian colors are not necessarily
             used by simulators, but do appear in the debugging diagram.
     """
     regionContainedIn: network.walkableRegion
     position: new Point on network.walkableRegion
-    heading: Range(0, 360) deg
+    parentOrientation: Range(0, 360) deg
     viewAngle: 90 deg
     width: 0.75
     length: 0.75
     color: [0, 0.5, 1]
 
 ## Utility functions
```

### Comparing `scenic-3.0.0b2/src/scenic/domains/driving/roads.py` & `scenic-3.0.0rc1/src/scenic/domains/driving/roads.py`

 * *Files 1% similar despite different names*

```diff
@@ -514,14 +514,21 @@
     # associated elements not actually part of this group
     _sidewalk: Union[Sidewalk, None] = None  #: Adjacent sidewalk, if any.
     _bikeLane: Union[Lane, None] = None
     _shoulder: Union[Shoulder, None] = None  #: Adjacent shoulder, if any.
     #: Opposite lane group of the same road, if any.
     _opposite: Union[LaneGroup, None] = None
 
+    def __attrs_post_init__(self):
+        super().__attrs_post_init__()
+
+        # Ensure lanes do not overlap
+        for i in range(len(self.lanes) - 1):
+            assert not self.lanes[i].polygon.overlaps(self.lanes[i + 1].polygon)
+
     @property
     def sidewalk(self) -> Sidewalk:
         """The adjacent sidewalk; rejects if there is none."""
         return _rejectIfNonexistent(self._sidewalk, "sidewalk")
 
     @property
     def bikeLane(self) -> Lane:
@@ -611,14 +618,18 @@
             ids = {}
             for i, lane in enumerate(self.forwardLanes, start=1):
                 ids[-i] = lane
             for i, lane in enumerate(self.backwardLanes, start=1):
                 ids[i] = lane
             self.lanesByOpenDriveID = ids
 
+        # Ensure lanes do not overlap
+        for i in range(len(self.lanes) - 1):
+            assert not self.lanes[i].polygon.overlaps(self.lanes[i + 1].polygon)
+
     def _defaultHeadingAt(self, point):
         point = _toVector(point)
         lane = self.laneAt(point)
         if lane:
             return lane.orientation[point]
         return super()._defaultHeadingAt(point)
 
@@ -908,19 +919,28 @@
             self.crossingRegion = PolygonalRegion.unionAll(self.crossings)
         if self.sidewalkRegion is None:
             self.sidewalkRegion = PolygonalRegion.unionAll(self.sidewalks)
         if self.shoulderRegion is None:
             self.shoulderRegion = PolygonalRegion.unionAll(self.shoulders)
 
         if self.drivableRegion is None:
-            self.drivableRegion = self.laneRegion.union(self.intersectionRegion)
+            self.drivableRegion = PolygonalRegion.unionAll(
+                (
+                    self.laneRegion,
+                    self.roadRegion,  # can contain points slightly outside laneRegion
+                    self.intersectionRegion,
+                )
+            )
         assert self.drivableRegion.containsRegion(
             self.laneRegion, tolerance=self.tolerance
         )
         assert self.drivableRegion.containsRegion(
+            self.roadRegion, tolerance=self.tolerance
+        )
+        assert self.drivableRegion.containsRegion(
             self.intersectionRegion, tolerance=self.tolerance
         )
         if self.walkableRegion is None:
             self.walkableRegion = self.sidewalkRegion.union(self.crossingRegion)
         assert self.walkableRegion.containsRegion(
             self.sidewalkRegion, tolerance=self.tolerance
         )
@@ -965,15 +985,15 @@
         attributes of the underlying Regions, or the serialization process itself are
         changed, so that cached networks will be properly regenerated (rather than being
         unpickled in an inconsistent state and causing errors later). Changes to the map
         geometry calculations should be included, even if the format itself is unchanged.
 
         :meta private:
         """
-        return 29
+        return 33
 
     class DigestMismatchError(Exception):
         """Exception raised when loading a cached map not matching the original file."""
 
         pass
 
     @classmethod
```

### Comparing `scenic-3.0.0b2/src/scenic/domains/driving/simulators.py` & `scenic-3.0.0rc1/src/scenic/domains/driving/simulators.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/formats/.DS_Store` & `scenic-3.0.0rc1/src/scenic/formats/.DS_Store`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/formats/opendrive/workspace.py` & `scenic-3.0.0rc1/src/scenic/formats/opendrive/workspace.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/formats/opendrive/xodr_parser.py` & `scenic-3.0.0rc1/src/scenic/formats/opendrive/xodr_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -565,25 +565,52 @@
                     next_lane_polys[id_] = cur_lane_polys.pop(pred_id) + [
                         cur_sec_lane_polys[id_]
                     ]
                 else:
                     next_lane_polys[id_] = [cur_sec_lane_polys[id_]]
             for id_ in cur_lane_polys:
                 poly = buffer_union(cur_lane_polys[id_], tolerance=tolerance)
+                self.lane_secs[i - 1].get_lane(id_).parent_lane_poly = len(lane_polys)
                 lane_polys.append(poly)
-                self.lane_secs[i - 1].get_lane(id_).parent_lane_poly = poly
             cur_lane_polys = next_lane_polys
         for id_ in cur_lane_polys:
             poly = buffer_union(cur_lane_polys[id_], tolerance=tolerance)
+            cur_sec.get_lane(id_).parent_lane_poly = len(lane_polys)
             lane_polys.append(poly)
-            cur_sec.get_lane(id_).parent_lane_poly = poly
         union_poly = buffer_union(sec_polys, tolerance=tolerance)
         if last_lefts and last_rights:
             self.end_bounds_left.update(last_lefts)
             self.end_bounds_right.update(last_rights)
+
+        # Difference and slightly erode all overlapping polygons
+        for i in range(len(sec_polys) - 1):
+            if sec_polys[i].overlaps(sec_polys[i + 1]):
+                sec_polys[i] = sec_polys[i].difference(sec_polys[i + 1]).buffer(-1e-6)
+                assert not sec_polys[i].overlaps(sec_polys[i + 1])
+
+        for polys in sec_lane_polys:
+            ids = sorted(polys)  # order adjacent lanes consecutively
+            for i in range(len(ids) - 1):
+                polyA, polyB = polys[ids[i]], polys[ids[i + 1]]
+                if polyA.overlaps(polyB):
+                    polys[ids[i]] = polyA.difference(polyB).buffer(-1e-6)
+                    assert not polys[ids[i]].overlaps(polyB)
+
+        for i in range(len(lane_polys) - 1):
+            if lane_polys[i].overlaps(lane_polys[i + 1]):
+                lane_polys[i] = lane_polys[i].difference(lane_polys[i + 1]).buffer(-1e-6)
+                assert not lane_polys[i].overlaps(lane_polys[i + 1])
+
+        # Set parent lane polygon references to corrected polygons
+        for sec in self.lane_secs:
+            for lane in sec.lanes.values():
+                parentIndex = lane.parent_lane_poly
+                if isinstance(parentIndex, int):
+                    lane.parent_lane_poly = lane_polys[parentIndex]
+
         return (sec_points, sec_polys, sec_lane_polys, lane_polys, union_poly)
 
     def calculate_geometry(
         self,
         num,
         tolerance,
         calc_gap,
```

### Comparing `scenic-3.0.0b2/src/scenic/simulators/.DS_Store` & `scenic-3.0.0rc1/src/scenic/simulators/.DS_Store`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/carla/.DS_Store` & `scenic-3.0.0rc1/src/scenic/simulators/carla/.DS_Store`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/carla/__init__.py` & `scenic-3.0.0rc1/src/scenic/simulators/carla/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Interface to the CARLA driving simulator.
 
+This interface must currently be used in `2D compatibility mode`.
+
 This interface has been tested with `CARLA <https://carla.org/>`_ versions 0.9.9,
 0.9.10, and 0.9.11.
 It supports dynamic scenarios involving vehicles, pedestrians, and props.
 
 The interface implements the :obj:`scenic.domains.driving` abstract domain, so any
 object types, behaviors, utility functions, etc. from that domain may be used freely.
 For details of additional CARLA-specific functionality, see the world model
```

### Comparing `scenic-3.0.0b2/src/scenic/simulators/carla/actions.py` & `scenic-3.0.0rc1/src/scenic/simulators/carla/actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Actions for dynamic agents in CARLA scenarios."""
 
 import math as _math
 
 import carla as _carla
 
 from scenic.domains.driving.actions import *
-import scenic.simulators.carla.model as _carlaModel
 import scenic.simulators.carla.utils.utils as _utils
 
 ################################################
 # Actions available to all carla.Actor objects #
 ################################################
 
 SetLocationAction = SetPositionAction  # TODO refactor
@@ -39,17 +38,24 @@
 
 
 #############################################
 # Actions specific to carla.Vehicle objects #
 #############################################
 
 
+class _CarlaVehicle:
+    # Mixin identifying CARLA vehicles.
+    # Used to avoid importing the Vehicle class from the CARLA model, which is
+    # a Scenic module not importable from Python.
+    pass
+
+
 class VehicleAction(Action):
     def canBeTakenBy(self, agent):
-        return isinstance(agent, _carlaModel.Vehicle)
+        return isinstance(agent, _CarlaVehicle)
 
 
 class SetManualGearShiftAction(VehicleAction):
     def __init__(self, manualGearShift):
         if not isinstance(manualGearShift, bool):
             raise RuntimeError("Manual gear shift must be a boolean.")
         self.manualGearShift = manualGearShift
@@ -127,17 +133,22 @@
 
 
 #################################################
 # Actions available to all carla.Walker objects #
 #################################################
 
 
+class _CarlaPedestrian:
+    # Mixin identifying CARLA pedestrians. (see _CarlaVehicle)
+    pass
+
+
 class PedestrianAction(Action):
     def canBeTakenBy(self, agent):
-        return isinstance(agent, _carlaModel.Pedestrian)
+        return isinstance(agent, _CarlaPedestrian)
 
 
 class SetJumpAction(PedestrianAction):
     def __init__(self, jump):
         if not isinstance(jump, bool):
             raise RuntimeError("Jump must be a boolean.")
         self.jump = jump
```

### Comparing `scenic-3.0.0b2/src/scenic/simulators/carla/behaviors.scenic` & `scenic-3.0.0rc1/src/scenic/simulators/carla/behaviors.scenic`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/carla/blueprints.scenic` & `scenic-3.0.0rc1/src/scenic/simulators/carla/blueprints.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,234 +1,233 @@
 """CARLA blueprints for cars, pedestrians, etc."""
 
 #: Mapping from current names of blueprints to ones in old CARLA versions.
 #:
 #: We provide a tuple of old names in case they change more than once.
 oldBlueprintNames = {
-      'vehicle.dodge.charger_police': ('vehicle.dodge_charger.police',),
-      'vehicle.lincoln.mkz_2017': ('vehicle.lincoln.mkz2017',),
-      'vehicle.mercedes.coupe': ('vehicle.mercedes-benz.coupe',),
-      'vehicle.mini.cooper_s': ('vehicle.mini.cooperst',),
-      'vehicle.ford.mustang': ('vehicle.mustang.mustang',),
+    "vehicle.dodge.charger_police": ("vehicle.dodge_charger.police",),
+    "vehicle.lincoln.mkz_2017": ("vehicle.lincoln.mkz2017",),
+    "vehicle.mercedes.coupe": ("vehicle.mercedes-benz.coupe",),
+    "vehicle.mini.cooper_s": ("vehicle.mini.cooperst",),
+    "vehicle.ford.mustang": ("vehicle.mustang.mustang",),
 }
 
 ## Vehicle blueprints
 
 #: blueprints for cars
 carModels = [
-      'vehicle.audi.a2',
-      'vehicle.audi.etron',
-      'vehicle.audi.tt',
-      'vehicle.bmw.grandtourer',
-      'vehicle.chevrolet.impala',
-      'vehicle.citroen.c3',
-      'vehicle.dodge.charger_police',
-      'vehicle.jeep.wrangler_rubicon', 
-      'vehicle.lincoln.mkz_2017',
-      'vehicle.mercedes.coupe',
-      'vehicle.mini.cooper_s',
-      'vehicle.ford.mustang',
-      'vehicle.nissan.micra',
-      'vehicle.nissan.patrol',
-      'vehicle.seat.leon',
-      'vehicle.tesla.model3',
-      'vehicle.toyota.prius',
-      'vehicle.volkswagen.t2'
+    "vehicle.audi.a2",
+    "vehicle.audi.etron",
+    "vehicle.audi.tt",
+    "vehicle.bmw.grandtourer",
+    "vehicle.chevrolet.impala",
+    "vehicle.citroen.c3",
+    "vehicle.dodge.charger_police",
+    "vehicle.jeep.wrangler_rubicon",
+    "vehicle.lincoln.mkz_2017",
+    "vehicle.mercedes.coupe",
+    "vehicle.mini.cooper_s",
+    "vehicle.ford.mustang",
+    "vehicle.nissan.micra",
+    "vehicle.nissan.patrol",
+    "vehicle.seat.leon",
+    "vehicle.tesla.model3",
+    "vehicle.toyota.prius",
+    "vehicle.volkswagen.t2",
 ]
 
 #: blueprints for bicycles
 bicycleModels = [
-      'vehicle.bh.crossbike',
-      'vehicle.diamondback.century',
-      'vehicle.gazelle.omafiets',
+    "vehicle.bh.crossbike",
+    "vehicle.diamondback.century",
+    "vehicle.gazelle.omafiets",
 ]
 
 #: blueprints for motorcycles
 motorcycleModels = [
-      'vehicle.harley-davidson.low_rider',
-      'vehicle.kawasaki.ninja',
-      'vehicle.yamaha.yzf',
+    "vehicle.harley-davidson.low_rider",
+    "vehicle.kawasaki.ninja",
+    "vehicle.yamaha.yzf",
 ]
 
 #: blueprints for trucks
 truckModels = [
-      'vehicle.carlamotors.carlacola',
-      'vehicle.tesla.cybertruck'
+    "vehicle.carlamotors.carlacola",
+    "vehicle.tesla.cybertruck",
 ]
 
 ## Prop blueprints
 
 #: blueprints for trash cans
 trashModels = [
-      'static.prop.trashcan01',
-      'static.prop.trashcan02',
-      'static.prop.trashcan03',
-      'static.prop.trashcan04',
-      'static.prop.trashcan05',
-      'static.prop.bin'
+    "static.prop.trashcan01",
+    "static.prop.trashcan02",
+    "static.prop.trashcan03",
+    "static.prop.trashcan04",
+    "static.prop.trashcan05",
+    "static.prop.bin",
 ]
 
 #: blueprints for traffic cones
 coneModels = [
-      'static.prop.constructioncone',
-      'static.prop.trafficcone01',
-      'static.prop.trafficcone02'
+    "static.prop.constructioncone",
+    "static.prop.trafficcone01",
+    "static.prop.trafficcone02",
 ]
 
 #: blueprints for road debris
 debrisModels = [
-      'static.prop.dirtdebris01',
-      'static.prop.dirtdebris02',
-      'static.prop.dirtdebris03'
+    "static.prop.dirtdebris01",
+    "static.prop.dirtdebris02",
+    "static.prop.dirtdebris03",
 ]
 
 #: blueprints for vending machines
 vendingMachineModels = [
-      'static.prop.vendingmachine'
+    "static.prop.vendingmachine",
 ]
 
 #: blueprints for chairs
 chairModels = [
-      'static.prop.plasticchair'
+    "static.prop.plasticchair",
 ]
 
 #: blueprints for bus stops
 busStopModels = [
-      'static.prop.busstop'
+    "static.prop.busstop",
 ]
 
 #: blueprints for roadside billboards
 advertisementModels = [
-      'static.prop.advertisement',
-      'static.prop.streetsign',
-      'static.prop.streetsign01',
-      'static.prop.streetsign04'
+    "static.prop.advertisement",
+    "static.prop.streetsign",
+    "static.prop.streetsign01",
+    "static.prop.streetsign04",
 ]
 
 #: blueprints for pieces of trash
 garbageModels = [
-      'static.prop.colacan',
-      'static.prop.garbage01',
-      'static.prop.garbage02',
-      'static.prop.garbage03',
-      'static.prop.garbage04',
-      'static.prop.garbage05',
-      'static.prop.garbage06',
-      'static.prop.plasticbag',
-      'static.prop.trashbag'
+    "static.prop.colacan",
+    "static.prop.garbage01",
+    "static.prop.garbage02",
+    "static.prop.garbage03",
+    "static.prop.garbage04",
+    "static.prop.garbage05",
+    "static.prop.garbage06",
+    "static.prop.plasticbag",
+    "static.prop.trashbag",
 ]
 
 #: blueprints for containers
 containerModels = [
-      'static.prop.container',
-      'static.prop.clothcontainer',
-      'static.prop.glasscontainer'
+    "static.prop.container",
+    "static.prop.clothcontainer",
+    "static.prop.glasscontainer",
 ]
 
 #: blueprints for tables
 tableModels = [
-      'static.prop.table',
-      'static.prop.plastictable'
+    "static.prop.table",
+    "static.prop.plastictable",
 ]
 
 #: blueprints for traffic barriers
 barrierModels = [
-      'static.prop.streetbarrier',
-      'static.prop.chainbarrier',
-      'static.prop.chainbarrierend'
+    "static.prop.streetbarrier",
+    "static.prop.chainbarrier",
+    "static.prop.chainbarrierend",
 ]
 
 #: blueprints for flowerpots
 plantpotModels = [
-      'static.prop.plantpot01',
-      'static.prop.plantpot02',
-      'static.prop.plantpot03',
-      'static.prop.plantpot04',
-      'static.prop.plantpot05',
-      'static.prop.plantpot06',
-      'static.prop.plantpot07',
-      'static.prop.plantpot08'
+    "static.prop.plantpot01",
+    "static.prop.plantpot02",
+    "static.prop.plantpot03",
+    "static.prop.plantpot04",
+    "static.prop.plantpot05",
+    "static.prop.plantpot06",
+    "static.prop.plantpot07",
+    "static.prop.plantpot08",
 ]
 
 #: blueprints for mailboxes
 mailboxModels = [
-      'static.prop.mailbox'
+    "static.prop.mailbox",
 ]
 
 #: blueprints for garden gnomes
 gnomeModels = [
-      'static.prop.gnome'
+    "static.prop.gnome",
 ]
 
 #: blueprints for creased boxes
 creasedboxModels = [
-      'static.prop.creasedbox01',
-      'static.prop.creasedbox02',
-      'static.prop.creasedbox03'
+    "static.prop.creasedbox01",
+    "static.prop.creasedbox02",
+    "static.prop.creasedbox03",
 ]
 
 #: blueprints for briefcases, suitcases, etc.
 caseModels = [
-      'static.prop.travelcase',
-      'static.prop.briefcase',
-      'static.prop.guitarcase'
+    "static.prop.travelcase",
+    "static.prop.briefcase",
+    "static.prop.guitarcase",
 ]
 
 #: blueprints for boxes
 boxModels = [
-      'static.prop.box01',
-      'static.prop.box02',
-      'static.prop.box03'
+    "static.prop.box01",
+    "static.prop.box02",
+    "static.prop.box03",
 ]
 
 #: blueprints for benches
 benchModels = [
-      'static.prop.bench01',
-      'static.prop.bench02',
-      'static.prop.bench03'
+    "static.prop.bench01",
+    "static.prop.bench02",
+    "static.prop.bench03",
 ]
 
 #: blueprints for barrels
 barrelModels = [
-      'static.prop.barrel'
+    "static.prop.barrel",
 ]
 
 #: blueprints for ATMs
 atmModels = [
-      'static.prop.atm'
+    "static.prop.atm",
 ]
 
 #: blueprints for kiosks
 kioskModels = [
-      'static.prop.kiosk_01'
+    "static.prop.kiosk_01",
 ]
 
 #: blueprints for iron plates
 ironplateModels = [
-      'static.prop.ironplank'
+    "static.prop.ironplank",
 ]
 
 #: blueprints for traffic warning signs
 trafficwarningModels = [
-      'static.prop.trafficwarning'
+    "static.prop.trafficwarning",
 ]
 
 ## Walker blueprints
 
 #: blueprints for pedestrians
 walkerModels = [
-      'walker.pedestrian.0001',
-      'walker.pedestrian.0002',
-      'walker.pedestrian.0003',
-      'walker.pedestrian.0004',
-      'walker.pedestrian.0005',
-      'walker.pedestrian.0006',
-      'walker.pedestrian.0007',
-      'walker.pedestrian.0008',
-      'walker.pedestrian.0009',
-      'walker.pedestrian.0010',
-      'walker.pedestrian.0011',
-      'walker.pedestrian.0012',
-      'walker.pedestrian.0013',
-      'walker.pedestrian.0014'
+    "walker.pedestrian.0001",
+    "walker.pedestrian.0002",
+    "walker.pedestrian.0003",
+    "walker.pedestrian.0004",
+    "walker.pedestrian.0005",
+    "walker.pedestrian.0006",
+    "walker.pedestrian.0007",
+    "walker.pedestrian.0008",
+    "walker.pedestrian.0009",
+    "walker.pedestrian.0010",
+    "walker.pedestrian.0011",
+    "walker.pedestrian.0012",
+    "walker.pedestrian.0013",
+    "walker.pedestrian.0014",
 ]
-
```

### Comparing `scenic-3.0.0b2/src/scenic/simulators/carla/misc.py` & `scenic-3.0.0rc1/src/scenic/simulators/carla/misc.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/carla/model.scenic` & `scenic-3.0.0rc1/src/scenic/simulators/carla/model.scenic`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 Global Parameters:
     carla_map (str): Name of the CARLA map to use, e.g. 'Town01'. Can also be set
         to ``None``, in which case CARLA will attempt to create a world from the
         **map** file used in the scenario (which must be an ``.xodr`` file).
     timestep (float): Timestep to use for simulations (i.e., how frequently Scenic
         interrupts CARLA to run behaviors, check requirements, etc.), in seconds. Default
         is 0.1 seconds.
+    snapToGroundDefault (bool): Default value for :prop:`snapToGround` on `CarlaActor` objects.
+        Default is True if :ref:`2D compatibility mode` is enabled and False otherwise. 
 
     weather (str or dict): Weather to use for the simulation. Can be either a
         string identifying one of the CARLA weather presets (e.g. 'ClearSunset') or a
         dictionary specifying all the weather parameters (see `carla.WeatherParameters`_).
         Default is a uniform distribution over all the weather presets.
 
     address (str): IP address at which to connect to CARLA. Default is localhost
@@ -35,24 +37,25 @@
         for no. Default 1.
     record (str): If nonempty, folder in which to save CARLA record files for
         replaying the simulations.
 
 .. _carla.WeatherParameters: https://carla.readthedocs.io/en/latest/python_api/#carlaweatherparameters
 
 """
-
+import pathlib
 from scenic.domains.driving.model import *
 
 import scenic.simulators.carla.blueprints as blueprints
 from scenic.simulators.carla.behaviors import *
 from scenic.simulators.utils.colors import Color
 
 try:
     from scenic.simulators.carla.simulator import CarlaSimulator    # for use in scenarios
     from scenic.simulators.carla.actions import *
+    from scenic.simulators.carla.actions import _CarlaVehicle, _CarlaPedestrian
     import scenic.simulators.carla.utils.utils as _utils
 except ModuleNotFoundError:
     # for convenience when testing without the carla package
     from scenic.core.simulators import SimulatorInterfaceWarning
     import warnings
     warnings.warn('the "carla" package is not installed; '
                   'will not be able to run dynamic simulations',
@@ -62,15 +65,19 @@
         """Dummy simulator to allow compilation without the 'carla' package.
 
         :meta private:
         """
         raise RuntimeError('the "carla" package is required to run simulations '
                            'from this scenario')
 
-param carla_map = None
+    class _CarlaVehicle: pass
+    class _CarlaPedestrian: pass
+
+map_town = pathlib.Path(globalParameters.map).stem
+param carla_map = map_town
 param address = '127.0.0.1'
 param port = 2000
 param timeout = 10
 param render = 1
 if globalParameters.render not in [0, 1]:
     raise ValueError('render param must be either 0 or 1')
 param record = ''
@@ -87,14 +94,15 @@
     'CloudySunset',
     'WetSunset',
     'WetCloudySunset',
     'SoftRainSunset',
     'MidRainSunset',
     'HardRainSunset'
 )
+param snapToGroundDefault = is2DMode()
 
 simulator CarlaSimulator(
     carla_map=globalParameters.carla_map,
     map_path=globalParameters.map,
     address=globalParameters.address,
     port=int(globalParameters.port),
     timeout=int(globalParameters.timeout),
@@ -109,20 +117,23 @@
     Properties:
         carlaActor (dynamic): Set during simulations to the ``carla.Actor`` representing this
             object.
         blueprint (str): Identifier of the CARLA blueprint specifying the type of object.
         rolename (str): Can be used to differentiate specific actors during runtime. Default
             value ``None``.
         physics (bool): Whether physics is enabled for this object in CARLA. Default true.
+        snapToGround (bool): Whether or not to snap this object to the ground when placed in CARLA.
+            The default is set by the ``snapToGroundDefault`` global parameter above.
     """
     carlaActor: None
     blueprint: None
     rolename: None
     color: None
     physics: True
+    snapToGround: globalParameters.snapToGroundDefault
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._control = None    # used internally to accumulate control updates
 
     @property
     def control(self):
@@ -136,15 +147,15 @@
     def setVelocity(self, vel):
         cvel = _utils.scenicToCarlaVector3D(*vel)
         if hasattr(self.carlaActor, 'set_target_velocity'):
             self.carlaActor.set_target_velocity(cvel)
         else:
             self.carlaActor.set_velocity(cvel)
 
-class Vehicle(Vehicle, CarlaActor, Steers):
+class Vehicle(Vehicle, CarlaActor, Steers, _CarlaVehicle):
     """Abstract class for steerable vehicles."""
 
     def setThrottle(self, throttle):
         self.control.throttle = throttle
 
     def setSteering(self, steering):
         self.control.steer = steering
@@ -190,15 +201,15 @@
 
 class Truck(Vehicle):
     width: 3
     length: 7
     blueprint: Uniform(*blueprints.truckModels)
 
 
-class Pedestrian(Pedestrian, CarlaActor, Walks):
+class Pedestrian(Pedestrian, CarlaActor, Walks, _CarlaPedestrian):
     """A pedestrian.
 
     The default ``blueprint`` (see `CarlaActor`) is a uniform distribution over the
     blueprints listed in :obj:`scenic.simulators.carla.blueprints.walkerModels`.
     """
     width: 0.5
     length: 0.5
@@ -213,20 +224,20 @@
         self.control.speed = speed
 
 
 class Prop(CarlaActor):
     """Abstract class for props, i.e. non-moving objects.
 
     Properties:
-        heading (float): Default value overridden to be uniformly random.
+        parentOrientation (Orientation): Default value overridden to have uniformly random yaw.
         physics (bool): Default value overridden to be false.
     """
     regionContainedIn: road
     position: new Point on road
-    heading: Range(0, 360) deg
+    parentOrientation: Range(0, 360) deg
     width: 0.5
     length: 0.5
     physics: False
 
 class Trash(Prop):
     blueprint: Uniform(*blueprints.trashModels)
```

### Comparing `scenic-3.0.0b2/src/scenic/simulators/carla/simulator.py` & `scenic-3.0.0rc1/src/scenic/simulators/carla/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         self.client.set_timeout(timeout)  # limits networking operations (seconds)
         if carla_map is not None:
             try:
                 self.world = self.client.load_world(carla_map)
             except Exception as e:
                 raise RuntimeError(f"CARLA could not load world '{carla_map}'") from e
         else:
-            if map_path.endswith(".xodr"):
+            if str(map_path).endswith(".xodr"):
                 with open(map_path) as odr_file:
                     self.world = self.client.generate_opendrive_world(odr_file.read())
             else:
                 raise RuntimeError("CARLA only supports OpenDrive maps")
         self.timestep = timestep
 
         if traffic_manager_port is None:
@@ -135,14 +135,16 @@
             )
             self.cameraManager = None
 
         if self.record:
             if not os.path.exists(self.record):
                 os.mkdir(self.record)
             name = "{}/scenario{}.log".format(self.record, self.scenario_number)
+            # Carla is looking for an absolute path, so convert it if necessary.
+            name = os.path.abspath(name)
             self.client.start_recorder(name)
 
         # Create objects.
         super().setup()
 
         # Set up camera manager and collision sensor for ego
         if self.render:
@@ -199,15 +201,18 @@
 
         # set walker as not invincible
         if blueprint.has_attribute("is_invincible"):
             blueprint.set_attribute("is_invincible", "False")
 
         # Set up transform
         loc = utils.scenicToCarlaLocation(
-            obj.position, world=self.world, blueprint=obj.blueprint
+            obj.position,
+            world=self.world,
+            blueprint=obj.blueprint,
+            snapToGround=obj.snapToGround,
         )
         rot = utils.scenicToCarlaRotation(obj.orientation)
         transform = carla.Transform(loc, rot)
 
         # Color, cannot be set for Pedestrians
         if blueprint.has_attribute("color") and obj.color is not None:
             c = obj.color
```

### Comparing `scenic-3.0.0b2/src/scenic/simulators/carla/utils/utils.py` & `scenic-3.0.0rc1/src/scenic/simulators/carla/utils/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import carla
 import scipy
 
 from scenic.core.geometry import normalizeAngle
 from scenic.core.vectors import Orientation, Vector
 
 
-def snapToGround(world, location, blueprint):
+def _snapToGround(world, location, blueprint):
     """Mutates @location to have the same z-coordinate as the nearest waypoint in @world."""
     waypoint = world.get_map().get_waypoint(location)
     # patch to avoid the spawn error issue with vehicles and walkers.
     z_offset = 0
     if blueprint is not None and ("vehicle" in blueprint or "walker" in blueprint):
         z_offset = 0.5
 
@@ -21,46 +21,41 @@
 
 def scenicToCarlaVector3D(x, y, z=0.0):
     # NOTE: Used for velocity, acceleration; superclass of carla.Location
     z = 0.0 if z is None else z
     return carla.Vector3D(x, -y, z)
 
 
-def scenicToCarlaLocation(pos, z=None, world=None, blueprint=None):
-    if z is None:
+def scenicToCarlaLocation(pos, world=None, blueprint=None, snapToGround=False):
+    if snapToGround:
         assert world is not None
-        return snapToGround(world, carla.Location(pos.x, -pos.y, 0.0), blueprint)
-    return carla.Location(pos.x, -pos.y, z)
+        return _snapToGround(world, carla.Location(pos.x, -pos.y, 0.0), blueprint)
+    return carla.Location(pos.x, -pos.y, pos.z)
 
 
 def scenicToCarlaRotation(orientation):
-    pitch, yaw, roll = orientation.r.as_euler("XZY", degrees=True)
+    # CARLA uses intrinsic yaw, pitch, roll rotations (in that order), like Scenic,
+    # but with yaw being left-handed and with zero yaw being East.
+    yaw, pitch, roll = orientation.r.as_euler("ZXY", degrees=True)
     yaw = -yaw - 90
     return carla.Rotation(pitch=pitch, yaw=yaw, roll=roll)
 
 
-def scenicSpeedToCarlaVelocity(speed, heading):
-    currYaw = scenicToCarlaRotation(heading).yaw
-    xVel = speed * math.cos(currYaw)
-    yVel = speed * math.sin(currYaw)
-    return scenicToCarlaVector3D(xVel, yVel)
-
-
 def carlaToScenicPosition(loc):
     return Vector(loc.x, -loc.y, loc.z)
 
 
 def carlaToScenicElevation(loc):
     return loc.z
 
 
 def carlaToScenicOrientation(rot):
-    angles = (rot.pitch, -rot.yaw - 90, rot.roll)
+    angles = (-rot.yaw - 90, rot.pitch, rot.roll)
     r = scipy.spatial.transform.Rotation.from_euler(
-        seq="XZY", angles=angles, degrees=True
+        seq="ZXY", angles=angles, degrees=True
     )
     return Orientation(r)
 
 
 def carlaToScenicHeading(rot):
     return normalizeAngle(-math.radians(rot.yaw + 90))
```

### Comparing `scenic-3.0.0b2/src/scenic/simulators/carla/utils/visuals.py` & `scenic-3.0.0rc1/src/scenic/simulators/carla/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/gta/.DS_Store` & `scenic-3.0.0rc1/src/scenic/simulators/gta/.DS_Store`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/gta/center_detection.py` & `scenic-3.0.0rc1/src/scenic/simulators/gta/center_detection.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/gta/img_modf.py` & `scenic-3.0.0rc1/src/scenic/simulators/gta/img_modf.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/gta/interface.py` & `scenic-3.0.0rc1/src/scenic/simulators/gta/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,18 +51,17 @@
     def Config(scene):
         ego = scene.egoObject
         vehicles = [GTA.Vehicle(car) for car in scene.objects if car is not ego]
         cameraLoc = GTA.langToGTACoords(ego.position)
         cameraHeading = GTA.langToGTAHeading(ego.heading)
 
         params = dict(scene.params)
-        time = int(round(params.pop("time")))
-        minute = time % 60
-        hour = int((time - minute) / 60)
-        assert hour < 24
+        time = int(round(params.pop("time"))) % 1440
+        hour, minute = divmod(time, 60)
+        assert hour < 24, scene.params["time"]
         weather = params.pop("weather")
         for param in params:
             print(f'WARNING: unused scene parameter "{param}"')
 
         return messages.Formal_Config(
             cameraLoc, [hour, minute], weather, vehicles, cameraHeading
         )
```

### Comparing `scenic-3.0.0b2/src/scenic/simulators/gta/messages.py` & `scenic-3.0.0rc1/src/scenic/simulators/gta/messages.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/gta/model.scenic` & `scenic-3.0.0rc1/src/scenic/simulators/gta/model.scenic`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/lgsvl/actions.py` & `scenic-3.0.0rc1/src/scenic/simulators/lgsvl/actions.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/lgsvl/behaviors.scenic` & `scenic-3.0.0rc1/src/scenic/simulators/lgsvl/behaviors.scenic`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/lgsvl/model.scenic` & `scenic-3.0.0rc1/src/scenic/simulators/lgsvl/model.scenic`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 """Scenic world model for the LGSVL Simulator."""
 
 from scenic.domains.driving.model import *
 from scenic.simulators.lgsvl.behaviors import *
 
+# Deprecation error on import, but allow for doc building.
+try:
+    import sphinx
+    if not sphinx._buildingScenicDocs:
+        raise RuntimeError("The LGSVL Simulator interface was deprecated in Scenic 3."
+            " To continue to use the interface, please use Scenic 2.")
+except ModuleNotFoundError:
+    pass
+
 try:
     import lgsvl
     EGO_TYPE = lgsvl.AgentType.EGO
     NPC_TYPE = lgsvl.AgentType.NPC
     PEDESTRIAN_TYPE = lgsvl.AgentType.PEDESTRIAN
     LINCOLN_MODULAR = lgsvl.wise.DefaultAssets.ego_lincoln2017mkz_apollo5_modular
     from scenic.simulators.lgsvl.simulator import LGSVLSimulator
```

### Comparing `scenic-3.0.0b2/src/scenic/simulators/lgsvl/simulator.py` & `scenic-3.0.0rc1/src/scenic/simulators/lgsvl/simulator.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/lgsvl/utils.py` & `scenic-3.0.0rc1/src/scenic/simulators/lgsvl/utils.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/newtonian/car.png` & `scenic-3.0.0rc1/src/scenic/simulators/newtonian/car.png`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/newtonian/driving_model.scenic` & `scenic-3.0.0rc1/src/scenic/simulators/newtonian/driving_model.scenic`

 * *Files 0% similar despite different names*

```diff
@@ -57,9 +57,9 @@
         return True
 
 class Pedestrian(Pedestrian, NewtonianActor, Walks):
     pass
 
 class Debris:
     """Abstract class for debris scattered randomly in the workspace."""
-    position: Point in workspace
+    position: new Point in workspace
     yaw: Range(0, 360) deg
```

### Comparing `scenic-3.0.0b2/src/scenic/simulators/newtonian/simulator.py` & `scenic-3.0.0rc1/src/scenic/simulators/newtonian/simulator.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/utils/colors.py` & `scenic-3.0.0rc1/src/scenic/simulators/utils/colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,18 @@
         self.baseColor = baseColor
         self.hueNoise = hueNoise
         self.satNoise = satNoise
         self.lightNoise = lightNoise
 
     @staticmethod
     def addNoiseTo(color, hueNoise, lightNoise, satNoise):
-        hue, lightness, saturation = colorsys.rgb_to_hls(*color)
+        try:
+            hue, lightness, saturation = colorsys.rgb_to_hls(*color[:3])
+        except ZeroDivisionError:
+            hue, lightness, saturation = 0.0, 1.0, 0.0
         hue = max(0, min(1, hue + hueNoise))
         lightness = max(0, min(1, lightness + lightNoise))
         saturation = max(0, min(1, saturation + satNoise))
         return colorsys.hls_to_rgb(hue, lightness, saturation)
 
     def sampleGiven(self, value):
         bc = value[self.baseColor]
@@ -112,11 +115,11 @@
     """Mutator that adds Gaussian HSL noise to the ``color`` property."""
 
     def appliedTo(self, obj):
         stddev = 0.05 * obj.mutationScale
         hueNoise = random.gauss(0, stddev)
         satNoise = random.gauss(0, stddev)
         lightNoise = random.gauss(0, stddev)
-        color = NoisyColorDistribution.addNoiseTo(
+        obj.color = NoisyColorDistribution.addNoiseTo(
             obj.color, hueNoise, lightNoise, satNoise
         )
-        return (obj._copyWith(color=color), True)  # allow further mutation
+        return (obj, True)  # allow further mutation
```

### Comparing `scenic-3.0.0b2/src/scenic/simulators/webots/.DS_Store` & `scenic-3.0.0rc1/src/scenic/simulators/webots/.DS_Store`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/webots/WBT.g4` & `scenic-3.0.0rc1/src/scenic/simulators/webots/WBT.g4`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/webots/WBTLexer.py` & `scenic-3.0.0rc1/src/scenic/simulators/webots/WBTLexer.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/webots/WBTParser.py` & `scenic-3.0.0rc1/src/scenic/simulators/webots/WBTParser.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/webots/WBTVisitor.py` & `scenic-3.0.0rc1/src/scenic/simulators/webots/WBTVisitor.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/webots/actions.py` & `scenic-3.0.0rc1/src/scenic/simulators/webots/actions.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/webots/guideways/.DS_Store` & `scenic-3.0.0rc1/src/scenic/simulators/webots/guideways/.DS_Store`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/webots/guideways/interface.py` & `scenic-3.0.0rc1/src/scenic/simulators/webots/guideways/interface.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/webots/guideways/model.scenic` & `scenic-3.0.0rc1/src/scenic/simulators/webots/guideways/model.scenic`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/webots/mars/.DS_Store` & `scenic-3.0.0rc1/src/scenic/simulators/webots/mars/.DS_Store`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/webots/model.scenic` & `scenic-3.0.0rc1/src/scenic/simulators/webots/model.scenic`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/webots/road/.DS_Store` & `scenic-3.0.0rc1/src/scenic/simulators/webots/road/.DS_Store`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/webots/road/car_models.py` & `scenic-3.0.0rc1/src/scenic/simulators/webots/road/car_models.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/webots/road/interface.py` & `scenic-3.0.0rc1/src/scenic/simulators/webots/road/interface.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/webots/road/model.scenic` & `scenic-3.0.0rc1/src/scenic/simulators/webots/road/model.scenic`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/webots/simulator.py` & `scenic-3.0.0rc1/src/scenic/simulators/webots/simulator.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/webots/utils.py` & `scenic-3.0.0rc1/src/scenic/simulators/webots/utils.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/simulators/webots/world_parser.py` & `scenic-3.0.0rc1/src/scenic/simulators/webots/world_parser.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/syntax/.DS_Store` & `scenic-3.0.0rc1/src/scenic/syntax/.DS_Store`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/syntax/__init__.py` & `scenic-3.0.0rc1/src/scenic/syntax/__init__.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/syntax/ast.py` & `scenic-3.0.0rc1/src/scenic/syntax/ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,36 +356,39 @@
 
     def __init__(
         self, value: ast.AST, name: Optional[str] = None, *args: any, **kwargs: any
     ) -> None:
         super().__init__(*args, **kwargs)
         self.value = value
         self.name = name
+        self._fields = ["value", "name"]
 
 
 class RecordInitial(AST):
     __match_args__ = ("value", "name")
 
     def __init__(
         self, value: ast.AST, name: Optional[str] = None, *args: any, **kwargs: any
     ) -> None:
         super().__init__(*args, **kwargs)
         self.value = value
         self.name = name
+        self._fields = ["value", "name"]
 
 
 class RecordFinal(AST):
     __match_args__ = ("value", "name")
 
     def __init__(
         self, value: ast.AST, name: Optional[str] = None, *args: any, **kwargs: any
     ) -> None:
         super().__init__(*args, **kwargs)
         self.value = value
         self.name = name
+        self._fields = ["value", "name"]
 
 
 class Mutate(AST):
     __match_args__ = ("elts", "scale")
 
     def __init__(
         self,
@@ -519,15 +522,15 @@
 
     def __init__(
         self, elts: typing.List[ast.AST], cond: ast.AST, *args: any, **kwargs: any
     ) -> None:
         super().__init__(*args, **kwargs)
         self.elts = elts
         self.cond = cond
-        self._fields = ["value", "cond"]
+        self._fields = ["elts", "cond"]
 
 
 class DoChoose(AST):
     __match_args__ = ("elts",)
 
     def __init__(self, elts: typing.List[ast.AST], *args: any, **kwargs: any) -> None:
         super().__init__(*args, **kwargs)
@@ -1031,14 +1034,15 @@
         target: ast.AST,
         *args: any,
         **kwargs: any,
     ) -> None:
         super().__init__(*args, **kwargs)
         self.position = position
         self.target = target
+        self._fields = ["position", "target"]
 
 
 class Front(AST):
     "Represents position of :scenic:`front of` operator"
     functionName = "Front"
 
     def __init__(self, *args: any, **kwargs: any) -> None:
@@ -1183,14 +1187,15 @@
 
 class DegOp(AST):
     __match_args__ = ("operand",)
 
     def __init__(self, operand: ast.AST, *args: any, **kwargs: any) -> None:
         super().__init__(*args, **kwargs)
         self.operand = operand
+        self._fields = ["operand"]
 
 
 class VectorOp(AST):
     __match_args__ = ("left", "right")
 
     def __init__(self, left: ast.AST, right: ast.AST, *args: any, **kwargs: any) -> None:
         super().__init__(*args, **kwargs)
@@ -1202,23 +1207,25 @@
 class FieldAtOp(AST):
     __match_args__ = ("left", "right")
 
     def __init__(self, left: ast.AST, right: ast.AST, *args: any, **kwargs: any) -> None:
         super().__init__(*args, **kwargs)
         self.left = left
         self.right = right
+        self._fields = ["left", "right"]
 
 
 class RelativeToOp(AST):
     __match_args__ = ("left", "right")
 
     def __init__(self, left: ast.AST, right: ast.AST, *args: any, **kwargs: any) -> None:
         super().__init__(*args, **kwargs)
         self.left = left
         self.right = right
+        self._fields = ["left", "right"]
 
 
 class OffsetAlongOp(AST):
     __match_args__ = ("base", "direction", "offset")
 
     def __init__(
         self,
@@ -1228,16 +1235,28 @@
         *args: any,
         **kwargs: any,
     ) -> None:
         super().__init__(*args, **kwargs)
         self.base = base
         self.direction = direction
         self.offset = offset
+        self._fields = ["base", "direction", "offset"]
 
 
 class CanSeeOp(AST):
     __match_args__ = ("left", "right")
 
     def __init__(self, left: ast.AST, right: ast.AST, *args: any, **kwargs: any) -> None:
         super().__init__(*args, **kwargs)
         self.left = left
         self.right = right
+        self._fields = ["left", "right"]
+
+
+class IntersectsOp(AST):
+    __match_args__ = ("left", "right")
+
+    def __init__(self, left: ast.AST, right: ast.AST, *args: any, **kwargs: any) -> None:
+        super().__init__(*args, **kwargs)
+        self.left = left
+        self.right = right
+        self._fields = ["left", "right"]
```

### Comparing `scenic-3.0.0b2/src/scenic/syntax/compiler.py` & `scenic-3.0.0rc1/src/scenic/syntax/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -491,17 +491,19 @@
                     ctx = "inside a behavior"
                 elif self.inMonitor and Context.MONITOR not in allowedContext:
                     ctx = "inside a monitor"
                 elif self.inCompose and Context.COMPOSE not in allowedContext:
                     ctx = "inside a compose block"
                 if ctx:
                     raise self.makeSyntaxError(
-                        f'Cannot use "{node.__class__.__name__}" {ctx}'
-                        if errorBuilder is None
-                        else errorBuilder(ctx),
+                        (
+                            f'Cannot use "{node.__class__.__name__}" {ctx}'
+                            if errorBuilder is None
+                            else errorBuilder(ctx)
+                        ),
                         node,
                     )
                 return visitor(self, node)
 
             return check_and_visit
 
         return decorator
@@ -1104,17 +1106,19 @@
 
     @context(Context.TOP_LEVEL)
     def visit_Mutate(self, node: s.Mutate):
         return ast.Expr(
             value=ast.Call(
                 func=ast.Name(id="mutate", ctx=loadCtx),
                 args=[self.visit(el) for el in node.elts],
-                keywords=[ast.keyword(arg="scale", value=self.visit(node.scale))]
-                if node.scale is not None
-                else [],
+                keywords=(
+                    [ast.keyword(arg="scale", value=self.visit(node.scale))]
+                    if node.scale is not None
+                    else []
+                ),
             )
         )
 
     @context(Context.TOP_LEVEL)
     def visit_Param(self, node: s.Param):
         d = dict()
         for parameter in node.elts:
@@ -1350,17 +1354,19 @@
                 func=ast.Name(functionName, loadCtx),
                 args=[
                     ast.Constant(requirementId),  # requirement IDre
                     newBody,  # body
                     ast.Constant(lineno),  # line number
                     ast.Constant(name),  # requirement name
                 ],
-                keywords=[ast.keyword(arg="prob", value=ast.Constant(prob))]
-                if prob is not None
-                else [],
+                keywords=(
+                    [ast.keyword(arg="prob", value=ast.Constant(prob))]
+                    if prob is not None
+                    else []
+                ),
             )
         )
 
     @context(Context.TOP_LEVEL)
     def visit_TerminateAfter(self, node: s.TerminateAfter):
         return ast.copy_location(
             ast.Expr(
@@ -1464,17 +1470,19 @@
             ),
         )
 
     def visit_BeyondSpecifier(self, node: s.BeyondSpecifier):
         return ast.Call(
             func=ast.Name(id="Beyond", ctx=loadCtx),
             args=[self.visit(node.position), self.visit(node.offset)],
-            keywords=[ast.keyword(arg="fromPt", value=self.visit(node.base))]
-            if node.base is not None
-            else [],
+            keywords=(
+                [ast.keyword(arg="fromPt", value=self.visit(node.base))]
+                if node.base is not None
+                else []
+            ),
         )
 
     def visit_VisibleSpecifier(self, node: s.VisibleSpecifier):
         if node.base is not None:
             return ast.Call(
                 func=ast.Name(id="VisibleFrom", ctx=loadCtx),
                 args=[self.visit(node.base)],
@@ -1520,17 +1528,19 @@
             keywords=[],
         )
 
     def visit_FollowingSpecifier(self, node: s.FollowingSpecifier):
         return ast.Call(
             func=ast.Name(id="Following", ctx=loadCtx),
             args=[self.visit(node.field), self.visit(node.distance)],
-            keywords=[ast.keyword(arg="fromPt", value=self.visit(node.base))]
-            if node.base is not None
-            else [],
+            keywords=(
+                [ast.keyword(arg="fromPt", value=self.visit(node.base))]
+                if node.base is not None
+                else []
+            ),
         )
 
     def visit_FacingSpecifier(self, node: s.FacingSpecifier):
         return ast.Call(
             func=ast.Name(id="Facing", ctx=loadCtx),
             args=[self.visit(node.heading)],
             keywords=[],
@@ -1566,64 +1576,76 @@
             keywords=[],
         )
 
     def visit_ApparentlyFacingSpecifier(self, node: s.ApparentlyFacingSpecifier):
         return ast.Call(
             func=ast.Name(id="ApparentlyFacing", ctx=loadCtx),
             args=[self.visit(node.heading)],
-            keywords=[ast.keyword(arg="fromPt", value=self.visit(node.base))]
-            if node.base is not None
-            else [],
+            keywords=(
+                [ast.keyword(arg="fromPt", value=self.visit(node.base))]
+                if node.base is not None
+                else []
+            ),
         )
 
     # Operators
 
     def visit_RelativePositionOp(self, node: s.RelativePositionOp):
         return ast.Call(
             func=ast.Name(id="RelativePosition", ctx=loadCtx),
             args=[self.visit(node.target)],
-            keywords=[]
-            if node.base is None
-            else [ast.keyword(arg="Y", value=self.visit(node.base))],
+            keywords=(
+                []
+                if node.base is None
+                else [ast.keyword(arg="Y", value=self.visit(node.base))]
+            ),
         )
 
     def visit_RelativeHeadingOp(self, node: s.RelativeHeadingOp):
         return ast.Call(
             func=ast.Name(id="RelativeHeading", ctx=loadCtx),
             args=[self.visit(node.target)],
-            keywords=[]
-            if node.base is None
-            else [ast.keyword(arg="Y", value=self.visit(node.base))],
+            keywords=(
+                []
+                if node.base is None
+                else [ast.keyword(arg="Y", value=self.visit(node.base))]
+            ),
         )
 
     def visit_ApparentHeadingOp(self, node: s.ApparentHeadingOp):
         return ast.Call(
             func=ast.Name(id="ApparentHeading", ctx=loadCtx),
             args=[self.visit(node.target)],
-            keywords=[]
-            if node.base is None
-            else [ast.keyword(arg="Y", value=self.visit(node.base))],
+            keywords=(
+                []
+                if node.base is None
+                else [ast.keyword(arg="Y", value=self.visit(node.base))]
+            ),
         )
 
     def visit_DistanceFromOp(self, node: s.DistanceFromOp):
         return ast.Call(
             func=ast.Name(id="DistanceFrom", ctx=loadCtx),
             args=[self.visit(node.target)],
-            keywords=[ast.keyword(arg="Y", value=self.visit(node.base))]
-            if node.base is not None
-            else [],
+            keywords=(
+                [ast.keyword(arg="Y", value=self.visit(node.base))]
+                if node.base is not None
+                else []
+            ),
         )
 
     def visit_DistancePastOp(self, node: s.DistancePastOp):
         return ast.Call(
             func=ast.Name(id="DistancePast", ctx=loadCtx),
             args=[self.visit(node.target)],
-            keywords=[]
-            if node.base is None
-            else [ast.keyword(arg="Y", value=self.visit(node.base))],
+            keywords=(
+                []
+                if node.base is None
+                else [ast.keyword(arg="Y", value=self.visit(node.base))]
+            ),
         )
 
     def visit_AngleFromOp(self, node: s.AngleFromOp):
         assert (
             node.base is not None or node.target is not None
         ), "neither target nor base were specified in AngleFromOp"
         keywords = []
@@ -1742,7 +1764,17 @@
             func=ast.Name(id="CanSee", ctx=loadCtx),
             args=[
                 self.visit(node.left),
                 self.visit(node.right),
             ],
             keywords=[],
         )
+
+    def visit_IntersectsOp(self, node: s.IntersectsOp):
+        return ast.Call(
+            func=ast.Name(id="Intersects", ctx=loadCtx),
+            args=[
+                self.visit(node.left),
+                self.visit(node.right),
+            ],
+            keywords=[],
+        )
```

### Comparing `scenic-3.0.0b2/src/scenic/syntax/parser.py` & `scenic-3.0.0rc1/src/scenic/syntax/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import enum
 import io
 import itertools
 import os
 import sys
 import token
 from typing import (
-    Any, Callable, Iterator, List, Literal, Tuple, TypeVar, Union, NoReturn
+    Any, Callable, Iterator, List, Literal, NoReturn, Sequence, Tuple, TypeVar, Union
 )
 
 from pegen.tokenizer import Tokenizer
 
 import scenic.syntax.ast as s
 from scenic.core.errors import ScenicParseError
 
@@ -232,26 +232,105 @@
             return node
 
     def set_expr_context(self, node, context):
         """Set the context (Load, Store, Del) of an ast node."""
         node.ctx = context
         return node
 
-    def ensure_real(self, number: ast.Constant):
+    def ensure_real(self, number: ast.Constant) -> float:
         value = ast.literal_eval(number.string)
         if type(value) is complex:
             self.raise_syntax_error_known_location("real number required in complex literal", number)
         return value
 
-    def ensure_imaginary(self, number:  ast.Constant):
+    def ensure_imaginary(self, number: ast.Constant) -> complex:
         value = ast.literal_eval(number.string)
         if type(value) is not complex:
             self.raise_syntax_error_known_location("imaginary number required in complex literal", number)
         return value
 
+    def check_fstring_conversion(self, mark: tokenize.TokenInfo, name: tokenize.TokenInfo) -> tokenize.TokenInfo:
+        if mark.lineno != name.lineno or mark.col_offset != name.col_offset:
+            self.raise_syntax_error_known_range(
+                "f-string: conversion type must come right after the exclamanation mark",
+                mark,
+                name
+            )
+
+        s = name.string
+        if len(s) > 1 or s not in ("s", "r", "a"):
+            self.raise_syntax_error_known_location(
+                f"f-string: invalid conversion character '{s}': expected 's', 'r', or 'a'",
+                name,
+            )
+
+        return name
+
+    def _concat_strings_in_constant(self, parts) -> Union[str, bytes]:
+        s = ast.literal_eval(parts[0].string)
+        for ss in parts[1:]:
+            s += ast.literal_eval(ss.string)
+        args = dict(
+            value=s,
+            lineno=parts[0].start[0],
+            col_offset=parts[0].start[1],
+            end_lineno=parts[-1].end[0],
+            end_col_offset=parts[0].end[1],
+        )
+        if parts[0].string.startswith("u"):
+            args["kind"] = "u"
+        return ast.Constant(**args)
+
+
+    def concatenate_strings(self, parts):
+        """Concatenate multiple tokens and ast.JoinedStr"""
+        # Get proper start and stop
+        start = end = None
+        if isinstance(parts[0], ast.JoinedStr):
+            start = parts[0].lineno, parts[0].col_offset
+        if isinstance(parts[-1], ast.JoinedStr):
+            end = parts[-1].end_lineno, parts[-1].end_col_offset
+
+        # Combine the different parts
+        seen_joined = False
+        values = []
+        ss = []
+        for p in parts:
+            if isinstance(p, ast.JoinedStr):
+                seen_joined = True
+                if ss:
+                    values.append(self._concat_strings_in_constant(ss))
+                    ss.clear()
+                values.extend(p.values)
+            else:
+                ss.append(p)
+
+        if ss:
+            values.append(self._concat_strings_in_constant(ss))
+
+        consolidated = []
+        for p in values:
+            if consolidated and isinstance(consolidated[-1], ast.Constant) and isinstance(p, ast.Constant):
+                consolidated[-1].value += p.value
+                consolidated[-1].end_lineno = p.end_lineno
+                consolidated[-1].end_col_offset = p.end_col_offset
+            else:
+                consolidated.append(p)
+
+        if not seen_joined and len(values) == 1 and isinstance(values[0], ast.Constant):
+            return values[0]
+        else:
+            return ast.JoinedStr(
+                values=consolidated,
+                lineno=start[0] if start else values[0].lineno,
+                col_offset=start[1] if start else values[0].col_offset,
+                end_lineno=end[0] if end else values[-1].end_lineno,
+                end_col_offset=end[1] if end else values[-1].end_col_offset,
+            )
+
     def generate_ast_for_string(self, tokens):
         """Generate AST nodes for strings."""
         err_args = None
         line_offset = tokens[0].start[0]
         line = line_offset
         col_offset = 0
         source = "(\n"
@@ -398,23 +477,27 @@
 
     def make_syntax_error(self, message: str) -> None:
         return self._build_syntax_error(message)
 
     def expect_forced(self, res: Any, expectation: str) -> Optional[tokenize.TokenInfo]:
         if res is None:
             last_token = self._tokenizer.diagnose()
+            end = last_token.start
+            if sys.version_info >= (3, 12) or (sys.version_info >= (3, 11) and last_token.type != 4):  # i.e. not a 
+
+                end = last_token.end
             self.raise_raw_syntax_error(
-                f"expected {expectation}", last_token.start, last_token.start
+                f"expected {expectation}", last_token.start, end
             )
         return res
 
     def raise_syntax_error(self, message: str) -> NoReturn:
         """Raise a syntax error."""
         tok = self._tokenizer.diagnose()
-        raise self._build_syntax_error(message, tok.start, tok.end if tok.type != 4 else tok.start)
+        raise self._build_syntax_error(message, tok.start, tok.end if sys.version_info >= (3, 12) or tok.type != 4 else tok.start)
 
     def raise_syntax_error_known_location(
         self, message: str, node: Union[ast.AST, tokenize.TokenInfo]
     ) -> NoReturn:
         """Raise a syntax error that occured at a given AST node."""
         if isinstance(node, tokenize.TokenInfo):
             start = node.start
@@ -468,14 +551,18 @@
         if target in (Target.STAR_TARGETS, Target.FOR_TARGETS):
             msg = f"cannot assign to {self.get_expr_name(invalid_target)}"
         else:
             msg = f"cannot delete {self.get_expr_name(invalid_target)}"
 
         self.raise_syntax_error_known_location(msg, invalid_target)
 
+    def raise_syntax_error_on_next_token(self, message: str) -> NoReturn:
+        next_token = self._tokenizer.peek()
+        raise self._build_syntax_error(message, next_token.start, next_token.end)
+
     # scenic helpers
     def extend_new_specifiers(self, node: s.New, specifiers: List[ast.AST]) -> s.New:
         node.specifiers.extend(specifiers)
         return node
 
 # Keywords and soft keywords are listed at the end of the parser definition.
 class ScenicParser(Parser):
@@ -550,30 +637,38 @@
             (self.expect('ENDMARKER'))
         ):
             return ast . FunctionType ( argtypes = a , returns = b );
         self._reset(mark)
         return None;
 
     @memoize
-    def fstring(self) -> Optional[ast . Expr]:
-        # fstring: star_expressions
+    def fstring(self) -> Optional[Any]:
+        # fstring: FSTRING_START fstring_mid* FSTRING_END
         mark = self._mark()
+        tok = self._tokenizer.peek()
+        start_lineno, start_col_offset = tok.start
         if (
-            (star_expressions := self.star_expressions())
+            (self.fstring_start())
+            and
+            (b := self._loop0_3(),)
+            and
+            (self.fstring_end())
         ):
-            return star_expressions;
+            tok = self._tokenizer.get_last_non_whitespace_token()
+            end_lineno, end_col_offset = tok.end
+            return ast . JoinedStr ( values = b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
     @memoize
     def statements(self) -> Optional[list]:
         # statements: statement+
         mark = self._mark()
         if (
-            (a := self._loop1_3())
+            (a := self._loop1_4())
         ):
             return list ( itertools . chain . from_iterable ( a ) );
         self._reset(mark)
         return None;
 
     @memoize
     def statement(self) -> Optional[list]:
@@ -643,15 +738,15 @@
             (self.negative_lookahead(self.expect, ';'))
             and
             (self.expect('NEWLINE'))
         ):
             return [a];
         self._reset(mark)
         if (
-            (a := self._gather_4())
+            (a := self._gather_5())
             and
             (self.expect(';'),)
             and
             (self.expect('NEWLINE'))
         ):
             return a;
         self._reset(mark)
@@ -667,51 +762,58 @@
             (self.negative_lookahead(self.expect, ';'))
             and
             (self.expect('NEWLINE'))
         ):
             return [a];
         self._reset(mark)
         if (
-            (a := self._gather_6())
+            (a := self._gather_7())
             and
             (self.expect(';'),)
             and
             (self.expect('NEWLINE'))
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
     def simple_stmt(self) -> Optional[Any]:
-        # simple_stmt: assignment | star_expressions | &'return' return_stmt | &('import' | 'from') import_stmt | &'raise' raise_stmt | 'pass' | &'del' del_stmt | &'yield' yield_stmt | &'assert' assert_stmt | 'break' | 'continue' | &'global' global_stmt | &'nonlocal' nonlocal_stmt
+        # simple_stmt: assignment | &"type" type_alias | star_expressions | &'return' return_stmt | &('import' | 'from') import_stmt | &'raise' raise_stmt | 'pass' | &'del' del_stmt | &'yield' yield_stmt | &'assert' assert_stmt | 'break' | 'continue' | &'global' global_stmt | &'nonlocal' nonlocal_stmt
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (assignment := self.assignment())
         ):
             return assignment;
         self._reset(mark)
         if (
+            (self.positive_lookahead(self.expect, "type"))
+            and
+            (type_alias := self.type_alias())
+        ):
+            return type_alias;
+        self._reset(mark)
+        if (
             (e := self.star_expressions())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Expr ( value = e , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (self.positive_lookahead(self.expect, 'return'))
             and
             (return_stmt := self.return_stmt())
         ):
             return return_stmt;
         self._reset(mark)
         if (
-            (self.positive_lookahead(self._tmp_8, ))
+            (self.positive_lookahead(self._tmp_9, ))
             and
             (import_stmt := self.import_stmt())
         ):
             return import_stmt;
         self._reset(mark)
         if (
             (self.positive_lookahead(self.expect, 'raise'))
@@ -779,43 +881,43 @@
         return None;
 
     @memoize
     def compound_stmt(self) -> Optional[Any]:
         # compound_stmt: &('def' | '@' | 'async') function_def | &'if' if_stmt | &('class' | '@') class_def | &('with' | 'async') with_stmt | &('for' | 'async') for_stmt | &'try' try_stmt | &'while' while_stmt | match_stmt
         mark = self._mark()
         if (
-            (self.positive_lookahead(self._tmp_9, ))
+            (self.positive_lookahead(self._tmp_10, ))
             and
             (function_def := self.function_def())
         ):
             return function_def;
         self._reset(mark)
         if (
             (self.positive_lookahead(self.expect, 'if'))
             and
             (if_stmt := self.if_stmt())
         ):
             return if_stmt;
         self._reset(mark)
         if (
-            (self.positive_lookahead(self._tmp_10, ))
+            (self.positive_lookahead(self._tmp_11, ))
             and
             (class_def := self.class_def())
         ):
             return class_def;
         self._reset(mark)
         if (
-            (self.positive_lookahead(self._tmp_11, ))
+            (self.positive_lookahead(self._tmp_12, ))
             and
             (with_stmt := self.with_stmt())
         ):
             return with_stmt;
         self._reset(mark)
         if (
-            (self.positive_lookahead(self._tmp_12, ))
+            (self.positive_lookahead(self._tmp_13, ))
             and
             (for_stmt := self.for_stmt())
         ):
             return for_stmt;
         self._reset(mark)
         if (
             (self.positive_lookahead(self.expect, 'try'))
@@ -1009,37 +1111,37 @@
         if (
             (a := self.name())
             and
             (self.expect(':'))
             and
             (b := self.expression())
             and
-            (c := self._tmp_13(),)
+            (c := self._tmp_14(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return self . check_version ( ( 3 , 6 ) , "Variable annotation syntax is" , ast . AnnAssign ( target = ast . Name ( id = a . string , ctx = Store , lineno = a . start [0] , col_offset = a . start [1] , end_lineno = a . end [0] , end_col_offset = a . end [1] , ) , annotation = b , value = c , simple = 1 , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset , ) );
         self._reset(mark)
         if (
-            (a := self._tmp_14())
+            (a := self._tmp_15())
             and
             (self.expect(':'))
             and
             (b := self.expression())
             and
-            (c := self._tmp_15(),)
+            (c := self._tmp_16(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return self . check_version ( ( 3 , 6 ) , "Variable annotation syntax is" , ast . AnnAssign ( target = a , annotation = b , value = c , simple = 0 , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset , ) );
         self._reset(mark)
         if (
-            (a := self._loop1_16())
+            (a := self._loop1_17())
             and
-            (b := self._tmp_17())
+            (b := self._tmp_18())
             and
             (self.negative_lookahead(self.expect, '='))
             and
             (tc := self.type_comment(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
@@ -1049,15 +1151,15 @@
         if (
             (a := self.single_target())
             and
             (b := self.augassign())
             and
             (cut := True)
             and
-            (c := self._tmp_18())
+            (c := self._tmp_19())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . AugAssign ( target = a , op = b , value = c , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if cut:
             return None;
@@ -1181,15 +1283,15 @@
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect('raise'))
             and
             (a := self.expression())
             and
-            (b := self._tmp_19(),)
+            (b := self._tmp_20(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Raise ( exc = a , cause = b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (self.expect('raise'))
@@ -1205,15 +1307,15 @@
         # global_stmt: 'global' ','.NAME+
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect('global'))
             and
-            (a := self._gather_20())
+            (a := self._gather_21())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Global ( names = [n . string for n in a] , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
@@ -1222,15 +1324,15 @@
         # nonlocal_stmt: 'nonlocal' ','.NAME+
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect('nonlocal'))
             and
-            (a := self._gather_22())
+            (a := self._gather_23())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Nonlocal ( names = [n . string for n in a] , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
@@ -1241,15 +1343,15 @@
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect('del'))
             and
             (a := self.del_targets())
             and
-            (self.positive_lookahead(self._tmp_24, ))
+            (self.positive_lookahead(self._tmp_25, ))
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Delete ( targets = a , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             self.call_invalid_rules
@@ -1282,27 +1384,34 @@
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect('assert'))
             and
             (a := self.expression())
             and
-            (b := self._tmp_25(),)
+            (b := self._tmp_26(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Assert ( test = a , msg = b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
     @memoize
     def import_stmt(self) -> Optional[ast . Import]:
-        # import_stmt: import_name | import_from
+        # import_stmt: invalid_import | import_name | import_from
         mark = self._mark()
         if (
+            self.call_invalid_rules
+            and
+            (self.invalid_import())
+        ):
+            return None  # pragma: no cover;
+        self._reset(mark)
+        if (
             (import_name := self.import_name())
         ):
             return import_name;
         self._reset(mark)
         if (
             (import_from := self.import_from())
         ):
@@ -1332,30 +1441,30 @@
         # import_from: 'from' (('.' | '...'))* dotted_name 'import' import_from_targets | 'from' (('.' | '...'))+ 'import' import_from_targets
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect('from'))
             and
-            (a := self._loop0_26(),)
+            (a := self._loop0_27(),)
             and
             (b := self.dotted_name())
             and
             (self.expect('import'))
             and
             (c := self.import_from_targets())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . ImportFrom ( module = b , names = c , level = self . extract_import_level ( a ) , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (self.expect('from'))
             and
-            (a := self._loop1_27())
+            (a := self._loop1_28())
             and
             (self.expect('import'))
             and
             (b := self.import_from_targets())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
@@ -1404,58 +1513,58 @@
         return None;
 
     @memoize
     def import_from_as_names(self) -> Optional[List [ast . alias]]:
         # import_from_as_names: ','.import_from_as_name+
         mark = self._mark()
         if (
-            (a := self._gather_28())
+            (a := self._gather_29())
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
     def import_from_as_name(self) -> Optional[ast . alias]:
         # import_from_as_name: NAME ['as' NAME]
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (a := self.name())
             and
-            (b := self._tmp_30(),)
+            (b := self._tmp_31(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . alias ( name = a . string , asname = b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
     @memoize
     def dotted_as_names(self) -> Optional[List [ast . alias]]:
         # dotted_as_names: ','.dotted_as_name+
         mark = self._mark()
         if (
-            (a := self._gather_31())
+            (a := self._gather_32())
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
     def dotted_as_name(self) -> Optional[ast . alias]:
         # dotted_as_name: dotted_name ['as' NAME]
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (a := self.dotted_name())
             and
-            (b := self._tmp_33(),)
+            (b := self._tmp_34(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . alias ( name = a , asname = b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
@@ -1509,31 +1618,31 @@
         return None;
 
     @memoize
     def decorators(self) -> Optional[Any]:
         # decorators: decorator+
         mark = self._mark()
         if (
-            (_loop1_34 := self._loop1_34())
+            (_loop1_35 := self._loop1_35())
         ):
-            return _loop1_34;
+            return _loop1_35;
         self._reset(mark)
         return None;
 
     @memoize
     def decorator(self) -> Optional[Any]:
         # decorator: ('@' dec_maybe_call NEWLINE) | ('@' named_expression NEWLINE)
         mark = self._mark()
         if (
-            (a := self._tmp_35())
+            (a := self._tmp_36())
         ):
             return a;
         self._reset(mark)
         if (
-            (a := self._tmp_36())
+            (a := self._tmp_37())
         ):
             return self . check_version ( ( 3 , 9 ) , "Generic decorator are" , a );
         self._reset(mark)
         return None;
 
     @memoize
     def dec_maybe_call(self) -> Optional[Any]:
@@ -1603,15 +1712,15 @@
         ):
             return class_def_raw;
         self._reset(mark)
         return None;
 
     @memoize
     def class_def_raw(self) -> Optional[ast . ClassDef]:
-        # class_def_raw: invalid_class_def_raw | 'class' NAME ['(' arguments? ')'] &&':' scenic_class_def_block
+        # class_def_raw: invalid_class_def_raw | 'class' NAME type_params? ['(' arguments? ')'] &&':' scenic_class_def_block
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             self.call_invalid_rules
             and
             (self.invalid_class_def_raw())
@@ -1619,23 +1728,25 @@
             return None  # pragma: no cover;
         self._reset(mark)
         if (
             (self.expect('class'))
             and
             (a := self.name())
             and
-            (b := self._tmp_37(),)
+            (t := self.type_params(),)
+            and
+            (b := self._tmp_38(),)
             and
             (self.expect_forced(self.expect(':'), "':'"))
             and
             (c := self.scenic_class_def_block())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
-            return ast . ClassDef ( a . string , bases = b [0] if b else [] , keywords = b [1] if b else [] , body = c , decorator_list = [] , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset , );
+            return ( ast . ClassDef ( a . string , bases = b [0] if b else [] , keywords = b [1] if b else [] , body = c , decorator_list = [] , type_params = t or [] , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset , ) if sys . version_info >= ( 3 , 12 ) else ast . ClassDef ( a . string , bases = b [0] if b else [] , keywords = b [1] if b else [] , body = c , decorator_list = [] , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset , ) );
         self._reset(mark)
         return None;
 
     @memoize
     def scenic_class_def_block(self) -> Optional[Any]:
         # scenic_class_def_block: NEWLINE INDENT scenic_class_statements DEDENT | simple_stmts | invalid_block
         mark = self._mark()
@@ -1665,15 +1776,15 @@
         return None;
 
     @memoize
     def scenic_class_statements(self) -> Optional[list]:
         # scenic_class_statements: scenic_class_statement+
         mark = self._mark()
         if (
-            (a := self._loop1_38())
+            (a := self._loop1_39())
         ):
             return list ( itertools . chain . from_iterable ( a ) );
         self._reset(mark)
         return None;
 
     @memoize
     def scenic_class_statement(self) -> Optional[list]:
@@ -1706,15 +1817,15 @@
         # scenic_class_property_stmt: NAME ['[' ','.scenic_class_property_attribute+ ']'] ':' expression NEWLINE
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (a := self.name())
             and
-            (b := self._tmp_39(),)
+            (b := self._tmp_40(),)
             and
             (self.expect(':'))
             and
             (c := self.expression())
             and
             (self.expect('NEWLINE'))
         ):
@@ -1726,28 +1837,28 @@
 
     @memoize
     def scenic_class_property_attribute(self) -> Optional[Any]:
         # scenic_class_property_attribute: &&("additive" | "dynamic" | "final")
         # nullable=True
         mark = self._mark()
         if (
-            (forced := self.expect_forced(self._tmp_40(), '''("additive" | "dynamic" | "final")'''))
+            (forced := self.expect_forced(self._tmp_41(), '''("additive" | "dynamic" | "final")'''))
         ):
             return forced;
         self._reset(mark)
         return None;
 
     @memoize
     def scenic_assign_new_stmt(self) -> Optional[Any]:
         # scenic_assign_new_stmt: ((star_targets '='))+ (scenic_new_block) !'=' TYPE_COMMENT?
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
-            (a := self._loop1_41())
+            (a := self._loop1_42())
             and
             (b := self.scenic_new_block())
             and
             (self.negative_lookahead(self.expect, '='))
             and
             (tc := self.type_comment(),)
         ):
@@ -1813,24 +1924,24 @@
         return None;
 
     @memoize
     def scenic_new_block_body(self) -> Optional[Any]:
         # scenic_new_block_body: ((scenic_specifiers ',' NEWLINE))* scenic_specifiers NEWLINE | ((scenic_specifiers ',' NEWLINE))+
         mark = self._mark()
         if (
-            (b := self._loop0_42(),)
+            (b := self._loop0_43(),)
             and
             (c := self.scenic_specifiers())
             and
             (self.expect('NEWLINE'))
         ):
             return list ( itertools . chain . from_iterable ( b ) ) + c;
         self._reset(mark)
         if (
-            (b := self._loop1_43())
+            (b := self._loop1_44())
         ):
             return list ( itertools . chain . from_iterable ( b ) );
         self._reset(mark)
         return None;
 
     @memoize
     def scenic_behavior_def(self) -> Optional[Any]:
@@ -1864,15 +1975,15 @@
         # scenic_behavior_def_block: NEWLINE INDENT [STRING NEWLINE] scenic_behavior_header? scenic_behavior_statements DEDENT | invalid_block
         mark = self._mark()
         if (
             (self.expect('NEWLINE'))
             and
             (self.expect('INDENT'))
             and
-            (a := self._tmp_44(),)
+            (a := self._tmp_45(),)
             and
             (b := self.scenic_behavior_header(),)
             and
             (c := self.scenic_behavior_statements())
             and
             (self.expect('DEDENT'))
         ):
@@ -1888,15 +1999,15 @@
         return None;
 
     @memoize
     def scenic_behavior_statements(self) -> Optional[list]:
         # scenic_behavior_statements: scenic_behavior_statement+
         mark = self._mark()
         if (
-            (a := self._loop1_45())
+            (a := self._loop1_46())
         ):
             return list ( itertools . chain . from_iterable ( a ) );
         self._reset(mark)
         return None;
 
     @memoize
     def scenic_behavior_statement(self) -> Optional[list]:
@@ -1939,15 +2050,15 @@
         return None;
 
     @memoize
     def scenic_behavior_header(self) -> Optional[Any]:
         # scenic_behavior_header: (((scenic_precondition_stmt | scenic_invariant_stmt) NEWLINE))+
         mark = self._mark()
         if (
-            (a := self._loop1_46())
+            (a := self._loop1_47())
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
     def scenic_precondition_stmt(self) -> Optional[Any]:
@@ -2041,30 +2152,30 @@
         # scenic_monitor_def_block: NEWLINE INDENT [STRING NEWLINE] scenic_monitor_statements DEDENT
         mark = self._mark()
         if (
             (self.expect('NEWLINE'))
             and
             (self.expect('INDENT'))
             and
-            (a := self._tmp_47(),)
+            (a := self._tmp_48(),)
             and
             (b := self.scenic_monitor_statements())
             and
             (self.expect('DEDENT'))
         ):
             return ( a , b );
         self._reset(mark)
         return None;
 
     @memoize
     def scenic_monitor_statements(self) -> Optional[list]:
         # scenic_monitor_statements: statement+
         mark = self._mark()
         if (
-            (a := self._loop1_48())
+            (a := self._loop1_49())
         ):
             return list ( itertools . chain . from_iterable ( a ) );
         self._reset(mark)
         return None;
 
     @memoize
     def scenic_scenario_def(self) -> Optional[Any]:
@@ -2073,15 +2184,15 @@
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect("scenario"))
             and
             (a := self.name())
             and
-            (b := self._tmp_49(),)
+            (b := self._tmp_50(),)
             and
             (self.expect_forced(self.expect(':'), "':'"))
             and
             (c := self.scenic_scenario_def_block())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
@@ -2094,15 +2205,15 @@
         # scenic_scenario_def_block: NEWLINE INDENT [STRING NEWLINE] scenic_behavior_header? scenic_scenario_setup_block? scenic_scenario_compose_block? DEDENT | NEWLINE INDENT [STRING NEWLINE] statements DEDENT
         mark = self._mark()
         if (
             (self.expect('NEWLINE'))
             and
             (self.expect('INDENT'))
             and
-            (a := self._tmp_50(),)
+            (a := self._tmp_51(),)
             and
             (b := self.scenic_behavior_header(),)
             and
             (c := self.scenic_scenario_setup_block(),)
             and
             (d := self.scenic_scenario_compose_block(),)
             and
@@ -2111,15 +2222,15 @@
             return ( a , b or [] , c or [] , d or [] );
         self._reset(mark)
         if (
             (self.expect('NEWLINE'))
             and
             (self.expect('INDENT'))
             and
-            (a := self._tmp_51(),)
+            (a := self._tmp_52(),)
             and
             (b := self.statements())
             and
             (self.expect('DEDENT'))
         ):
             return ( a , [] , b , [] );
         self._reset(mark)
@@ -2207,15 +2318,15 @@
         ):
             return self . set_decorators ( f , [] );
         self._reset(mark)
         return None;
 
     @memoize
     def function_def_raw(self) -> Optional[Union [ast . FunctionDef , ast . AsyncFunctionDef]]:
-        # function_def_raw: invalid_def_raw | 'def' NAME &&'(' params? ')' ['->' expression] &&':' func_type_comment? block | 'async' 'def' NAME &&'(' params? ')' ['->' expression] &&':' func_type_comment? block
+        # function_def_raw: invalid_def_raw | 'def' NAME type_params? &&'(' params? ')' ['->' expression] &&':' func_type_comment? block | 'async' 'def' NAME type_params? &&'(' params? ')' ['->' expression] &&':' func_type_comment? block
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             self.call_invalid_rules
             and
             (self.invalid_def_raw())
@@ -2223,56 +2334,60 @@
             return None  # pragma: no cover;
         self._reset(mark)
         if (
             (self.expect('def'))
             and
             (n := self.name())
             and
+            (t := self.type_params(),)
+            and
             (self.expect_forced(self.expect('('), "'('"))
             and
             (params := self.params(),)
             and
             (self.expect(')'))
             and
-            (a := self._tmp_52(),)
+            (a := self._tmp_53(),)
             and
             (self.expect_forced(self.expect(':'), "':'"))
             and
             (tc := self.func_type_comment(),)
             and
             (b := self.block())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
-            return ast . FunctionDef ( name = n . string , args = params or self . make_arguments ( None , [] , None , [] , None ) , returns = a , body = b , type_comment = tc , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset , );
+            return ( ast . FunctionDef ( name = n . string , args = params or self . make_arguments ( None , [] , None , [] , None ) , returns = a , body = b , type_comment = tc , type_params = t or [] , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset , ) if sys . version_info >= ( 3 , 12 ) else ast . FunctionDef ( name = n . string , args = params or self . make_arguments ( None , [] , None , [] , None ) , returns = a , body = b , type_comment = tc , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset , ) );
         self._reset(mark)
         if (
             (self.expect('async'))
             and
             (self.expect('def'))
             and
             (n := self.name())
             and
+            (t := self.type_params(),)
+            and
             (self.expect_forced(self.expect('('), "'('"))
             and
             (params := self.params(),)
             and
             (self.expect(')'))
             and
-            (a := self._tmp_53(),)
+            (a := self._tmp_54(),)
             and
             (self.expect_forced(self.expect(':'), "':'"))
             and
             (tc := self.func_type_comment(),)
             and
             (b := self.block())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
-            return self . check_version ( ( 3 , 5 ) , "Async functions are" , ast . AsyncFunctionDef ( name = n . string , args = params or self . make_arguments ( None , [] , None , [] , None ) , returns = a , body = b , type_comment = tc , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset , ) );
+            return ( self . check_version ( ( 3 , 5 ) , "Async functions are" , ast . AsyncFunctionDef ( name = n . string , args = params or self . make_arguments ( None , [] , None , [] , None ) , returns = a , body = b , type_comment = tc , type_params = t or [] , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset , ) ) if sys . version_info >= ( 3 , 12 ) else self . check_version ( ( 3 , 5 ) , "Async functions are" , ast . AsyncFunctionDef ( name = n . string , args = params or self . make_arguments ( None , [] , None , [] , None ) , returns = a , body = b , type_comment = tc , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset , ) ) );
         self._reset(mark)
         return None;
 
     @memoize
     def params(self) -> Optional[Any]:
         # params: invalid_parameters | parameters
         mark = self._mark()
@@ -2293,42 +2408,42 @@
     @memoize
     def parameters(self) -> Optional[ast . arguments]:
         # parameters: slash_no_default param_no_default* param_with_default* star_etc? | slash_with_default param_with_default* star_etc? | param_no_default+ param_with_default* star_etc? | param_with_default+ star_etc? | star_etc
         mark = self._mark()
         if (
             (a := self.slash_no_default())
             and
-            (b := self._loop0_54(),)
+            (b := self._loop0_55(),)
             and
-            (c := self._loop0_55(),)
+            (c := self._loop0_56(),)
             and
             (d := self.star_etc(),)
         ):
             return self . check_version ( ( 3 , 8 ) , "Positional only arguments are" , self . make_arguments ( a , [] , b , c , d ) );
         self._reset(mark)
         if (
             (a := self.slash_with_default())
             and
-            (b := self._loop0_56(),)
+            (b := self._loop0_57(),)
             and
             (c := self.star_etc(),)
         ):
             return self . check_version ( ( 3 , 8 ) , "Positional only arguments are" , self . make_arguments ( None , a , None , b , c ) , );
         self._reset(mark)
         if (
-            (a := self._loop1_57())
+            (a := self._loop1_58())
             and
-            (b := self._loop0_58(),)
+            (b := self._loop0_59(),)
             and
             (c := self.star_etc(),)
         ):
             return self . make_arguments ( None , [] , a , b , c );
         self._reset(mark)
         if (
-            (a := self._loop1_59())
+            (a := self._loop1_60())
             and
             (b := self.star_etc(),)
         ):
             return self . make_arguments ( None , [] , None , a , b );
         self._reset(mark)
         if (
             (a := self.star_etc())
@@ -2338,89 +2453,100 @@
         return None;
 
     @memoize
     def slash_no_default(self) -> Optional[List [Tuple [ast . arg , None]]]:
         # slash_no_default: param_no_default+ '/' ',' | param_no_default+ '/' &')'
         mark = self._mark()
         if (
-            (a := self._loop1_60())
+            (a := self._loop1_61())
             and
             (self.expect('/'))
             and
             (self.expect(','))
         ):
             return [( p , None ) for p in a];
         self._reset(mark)
         if (
-            (a := self._loop1_61())
+            (a := self._loop1_62())
             and
             (self.expect('/'))
             and
             (self.positive_lookahead(self.expect, ')'))
         ):
             return [( p , None ) for p in a];
         self._reset(mark)
         return None;
 
     @memoize
     def slash_with_default(self) -> Optional[List [Tuple [ast . arg , Any]]]:
         # slash_with_default: param_no_default* param_with_default+ '/' ',' | param_no_default* param_with_default+ '/' &')'
         mark = self._mark()
         if (
-            (a := self._loop0_62(),)
+            (a := self._loop0_63(),)
             and
-            (b := self._loop1_63())
+            (b := self._loop1_64())
             and
             (self.expect('/'))
             and
             (self.expect(','))
         ):
             return ( [( p , None ) for p in a] if a else [] ) + b;
         self._reset(mark)
         if (
-            (a := self._loop0_64(),)
+            (a := self._loop0_65(),)
             and
-            (b := self._loop1_65())
+            (b := self._loop1_66())
             and
             (self.expect('/'))
             and
             (self.positive_lookahead(self.expect, ')'))
         ):
             return ( [( p , None ) for p in a] if a else [] ) + b;
         self._reset(mark)
         return None;
 
     @memoize
     def star_etc(self) -> Optional[Tuple [Optional [ast . arg] , List [Tuple [ast . arg , Any]] , Optional [ast . arg]]]:
-        # star_etc: invalid_star_etc | '*' param_no_default param_maybe_default* kwds? | '*' ',' param_maybe_default+ kwds? | kwds
+        # star_etc: invalid_star_etc | '*' param_no_default param_maybe_default* kwds? | '*' param_no_default_star_annotation param_maybe_default* kwds? | '*' ',' param_maybe_default+ kwds? | kwds
         mark = self._mark()
         if (
             self.call_invalid_rules
             and
             (self.invalid_star_etc())
         ):
             return None  # pragma: no cover;
         self._reset(mark)
         if (
             (self.expect('*'))
             and
             (a := self.param_no_default())
             and
-            (b := self._loop0_66(),)
+            (b := self._loop0_67(),)
+            and
+            (c := self.kwds(),)
+        ):
+            return ( a , b , c );
+        self._reset(mark)
+        if (
+            (self.expect('*'))
+            and
+            (a := self.param_no_default_star_annotation())
+            and
+            (b := self._loop0_68(),)
             and
             (c := self.kwds(),)
         ):
             return ( a , b , c );
         self._reset(mark)
         if (
             (self.expect('*'))
             and
             (self.expect(','))
             and
-            (b := self._loop1_67())
+            (b := self._loop1_69())
             and
             (c := self.kwds(),)
         ):
             return ( None , b , c );
         self._reset(mark)
         if (
             (a := self.kwds())
@@ -2470,14 +2596,38 @@
             (self.positive_lookahead(self.expect, ')'))
         ):
             return self . set_arg_type_comment ( a , tc );
         self._reset(mark)
         return None;
 
     @memoize
+    def param_no_default_star_annotation(self) -> Optional[ast . arg]:
+        # param_no_default_star_annotation: param_star_annotation ',' TYPE_COMMENT? | param_star_annotation TYPE_COMMENT? &')'
+        mark = self._mark()
+        if (
+            (a := self.param_star_annotation())
+            and
+            (self.expect(','))
+            and
+            (tc := self.type_comment(),)
+        ):
+            return self . set_arg_type_comment ( a , tc );
+        self._reset(mark)
+        if (
+            (a := self.param_star_annotation())
+            and
+            (tc := self.type_comment(),)
+            and
+            (self.positive_lookahead(self.expect, ')'))
+        ):
+            return self . set_arg_type_comment ( a , tc );
+        self._reset(mark)
+        return None;
+
+    @memoize
     def param_with_default(self) -> Optional[Tuple [ast . arg , Any]]:
         # param_with_default: param default ',' TYPE_COMMENT? | param default TYPE_COMMENT? &')'
         mark = self._mark()
         if (
             (a := self.param())
             and
             (c := self.default())
@@ -2543,27 +2693,57 @@
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . arg ( arg = a . string , annotation = b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
     @memoize
+    def param_star_annotation(self) -> Optional[Any]:
+        # param_star_annotation: NAME star_annotation
+        mark = self._mark()
+        tok = self._tokenizer.peek()
+        start_lineno, start_col_offset = tok.start
+        if (
+            (a := self.name())
+            and
+            (b := self.star_annotation())
+        ):
+            tok = self._tokenizer.get_last_non_whitespace_token()
+            end_lineno, end_col_offset = tok.end
+            return ast . arg ( arg = a . string , annotations = b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
+        self._reset(mark)
+        return None;
+
+    @memoize
     def annotation(self) -> Optional[Any]:
         # annotation: ':' expression
         mark = self._mark()
         if (
             (self.expect(':'))
             and
             (a := self.expression())
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
+    def star_annotation(self) -> Optional[Any]:
+        # star_annotation: ':' star_expression
+        mark = self._mark()
+        if (
+            (self.expect(':'))
+            and
+            (a := self.star_expression())
+        ):
+            return a;
+        self._reset(mark)
+        return None;
+
+    @memoize
     def default(self) -> Optional[Any]:
         # default: '=' expression | invalid_default
         mark = self._mark()
         if (
             (self.expect('='))
             and
             (a := self.expression())
@@ -2811,15 +2991,15 @@
             return None  # pragma: no cover;
         self._reset(mark)
         if (
             (self.expect('with'))
             and
             (self.expect('('))
             and
-            (a := self._gather_68())
+            (a := self._gather_70())
             and
             (self.expect(','),)
             and
             (self.expect(')'))
             and
             (self.expect(':'))
             and
@@ -2828,15 +3008,15 @@
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return self . check_version ( ( 3 , 9 ) , "Parenthesized with items" , ast . With ( items = a , body = b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset ) );
         self._reset(mark)
         if (
             (self.expect('with'))
             and
-            (a := self._gather_70())
+            (a := self._gather_72())
             and
             (self.expect(':'))
             and
             (tc := self.type_comment(),)
             and
             (b := self.block())
         ):
@@ -2847,15 +3027,15 @@
         if (
             (self.expect('async'))
             and
             (self.expect('with'))
             and
             (self.expect('('))
             and
-            (a := self._gather_72())
+            (a := self._gather_74())
             and
             (self.expect(','),)
             and
             (self.expect(')'))
             and
             (self.expect(':'))
             and
@@ -2866,15 +3046,15 @@
             return self . check_version ( ( 3 , 9 ) , "Parenthesized with items" , ast . AsyncWith ( items = a , body = b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset ) );
         self._reset(mark)
         if (
             (self.expect('async'))
             and
             (self.expect('with'))
             and
-            (a := self._gather_74())
+            (a := self._gather_76())
             and
             (self.expect(':'))
             and
             (tc := self.type_comment(),)
             and
             (b := self.block())
         ):
@@ -2898,15 +3078,15 @@
         if (
             (e := self.expression())
             and
             (self.expect('as'))
             and
             (t := self.star_target())
             and
-            (self.positive_lookahead(self._tmp_76, ))
+            (self.positive_lookahead(self._tmp_78, ))
         ):
             return ast . withitem ( context_expr = e , optional_vars = t );
         self._reset(mark)
         if (
             self.call_invalid_rules
             and
             (self.invalid_with_item())
@@ -2918,15 +3098,15 @@
         ):
             return ast . withitem ( context_expr = e , optional_vars = None );
         self._reset(mark)
         return None;
 
     @memoize
     def try_stmt(self) -> Optional[ast . Try]:
-        # try_stmt: invalid_try_stmt | 'try' &&':' block finally_block | 'try' &&':' block except_block+ else_block? finally_block?
+        # try_stmt: invalid_try_stmt | 'try' &&':' block finally_block | 'try' &&':' block except_block+ else_block? finally_block? | 'try' &&':' block except_star_block+ else_block? finally_block?
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             self.call_invalid_rules
             and
             (self.invalid_try_stmt())
@@ -2949,24 +3129,41 @@
         if (
             (self.expect('try'))
             and
             (self.expect_forced(self.expect(':'), "':'"))
             and
             (b := self.block())
             and
-            (ex := self._loop1_77())
+            (ex := self._loop1_79())
             and
             (el := self.else_block(),)
             and
             (f := self.finally_block(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Try ( body = b , handlers = ex , orelse = el or [] , finalbody = f or [] , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
+        if (
+            (self.expect('try'))
+            and
+            (self.expect_forced(self.expect(':'), "':'"))
+            and
+            (b := self.block())
+            and
+            (ex := self._loop1_80())
+            and
+            (el := self.else_block(),)
+            and
+            (f := self.finally_block(),)
+        ):
+            tok = self._tokenizer.get_last_non_whitespace_token()
+            end_lineno, end_col_offset = tok.end
+            return self . check_version ( ( 3 , 11 ) , "Exception groups are" , ( ast . TryStar ( body = b , handlers = ex , orelse = el or [] , finalbody = f or [] , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset ) if sys . version_info >= ( 3 , 11 ) else None ) );
+        self._reset(mark)
         return None;
 
     @memoize
     def scenic_try_interrupt_stmt(self) -> Optional[s . TryInterrupt]:
         # scenic_try_interrupt_stmt: 'try' &&':' block interrupt_when_block+ except_block* else_block? finally_block?
         mark = self._mark()
         tok = self._tokenizer.peek()
@@ -2974,17 +3171,17 @@
         if (
             (self.expect('try'))
             and
             (self.expect_forced(self.expect(':'), "':'"))
             and
             (b := self.block())
             and
-            (iw := self._loop1_78())
+            (iw := self._loop1_81())
             and
-            (ex := self._loop0_79(),)
+            (ex := self._loop0_82(),)
             and
             (el := self.else_block(),)
             and
             (f := self.finally_block(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
@@ -3029,15 +3226,15 @@
             return None  # pragma: no cover;
         self._reset(mark)
         if (
             (self.expect('except'))
             and
             (e := self.expression())
             and
-            (t := self._tmp_80(),)
+            (t := self._tmp_83(),)
             and
             (self.expect(':'))
             and
             (b := self.block())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
@@ -3060,14 +3257,53 @@
             (self.invalid_except_stmt())
         ):
             return None  # pragma: no cover;
         self._reset(mark)
         return None;
 
     @memoize
+    def except_star_block(self) -> Optional[ast . ExceptHandler]:
+        # except_star_block: invalid_except_star_stmt_indent | 'except' '*' expression ['as' NAME] ':' block | invalid_except_stmt
+        mark = self._mark()
+        tok = self._tokenizer.peek()
+        start_lineno, start_col_offset = tok.start
+        if (
+            self.call_invalid_rules
+            and
+            (self.invalid_except_star_stmt_indent())
+        ):
+            return None  # pragma: no cover;
+        self._reset(mark)
+        if (
+            (self.expect('except'))
+            and
+            (self.expect('*'))
+            and
+            (e := self.expression())
+            and
+            (t := self._tmp_84(),)
+            and
+            (self.expect(':'))
+            and
+            (b := self.block())
+        ):
+            tok = self._tokenizer.get_last_non_whitespace_token()
+            end_lineno, end_col_offset = tok.end
+            return ast . ExceptHandler ( type = e , name = t , body = b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
+        self._reset(mark)
+        if (
+            self.call_invalid_rules
+            and
+            (self.invalid_except_stmt())
+        ):
+            return None  # pragma: no cover;
+        self._reset(mark)
+        return None;
+
+    @memoize
     def finally_block(self) -> Optional[list]:
         # finally_block: invalid_finally_stmt | 'finally' &&':' block
         mark = self._mark()
         if (
             self.call_invalid_rules
             and
             (self.invalid_finally_stmt())
@@ -3098,15 +3334,15 @@
             and
             (self.expect(':'))
             and
             (self.expect('NEWLINE'))
             and
             (self.expect('INDENT'))
             and
-            (cases := self._loop1_81())
+            (cases := self._loop1_85())
             and
             (self.expect('DEDENT'))
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Match ( subject = subject , cases = cases , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
@@ -3247,15 +3483,15 @@
     @memoize
     def or_pattern(self) -> Optional["ast.MatchOr"]:
         # or_pattern: '|'.closed_pattern+
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
-            (patterns := self._gather_82())
+            (patterns := self._gather_86())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . MatchOr ( patterns = patterns , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset ) if len ( patterns ) > 1 else patterns [0];
         self._reset(mark)
         return None;
 
@@ -3310,15 +3546,15 @@
         # literal_pattern: signed_number !('+' | '-') | complex_number | strings | 'None' | 'True' | 'False'
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (value := self.signed_number())
             and
-            (self.negative_lookahead(self._tmp_84, ))
+            (self.negative_lookahead(self._tmp_88, ))
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . MatchValue ( value = value , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (value := self.complex_number())
@@ -3362,15 +3598,15 @@
         # literal_expr: signed_number !('+' | '-') | complex_number | strings | 'None' | 'True' | 'False'
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (signed_number := self.signed_number())
             and
-            (self.negative_lookahead(self._tmp_85, ))
+            (self.negative_lookahead(self._tmp_89, ))
         ):
             return signed_number;
         self._reset(mark)
         if (
             (complex_number := self.complex_number())
         ):
             return complex_number;
@@ -3529,15 +3765,15 @@
         # pattern_capture_target: !"_" NAME !('.' | '(' | '=')
         mark = self._mark()
         if (
             (self.negative_lookahead(self.expect, "_"))
             and
             (name := self.name())
             and
-            (self.negative_lookahead(self._tmp_86, ))
+            (self.negative_lookahead(self._tmp_90, ))
         ):
             return name . string;
         self._reset(mark)
         return None;
 
     @memoize
     def wildcard_pattern(self) -> Optional["ast.MatchAs"]:
@@ -3559,15 +3795,15 @@
         # value_pattern: attr !('.' | '(' | '=')
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (attr := self.attr())
             and
-            (self.negative_lookahead(self._tmp_87, ))
+            (self.negative_lookahead(self._tmp_91, ))
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . MatchValue ( value = attr , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
@@ -3671,15 +3907,15 @@
         return None;
 
     @memoize
     def maybe_sequence_pattern(self) -> Optional[Any]:
         # maybe_sequence_pattern: ','.maybe_star_pattern+ ','?
         mark = self._mark()
         if (
-            (patterns := self._gather_88())
+            (patterns := self._gather_92())
             and
             (self.expect(','),)
         ):
             return patterns;
         self._reset(mark)
         return None;
 
@@ -3786,26 +4022,26 @@
         return None;
 
     @memoize
     def items_pattern(self) -> Optional[Any]:
         # items_pattern: ','.key_value_pattern+
         mark = self._mark()
         if (
-            (_gather_90 := self._gather_90())
+            (_gather_94 := self._gather_94())
         ):
-            return _gather_90;
+            return _gather_94;
         self._reset(mark)
         return None;
 
     @memoize
     def key_value_pattern(self) -> Optional[Any]:
         # key_value_pattern: (literal_expr | attr) ':' pattern
         mark = self._mark()
         if (
-            (key := self._tmp_92())
+            (key := self._tmp_96())
             and
             (self.expect(':'))
             and
             (pattern := self.pattern())
         ):
             return ( key , pattern );
         self._reset(mark)
@@ -3900,28 +4136,28 @@
         return None;
 
     @memoize
     def positional_patterns(self) -> Optional[Any]:
         # positional_patterns: ','.pattern+
         mark = self._mark()
         if (
-            (args := self._gather_93())
+            (args := self._gather_97())
         ):
             return args;
         self._reset(mark)
         return None;
 
     @memoize
     def keyword_patterns(self) -> Optional[Any]:
         # keyword_patterns: ','.keyword_pattern+
         mark = self._mark()
         if (
-            (_gather_95 := self._gather_95())
+            (_gather_99 := self._gather_99())
         ):
-            return _gather_95;
+            return _gather_99;
         self._reset(mark)
         return None;
 
     @memoize
     def keyword_pattern(self) -> Optional[Any]:
         # keyword_pattern: NAME '=' pattern
         mark = self._mark()
@@ -3933,23 +4169,144 @@
             (value := self.pattern())
         ):
             return ( arg . string , value );
         self._reset(mark)
         return None;
 
     @memoize
+    def type_alias(self) -> Optional["ast.TypeAlias"]:
+        # type_alias: "type" NAME type_params? '=' expression
+        mark = self._mark()
+        tok = self._tokenizer.peek()
+        start_lineno, start_col_offset = tok.start
+        if (
+            (self.expect("type"))
+            and
+            (n := self.name())
+            and
+            (t := self.type_params(),)
+            and
+            (self.expect('='))
+            and
+            (b := self.expression())
+        ):
+            tok = self._tokenizer.get_last_non_whitespace_token()
+            end_lineno, end_col_offset = tok.end
+            return self . check_version ( ( 3 , 12 ) , "Type statement is" , ( ast . TypeAlias ( name = ast . Name ( id = n . string , ctx = Store , lineno = n . start [0] , col_offset = n . start [1] , end_lineno = n . end [0] , end_col_offset = n . end [1] , ) , type_params = t or [] , value = b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset ) if sys . version_info >= ( 3 , 12 ) else None ) );
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def type_params(self) -> Optional[list]:
+        # type_params: '[' type_param_seq ']'
+        mark = self._mark()
+        if (
+            (self.expect('['))
+            and
+            (t := self.type_param_seq())
+            and
+            (self.expect(']'))
+        ):
+            return self . check_version ( ( 3 , 12 ) , "Type parameter lists are" , t );
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def type_param_seq(self) -> Optional[Any]:
+        # type_param_seq: ','.type_param+ ','?
+        mark = self._mark()
+        if (
+            (a := self._gather_101())
+            and
+            (self.expect(','),)
+        ):
+            return a;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def type_param(self) -> Optional[Any]:
+        # type_param: NAME type_param_bound? | '*' NAME ":" expression | '*' NAME | '**' NAME ":" expression | '**' NAME
+        mark = self._mark()
+        tok = self._tokenizer.peek()
+        start_lineno, start_col_offset = tok.start
+        if (
+            (a := self.name())
+            and
+            (b := self.type_param_bound(),)
+        ):
+            tok = self._tokenizer.get_last_non_whitespace_token()
+            end_lineno, end_col_offset = tok.end
+            return ast . TypeVar ( name = a . string , bound = b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset ) if sys . version_info >= ( 3 , 12 ) else object ( );
+        self._reset(mark)
+        if (
+            (self.expect('*'))
+            and
+            (self.name())
+            and
+            (colon := self.expect(":"))
+            and
+            (e := self.expression())
+        ):
+            return self . raise_syntax_error_starting_from ( "cannot use constraints with TypeVarTuple" if isinstance ( e , ast . Tuple ) else "cannot use bound with TypeVarTuple" , colon );
+        self._reset(mark)
+        if (
+            (self.expect('*'))
+            and
+            (a := self.name())
+        ):
+            tok = self._tokenizer.get_last_non_whitespace_token()
+            end_lineno, end_col_offset = tok.end
+            return ast . TypeVarTuple ( name = a . string , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset ) if sys . version_info >= ( 3 , 12 ) else object ( );
+        self._reset(mark)
+        if (
+            (self.expect('**'))
+            and
+            (self.name())
+            and
+            (colon := self.expect(":"))
+            and
+            (e := self.expression())
+        ):
+            return self . raise_syntax_error_starting_from ( "cannot use constraints with ParamSpec" if isinstance ( e , ast . Tuple ) else "cannot use bound with ParamSpec" , colon );
+        self._reset(mark)
+        if (
+            (self.expect('**'))
+            and
+            (a := self.name())
+        ):
+            tok = self._tokenizer.get_last_non_whitespace_token()
+            end_lineno, end_col_offset = tok.end
+            return ast . ParamSpec ( name = a . string , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset ) if sys . version_info >= ( 3 , 12 ) else object ( );
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def type_param_bound(self) -> Optional[Any]:
+        # type_param_bound: ":" expression
+        mark = self._mark()
+        if (
+            (self.expect(":"))
+            and
+            (e := self.expression())
+        ):
+            return e;
+        self._reset(mark)
+        return None;
+
+    @memoize
     def expressions(self) -> Optional[Any]:
         # expressions: expression ((',' expression))+ ','? | expression ',' | expression
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (a := self.expression())
             and
-            (b := self._loop1_97())
+            (b := self._loop1_103())
             and
             (self.expect(','),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Tuple ( elts = [a] + b , ctx = Load , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
@@ -4103,15 +4460,15 @@
         # star_expressions: star_expression ((',' star_expression))+ ','? | star_expression ',' | star_expression
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (a := self.star_expression())
             and
-            (b := self._loop1_98())
+            (b := self._loop1_104())
             and
             (self.expect(','),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Tuple ( elts = [a] + b , ctx = Load , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
@@ -4154,15 +4511,15 @@
         return None;
 
     @memoize
     def star_named_expressions(self) -> Optional[Any]:
         # star_named_expressions: ','.star_named_expression+ ','?
         mark = self._mark()
         if (
-            (a := self._gather_99())
+            (a := self._gather_105())
             and
             (self.expect(','),)
         ):
             return a;
         self._reset(mark)
         return None;
 
@@ -4333,15 +4690,15 @@
             return None  # pragma: no cover;
         self._reset(mark)
         if (
             (a := self.scenic_temporal_disjunction())
             and
             (self.expect("implies"))
             and
-            (b := self._tmp_101())
+            (b := self._tmp_107())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . ImpliesOp ( a , b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (scenic_temporal_disjunction := self.scenic_temporal_disjunction())
@@ -4355,15 +4712,15 @@
         # disjunction: conjunction (('or' conjunction))+ | conjunction
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (a := self.conjunction())
             and
-            (b := self._loop1_102())
+            (b := self._loop1_108())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . BoolOp ( op = ast . Or ( ) , values = [a] + b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (conjunction := self.conjunction())
@@ -4377,15 +4734,15 @@
         # scenic_temporal_disjunction: scenic_temporal_conjunction (('or' (scenic_temporal_prefix | scenic_temporal_conjunction)))+ | scenic_temporal_conjunction
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (a := self.scenic_temporal_conjunction())
             and
-            (b := self._loop1_103())
+            (b := self._loop1_109())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . BoolOp ( op = ast . Or ( ) , values = [a] + b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (scenic_temporal_conjunction := self.scenic_temporal_conjunction())
@@ -4399,15 +4756,15 @@
         # conjunction: inversion (('and' inversion))+ | inversion
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (a := self.inversion())
             and
-            (b := self._loop1_104())
+            (b := self._loop1_110())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . BoolOp ( op = ast . And ( ) , values = [a] + b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (inversion := self.inversion())
@@ -4421,15 +4778,15 @@
         # scenic_temporal_conjunction: scenic_temporal_inversion (('and' (scenic_temporal_prefix | scenic_temporal_inversion)))+ | scenic_temporal_inversion
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (a := self.scenic_temporal_inversion())
             and
-            (b := self._loop1_105())
+            (b := self._loop1_111())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . BoolOp ( op = ast . And ( ) , values = [a] + b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (scenic_temporal_inversion := self.scenic_temporal_inversion())
@@ -4443,15 +4800,15 @@
         # inversion: 'not' !("visible" inversion) inversion | comparison
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect('not'))
             and
-            (self.negative_lookahead(self._tmp_106, ))
+            (self.negative_lookahead(self._tmp_112, ))
             and
             (a := self.inversion())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . UnaryOp ( op = ast . Not ( ) , operand = a , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
@@ -4467,17 +4824,17 @@
         # scenic_temporal_inversion: 'not' !("visible" scenic_temporal_inversion) (scenic_temporal_prefix | scenic_temporal_inversion) | scenic_temporal_group | comparison
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect('not'))
             and
-            (self.negative_lookahead(self._tmp_107, ))
+            (self.negative_lookahead(self._tmp_113, ))
             and
-            (a := self._tmp_108())
+            (a := self._tmp_114())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . UnaryOp ( op = ast . Not ( ) , operand = a , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (scenic_temporal_group := self.scenic_temporal_group())
@@ -4498,15 +4855,15 @@
         if (
             (self.expect('('))
             and
             (a := self.scenic_temporal_expression())
             and
             (self.expect(')'))
             and
-            (self.positive_lookahead(self._tmp_109, ))
+            (self.positive_lookahead(self._tmp_115, ))
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
     def scenic_new_expr(self) -> Optional[Any]:
@@ -4528,15 +4885,15 @@
         return None;
 
     @memoize
     def scenic_specifiers(self) -> Optional[Any]:
         # scenic_specifiers: ','.scenic_specifier+
         mark = self._mark()
         if (
-            (ss := self._gather_110())
+            (ss := self._gather_116())
         ):
             return ss;
         self._reset(mark)
         return None;
 
     @memoize
     def scenic_specifier(self) -> Optional[Any]:
@@ -4609,48 +4966,48 @@
             return s . OffsetAlongSpecifier ( direction = d , offset = o , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (direction := self.scenic_specifier_position_direction())
             and
             (position := self.expression())
             and
-            (distance := self._tmp_112(),)
+            (distance := self._tmp_118(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . DirectionOfSpecifier ( direction = direction , position = position , distance = distance , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (self.expect("beyond"))
             and
             (v := self.expression())
             and
             (self.expect('by'))
             and
             (o := self.expression())
             and
-            (b := self._tmp_113(),)
+            (b := self._tmp_119(),)
         ):
             return s . BeyondSpecifier ( position = v , offset = o , base = b );
         self._reset(mark)
         if (
             (self.expect("visible"))
             and
-            (b := self._tmp_114(),)
+            (b := self._tmp_120(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . VisibleSpecifier ( base = b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (self.expect('not'))
             and
             (self.expect("visible"))
             and
-            (b := self._tmp_115(),)
+            (b := self._tmp_121(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . NotVisibleSpecifier ( base = b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (self.expect('in'))
@@ -4682,15 +5039,15 @@
             return s . ContainedInSpecifier ( region = r , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (self.expect("following"))
             and
             (f := self.expression())
             and
-            (b := self._tmp_116(),)
+            (b := self._tmp_122(),)
             and
             (self.expect('for'))
             and
             (d := self.expression())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
@@ -4760,15 +5117,15 @@
         if (
             (self.expect("apparently"))
             and
             (self.expect("facing"))
             and
             (h := self.expression())
             and
-            (v := self._tmp_117(),)
+            (v := self._tmp_123(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . ApparentlyFacingSpecifier ( heading = h , base = v , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
@@ -4833,15 +5190,15 @@
         # comparison: bitwise_or compare_op_bitwise_or_pair+ | bitwise_or
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (a := self.bitwise_or())
             and
-            (b := self._loop1_118())
+            (b := self._loop1_124())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Compare ( left = a , ops = self . get_comparison_ops ( b ) , comparators = self . get_comparators ( b ) , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (bitwise_or := self.bitwise_or())
@@ -5038,15 +5395,15 @@
         ):
             return ( ast . Is ( ) , a );
         self._reset(mark)
         return None;
 
     @memoize_left_rec
     def bitwise_or(self) -> Optional[Any]:
-        # bitwise_or: scenic_visible_from | scenic_not_visible_from | scenic_can_see | bitwise_or '|' bitwise_xor | bitwise_xor
+        # bitwise_or: scenic_visible_from | scenic_not_visible_from | scenic_can_see | scenic_intersects | bitwise_or '|' bitwise_xor | bitwise_xor
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (scenic_visible_from := self.scenic_visible_from())
         ):
             return scenic_visible_from;
@@ -5058,14 +5415,19 @@
         self._reset(mark)
         if (
             (scenic_can_see := self.scenic_can_see())
         ):
             return scenic_can_see;
         self._reset(mark)
         if (
+            (scenic_intersects := self.scenic_intersects())
+        ):
+            return scenic_intersects;
+        self._reset(mark)
+        if (
             (a := self.bitwise_or())
             and
             (self.expect('|'))
             and
             (b := self.bitwise_xor())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
@@ -5140,14 +5502,33 @@
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . CanSeeOp ( left = a , right = b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
+    @logger
+    def scenic_intersects(self) -> Optional[Any]:
+        # scenic_intersects: bitwise_or "intersects" bitwise_xor
+        mark = self._mark()
+        tok = self._tokenizer.peek()
+        start_lineno, start_col_offset = tok.start
+        if (
+            (a := self.bitwise_or())
+            and
+            (self.expect("intersects"))
+            and
+            (b := self.bitwise_xor())
+        ):
+            tok = self._tokenizer.get_last_non_whitespace_token()
+            end_lineno, end_col_offset = tok.end
+            return s . IntersectsOp ( left = a , right = b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
+        self._reset(mark)
+        return None;
+
     @memoize_left_rec
     def bitwise_xor(self) -> Optional[Any]:
         # bitwise_xor: scenic_offset_along | bitwise_xor '^' bitwise_and | bitwise_and
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
@@ -5232,15 +5613,15 @@
         # scenic_relative_to: bitwise_and ("relative" 'to' | "offset" 'by') shift_expr
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (a := self.bitwise_and())
             and
-            (self._tmp_119())
+            (self._tmp_125())
             and
             (b := self.shift_expr())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . RelativeToOp ( left = a , right = b , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
@@ -5538,15 +5919,15 @@
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . DistanceFromOp ( target = e1 , base = e2 , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (self.expect("distance"))
             and
-            (self._tmp_120())
+            (self._tmp_126())
             and
             (e1 := self.scenic_prefix_operators())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . DistanceFromOp ( target = e1 , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
@@ -6154,27 +6535,27 @@
         ):
             return atom;
         self._reset(mark)
         return None;
 
     @memoize
     def slices(self) -> Optional[Any]:
-        # slices: slice !',' | ','.slice+ ','?
+        # slices: slice !',' | ','.(slice | starred_expression)+ ','?
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (a := self.slice())
             and
             (self.negative_lookahead(self.expect, ','))
         ):
             return a;
         self._reset(mark)
         if (
-            (a := self._gather_121())
+            (a := self._gather_127())
             and
             (self.expect(','),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Tuple ( elts = a , ctx = Load , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset ) if sys . version_info >= ( 3 , 9 ) else ( ast . ExtSlice ( dims = a , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset ) if any ( isinstance ( e , ast . Slice ) for e in a ) else ast . Index ( value = ast . Tuple ( elts = [e . value for e in a] , ctx = Load , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset ) , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset ) );
         self._reset(mark)
@@ -6189,30 +6570,30 @@
         if (
             (a := self.expression(),)
             and
             (self.expect(':'))
             and
             (b := self.expression(),)
             and
-            (c := self._tmp_123(),)
+            (c := self._tmp_129(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Slice ( lower = a , upper = b , step = c , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (a := self.named_expression())
         ):
             return a if sys . version_info >= ( 3 , 9 ) or isinstance ( a , ast . Slice ) else ast . Index ( value = a , lineno = a . lineno , col_offset = a . col_offset , end_lineno = a . end_lineno , end_col_offset = a . end_col_offset );
         self._reset(mark)
         return None;
 
     @memoize
     def atom(self) -> Optional[Any]:
-        # atom: "initial" "scenario" | NAME | 'True' | 'False' | 'None' | &STRING strings | NUMBER | &'(' (tuple | group | genexp) | &'[' (list | listcomp) | &'{' (dict | set | dictcomp | setcomp) | '...'
+        # atom: "initial" "scenario" | NAME | 'True' | 'False' | 'None' | &(STRING | FSTRING_START) strings | NUMBER | &'(' (tuple | group | genexp) | &'[' (list | listcomp) | &'{' (dict | set | dictcomp | setcomp) | '...'
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect("initial"))
             and
             (self.expect("scenario"))
@@ -6246,15 +6627,15 @@
             (self.expect('None'))
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Constant ( value = None , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset ) if sys . version_info >= ( 3 , 9 ) else ast . Constant ( value = None , kind = None , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
-            (self.positive_lookahead(self.string, ))
+            (self.positive_lookahead(self._tmp_130, ))
             and
             (strings := self.strings())
         ):
             return strings;
         self._reset(mark)
         if (
             (a := self.number())
@@ -6262,31 +6643,31 @@
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Constant ( value = ast . literal_eval ( a . string ) , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset ) if sys . version_info >= ( 3 , 9 ) else ast . Constant ( value = ast . literal_eval ( a . string ) , kind = None , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (self.positive_lookahead(self.expect, '('))
             and
-            (_tmp_124 := self._tmp_124())
+            (_tmp_131 := self._tmp_131())
         ):
-            return _tmp_124;
+            return _tmp_131;
         self._reset(mark)
         if (
             (self.positive_lookahead(self.expect, '['))
             and
-            (_tmp_125 := self._tmp_125())
+            (_tmp_132 := self._tmp_132())
         ):
-            return _tmp_125;
+            return _tmp_132;
         self._reset(mark)
         if (
             (self.positive_lookahead(self.expect, '{'))
             and
-            (_tmp_126 := self._tmp_126())
+            (_tmp_133 := self._tmp_133())
         ):
-            return _tmp_126;
+            return _tmp_133;
         self._reset(mark)
         if (
             (self.expect('...'))
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Constant ( value = Ellipsis , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset ) if sys . version_info >= ( 3 , 9 ) else ast . Constant ( value = Ellipsis , kind = None , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
@@ -6296,15 +6677,15 @@
     @memoize
     def group(self) -> Optional[Any]:
         # group: '(' (yield_expr | named_expression) ')' | invalid_group
         mark = self._mark()
         if (
             (self.expect('('))
             and
-            (a := self._tmp_127())
+            (a := self._tmp_134())
             and
             (self.expect(')'))
         ):
             return a;
         self._reset(mark)
         if (
             self.call_invalid_rules
@@ -6357,42 +6738,42 @@
     @memoize
     def lambda_parameters(self) -> Optional[ast . arguments]:
         # lambda_parameters: lambda_slash_no_default lambda_param_no_default* lambda_param_with_default* lambda_star_etc? | lambda_slash_with_default lambda_param_with_default* lambda_star_etc? | lambda_param_no_default+ lambda_param_with_default* lambda_star_etc? | lambda_param_with_default+ lambda_star_etc? | lambda_star_etc
         mark = self._mark()
         if (
             (a := self.lambda_slash_no_default())
             and
-            (b := self._loop0_128(),)
+            (b := self._loop0_135(),)
             and
-            (c := self._loop0_129(),)
+            (c := self._loop0_136(),)
             and
             (d := self.lambda_star_etc(),)
         ):
             return self . make_arguments ( a , [] , b , c , d );
         self._reset(mark)
         if (
             (a := self.lambda_slash_with_default())
             and
-            (b := self._loop0_130(),)
+            (b := self._loop0_137(),)
             and
             (c := self.lambda_star_etc(),)
         ):
             return self . make_arguments ( None , a , None , b , c );
         self._reset(mark)
         if (
-            (a := self._loop1_131())
+            (a := self._loop1_138())
             and
-            (b := self._loop0_132(),)
+            (b := self._loop0_139(),)
             and
             (c := self.lambda_star_etc(),)
         ):
             return self . make_arguments ( None , [] , a , b , c );
         self._reset(mark)
         if (
-            (a := self._loop1_133())
+            (a := self._loop1_140())
             and
             (b := self.lambda_star_etc(),)
         ):
             return self . make_arguments ( None , [] , None , a , b );
         self._reset(mark)
         if (
             (a := self.lambda_star_etc())
@@ -6402,52 +6783,52 @@
         return None;
 
     @memoize
     def lambda_slash_no_default(self) -> Optional[List [Tuple [ast . arg , None]]]:
         # lambda_slash_no_default: lambda_param_no_default+ '/' ',' | lambda_param_no_default+ '/' &':'
         mark = self._mark()
         if (
-            (a := self._loop1_134())
+            (a := self._loop1_141())
             and
             (self.expect('/'))
             and
             (self.expect(','))
         ):
             return [( p , None ) for p in a];
         self._reset(mark)
         if (
-            (a := self._loop1_135())
+            (a := self._loop1_142())
             and
             (self.expect('/'))
             and
             (self.positive_lookahead(self.expect, ':'))
         ):
             return [( p , None ) for p in a];
         self._reset(mark)
         return None;
 
     @memoize
     def lambda_slash_with_default(self) -> Optional[List [Tuple [ast . arg , Any]]]:
         # lambda_slash_with_default: lambda_param_no_default* lambda_param_with_default+ '/' ',' | lambda_param_no_default* lambda_param_with_default+ '/' &':'
         mark = self._mark()
         if (
-            (a := self._loop0_136(),)
+            (a := self._loop0_143(),)
             and
-            (b := self._loop1_137())
+            (b := self._loop1_144())
             and
             (self.expect('/'))
             and
             (self.expect(','))
         ):
             return ( [( p , None ) for p in a] if a else [] ) + b;
         self._reset(mark)
         if (
-            (a := self._loop0_138(),)
+            (a := self._loop0_145(),)
             and
-            (b := self._loop1_139())
+            (b := self._loop1_146())
             and
             (self.expect('/'))
             and
             (self.positive_lookahead(self.expect, ':'))
         ):
             return ( [( p , None ) for p in a] if a else [] ) + b;
         self._reset(mark)
@@ -6465,26 +6846,26 @@
             return None  # pragma: no cover;
         self._reset(mark)
         if (
             (self.expect('*'))
             and
             (a := self.lambda_param_no_default())
             and
-            (b := self._loop0_140(),)
+            (b := self._loop0_147(),)
             and
             (c := self.lambda_kwds(),)
         ):
             return ( a , b , c );
         self._reset(mark)
         if (
             (self.expect('*'))
             and
             (self.expect(','))
             and
-            (b := self._loop1_141())
+            (b := self._loop1_148())
             and
             (c := self.lambda_kwds(),)
         ):
             return ( None , b , c );
         self._reset(mark)
         if (
             (a := self.lambda_kwds())
@@ -6659,15 +7040,15 @@
         # scenic_param_stmt: "param" (','.scenic_param_stmt_param+)
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect("param"))
             and
-            (elts := self._gather_142())
+            (elts := self._gather_149())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . Param ( elts = elts , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
@@ -6715,15 +7096,15 @@
         if (
             (self.expect('require'))
             and
             (self.expect("monitor"))
             and
             (e := self.expression())
             and
-            (n := self._tmp_144(),)
+            (n := self._tmp_151(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . RequireMonitor ( monitor = e , name = n , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             self.call_invalid_rules
@@ -6731,32 +7112,32 @@
             (self.invalid_scenic_require_prob())
         ):
             return None  # pragma: no cover;
         self._reset(mark)
         if (
             (self.expect('require'))
             and
-            (p := self._tmp_145(),)
+            (p := self._tmp_152(),)
             and
             (e := self.scenic_temporal_expression())
             and
-            (n := self._tmp_146(),)
+            (n := self._tmp_153(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . Require ( cond = e , prob = p , name = n , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
     @memoize
     def scenic_require_stmt_name(self) -> Optional[Any]:
         # scenic_require_stmt_name: (NAME | NUMBER) | STRING
         mark = self._mark()
         if (
-            (a := self._tmp_147())
+            (a := self._tmp_154())
         ):
             return a . string;
         self._reset(mark)
         if (
             (a := self.string())
         ):
             return a . string [1 : - 1];
@@ -6770,15 +7151,15 @@
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect("record"))
             and
             (e := self.expression())
             and
-            (n := self._tmp_148(),)
+            (n := self._tmp_155(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . Record ( value = e , name = n , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
@@ -6791,15 +7172,15 @@
         if (
             (self.expect("record"))
             and
             (self.expect("initial"))
             and
             (e := self.expression())
             and
-            (n := self._tmp_149(),)
+            (n := self._tmp_156(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . RecordInitial ( value = e , name = n , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
@@ -6812,15 +7193,15 @@
         if (
             (self.expect("record"))
             and
             (self.expect("final"))
             and
             (e := self.expression())
             and
-            (n := self._tmp_150(),)
+            (n := self._tmp_157(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . RecordFinal ( value = e , name = n , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
@@ -6829,17 +7210,17 @@
         # scenic_mutate_stmt: "mutate" (','.scenic_mutate_stmt_id+)? ['by' expression]
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect("mutate"))
             and
-            (elts := self._gather_151(),)
+            (elts := self._gather_158(),)
             and
-            (scale := self._tmp_153(),)
+            (scale := self._tmp_160(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . Mutate ( elts = elts if elts is not None else [] , scale = scale , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
@@ -6878,15 +7259,15 @@
         # scenic_take_stmt: "take" (','.expression+)
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect("take"))
             and
-            (elts := self._gather_154())
+            (elts := self._gather_161())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . Take ( elts = elts , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
@@ -6916,15 +7297,15 @@
             and
             (self.expect("simulation"))
             and
             (self.expect("when"))
             and
             (v := self.expression())
             and
-            (n := self._tmp_156(),)
+            (n := self._tmp_163(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . TerminateSimulationWhen ( v , name = n , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
@@ -6937,15 +7318,15 @@
         if (
             (self.expect("terminate"))
             and
             (self.expect("when"))
             and
             (v := self.expression())
             and
-            (n := self._tmp_157(),)
+            (n := self._tmp_164(),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . TerminateWhen ( v , name = n , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
@@ -7007,15 +7388,15 @@
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect('do'))
             and
             (self.expect("choose"))
             and
-            (e := self._gather_158())
+            (e := self._gather_165())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . DoChoose ( e , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
@@ -7026,15 +7407,15 @@
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect('do'))
             and
             (self.expect("shuffle"))
             and
-            (e := self._gather_160())
+            (e := self._gather_167())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . DoShuffle ( e , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
@@ -7043,15 +7424,15 @@
         # scenic_do_for_stmt: 'do' (','.expression+) 'for' scenic_dynamic_duration
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect('do'))
             and
-            (e := self._gather_162())
+            (e := self._gather_169())
             and
             (self.expect('for'))
             and
             (u := self.scenic_dynamic_duration())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
@@ -7097,15 +7478,15 @@
         # scenic_do_until_stmt: 'do' (','.disjunction+) 'until' expression
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect('do'))
             and
-            (e := self._gather_164())
+            (e := self._gather_171())
             and
             (self.expect('until'))
             and
             (cond := self.expression())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
@@ -7118,15 +7499,15 @@
         # scenic_do_stmt: 'do' (','.expression+)
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect('do'))
             and
-            (e := self._gather_166())
+            (e := self._gather_173())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . Do ( elts = e , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
@@ -7144,53 +7525,166 @@
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . Simulator ( value = e , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
     @memoize
-    def strings(self) -> Optional[ast . Str]:
-        # strings: STRING+
+    def fstring_mid(self) -> Optional[Any]:
+        # fstring_mid: fstring_replacement_field | FSTRING_MIDDLE
         mark = self._mark()
+        tok = self._tokenizer.peek()
+        start_lineno, start_col_offset = tok.start
         if (
-            (a := self._loop1_168())
+            (fstring_replacement_field := self.fstring_replacement_field())
         ):
-            return self . generate_ast_for_string ( a );
+            return fstring_replacement_field;
+        self._reset(mark)
+        if (
+            (t := self.fstring_middle())
+        ):
+            tok = self._tokenizer.get_last_non_whitespace_token()
+            end_lineno, end_col_offset = tok.end
+            return ast . Constant ( value = t . string , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def fstring_replacement_field(self) -> Optional[Any]:
+        # fstring_replacement_field: '{' (yield_expr | star_expressions) "="? fstring_conversion? fstring_full_format_spec? '}' | invalid_replacement_field
+        mark = self._mark()
+        tok = self._tokenizer.peek()
+        start_lineno, start_col_offset = tok.start
+        if (
+            (self.expect('{'))
+            and
+            (a := self._tmp_175())
+            and
+            (debug_expr := self.expect("="),)
+            and
+            (conversion := self.fstring_conversion(),)
+            and
+            (format := self.fstring_full_format_spec(),)
+            and
+            (self.expect('}'))
+        ):
+            tok = self._tokenizer.get_last_non_whitespace_token()
+            end_lineno, end_col_offset = tok.end
+            return ast . FormattedValue ( value = a , conversion = ( conversion . decode ( ) [0] if conversion else ( b'r' [0] if debug_expr else - 1 ) ) , format_spec = format , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
+        self._reset(mark)
+        if (
+            self.call_invalid_rules
+            and
+            (self.invalid_replacement_field())
+        ):
+            return None  # pragma: no cover;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def fstring_conversion(self) -> Optional[int]:
+        # fstring_conversion: "!" NAME
+        mark = self._mark()
+        if (
+            (conv_token := self.expect("!"))
+            and
+            (conv := self.name())
+        ):
+            return self . check_fstring_conversion ( conv_token , conv );
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def fstring_full_format_spec(self) -> Optional[Any]:
+        # fstring_full_format_spec: ':' fstring_format_spec*
+        mark = self._mark()
+        tok = self._tokenizer.peek()
+        start_lineno, start_col_offset = tok.start
+        if (
+            (self.expect(':'))
+            and
+            (spec := self._loop0_176(),)
+        ):
+            tok = self._tokenizer.get_last_non_whitespace_token()
+            end_lineno, end_col_offset = tok.end
+            return ast . JoinedStr ( values = spec if spec and ( len ( spec ) > 1 or spec [0] . value ) else [] , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset , );
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def fstring_format_spec(self) -> Optional[Any]:
+        # fstring_format_spec: FSTRING_MIDDLE | fstring_replacement_field
+        mark = self._mark()
+        tok = self._tokenizer.peek()
+        start_lineno, start_col_offset = tok.start
+        if (
+            (t := self.fstring_middle())
+        ):
+            tok = self._tokenizer.get_last_non_whitespace_token()
+            end_lineno, end_col_offset = tok.end
+            return ast . Constant ( value = t . string , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
+        self._reset(mark)
+        if (
+            (fstring_replacement_field := self.fstring_replacement_field())
+        ):
+            return fstring_replacement_field;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def strings(self) -> Optional[Any]:
+        # strings: ((fstring | STRING))+
+        mark = self._mark()
+        if (
+            (a := self._loop1_177())
+        ):
+            return self . concatenate_strings ( a ) if sys . version_info >= ( 3 , 12 ) else self . generate_ast_for_string ( a );
         self._reset(mark)
         return None;
 
     @memoize
     def list(self) -> Optional[ast . List]:
-        # list: '[' star_named_expressions? ']'
+        # list: '[' star_named_expressions? ']' | '**' expression '=' expression
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect('['))
             and
             (a := self.star_named_expressions(),)
             and
             (self.expect(']'))
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . List ( elts = a or [] , ctx = Load , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
+        if (
+            (a := self.expect('**'))
+            and
+            (self.expression())
+            and
+            (self.expect('='))
+            and
+            (b := self.expression())
+        ):
+            return self . raise_syntax_error_known_range ( "cannot assign to keyword argument unpacking" , a , b );
+        self._reset(mark)
         return None;
 
     @memoize
     def tuple(self) -> Optional[ast . Tuple]:
         # tuple: '(' [star_named_expression ',' star_named_expressions?] ')'
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect('('))
             and
-            (a := self._tmp_169(),)
+            (a := self._tmp_178(),)
             and
             (self.expect(')'))
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Tuple ( elts = a or [] , ctx = Load , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
@@ -7246,15 +7740,15 @@
         return None;
 
     @memoize
     def double_starred_kvpairs(self) -> Optional[list]:
         # double_starred_kvpairs: ','.double_starred_kvpair+ ','?
         mark = self._mark()
         if (
-            (a := self._gather_170())
+            (a := self._gather_179())
             and
             (self.expect(','),)
         ):
             return a;
         self._reset(mark)
         return None;
 
@@ -7292,15 +7786,15 @@
         return None;
 
     @memoize
     def for_if_clauses(self) -> Optional[List [ast . comprehension]]:
         # for_if_clauses: for_if_clause+
         mark = self._mark()
         if (
-            (a := self._loop1_172())
+            (a := self._loop1_181())
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
     def for_if_clause(self) -> Optional[ast . comprehension]:
@@ -7316,15 +7810,15 @@
             and
             (self.expect('in'))
             and
             (cut := True)
             and
             (b := self.disjunction())
             and
-            (c := self._loop0_173(),)
+            (c := self._loop0_182(),)
         ):
             return self . check_version ( ( 3 , 6 ) , "Async comprehensions are" , ast . comprehension ( target = a , iter = b , ifs = c , is_async = 1 ) );
         self._reset(mark)
         if cut:
             return None;
         cut = False
         if (
@@ -7334,15 +7828,15 @@
             and
             (self.expect('in'))
             and
             (cut := True)
             and
             (b := self.disjunction())
             and
-            (c := self._loop0_174(),)
+            (c := self._loop0_183(),)
         ):
             return ast . comprehension ( target = a , iter = b , ifs = c , is_async = 0 );
         self._reset(mark)
         if cut:
             return None;
         if (
             self.call_invalid_rules
@@ -7414,15 +7908,15 @@
         # genexp: '(' (assignment_expression | expression !':=') for_if_clauses ')' | invalid_comprehension
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect('('))
             and
-            (a := self._tmp_175())
+            (a := self._tmp_184())
             and
             (b := self.for_if_clauses())
             and
             (self.expect(')'))
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
@@ -7488,17 +7982,17 @@
         return None;
 
     @memoize
     def args(self) -> Optional[Tuple [list , list]]:
         # args: ','.(starred_expression | (assignment_expression | expression !':=') !'=')+ [',' kwargs] | kwargs
         mark = self._mark()
         if (
-            (a := self._gather_176())
+            (a := self._gather_185())
             and
-            (b := self._tmp_178(),)
+            (b := self._tmp_187(),)
         ):
             return ( a + ( [e for e in b if isinstance ( e , ast . Starred )] if b else [] ) , ( [e for e in b if not isinstance ( e , ast . Starred )] if b else [] ) );
         self._reset(mark)
         if (
             (a := self.kwargs())
         ):
             return ( [e for e in a if isinstance ( e , ast . Starred )] , [e for e in a if not isinstance ( e , ast . Starred )] );
@@ -7506,41 +8000,48 @@
         return None;
 
     @memoize
     def kwargs(self) -> Optional[list]:
         # kwargs: ','.kwarg_or_starred+ ',' ','.kwarg_or_double_starred+ | ','.kwarg_or_starred+ | ','.kwarg_or_double_starred+
         mark = self._mark()
         if (
-            (a := self._gather_179())
+            (a := self._gather_188())
             and
             (self.expect(','))
             and
-            (b := self._gather_181())
+            (b := self._gather_190())
         ):
             return a + b;
         self._reset(mark)
         if (
-            (_gather_183 := self._gather_183())
+            (_gather_192 := self._gather_192())
         ):
-            return _gather_183;
+            return _gather_192;
         self._reset(mark)
         if (
-            (_gather_185 := self._gather_185())
+            (_gather_194 := self._gather_194())
         ):
-            return _gather_185;
+            return _gather_194;
         self._reset(mark)
         return None;
 
     @memoize
     def starred_expression(self) -> Optional[Any]:
-        # starred_expression: '*' expression
+        # starred_expression: invalid_starred_expression | '*' expression
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
+            self.call_invalid_rules
+            and
+            (self.invalid_starred_expression())
+        ):
+            return None  # pragma: no cover;
+        self._reset(mark)
+        if (
             (self.expect('*'))
             and
             (a := self.expression())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Starred ( value = a , ctx = Load , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
@@ -7625,45 +8126,45 @@
             (self.negative_lookahead(self.expect, ','))
         ):
             return a;
         self._reset(mark)
         if (
             (a := self.star_target())
             and
-            (b := self._loop0_187(),)
+            (b := self._loop0_196(),)
             and
             (self.expect(','),)
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Tuple ( elts = [a] + b , ctx = Store , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
     @memoize
     def star_targets_list_seq(self) -> Optional[list]:
         # star_targets_list_seq: ','.star_target+ ','?
         mark = self._mark()
         if (
-            (a := self._gather_188())
+            (a := self._gather_197())
             and
             (self.expect(','),)
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
     def star_targets_tuple_seq(self) -> Optional[list]:
         # star_targets_tuple_seq: star_target ((',' star_target))+ ','? | star_target ','
         mark = self._mark()
         if (
             (a := self.star_target())
             and
-            (b := self._loop1_190())
+            (b := self._loop1_199())
             and
             (self.expect(','),)
         ):
             return [a] + b;
         self._reset(mark)
         if (
             (a := self.star_target())
@@ -7679,15 +8180,15 @@
         # star_target: '*' (!'*' star_target) | target_with_star_atom
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect('*'))
             and
-            (a := self._tmp_191())
+            (a := self._tmp_200())
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return ast . Starred ( value = self . set_expr_context ( a , Store ) , ctx = Store , lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         if (
             (target_with_star_atom := self.target_with_star_atom())
@@ -7939,15 +8440,15 @@
         return None;
 
     @memoize
     def del_targets(self) -> Optional[Any]:
         # del_targets: ','.del_target+ ','?
         mark = self._mark()
         if (
-            (a := self._gather_192())
+            (a := self._gather_201())
             and
             (self.expect(','),)
         ):
             return a;
         self._reset(mark)
         return None;
 
@@ -8039,15 +8540,15 @@
         return None;
 
     @memoize
     def type_expressions(self) -> Optional[list]:
         # type_expressions: ','.expression+ ',' '*' expression ',' '**' expression | ','.expression+ ',' '*' expression | ','.expression+ ',' '**' expression | '*' expression ',' '**' expression | '*' expression | '**' expression | ','.expression+
         mark = self._mark()
         if (
-            (a := self._gather_194())
+            (a := self._gather_203())
             and
             (self.expect(','))
             and
             (self.expect('*'))
             and
             (b := self.expression())
             and
@@ -8056,26 +8557,26 @@
             (self.expect('**'))
             and
             (c := self.expression())
         ):
             return a + [b , c];
         self._reset(mark)
         if (
-            (a := self._gather_196())
+            (a := self._gather_205())
             and
             (self.expect(','))
             and
             (self.expect('*'))
             and
             (b := self.expression())
         ):
             return a + [b];
         self._reset(mark)
         if (
-            (a := self._gather_198())
+            (a := self._gather_207())
             and
             (self.expect(','))
             and
             (self.expect('**'))
             and
             (b := self.expression())
         ):
@@ -8105,30 +8606,30 @@
             (self.expect('**'))
             and
             (a := self.expression())
         ):
             return [a];
         self._reset(mark)
         if (
-            (a := self._gather_200())
+            (a := self._gather_209())
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
     def func_type_comment(self) -> Optional[Any]:
         # func_type_comment: NEWLINE TYPE_COMMENT &(NEWLINE INDENT) | invalid_double_type_comments | TYPE_COMMENT
         mark = self._mark()
         if (
             (self.expect('NEWLINE'))
             and
             (t := self.type_comment())
             and
-            (self.positive_lookahead(self._tmp_202, ))
+            (self.positive_lookahead(self._tmp_211, ))
         ):
             return t . string;
         self._reset(mark)
         if (
             self.call_invalid_rules
             and
             (self.invalid_double_type_comments())
@@ -8140,15 +8641,15 @@
         ):
             return type_comment;
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_arguments(self) -> Optional[NoReturn]:
-        # invalid_arguments: args ',' '*' | expression for_if_clauses ',' [args | expression for_if_clauses] | NAME '=' expression for_if_clauses | args for_if_clauses | args ',' expression for_if_clauses | args ',' args
+        # invalid_arguments: args ',' '*' | expression for_if_clauses ',' [args | expression for_if_clauses] | NAME '=' expression for_if_clauses | [(args ',')] NAME '=' &(',' | ')') | args for_if_clauses | args ',' expression for_if_clauses | args ',' args
         mark = self._mark()
         if (
             (a := self.args())
             and
             (self.expect(','))
             and
             (self.expect('*'))
@@ -8158,15 +8659,15 @@
         if (
             (a := self.expression())
             and
             (b := self.for_if_clauses())
             and
             (self.expect(','))
             and
-            (self._tmp_203(),)
+            (self._tmp_212(),)
         ):
             return self . raise_syntax_error_known_range ( "Generator expression must be parenthesized" , a , ( b [- 1] . ifs [- 1] if b [- 1] . ifs else b [- 1] . iter ) );
         self._reset(mark)
         if (
             (a := self.name())
             and
             (b := self.expect('='))
@@ -8174,14 +8675,25 @@
             (self.expression())
             and
             (self.for_if_clauses())
         ):
             return self . raise_syntax_error_known_range ( "invalid syntax. Maybe you meant '==' or ':=' instead of '='?" , a , b );
         self._reset(mark)
         if (
+            (self._tmp_213(),)
+            and
+            (a := self.name())
+            and
+            (b := self.expect('='))
+            and
+            (self.positive_lookahead(self._tmp_214, ))
+        ):
+            return self . raise_syntax_error_known_range ( "expected argument value expression" , a , b );
+        self._reset(mark)
+        if (
             (a := self.args())
             and
             (b := self.for_if_clauses())
         ):
             return self . raise_syntax_error_known_range ( "Generator expression must be parenthesized" , a [0] [- 1] , ( b [- 1] . ifs [- 1] if b [- 1] . ifs else b [- 1] . iter ) , ) if len ( a [0] ) > 1 else None;
         self._reset(mark)
         if (
@@ -8207,15 +8719,15 @@
         return None;
 
     @memoize
     def invalid_kwarg(self) -> Optional[NoReturn]:
         # invalid_kwarg: ('True' | 'False' | 'None') '=' | NAME '=' expression for_if_clauses | !(NAME '=') expression '='
         mark = self._mark()
         if (
-            (a := self._tmp_204())
+            (a := self._tmp_215())
             and
             (b := self.expect('='))
         ):
             return self . raise_syntax_error_known_range ( f"cannot assign to {a.string}" , a , b );
         self._reset(mark)
         if (
             (a := self.name())
@@ -8225,15 +8737,15 @@
             (self.expression())
             and
             (self.for_if_clauses())
         ):
             return self . raise_syntax_error_known_range ( "invalid syntax. Maybe you meant '==' or ':=' instead of '='?" , a , b );
         self._reset(mark)
         if (
-            (self.negative_lookahead(self._tmp_205, ))
+            (self.negative_lookahead(self._tmp_216, ))
             and
             (a := self.expression())
             and
             (b := self.expect('='))
         ):
             return self . raise_syntax_error_known_range ( "expression cannot contain assignment, perhaps you meant \"==\"?" , a , b , );
         self._reset(mark)
@@ -8300,33 +8812,33 @@
             return lambdef;
         self._reset(mark)
         self.call_invalid_rules = _prev_call_invalid
         return None;
 
     @memoize
     def invalid_legacy_expression(self) -> Optional[Any]:
-        # invalid_legacy_expression: NAME !'(' expression_without_invalid
+        # invalid_legacy_expression: NAME !'(' star_expressions
         mark = self._mark()
         if (
             (a := self.name())
             and
             (self.negative_lookahead(self.expect, '('))
             and
-            (b := self.expression_without_invalid())
+            (b := self.star_expressions())
         ):
             return self . raise_syntax_error_known_range ( f"Missing parentheses in call to '{a.string}' . Did you mean {a.string}(...)?" , a , b , ) if a . string in ( "exec" , "print" ) else None;
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_expression(self) -> Optional[NoReturn]:
-        # invalid_expression: !(NAME STRING | SOFT_KEYWORD) disjunction !SOFT_KEYWORD expression_without_invalid | disjunction 'if' disjunction !('else' | ':')
+        # invalid_expression: !(NAME STRING | SOFT_KEYWORD) disjunction !SOFT_KEYWORD expression_without_invalid | disjunction 'if' disjunction !('else' | ':') | 'lambda' lambda_params? ':' &(FSTRING_MIDDLE | fstring_replacement_field)
         mark = self._mark()
         if (
-            (self.negative_lookahead(self._tmp_206, ))
+            (self.negative_lookahead(self._tmp_217, ))
             and
             (a := self.disjunction())
             and
             (self.negative_lookahead(self.soft_keyword, ))
             and
             (b := self.expression_without_invalid())
         ):
@@ -8335,18 +8847,29 @@
         if (
             (a := self.disjunction())
             and
             (self.expect('if'))
             and
             (b := self.disjunction())
             and
-            (self.negative_lookahead(self._tmp_207, ))
+            (self.negative_lookahead(self._tmp_218, ))
         ):
             return self . raise_syntax_error_known_range ( "expected 'else' after 'if' expression" , a , b );
         self._reset(mark)
+        if (
+            (a := self.expect('lambda'))
+            and
+            (self.lambda_params(),)
+            and
+            (b := self.expect(':'))
+            and
+            (self.positive_lookahead(self._tmp_219, ))
+        ):
+            return self . raise_syntax_error_known_range ( "f-string: lambda expressions are not allowed without parentheses" , a , b );
+        self._reset(mark)
         return None;
 
     @memoize
     def invalid_named_expression(self) -> Optional[NoReturn]:
         # invalid_named_expression: expression ':=' expression | NAME '=' bitwise_or !('=' | ':=') | !(list | tuple | genexp | 'True' | 'None' | 'False') bitwise_or '=' bitwise_or !('=' | ':=')
         mark = self._mark()
         if (
@@ -8361,28 +8884,28 @@
         if (
             (a := self.name())
             and
             (self.expect('='))
             and
             (b := self.bitwise_or())
             and
-            (self.negative_lookahead(self._tmp_208, ))
+            (self.negative_lookahead(self._tmp_220, ))
         ):
             return ( None if self . in_recursive_rule else self . raise_syntax_error_known_range ( "invalid syntax. Maybe you meant '==' or ':=' instead of '='?" , a , b ) );
         self._reset(mark)
         if (
-            (self.negative_lookahead(self._tmp_209, ))
+            (self.negative_lookahead(self._tmp_221, ))
             and
             (a := self.bitwise_or())
             and
             (self.expect('='))
             and
             (self.bitwise_or())
             and
-            (self.negative_lookahead(self._tmp_210, ))
+            (self.negative_lookahead(self._tmp_222, ))
         ):
             return ( None if self . in_recursive_rule else self . raise_syntax_error_known_location ( f"cannot assign to {self.get_expr_name(a)} here. Maybe you meant '==' instead of '='?" , a ) );
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_scenic_until(self) -> Optional[NoReturn]:
@@ -8419,23 +8942,23 @@
         # invalid_scenic_require_prob: 'require' '[' !(NUMBER ']') expression ']' scenic_temporal_expression ['as' scenic_require_stmt_name]
         mark = self._mark()
         if (
             (self.expect('require'))
             and
             (self.expect('['))
             and
-            (self.negative_lookahead(self._tmp_211, ))
+            (self.negative_lookahead(self._tmp_223, ))
             and
             (p := self.expression())
             and
             (self.expect(']'))
             and
             (self.scenic_temporal_expression())
             and
-            (self._tmp_212(),)
+            (self._tmp_224(),)
         ):
             return self . raise_syntax_error_known_location ( f"'require' probability must be a constant" , p );
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_scenic_dynamic_duration(self) -> Optional[NoReturn]:
@@ -8464,15 +8987,15 @@
             return self . raise_syntax_error_known_location ( f"only single target (not {self.get_expr_name(a)}) can be annotated" , a );
         self._reset(mark)
         if (
             (a := self.star_named_expression())
             and
             (self.expect(','))
             and
-            (self._loop0_213(),)
+            (self._loop0_225(),)
             and
             (self.expect(':'))
             and
             (self.expression())
         ):
             return self . raise_syntax_error_known_location ( "only single target (not tuple) can be annotated" , a );
         self._reset(mark)
@@ -8482,37 +9005,37 @@
             (self.expect(':'))
             and
             (self.expression())
         ):
             return self . raise_syntax_error_known_location ( "illegal target for annotation" , a );
         self._reset(mark)
         if (
-            (self._loop0_214(),)
+            (self._loop0_226(),)
             and
             (a := self.star_expressions())
             and
             (self.expect('='))
         ):
             return self . raise_syntax_error_invalid_target ( Target . STAR_TARGETS , a );
         self._reset(mark)
         if (
-            (self._loop0_215(),)
+            (self._loop0_227(),)
             and
             (a := self.yield_expr())
             and
             (self.expect('='))
         ):
             return self . raise_syntax_error_known_location ( "assignment to yield expression not possible" , a );
         self._reset(mark)
         if (
             (a := self.star_expressions())
             and
             (self.augassign())
             and
-            (self._tmp_216())
+            (self._tmp_228())
         ):
             return self . raise_syntax_error_known_location ( f"'{self.get_expr_name(a)}' is an illegal expression for augmented assignment" , a );
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_ann_assign_target(self) -> Optional[ast . AST]:
@@ -8568,37 +9091,37 @@
         return None;
 
     @memoize
     def invalid_comprehension(self) -> Optional[NoReturn]:
         # invalid_comprehension: ('[' | '(' | '{') starred_expression for_if_clauses | ('[' | '{') star_named_expression ',' star_named_expressions for_if_clauses | ('[' | '{') star_named_expression ',' for_if_clauses
         mark = self._mark()
         if (
-            (self._tmp_217())
+            (self._tmp_229())
             and
             (a := self.starred_expression())
             and
             (self.for_if_clauses())
         ):
             return self . raise_syntax_error_known_location ( "iterable unpacking cannot be used in comprehension" , a );
         self._reset(mark)
         if (
-            (self._tmp_218())
+            (self._tmp_230())
             and
             (a := self.star_named_expression())
             and
             (self.expect(','))
             and
             (b := self.star_named_expressions())
             and
             (self.for_if_clauses())
         ):
             return self . raise_syntax_error_known_range ( "did you forget parentheses around the comprehension target?" , a , b [- 1] );
         self._reset(mark)
         if (
-            (self._tmp_219())
+            (self._tmp_231())
             and
             (a := self.star_named_expression())
             and
             (b := self.expect(','))
             and
             (self.for_if_clauses())
         ):
@@ -8623,73 +9146,75 @@
         ):
             return self . raise_syntax_error_known_location ( "dict unpacking cannot be used in dict comprehension" , a );
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_parameters(self) -> Optional[NoReturn]:
-        # invalid_parameters: param_no_default* invalid_parameters_helper param_no_default | param_no_default* '(' param_no_default+ ','? ')' | "/" ',' | (slash_no_default | slash_with_default) param_maybe_default* '/' | [(slash_no_default | slash_with_default)] param_maybe_default* '*' (',' | param_no_default) param_maybe_default* '/' | param_maybe_default+ '/' '*'
+        # invalid_parameters: "/" ',' | (slash_no_default | slash_with_default) param_maybe_default* '/' | slash_no_default? param_no_default* invalid_parameters_helper param_no_default | param_no_default* '(' param_no_default+ ','? ')' | [(slash_no_default | slash_with_default)] param_maybe_default* '*' (',' | param_no_default) param_maybe_default* '/' | param_maybe_default+ '/' '*'
         mark = self._mark()
         if (
+            (a := self.expect("/"))
+            and
+            (self.expect(','))
+        ):
+            return self . raise_syntax_error_known_location ( "at least one argument must precede /" , a );
+        self._reset(mark)
+        if (
+            (self._tmp_232())
+            and
+            (self._loop0_233(),)
+            and
+            (a := self.expect('/'))
+        ):
+            return self . raise_syntax_error_known_location ( "/ may appear only once" , a );
+        self._reset(mark)
+        if (
             self.call_invalid_rules
             and
-            (self._loop0_220(),)
+            (self.slash_no_default(),)
+            and
+            (self._loop0_234(),)
             and
             (self.invalid_parameters_helper())
             and
             (a := self.param_no_default())
         ):
-            return self . raise_syntax_error_known_location ( "non-default argument follows default argument" , a );
+            return self . raise_syntax_error_known_location ( "parameter without a default follows parameter with a default" , a );
         self._reset(mark)
         if (
-            (self._loop0_221(),)
+            (self._loop0_235(),)
             and
             (a := self.expect('('))
             and
-            (self._loop1_222())
+            (self._loop1_236())
             and
             (self.expect(','),)
             and
             (b := self.expect(')'))
         ):
             return self . raise_syntax_error_known_range ( "Function parameters cannot be parenthesized" , a , b );
         self._reset(mark)
         if (
-            (a := self.expect("/"))
-            and
-            (self.expect(','))
-        ):
-            return self . raise_syntax_error_known_location ( "at least one argument must precede /" , a );
-        self._reset(mark)
-        if (
-            (self._tmp_223())
-            and
-            (self._loop0_224(),)
-            and
-            (a := self.expect('/'))
-        ):
-            return self . raise_syntax_error_known_location ( "/ may appear only once" , a );
-        self._reset(mark)
-        if (
-            (self._tmp_225(),)
+            (self._tmp_237(),)
             and
-            (self._loop0_226(),)
+            (self._loop0_238(),)
             and
             (self.expect('*'))
             and
-            (self._tmp_227())
+            (self._tmp_239())
             and
-            (self._loop0_228(),)
+            (self._loop0_240(),)
             and
             (a := self.expect('/'))
         ):
             return self . raise_syntax_error_known_location ( "/ must be ahead of *" , a );
         self._reset(mark)
         if (
-            (self._loop1_229())
+            (self._loop1_241())
             and
             (self.expect('/'))
             and
             (a := self.expect('*'))
         ):
             return self . raise_syntax_error_known_location ( "expected comma between / and *" , a );
         self._reset(mark)
@@ -8698,28 +9223,28 @@
     @memoize
     def invalid_default(self) -> Optional[Any]:
         # invalid_default: '=' &(')' | ',')
         mark = self._mark()
         if (
             (a := self.expect('='))
             and
-            (self.positive_lookahead(self._tmp_230, ))
+            (self.positive_lookahead(self._tmp_242, ))
         ):
             return self . raise_syntax_error_known_location ( "expected default value expression" , a );
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_star_etc(self) -> Optional[Any]:
         # invalid_star_etc: '*' (')' | ',' (')' | '**')) | '*' ',' TYPE_COMMENT | '*' param '=' | '*' (param_no_default | ',') param_maybe_default* '*' (param_no_default | ',')
         mark = self._mark()
         if (
             (a := self.expect('*'))
             and
-            (self._tmp_231())
+            (self._tmp_243())
         ):
             return self . raise_syntax_error_known_location ( "named arguments must follow bare *" , a );
         self._reset(mark)
         if (
             (self.expect('*'))
             and
             (self.expect(','))
@@ -8736,21 +9261,21 @@
             (a := self.expect('='))
         ):
             return self . raise_syntax_error_known_location ( "var-positional argument cannot have default value" , a );
         self._reset(mark)
         if (
             (self.expect('*'))
             and
-            (self._tmp_232())
+            (self._tmp_244())
             and
-            (self._loop0_233(),)
+            (self._loop0_245(),)
             and
             (a := self.expect('*'))
             and
-            (self._tmp_234())
+            (self._tmp_246())
         ):
             return self . raise_syntax_error_known_location ( "* argument may appear only once" , a );
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_kwds(self) -> Optional[Any]:
@@ -8779,15 +9304,15 @@
         if (
             (self.expect('**'))
             and
             (self.param())
             and
             (self.expect(','))
             and
-            (a := self._tmp_235())
+            (a := self._tmp_247())
         ):
             return self . raise_syntax_error_known_location ( "arguments cannot follow var-keyword argument" , a );
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_parameters_helper(self) -> Optional[Any]:
@@ -8795,81 +9320,83 @@
         mark = self._mark()
         if (
             (a := self.slash_with_default())
         ):
             return [a];
         self._reset(mark)
         if (
-            (a := self._loop1_236())
+            (a := self._loop1_248())
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_lambda_parameters(self) -> Optional[NoReturn]:
-        # invalid_lambda_parameters: lambda_param_no_default* invalid_lambda_parameters_helper lambda_param_no_default | lambda_param_no_default* '(' ','.lambda_param+ ','? ')' | "/" ',' | (lambda_slash_no_default | lambda_slash_with_default) lambda_param_maybe_default* '/' | [(lambda_slash_no_default | lambda_slash_with_default)] lambda_param_maybe_default* '*' (',' | lambda_param_no_default) lambda_param_maybe_default* '/' | lambda_param_maybe_default+ '/' '*'
+        # invalid_lambda_parameters: "/" ',' | (lambda_slash_no_default | lambda_slash_with_default) lambda_param_maybe_default* '/' | lambda_slash_no_default? lambda_param_no_default* invalid_lambda_parameters_helper lambda_param_no_default | lambda_param_no_default* '(' ','.lambda_param+ ','? ')' | [(lambda_slash_no_default | lambda_slash_with_default)] lambda_param_maybe_default* '*' (',' | lambda_param_no_default) lambda_param_maybe_default* '/' | lambda_param_maybe_default+ '/' '*'
         mark = self._mark()
         if (
+            (a := self.expect("/"))
+            and
+            (self.expect(','))
+        ):
+            return self . raise_syntax_error_known_location ( "at least one argument must precede /" , a );
+        self._reset(mark)
+        if (
+            (self._tmp_249())
+            and
+            (self._loop0_250(),)
+            and
+            (a := self.expect('/'))
+        ):
+            return self . raise_syntax_error_known_location ( "/ may appear only once" , a );
+        self._reset(mark)
+        if (
             self.call_invalid_rules
             and
-            (self._loop0_237(),)
+            (self.lambda_slash_no_default(),)
+            and
+            (self._loop0_251(),)
             and
             (self.invalid_lambda_parameters_helper())
             and
             (a := self.lambda_param_no_default())
         ):
-            return self . raise_syntax_error_known_location ( "non-default argument follows default argument" , a );
+            return self . raise_syntax_error_known_location ( "parameter without a default follows parameter with a default" , a );
         self._reset(mark)
         if (
-            (self._loop0_238(),)
+            (self._loop0_252(),)
             and
             (a := self.expect('('))
             and
-            (self._gather_239())
+            (self._gather_253())
             and
             (self.expect(','),)
             and
             (b := self.expect(')'))
         ):
             return self . raise_syntax_error_known_range ( "Lambda expression parameters cannot be parenthesized" , a , b );
         self._reset(mark)
         if (
-            (a := self.expect("/"))
+            (self._tmp_255(),)
             and
-            (self.expect(','))
-        ):
-            return self . raise_syntax_error_known_location ( "at least one argument must precede /" , a );
-        self._reset(mark)
-        if (
-            (self._tmp_241())
-            and
-            (self._loop0_242(),)
-            and
-            (a := self.expect('/'))
-        ):
-            return self . raise_syntax_error_known_location ( "/ may appear only once" , a );
-        self._reset(mark)
-        if (
-            (self._tmp_243(),)
-            and
-            (self._loop0_244(),)
+            (self._loop0_256(),)
             and
             (self.expect('*'))
             and
-            (self._tmp_245())
+            (self._tmp_257())
             and
-            (self._loop0_246(),)
+            (self._loop0_258(),)
             and
             (a := self.expect('/'))
         ):
             return self . raise_syntax_error_known_location ( "/ must be ahead of *" , a );
         self._reset(mark)
         if (
-            (self._loop1_247())
+            (self._loop1_259())
             and
             (self.expect('/'))
             and
             (a := self.expect('*'))
         ):
             return self . raise_syntax_error_known_location ( "expected comma between / and *" , a );
         self._reset(mark)
@@ -8881,28 +9408,28 @@
         mark = self._mark()
         if (
             (a := self.lambda_slash_with_default())
         ):
             return [a];
         self._reset(mark)
         if (
-            (a := self._loop1_248())
+            (a := self._loop1_260())
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_lambda_star_etc(self) -> Optional[NoReturn]:
         # invalid_lambda_star_etc: '*' (':' | ',' (':' | '**')) | '*' lambda_param '=' | '*' (lambda_param_no_default | ',') lambda_param_maybe_default* '*' (lambda_param_no_default | ',')
         mark = self._mark()
         if (
             (self.expect('*'))
             and
-            (self._tmp_249())
+            (self._tmp_261())
         ):
             return self . raise_syntax_error ( "named arguments must follow bare *" );
         self._reset(mark)
         if (
             (self.expect('*'))
             and
             (self.lambda_param())
@@ -8910,21 +9437,21 @@
             (a := self.expect('='))
         ):
             return self . raise_syntax_error_known_location ( "var-positional argument cannot have default value" , a );
         self._reset(mark)
         if (
             (self.expect('*'))
             and
-            (self._tmp_250())
+            (self._tmp_262())
             and
-            (self._loop0_251(),)
+            (self._loop0_263(),)
             and
             (a := self.expect('*'))
             and
-            (self._tmp_252())
+            (self._tmp_264())
         ):
             return self . raise_syntax_error_known_location ( "* argument may appear only once" , a );
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_lambda_kwds(self) -> Optional[Any]:
@@ -8953,15 +9480,15 @@
         if (
             (self.expect('**'))
             and
             (self.lambda_param())
             and
             (self.expect(','))
             and
-            (a := self._tmp_253())
+            (a := self._tmp_265())
         ):
             return self . raise_syntax_error_known_location ( "arguments cannot follow var-keyword argument" , a );
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_double_type_comments(self) -> Optional[NoReturn]:
@@ -8989,15 +9516,15 @@
         if (
             (self.expression())
             and
             (self.expect('as'))
             and
             (a := self.expression())
             and
-            (self.positive_lookahead(self._tmp_254, ))
+            (self.positive_lookahead(self._tmp_266, ))
         ):
             return self . raise_syntax_error_invalid_target ( Target . STAR_TARGETS , a );
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_for_target(self) -> Optional[NoReturn]:
@@ -9037,14 +9564,31 @@
             (self.expect(')'))
         ):
             return self . raise_syntax_error_known_location ( "cannot use double starred expression here" , a );
         self._reset(mark)
         return None;
 
     @memoize
+    def invalid_import(self) -> Optional[Any]:
+        # invalid_import: 'import' ','.dotted_name+ 'from' dotted_name
+        mark = self._mark()
+        if (
+            (a := self.expect('import'))
+            and
+            (self._gather_267())
+            and
+            (self.expect('from'))
+            and
+            (self.dotted_name())
+        ):
+            return self . raise_syntax_error_starting_from ( "Did you mean to use 'from ... import ...' instead?" , a );
+        self._reset(mark)
+        return None;
+
+    @memoize
     def invalid_import_from_targets(self) -> Optional[NoReturn]:
         # invalid_import_from_targets: import_from_as_names ',' NEWLINE
         mark = self._mark()
         if (
             (self.import_from_as_names())
             and
             (self.expect(','))
@@ -9060,28 +9604,28 @@
         # invalid_with_stmt: 'async'? 'with' ','.(expression ['as' star_target])+ &&':' | 'async'? 'with' '(' ','.(expressions ['as' star_target])+ ','? ')' &&':'
         mark = self._mark()
         if (
             (self.expect('async'),)
             and
             (self.expect('with'))
             and
-            (self._gather_255())
+            (self._gather_269())
             and
             (self.expect_forced(self.expect(':'), "':'"))
         ):
             return None  # pragma: no cover;
         self._reset(mark)
         if (
             (self.expect('async'),)
             and
             (self.expect('with'))
             and
             (self.expect('('))
             and
-            (self._gather_257())
+            (self._gather_271())
             and
             (self.expect(','),)
             and
             (self.expect(')'))
             and
             (self.expect_forced(self.expect(':'), "':'"))
         ):
@@ -9094,15 +9638,15 @@
         # invalid_with_stmt_indent: 'async'? 'with' ','.(expression ['as' star_target])+ ':' NEWLINE !INDENT | 'async'? 'with' '(' ','.(expressions ['as' star_target])+ ','? ')' ':' NEWLINE !INDENT
         mark = self._mark()
         if (
             (self.expect('async'),)
             and
             (a := self.expect('with'))
             and
-            (self._gather_259())
+            (self._gather_273())
             and
             (self.expect(':'))
             and
             (self.expect('NEWLINE'))
             and
             (self.negative_lookahead(self.expect, 'INDENT'))
         ):
@@ -9111,15 +9655,15 @@
         if (
             (self.expect('async'),)
             and
             (a := self.expect('with'))
             and
             (self.expect('('))
             and
-            (self._gather_261())
+            (self._gather_275())
             and
             (self.expect(','),)
             and
             (self.expect(')'))
             and
             (self.expect(':'))
             and
@@ -9129,15 +9673,15 @@
         ):
             return self . raise_indentation_error ( f"expected an indented block after 'with' statement on line {a.start[0]}" );
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_try_stmt(self) -> Optional[NoReturn]:
-        # invalid_try_stmt: 'try' ':' NEWLINE !INDENT | 'try' ':' block !('except' | 'finally')
+        # invalid_try_stmt: 'try' ':' NEWLINE !INDENT | 'try' ':' block !('except' | 'finally') | 'try' ':' block* except_block+ 'except' '*' expression ['as' NAME] ':' | 'try' ':' block* except_star_block+ 'except' [expression ['as' NAME]] ':'
         mark = self._mark()
         if (
             (a := self.expect('try'))
             and
             (self.expect(':'))
             and
             (self.expect('NEWLINE'))
@@ -9149,57 +9693,110 @@
         if (
             (self.expect('try'))
             and
             (self.expect(':'))
             and
             (self.block())
             and
-            (self.negative_lookahead(self._tmp_263, ))
+            (self.negative_lookahead(self._tmp_277, ))
         ):
             return self . raise_syntax_error ( "expected 'except' or 'finally' block" );
         self._reset(mark)
+        if (
+            (self.expect('try'))
+            and
+            (self.expect(':'))
+            and
+            (self._loop0_278(),)
+            and
+            (self._loop1_279())
+            and
+            (a := self.expect('except'))
+            and
+            (b := self.expect('*'))
+            and
+            (self.expression())
+            and
+            (self._tmp_280(),)
+            and
+            (self.expect(':'))
+        ):
+            return self . raise_syntax_error_known_range ( "cannot have both 'except' and 'except*' on the same 'try'" , a , b );
+        self._reset(mark)
+        if (
+            (self.expect('try'))
+            and
+            (self.expect(':'))
+            and
+            (self._loop0_281(),)
+            and
+            (self._loop1_282())
+            and
+            (a := self.expect('except'))
+            and
+            (self._tmp_283(),)
+            and
+            (self.expect(':'))
+        ):
+            return self . raise_syntax_error_known_location ( "cannot have both 'except' and 'except*' on the same 'try'" , a );
+        self._reset(mark)
         return None;
 
     @memoize
     def invalid_except_stmt(self) -> Optional[None]:
-        # invalid_except_stmt: 'except' expression ',' expressions ['as' NAME] ':' | 'except' expression ['as' NAME] NEWLINE | 'except' NEWLINE
+        # invalid_except_stmt: 'except' '*'? expression ',' expressions ['as' NAME] ':' | 'except' '*'? expression ['as' NAME] NEWLINE | 'except' '*'? NEWLINE | 'except' '*' (NEWLINE | ':')
         mark = self._mark()
         if (
             (self.expect('except'))
             and
+            (self.expect('*'),)
+            and
             (a := self.expression())
             and
             (self.expect(','))
             and
             (self.expressions())
             and
-            (self._tmp_264(),)
+            (self._tmp_284(),)
             and
             (self.expect(':'))
         ):
             return self . raise_syntax_error_starting_from ( "multiple exception types must be parenthesized" , a );
         self._reset(mark)
         if (
             (self.expect('except'))
             and
+            (self.expect('*'),)
+            and
             (self.expression())
             and
-            (self._tmp_265(),)
+            (self._tmp_285(),)
             and
             (self.expect('NEWLINE'))
         ):
             return self . raise_syntax_error ( "expected ':'" );
         self._reset(mark)
         if (
             (self.expect('except'))
             and
+            (self.expect('*'),)
+            and
             (self.expect('NEWLINE'))
         ):
             return self . raise_syntax_error ( "expected ':'" );
         self._reset(mark)
+        if (
+            (self.expect('except'))
+            and
+            (self.expect('*'))
+            and
+            (self._tmp_286())
+        ):
+            return self . raise_syntax_error ( "expected one or more exception types" );
+        self._reset(mark)
         return None;
 
     @memoize
     def invalid_finally_stmt(self) -> Optional[NoReturn]:
         # invalid_finally_stmt: 'finally' ':' NEWLINE !INDENT
         mark = self._mark()
         if (
@@ -9220,15 +9817,15 @@
         # invalid_except_stmt_indent: 'except' expression ['as' NAME] ':' NEWLINE !INDENT | 'except' ':' NEWLINE !INDENT
         mark = self._mark()
         if (
             (a := self.expect('except'))
             and
             (self.expression())
             and
-            (self._tmp_266(),)
+            (self._tmp_287(),)
             and
             (self.expect(':'))
             and
             (self.expect('NEWLINE'))
             and
             (self.negative_lookahead(self.expect, 'INDENT'))
         ):
@@ -9244,14 +9841,37 @@
             (self.negative_lookahead(self.expect, 'INDENT'))
         ):
             return self . raise_indentation_error ( f"expected an indented block after 'except' statement on line {a.start[0]}" );
         self._reset(mark)
         return None;
 
     @memoize
+    def invalid_except_star_stmt_indent(self) -> Optional[Any]:
+        # invalid_except_star_stmt_indent: 'except' '*' expression ['as' NAME] ':' NEWLINE !INDENT
+        mark = self._mark()
+        if (
+            (a := self.expect('except'))
+            and
+            (self.expect('*'))
+            and
+            (self.expression())
+            and
+            (self._tmp_288(),)
+            and
+            (self.expect(':'))
+            and
+            (self.expect('NEWLINE'))
+            and
+            (self.negative_lookahead(self.expect, 'INDENT'))
+        ):
+            return self . raise_indentation_error ( f"expected an indented block after 'except*' statement on line {a.start[0]}" );
+        self._reset(mark)
+        return None;
+
+    @memoize
     def invalid_match_stmt(self) -> Optional[NoReturn]:
         # invalid_match_stmt: "match" subject_expr !':' | "match" subject_expr ':' NEWLINE !INDENT
         mark = self._mark()
         if (
             (self.expect("match"))
             and
             (self.subject_expr())
@@ -9351,15 +9971,15 @@
         return None;
 
     @memoize
     def invalid_class_argument_pattern(self) -> Optional[list]:
         # invalid_class_argument_pattern: [positional_patterns ','] keyword_patterns ',' positional_patterns
         mark = self._mark()
         if (
-            (self._tmp_267(),)
+            (self._tmp_289(),)
             and
             (self.keyword_patterns())
             and
             (self.expect(','))
             and
             (a := self.positional_patterns())
         ):
@@ -9466,17 +10086,32 @@
         ):
             return self . raise_indentation_error ( f"expected an indented block after 'while' statement on line {a.start[0]}" );
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_for_stmt(self) -> Optional[NoReturn]:
-        # invalid_for_stmt: 'async'? 'for' star_targets 'in' star_expressions ':' NEWLINE !INDENT
+        # invalid_for_stmt: ASYNC? 'for' star_targets 'in' star_expressions NEWLINE | 'async'? 'for' star_targets 'in' star_expressions ':' NEWLINE !INDENT
         mark = self._mark()
         if (
+            (self.expect('ASYNC'),)
+            and
+            (self.expect('for'))
+            and
+            (self.star_targets())
+            and
+            (self.expect('in'))
+            and
+            (self.star_expressions())
+            and
+            (self.expect('NEWLINE'))
+        ):
+            return self . raise_syntax_error ( "expected ':'" );
+        self._reset(mark)
+        if (
             (self.expect('async'),)
             and
             (a := self.expect('for'))
             and
             (self.star_targets())
             and
             (self.expect('in'))
@@ -9491,51 +10126,68 @@
         ):
             return self . raise_indentation_error ( f"expected an indented block after 'for' statement on line {a.start[0]}" );
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_def_raw(self) -> Optional[NoReturn]:
-        # invalid_def_raw: 'async'? 'def' NAME '(' params? ')' ['->' expression] ':' NEWLINE !INDENT
+        # invalid_def_raw: 'async'? 'def' NAME type_params? '(' params? ')' ['->' expression] ':' NEWLINE !INDENT
         mark = self._mark()
         if (
             (self.expect('async'),)
             and
             (a := self.expect('def'))
             and
             (self.name())
             and
+            (self.type_params(),)
+            and
             (self.expect('('))
             and
             (self.params(),)
             and
             (self.expect(')'))
             and
-            (self._tmp_268(),)
+            (self._tmp_290(),)
             and
             (self.expect(':'))
             and
             (self.expect('NEWLINE'))
             and
             (self.negative_lookahead(self.expect, 'INDENT'))
         ):
             return self . raise_indentation_error ( f"expected an indented block after function definition on line {a.start[0]}" );
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_class_def_raw(self) -> Optional[NoReturn]:
-        # invalid_class_def_raw: 'class' NAME ['(' arguments? ')'] ':' NEWLINE !INDENT
+        # invalid_class_def_raw: 'class' NAME type_params? ['(' arguments? ')'] NEWLINE | 'class' NAME type_params? ['(' arguments? ')'] ':' NEWLINE !INDENT
         mark = self._mark()
         if (
+            (self.expect('class'))
+            and
+            (self.name())
+            and
+            (self.type_params(),)
+            and
+            (self._tmp_291(),)
+            and
+            (self.expect('NEWLINE'))
+        ):
+            return self . raise_syntax_error ( "expected ':'" );
+        self._reset(mark)
+        if (
             (a := self.expect('class'))
             and
             (self.name())
             and
-            (self._tmp_269(),)
+            (self.type_params(),)
+            and
+            (self._tmp_292(),)
             and
             (self.expect(':'))
             and
             (self.expect('NEWLINE'))
             and
             (self.negative_lookahead(self.expect, 'INDENT'))
         ):
@@ -9546,15 +10198,15 @@
     @memoize
     def invalid_double_starred_kvpairs(self) -> Optional[None]:
         # invalid_double_starred_kvpairs: ','.double_starred_kvpair+ ',' invalid_kvpair | expression ':' '*' bitwise_or | expression ':' &('}' | ',')
         mark = self._mark()
         if (
             self.call_invalid_rules
             and
-            (self._gather_270())
+            (self._gather_293())
             and
             (self.expect(','))
             and
             (self.invalid_kvpair())
         ):
             return None  # pragma: no cover;
         self._reset(mark)
@@ -9570,23 +10222,23 @@
             return self . raise_syntax_error_starting_from ( "cannot use a starred expression in a dictionary value" , a );
         self._reset(mark)
         if (
             (self.expression())
             and
             (a := self.expect(':'))
             and
-            (self.positive_lookahead(self._tmp_272, ))
+            (self.positive_lookahead(self._tmp_295, ))
         ):
             return self . raise_syntax_error_known_location ( "expression expected after dictionary key and ':'" , a );
         self._reset(mark)
         return None;
 
     @memoize
     def invalid_kvpair(self) -> Optional[None]:
-        # invalid_kvpair: expression !(':') | expression ':' '*' bitwise_or | expression ':'
+        # invalid_kvpair: expression !(':') | expression ':' '*' bitwise_or | expression ':' &('}' | ',') | expression ':'
         mark = self._mark()
         if (
             (a := self.expression())
             and
             (self.negative_lookahead(self.expect, ':'))
         ):
             return self . raise_raw_syntax_error ( "':' expected after dictionary key" , ( a . lineno , a . col_offset ) , ( a . end_lineno , a . end_col_offset ) );
@@ -9602,20 +10254,183 @@
         ):
             return self . raise_syntax_error_starting_from ( "cannot use a starred expression in a dictionary value" , a );
         self._reset(mark)
         if (
             (self.expression())
             and
             (a := self.expect(':'))
+            and
+            (self.positive_lookahead(self._tmp_296, ))
+        ):
+            return self . raise_syntax_error_known_location ( "expression expected after dictionary key and ':'" , a );
+        self._reset(mark)
+        if (
+            (self.expression())
+            and
+            (a := self.expect(':'))
         ):
             return self . raise_syntax_error_known_location ( "expression expected after dictionary key and ':'" , a );
         self._reset(mark)
         return None;
 
     @memoize
+    def invalid_starred_expression(self) -> Optional[Any]:
+        # invalid_starred_expression: '*' expression '=' expression
+        mark = self._mark()
+        if (
+            (a := self.expect('*'))
+            and
+            (self.expression())
+            and
+            (self.expect('='))
+            and
+            (b := self.expression())
+        ):
+            return self . raise_syntax_error_known_range ( "cannot assign to iterable argument unpacking" , a , b );
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def invalid_replacement_field(self) -> Optional[Any]:
+        # invalid_replacement_field: '{' '=' | '{' '!' | '{' ':' | '{' '}' | '{' !(yield_expr | star_expressions) | '{' (yield_expr | star_expressions) !('=' | '!' | ':' | '}') | '{' (yield_expr | star_expressions) '=' !('!' | ':' | '}') | '{' (yield_expr | star_expressions) '='? invalid_conversion_character | '{' (yield_expr | star_expressions) '='? ['!' NAME] !(':' | '}') | '{' (yield_expr | star_expressions) '='? ['!' NAME] ':' fstring_format_spec* !'}' | '{' (yield_expr | star_expressions) '='? ['!' NAME] !'}'
+        mark = self._mark()
+        if (
+            (self.expect('{'))
+            and
+            (a := self.expect('='))
+        ):
+            return self . raise_syntax_error_known_location ( "f-string: valid expression required before '='" , a );
+        self._reset(mark)
+        if (
+            (self.expect('{'))
+            and
+            (a := self.expect('!'))
+        ):
+            return self . raise_syntax_error_known_location ( "f-string: valid expression required before '!'" , a );
+        self._reset(mark)
+        if (
+            (self.expect('{'))
+            and
+            (a := self.expect(':'))
+        ):
+            return self . raise_syntax_error_known_location ( "f-string: valid expression required before ':'" , a );
+        self._reset(mark)
+        if (
+            (self.expect('{'))
+            and
+            (a := self.expect('}'))
+        ):
+            return self . raise_syntax_error_known_location ( "f-string: valid expression required before '}'" , a );
+        self._reset(mark)
+        if (
+            (self.expect('{'))
+            and
+            (self.negative_lookahead(self._tmp_297, ))
+        ):
+            return self . raise_syntax_error_on_next_token ( "f-string: expecting a valid expression after '{'" );
+        self._reset(mark)
+        if (
+            (self.expect('{'))
+            and
+            (self._tmp_298())
+            and
+            (self.negative_lookahead(self._tmp_299, ))
+        ):
+            return self . raise_syntax_error_on_next_token ( "f-string: expecting '=', or '!', or ':', or '}'" );
+        self._reset(mark)
+        if (
+            (self.expect('{'))
+            and
+            (self._tmp_300())
+            and
+            (self.expect('='))
+            and
+            (self.negative_lookahead(self._tmp_301, ))
+        ):
+            return self . raise_syntax_error_on_next_token ( "f-string: expecting '!', or ':', or '}'" );
+        self._reset(mark)
+        if (
+            self.call_invalid_rules
+            and
+            (self.expect('{'))
+            and
+            (self._tmp_302())
+            and
+            (self.expect('='),)
+            and
+            (self.invalid_conversion_character())
+        ):
+            return None  # pragma: no cover;
+        self._reset(mark)
+        if (
+            (self.expect('{'))
+            and
+            (self._tmp_303())
+            and
+            (self.expect('='),)
+            and
+            (self._tmp_304(),)
+            and
+            (self.negative_lookahead(self._tmp_305, ))
+        ):
+            return self . raise_syntax_error_on_next_token ( "f-string: expecting ':' or '}'" );
+        self._reset(mark)
+        if (
+            (self.expect('{'))
+            and
+            (self._tmp_306())
+            and
+            (self.expect('='),)
+            and
+            (self._tmp_307(),)
+            and
+            (self.expect(':'))
+            and
+            (self._loop0_308(),)
+            and
+            (self.negative_lookahead(self.expect, '}'))
+        ):
+            return self . raise_syntax_error_on_next_token ( "f-string: expecting '}', or format specs" );
+        self._reset(mark)
+        if (
+            (self.expect('{'))
+            and
+            (self._tmp_309())
+            and
+            (self.expect('='),)
+            and
+            (self._tmp_310(),)
+            and
+            (self.negative_lookahead(self.expect, '}'))
+        ):
+            return self . raise_syntax_error_on_next_token ( "f-string: expecting '}'" );
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def invalid_conversion_character(self) -> Optional[Any]:
+        # invalid_conversion_character: '!' &(':' | '}') | '!' !NAME
+        mark = self._mark()
+        if (
+            (self.expect('!'))
+            and
+            (self.positive_lookahead(self._tmp_311, ))
+        ):
+            return self . raise_syntax_error_on_next_token ( "f-string: missing conversion character" );
+        self._reset(mark)
+        if (
+            (self.expect('!'))
+            and
+            (self.negative_lookahead(self.name, ))
+        ):
+            return self . raise_syntax_error_on_next_token ( "f-string: invalid conversion character" );
+        self._reset(mark)
+        return None;
+
+    @memoize
     def _loop0_1(self) -> Optional[Any]:
         # _loop0_1: NEWLINE
         mark = self._mark()
         children = []
         while (
             (_newline := self.expect('NEWLINE'))
         ):
@@ -9634,105 +10449,118 @@
         ):
             children.append(_newline)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_3(self) -> Optional[Any]:
-        # _loop1_3: statement
+    def _loop0_3(self) -> Optional[Any]:
+        # _loop0_3: fstring_mid
+        mark = self._mark()
+        children = []
+        while (
+            (fstring_mid := self.fstring_mid())
+        ):
+            children.append(fstring_mid)
+            mark = self._mark()
+        self._reset(mark)
+        return children;
+
+    @memoize
+    def _loop1_4(self) -> Optional[Any]:
+        # _loop1_4: statement
         mark = self._mark()
         children = []
         while (
             (statement := self.statement())
         ):
             children.append(statement)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_5(self) -> Optional[Any]:
-        # _loop0_5: ';' simple_stmt
+    def _loop0_6(self) -> Optional[Any]:
+        # _loop0_6: ';' simple_stmt
         mark = self._mark()
         children = []
         while (
             (self.expect(';'))
             and
             (elem := self.simple_stmt())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_4(self) -> Optional[Any]:
-        # _gather_4: simple_stmt _loop0_5
+    def _gather_5(self) -> Optional[Any]:
+        # _gather_5: simple_stmt _loop0_6
         mark = self._mark()
         if (
             (elem := self.simple_stmt())
             is not None
             and
-            (seq := self._loop0_5())
+            (seq := self._loop0_6())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_7(self) -> Optional[Any]:
-        # _loop0_7: ';' scenic_stmt
+    def _loop0_8(self) -> Optional[Any]:
+        # _loop0_8: ';' scenic_stmt
         mark = self._mark()
         children = []
         while (
             (self.expect(';'))
             and
             (elem := self.scenic_stmt())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_6(self) -> Optional[Any]:
-        # _gather_6: scenic_stmt _loop0_7
+    def _gather_7(self) -> Optional[Any]:
+        # _gather_7: scenic_stmt _loop0_8
         mark = self._mark()
         if (
             (elem := self.scenic_stmt())
             is not None
             and
-            (seq := self._loop0_7())
+            (seq := self._loop0_8())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_8(self) -> Optional[Any]:
-        # _tmp_8: 'import' | 'from'
+    def _tmp_9(self) -> Optional[Any]:
+        # _tmp_9: 'import' | 'from'
         mark = self._mark()
         if (
             (literal := self.expect('import'))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect('from'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_9(self) -> Optional[Any]:
-        # _tmp_9: 'def' | '@' | 'async'
+    def _tmp_10(self) -> Optional[Any]:
+        # _tmp_10: 'def' | '@' | 'async'
         mark = self._mark()
         if (
             (literal := self.expect('def'))
         ):
             return literal;
         self._reset(mark)
         if (
@@ -9744,77 +10572,77 @@
             (literal := self.expect('async'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_10(self) -> Optional[Any]:
-        # _tmp_10: 'class' | '@'
+    def _tmp_11(self) -> Optional[Any]:
+        # _tmp_11: 'class' | '@'
         mark = self._mark()
         if (
             (literal := self.expect('class'))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect('@'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_11(self) -> Optional[Any]:
-        # _tmp_11: 'with' | 'async'
+    def _tmp_12(self) -> Optional[Any]:
+        # _tmp_12: 'with' | 'async'
         mark = self._mark()
         if (
             (literal := self.expect('with'))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect('async'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_12(self) -> Optional[Any]:
-        # _tmp_12: 'for' | 'async'
+    def _tmp_13(self) -> Optional[Any]:
+        # _tmp_13: 'for' | 'async'
         mark = self._mark()
         if (
             (literal := self.expect('for'))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect('async'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_13(self) -> Optional[Any]:
-        # _tmp_13: '=' annotated_rhs
+    def _tmp_14(self) -> Optional[Any]:
+        # _tmp_14: '=' annotated_rhs
         mark = self._mark()
         if (
             (self.expect('='))
             and
             (d := self.annotated_rhs())
         ):
             return d;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_14(self) -> Optional[Any]:
-        # _tmp_14: '(' single_target ')' | single_subscript_attribute_target
+    def _tmp_15(self) -> Optional[Any]:
+        # _tmp_15: '(' single_target ')' | single_subscript_attribute_target
         mark = self._mark()
         if (
             (self.expect('('))
             and
             (b := self.single_target())
             and
             (self.expect(')'))
@@ -9825,374 +10653,374 @@
             (single_subscript_attribute_target := self.single_subscript_attribute_target())
         ):
             return single_subscript_attribute_target;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_15(self) -> Optional[Any]:
-        # _tmp_15: '=' annotated_rhs
+    def _tmp_16(self) -> Optional[Any]:
+        # _tmp_16: '=' annotated_rhs
         mark = self._mark()
         if (
             (self.expect('='))
             and
             (d := self.annotated_rhs())
         ):
             return d;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop1_16(self) -> Optional[Any]:
-        # _loop1_16: (star_targets '=')
+    def _loop1_17(self) -> Optional[Any]:
+        # _loop1_17: (star_targets '=')
         mark = self._mark()
         children = []
         while (
-            (_tmp_273 := self._tmp_273())
+            (_tmp_312 := self._tmp_312())
         ):
-            children.append(_tmp_273)
+            children.append(_tmp_312)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_17(self) -> Optional[Any]:
-        # _tmp_17: yield_expr | star_expressions
+    def _tmp_18(self) -> Optional[Any]:
+        # _tmp_18: yield_expr | star_expressions
         mark = self._mark()
         if (
             (yield_expr := self.yield_expr())
         ):
             return yield_expr;
         self._reset(mark)
         if (
             (star_expressions := self.star_expressions())
         ):
             return star_expressions;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_18(self) -> Optional[Any]:
-        # _tmp_18: yield_expr | star_expressions
+    def _tmp_19(self) -> Optional[Any]:
+        # _tmp_19: yield_expr | star_expressions
         mark = self._mark()
         if (
             (yield_expr := self.yield_expr())
         ):
             return yield_expr;
         self._reset(mark)
         if (
             (star_expressions := self.star_expressions())
         ):
             return star_expressions;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_19(self) -> Optional[Any]:
-        # _tmp_19: 'from' expression
+    def _tmp_20(self) -> Optional[Any]:
+        # _tmp_20: 'from' expression
         mark = self._mark()
         if (
             (self.expect('from'))
             and
             (z := self.expression())
         ):
             return z;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_21(self) -> Optional[Any]:
-        # _loop0_21: ',' NAME
+    def _loop0_22(self) -> Optional[Any]:
+        # _loop0_22: ',' NAME
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.name())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_20(self) -> Optional[Any]:
-        # _gather_20: NAME _loop0_21
+    def _gather_21(self) -> Optional[Any]:
+        # _gather_21: NAME _loop0_22
         mark = self._mark()
         if (
             (elem := self.name())
             is not None
             and
-            (seq := self._loop0_21())
+            (seq := self._loop0_22())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_23(self) -> Optional[Any]:
-        # _loop0_23: ',' NAME
+    def _loop0_24(self) -> Optional[Any]:
+        # _loop0_24: ',' NAME
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.name())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_22(self) -> Optional[Any]:
-        # _gather_22: NAME _loop0_23
+    def _gather_23(self) -> Optional[Any]:
+        # _gather_23: NAME _loop0_24
         mark = self._mark()
         if (
             (elem := self.name())
             is not None
             and
-            (seq := self._loop0_23())
+            (seq := self._loop0_24())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_24(self) -> Optional[Any]:
-        # _tmp_24: ';' | NEWLINE
+    def _tmp_25(self) -> Optional[Any]:
+        # _tmp_25: ';' | NEWLINE
         mark = self._mark()
         if (
             (literal := self.expect(';'))
         ):
             return literal;
         self._reset(mark)
         if (
             (_newline := self.expect('NEWLINE'))
         ):
             return _newline;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_25(self) -> Optional[Any]:
-        # _tmp_25: ',' expression
+    def _tmp_26(self) -> Optional[Any]:
+        # _tmp_26: ',' expression
         mark = self._mark()
         if (
             (self.expect(','))
             and
             (z := self.expression())
         ):
             return z;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_26(self) -> Optional[Any]:
-        # _loop0_26: ('.' | '...')
+    def _loop0_27(self) -> Optional[Any]:
+        # _loop0_27: ('.' | '...')
         mark = self._mark()
         children = []
         while (
-            (_tmp_274 := self._tmp_274())
+            (_tmp_313 := self._tmp_313())
         ):
-            children.append(_tmp_274)
+            children.append(_tmp_313)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_27(self) -> Optional[Any]:
-        # _loop1_27: ('.' | '...')
+    def _loop1_28(self) -> Optional[Any]:
+        # _loop1_28: ('.' | '...')
         mark = self._mark()
         children = []
         while (
-            (_tmp_275 := self._tmp_275())
+            (_tmp_314 := self._tmp_314())
         ):
-            children.append(_tmp_275)
+            children.append(_tmp_314)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_29(self) -> Optional[Any]:
-        # _loop0_29: ',' import_from_as_name
+    def _loop0_30(self) -> Optional[Any]:
+        # _loop0_30: ',' import_from_as_name
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.import_from_as_name())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_28(self) -> Optional[Any]:
-        # _gather_28: import_from_as_name _loop0_29
+    def _gather_29(self) -> Optional[Any]:
+        # _gather_29: import_from_as_name _loop0_30
         mark = self._mark()
         if (
             (elem := self.import_from_as_name())
             is not None
             and
-            (seq := self._loop0_29())
+            (seq := self._loop0_30())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_30(self) -> Optional[Any]:
-        # _tmp_30: 'as' NAME
+    def _tmp_31(self) -> Optional[Any]:
+        # _tmp_31: 'as' NAME
         mark = self._mark()
         if (
             (self.expect('as'))
             and
             (z := self.name())
         ):
             return z . string;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_32(self) -> Optional[Any]:
-        # _loop0_32: ',' dotted_as_name
+    def _loop0_33(self) -> Optional[Any]:
+        # _loop0_33: ',' dotted_as_name
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.dotted_as_name())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_31(self) -> Optional[Any]:
-        # _gather_31: dotted_as_name _loop0_32
+    def _gather_32(self) -> Optional[Any]:
+        # _gather_32: dotted_as_name _loop0_33
         mark = self._mark()
         if (
             (elem := self.dotted_as_name())
             is not None
             and
-            (seq := self._loop0_32())
+            (seq := self._loop0_33())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_33(self) -> Optional[Any]:
-        # _tmp_33: 'as' NAME
+    def _tmp_34(self) -> Optional[Any]:
+        # _tmp_34: 'as' NAME
         mark = self._mark()
         if (
             (self.expect('as'))
             and
             (z := self.name())
         ):
             return z . string;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop1_34(self) -> Optional[Any]:
-        # _loop1_34: decorator
+    def _loop1_35(self) -> Optional[Any]:
+        # _loop1_35: decorator
         mark = self._mark()
         children = []
         while (
             (decorator := self.decorator())
         ):
             children.append(decorator)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_35(self) -> Optional[Any]:
-        # _tmp_35: '@' dec_maybe_call NEWLINE
+    def _tmp_36(self) -> Optional[Any]:
+        # _tmp_36: '@' dec_maybe_call NEWLINE
         mark = self._mark()
         if (
             (self.expect('@'))
             and
             (f := self.dec_maybe_call())
             and
             (self.expect('NEWLINE'))
         ):
             return f;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_36(self) -> Optional[Any]:
-        # _tmp_36: '@' named_expression NEWLINE
+    def _tmp_37(self) -> Optional[Any]:
+        # _tmp_37: '@' named_expression NEWLINE
         mark = self._mark()
         if (
             (self.expect('@'))
             and
             (f := self.named_expression())
             and
             (self.expect('NEWLINE'))
         ):
             return f;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_37(self) -> Optional[Any]:
-        # _tmp_37: '(' arguments? ')'
+    def _tmp_38(self) -> Optional[Any]:
+        # _tmp_38: '(' arguments? ')'
         mark = self._mark()
         if (
             (self.expect('('))
             and
             (z := self.arguments(),)
             and
             (self.expect(')'))
         ):
             return z;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop1_38(self) -> Optional[Any]:
-        # _loop1_38: scenic_class_statement
+    def _loop1_39(self) -> Optional[Any]:
+        # _loop1_39: scenic_class_statement
         mark = self._mark()
         children = []
         while (
             (scenic_class_statement := self.scenic_class_statement())
         ):
             children.append(scenic_class_statement)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_39(self) -> Optional[Any]:
-        # _tmp_39: '[' ','.scenic_class_property_attribute+ ']'
+    def _tmp_40(self) -> Optional[Any]:
+        # _tmp_40: '[' ','.scenic_class_property_attribute+ ']'
         mark = self._mark()
         if (
             (self.expect('['))
             and
-            (attrs := self._gather_276())
+            (attrs := self._gather_315())
             and
             (self.expect(']'))
         ):
             return attrs;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_40(self) -> Optional[Any]:
-        # _tmp_40: "additive" | "dynamic" | "final"
+    def _tmp_41(self) -> Optional[Any]:
+        # _tmp_41: "additive" | "dynamic" | "final"
         mark = self._mark()
         tok = self._tokenizer.peek()
         start_lineno, start_col_offset = tok.start
         if (
             (self.expect("additive"))
         ):
             tok = self._tokenizer.get_last_non_whitespace_token()
@@ -10212,489 +11040,502 @@
             tok = self._tokenizer.get_last_non_whitespace_token()
             end_lineno, end_col_offset = tok.end
             return s . Final ( lineno=start_lineno, col_offset=start_col_offset, end_lineno=end_lineno, end_col_offset=end_col_offset );
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop1_41(self) -> Optional[Any]:
-        # _loop1_41: (star_targets '=')
+    def _loop1_42(self) -> Optional[Any]:
+        # _loop1_42: (star_targets '=')
         mark = self._mark()
         children = []
         while (
-            (_tmp_278 := self._tmp_278())
+            (_tmp_317 := self._tmp_317())
         ):
-            children.append(_tmp_278)
+            children.append(_tmp_317)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_42(self) -> Optional[Any]:
-        # _loop0_42: (scenic_specifiers ',' NEWLINE)
+    def _loop0_43(self) -> Optional[Any]:
+        # _loop0_43: (scenic_specifiers ',' NEWLINE)
         mark = self._mark()
         children = []
         while (
-            (_tmp_279 := self._tmp_279())
+            (_tmp_318 := self._tmp_318())
         ):
-            children.append(_tmp_279)
+            children.append(_tmp_318)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_43(self) -> Optional[Any]:
-        # _loop1_43: (scenic_specifiers ',' NEWLINE)
+    def _loop1_44(self) -> Optional[Any]:
+        # _loop1_44: (scenic_specifiers ',' NEWLINE)
         mark = self._mark()
         children = []
         while (
-            (_tmp_280 := self._tmp_280())
+            (_tmp_319 := self._tmp_319())
         ):
-            children.append(_tmp_280)
+            children.append(_tmp_319)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_44(self) -> Optional[Any]:
-        # _tmp_44: STRING NEWLINE
+    def _tmp_45(self) -> Optional[Any]:
+        # _tmp_45: STRING NEWLINE
         mark = self._mark()
         if (
             (x := self.string())
             and
             (self.expect('NEWLINE'))
         ):
             return x . string;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop1_45(self) -> Optional[Any]:
-        # _loop1_45: scenic_behavior_statement
+    def _loop1_46(self) -> Optional[Any]:
+        # _loop1_46: scenic_behavior_statement
         mark = self._mark()
         children = []
         while (
             (scenic_behavior_statement := self.scenic_behavior_statement())
         ):
             children.append(scenic_behavior_statement)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_46(self) -> Optional[Any]:
-        # _loop1_46: ((scenic_precondition_stmt | scenic_invariant_stmt) NEWLINE)
+    def _loop1_47(self) -> Optional[Any]:
+        # _loop1_47: ((scenic_precondition_stmt | scenic_invariant_stmt) NEWLINE)
         mark = self._mark()
         children = []
         while (
-            (_tmp_281 := self._tmp_281())
+            (_tmp_320 := self._tmp_320())
         ):
-            children.append(_tmp_281)
+            children.append(_tmp_320)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_47(self) -> Optional[Any]:
-        # _tmp_47: STRING NEWLINE
+    def _tmp_48(self) -> Optional[Any]:
+        # _tmp_48: STRING NEWLINE
         mark = self._mark()
         if (
             (x := self.string())
             and
             (self.expect('NEWLINE'))
         ):
             return x . string;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop1_48(self) -> Optional[Any]:
-        # _loop1_48: statement
+    def _loop1_49(self) -> Optional[Any]:
+        # _loop1_49: statement
         mark = self._mark()
         children = []
         while (
             (statement := self.statement())
         ):
             children.append(statement)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_49(self) -> Optional[Any]:
-        # _tmp_49: '(' params? ')'
+    def _tmp_50(self) -> Optional[Any]:
+        # _tmp_50: '(' params? ')'
         mark = self._mark()
         if (
             (self.expect('('))
             and
             (z := self.params(),)
             and
             (self.expect(')'))
         ):
             return z;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_50(self) -> Optional[Any]:
-        # _tmp_50: STRING NEWLINE
+    def _tmp_51(self) -> Optional[Any]:
+        # _tmp_51: STRING NEWLINE
         mark = self._mark()
         if (
             (x := self.string())
             and
             (self.expect('NEWLINE'))
         ):
             return x . string;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_51(self) -> Optional[Any]:
-        # _tmp_51: STRING NEWLINE
+    def _tmp_52(self) -> Optional[Any]:
+        # _tmp_52: STRING NEWLINE
         mark = self._mark()
         if (
             (x := self.string())
             and
             (self.expect('NEWLINE'))
         ):
             return x . string;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_52(self) -> Optional[Any]:
-        # _tmp_52: '->' expression
+    def _tmp_53(self) -> Optional[Any]:
+        # _tmp_53: '->' expression
         mark = self._mark()
         if (
             (self.expect('->'))
             and
             (z := self.expression())
         ):
             return z;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_53(self) -> Optional[Any]:
-        # _tmp_53: '->' expression
+    def _tmp_54(self) -> Optional[Any]:
+        # _tmp_54: '->' expression
         mark = self._mark()
         if (
             (self.expect('->'))
             and
             (z := self.expression())
         ):
             return z;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_54(self) -> Optional[Any]:
-        # _loop0_54: param_no_default
+    def _loop0_55(self) -> Optional[Any]:
+        # _loop0_55: param_no_default
         mark = self._mark()
         children = []
         while (
             (param_no_default := self.param_no_default())
         ):
             children.append(param_no_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_55(self) -> Optional[Any]:
-        # _loop0_55: param_with_default
+    def _loop0_56(self) -> Optional[Any]:
+        # _loop0_56: param_with_default
         mark = self._mark()
         children = []
         while (
             (param_with_default := self.param_with_default())
         ):
             children.append(param_with_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_56(self) -> Optional[Any]:
-        # _loop0_56: param_with_default
+    def _loop0_57(self) -> Optional[Any]:
+        # _loop0_57: param_with_default
         mark = self._mark()
         children = []
         while (
             (param_with_default := self.param_with_default())
         ):
             children.append(param_with_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_57(self) -> Optional[Any]:
-        # _loop1_57: param_no_default
+    def _loop1_58(self) -> Optional[Any]:
+        # _loop1_58: param_no_default
         mark = self._mark()
         children = []
         while (
             (param_no_default := self.param_no_default())
         ):
             children.append(param_no_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_58(self) -> Optional[Any]:
-        # _loop0_58: param_with_default
+    def _loop0_59(self) -> Optional[Any]:
+        # _loop0_59: param_with_default
         mark = self._mark()
         children = []
         while (
             (param_with_default := self.param_with_default())
         ):
             children.append(param_with_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_59(self) -> Optional[Any]:
-        # _loop1_59: param_with_default
+    def _loop1_60(self) -> Optional[Any]:
+        # _loop1_60: param_with_default
         mark = self._mark()
         children = []
         while (
             (param_with_default := self.param_with_default())
         ):
             children.append(param_with_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_60(self) -> Optional[Any]:
-        # _loop1_60: param_no_default
+    def _loop1_61(self) -> Optional[Any]:
+        # _loop1_61: param_no_default
         mark = self._mark()
         children = []
         while (
             (param_no_default := self.param_no_default())
         ):
             children.append(param_no_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_61(self) -> Optional[Any]:
-        # _loop1_61: param_no_default
+    def _loop1_62(self) -> Optional[Any]:
+        # _loop1_62: param_no_default
         mark = self._mark()
         children = []
         while (
             (param_no_default := self.param_no_default())
         ):
             children.append(param_no_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_62(self) -> Optional[Any]:
-        # _loop0_62: param_no_default
+    def _loop0_63(self) -> Optional[Any]:
+        # _loop0_63: param_no_default
         mark = self._mark()
         children = []
         while (
             (param_no_default := self.param_no_default())
         ):
             children.append(param_no_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_63(self) -> Optional[Any]:
-        # _loop1_63: param_with_default
+    def _loop1_64(self) -> Optional[Any]:
+        # _loop1_64: param_with_default
         mark = self._mark()
         children = []
         while (
             (param_with_default := self.param_with_default())
         ):
             children.append(param_with_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_64(self) -> Optional[Any]:
-        # _loop0_64: param_no_default
+    def _loop0_65(self) -> Optional[Any]:
+        # _loop0_65: param_no_default
         mark = self._mark()
         children = []
         while (
             (param_no_default := self.param_no_default())
         ):
             children.append(param_no_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_65(self) -> Optional[Any]:
-        # _loop1_65: param_with_default
+    def _loop1_66(self) -> Optional[Any]:
+        # _loop1_66: param_with_default
         mark = self._mark()
         children = []
         while (
             (param_with_default := self.param_with_default())
         ):
             children.append(param_with_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_66(self) -> Optional[Any]:
-        # _loop0_66: param_maybe_default
+    def _loop0_67(self) -> Optional[Any]:
+        # _loop0_67: param_maybe_default
+        mark = self._mark()
+        children = []
+        while (
+            (param_maybe_default := self.param_maybe_default())
+        ):
+            children.append(param_maybe_default)
+            mark = self._mark()
+        self._reset(mark)
+        return children;
+
+    @memoize
+    def _loop0_68(self) -> Optional[Any]:
+        # _loop0_68: param_maybe_default
         mark = self._mark()
         children = []
         while (
             (param_maybe_default := self.param_maybe_default())
         ):
             children.append(param_maybe_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_67(self) -> Optional[Any]:
-        # _loop1_67: param_maybe_default
+    def _loop1_69(self) -> Optional[Any]:
+        # _loop1_69: param_maybe_default
         mark = self._mark()
         children = []
         while (
             (param_maybe_default := self.param_maybe_default())
         ):
             children.append(param_maybe_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_69(self) -> Optional[Any]:
-        # _loop0_69: ',' with_item
+    def _loop0_71(self) -> Optional[Any]:
+        # _loop0_71: ',' with_item
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.with_item())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_68(self) -> Optional[Any]:
-        # _gather_68: with_item _loop0_69
+    def _gather_70(self) -> Optional[Any]:
+        # _gather_70: with_item _loop0_71
         mark = self._mark()
         if (
             (elem := self.with_item())
             is not None
             and
-            (seq := self._loop0_69())
+            (seq := self._loop0_71())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_71(self) -> Optional[Any]:
-        # _loop0_71: ',' with_item
+    def _loop0_73(self) -> Optional[Any]:
+        # _loop0_73: ',' with_item
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.with_item())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_70(self) -> Optional[Any]:
-        # _gather_70: with_item _loop0_71
+    def _gather_72(self) -> Optional[Any]:
+        # _gather_72: with_item _loop0_73
         mark = self._mark()
         if (
             (elem := self.with_item())
             is not None
             and
-            (seq := self._loop0_71())
+            (seq := self._loop0_73())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_73(self) -> Optional[Any]:
-        # _loop0_73: ',' with_item
+    def _loop0_75(self) -> Optional[Any]:
+        # _loop0_75: ',' with_item
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.with_item())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_72(self) -> Optional[Any]:
-        # _gather_72: with_item _loop0_73
+    def _gather_74(self) -> Optional[Any]:
+        # _gather_74: with_item _loop0_75
         mark = self._mark()
         if (
             (elem := self.with_item())
             is not None
             and
-            (seq := self._loop0_73())
+            (seq := self._loop0_75())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_75(self) -> Optional[Any]:
-        # _loop0_75: ',' with_item
+    def _loop0_77(self) -> Optional[Any]:
+        # _loop0_77: ',' with_item
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.with_item())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_74(self) -> Optional[Any]:
-        # _gather_74: with_item _loop0_75
+    def _gather_76(self) -> Optional[Any]:
+        # _gather_76: with_item _loop0_77
         mark = self._mark()
         if (
             (elem := self.with_item())
             is not None
             and
-            (seq := self._loop0_75())
+            (seq := self._loop0_77())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_76(self) -> Optional[Any]:
-        # _tmp_76: ',' | ')' | ':'
+    def _tmp_78(self) -> Optional[Any]:
+        # _tmp_78: ',' | ')' | ':'
         mark = self._mark()
         if (
             (literal := self.expect(','))
         ):
             return literal;
         self._reset(mark)
         if (
@@ -10706,143 +11547,169 @@
             (literal := self.expect(':'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop1_77(self) -> Optional[Any]:
-        # _loop1_77: except_block
+    def _loop1_79(self) -> Optional[Any]:
+        # _loop1_79: except_block
         mark = self._mark()
         children = []
         while (
             (except_block := self.except_block())
         ):
             children.append(except_block)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_78(self) -> Optional[Any]:
-        # _loop1_78: interrupt_when_block
+    def _loop1_80(self) -> Optional[Any]:
+        # _loop1_80: except_star_block
+        mark = self._mark()
+        children = []
+        while (
+            (except_star_block := self.except_star_block())
+        ):
+            children.append(except_star_block)
+            mark = self._mark()
+        self._reset(mark)
+        return children;
+
+    @memoize
+    def _loop1_81(self) -> Optional[Any]:
+        # _loop1_81: interrupt_when_block
         mark = self._mark()
         children = []
         while (
             (interrupt_when_block := self.interrupt_when_block())
         ):
             children.append(interrupt_when_block)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_79(self) -> Optional[Any]:
-        # _loop0_79: except_block
+    def _loop0_82(self) -> Optional[Any]:
+        # _loop0_82: except_block
         mark = self._mark()
         children = []
         while (
             (except_block := self.except_block())
         ):
             children.append(except_block)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_80(self) -> Optional[Any]:
-        # _tmp_80: 'as' NAME
+    def _tmp_83(self) -> Optional[Any]:
+        # _tmp_83: 'as' NAME
         mark = self._mark()
         if (
             (self.expect('as'))
             and
             (z := self.name())
         ):
             return z . string;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop1_81(self) -> Optional[Any]:
-        # _loop1_81: case_block
+    def _tmp_84(self) -> Optional[Any]:
+        # _tmp_84: 'as' NAME
+        mark = self._mark()
+        if (
+            (self.expect('as'))
+            and
+            (z := self.name())
+        ):
+            return z . string;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _loop1_85(self) -> Optional[Any]:
+        # _loop1_85: case_block
         mark = self._mark()
         children = []
         while (
             (case_block := self.case_block())
         ):
             children.append(case_block)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_83(self) -> Optional[Any]:
-        # _loop0_83: '|' closed_pattern
+    def _loop0_87(self) -> Optional[Any]:
+        # _loop0_87: '|' closed_pattern
         mark = self._mark()
         children = []
         while (
             (self.expect('|'))
             and
             (elem := self.closed_pattern())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_82(self) -> Optional[Any]:
-        # _gather_82: closed_pattern _loop0_83
+    def _gather_86(self) -> Optional[Any]:
+        # _gather_86: closed_pattern _loop0_87
         mark = self._mark()
         if (
             (elem := self.closed_pattern())
             is not None
             and
-            (seq := self._loop0_83())
+            (seq := self._loop0_87())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_84(self) -> Optional[Any]:
-        # _tmp_84: '+' | '-'
+    def _tmp_88(self) -> Optional[Any]:
+        # _tmp_88: '+' | '-'
         mark = self._mark()
         if (
             (literal := self.expect('+'))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect('-'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_85(self) -> Optional[Any]:
-        # _tmp_85: '+' | '-'
+    def _tmp_89(self) -> Optional[Any]:
+        # _tmp_89: '+' | '-'
         mark = self._mark()
         if (
             (literal := self.expect('+'))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect('-'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_86(self) -> Optional[Any]:
-        # _tmp_86: '.' | '(' | '='
+    def _tmp_90(self) -> Optional[Any]:
+        # _tmp_90: '.' | '(' | '='
         mark = self._mark()
         if (
             (literal := self.expect('.'))
         ):
             return literal;
         self._reset(mark)
         if (
@@ -10854,16 +11721,16 @@
             (literal := self.expect('='))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_87(self) -> Optional[Any]:
-        # _tmp_87: '.' | '(' | '='
+    def _tmp_91(self) -> Optional[Any]:
+        # _tmp_91: '.' | '(' | '='
         mark = self._mark()
         if (
             (literal := self.expect('.'))
         ):
             return literal;
         self._reset(mark)
         if (
@@ -10875,318 +11742,348 @@
             (literal := self.expect('='))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_89(self) -> Optional[Any]:
-        # _loop0_89: ',' maybe_star_pattern
+    def _loop0_93(self) -> Optional[Any]:
+        # _loop0_93: ',' maybe_star_pattern
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.maybe_star_pattern())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_88(self) -> Optional[Any]:
-        # _gather_88: maybe_star_pattern _loop0_89
+    def _gather_92(self) -> Optional[Any]:
+        # _gather_92: maybe_star_pattern _loop0_93
         mark = self._mark()
         if (
             (elem := self.maybe_star_pattern())
             is not None
             and
-            (seq := self._loop0_89())
+            (seq := self._loop0_93())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_91(self) -> Optional[Any]:
-        # _loop0_91: ',' key_value_pattern
+    def _loop0_95(self) -> Optional[Any]:
+        # _loop0_95: ',' key_value_pattern
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.key_value_pattern())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_90(self) -> Optional[Any]:
-        # _gather_90: key_value_pattern _loop0_91
+    def _gather_94(self) -> Optional[Any]:
+        # _gather_94: key_value_pattern _loop0_95
         mark = self._mark()
         if (
             (elem := self.key_value_pattern())
             is not None
             and
-            (seq := self._loop0_91())
+            (seq := self._loop0_95())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_92(self) -> Optional[Any]:
-        # _tmp_92: literal_expr | attr
+    def _tmp_96(self) -> Optional[Any]:
+        # _tmp_96: literal_expr | attr
         mark = self._mark()
         if (
             (literal_expr := self.literal_expr())
         ):
             return literal_expr;
         self._reset(mark)
         if (
             (attr := self.attr())
         ):
             return attr;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_94(self) -> Optional[Any]:
-        # _loop0_94: ',' pattern
+    def _loop0_98(self) -> Optional[Any]:
+        # _loop0_98: ',' pattern
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.pattern())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_93(self) -> Optional[Any]:
-        # _gather_93: pattern _loop0_94
+    def _gather_97(self) -> Optional[Any]:
+        # _gather_97: pattern _loop0_98
         mark = self._mark()
         if (
             (elem := self.pattern())
             is not None
             and
-            (seq := self._loop0_94())
+            (seq := self._loop0_98())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_96(self) -> Optional[Any]:
-        # _loop0_96: ',' keyword_pattern
+    def _loop0_100(self) -> Optional[Any]:
+        # _loop0_100: ',' keyword_pattern
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.keyword_pattern())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_95(self) -> Optional[Any]:
-        # _gather_95: keyword_pattern _loop0_96
+    def _gather_99(self) -> Optional[Any]:
+        # _gather_99: keyword_pattern _loop0_100
         mark = self._mark()
         if (
             (elem := self.keyword_pattern())
             is not None
             and
-            (seq := self._loop0_96())
+            (seq := self._loop0_100())
+            is not None
+        ):
+            return [elem] + seq;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _loop0_102(self) -> Optional[Any]:
+        # _loop0_102: ',' type_param
+        mark = self._mark()
+        children = []
+        while (
+            (self.expect(','))
+            and
+            (elem := self.type_param())
+        ):
+            children.append(elem)
+            mark = self._mark()
+        self._reset(mark)
+        return children;
+
+    @memoize
+    def _gather_101(self) -> Optional[Any]:
+        # _gather_101: type_param _loop0_102
+        mark = self._mark()
+        if (
+            (elem := self.type_param())
+            is not None
+            and
+            (seq := self._loop0_102())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop1_97(self) -> Optional[Any]:
-        # _loop1_97: (',' expression)
+    def _loop1_103(self) -> Optional[Any]:
+        # _loop1_103: (',' expression)
         mark = self._mark()
         children = []
         while (
-            (_tmp_282 := self._tmp_282())
+            (_tmp_321 := self._tmp_321())
         ):
-            children.append(_tmp_282)
+            children.append(_tmp_321)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_98(self) -> Optional[Any]:
-        # _loop1_98: (',' star_expression)
+    def _loop1_104(self) -> Optional[Any]:
+        # _loop1_104: (',' star_expression)
         mark = self._mark()
         children = []
         while (
-            (_tmp_283 := self._tmp_283())
+            (_tmp_322 := self._tmp_322())
         ):
-            children.append(_tmp_283)
+            children.append(_tmp_322)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_100(self) -> Optional[Any]:
-        # _loop0_100: ',' star_named_expression
+    def _loop0_106(self) -> Optional[Any]:
+        # _loop0_106: ',' star_named_expression
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.star_named_expression())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_99(self) -> Optional[Any]:
-        # _gather_99: star_named_expression _loop0_100
+    def _gather_105(self) -> Optional[Any]:
+        # _gather_105: star_named_expression _loop0_106
         mark = self._mark()
         if (
             (elem := self.star_named_expression())
             is not None
             and
-            (seq := self._loop0_100())
+            (seq := self._loop0_106())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_101(self) -> Optional[Any]:
-        # _tmp_101: scenic_temporal_prefix | scenic_temporal_disjunction
+    def _tmp_107(self) -> Optional[Any]:
+        # _tmp_107: scenic_temporal_prefix | scenic_temporal_disjunction
         mark = self._mark()
         if (
             (scenic_temporal_prefix := self.scenic_temporal_prefix())
         ):
             return scenic_temporal_prefix;
         self._reset(mark)
         if (
             (scenic_temporal_disjunction := self.scenic_temporal_disjunction())
         ):
             return scenic_temporal_disjunction;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop1_102(self) -> Optional[Any]:
-        # _loop1_102: ('or' conjunction)
+    def _loop1_108(self) -> Optional[Any]:
+        # _loop1_108: ('or' conjunction)
         mark = self._mark()
         children = []
         while (
-            (_tmp_284 := self._tmp_284())
+            (_tmp_323 := self._tmp_323())
         ):
-            children.append(_tmp_284)
+            children.append(_tmp_323)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_103(self) -> Optional[Any]:
-        # _loop1_103: ('or' (scenic_temporal_prefix | scenic_temporal_conjunction))
+    def _loop1_109(self) -> Optional[Any]:
+        # _loop1_109: ('or' (scenic_temporal_prefix | scenic_temporal_conjunction))
         mark = self._mark()
         children = []
         while (
-            (_tmp_285 := self._tmp_285())
+            (_tmp_324 := self._tmp_324())
         ):
-            children.append(_tmp_285)
+            children.append(_tmp_324)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_104(self) -> Optional[Any]:
-        # _loop1_104: ('and' inversion)
+    def _loop1_110(self) -> Optional[Any]:
+        # _loop1_110: ('and' inversion)
         mark = self._mark()
         children = []
         while (
-            (_tmp_286 := self._tmp_286())
+            (_tmp_325 := self._tmp_325())
         ):
-            children.append(_tmp_286)
+            children.append(_tmp_325)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_105(self) -> Optional[Any]:
-        # _loop1_105: ('and' (scenic_temporal_prefix | scenic_temporal_inversion))
+    def _loop1_111(self) -> Optional[Any]:
+        # _loop1_111: ('and' (scenic_temporal_prefix | scenic_temporal_inversion))
         mark = self._mark()
         children = []
         while (
-            (_tmp_287 := self._tmp_287())
+            (_tmp_326 := self._tmp_326())
         ):
-            children.append(_tmp_287)
+            children.append(_tmp_326)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_106(self) -> Optional[Any]:
-        # _tmp_106: "visible" inversion
+    def _tmp_112(self) -> Optional[Any]:
+        # _tmp_112: "visible" inversion
         mark = self._mark()
         if (
             (literal := self.expect("visible"))
             and
             (inversion := self.inversion())
         ):
             return [literal, inversion];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_107(self) -> Optional[Any]:
-        # _tmp_107: "visible" scenic_temporal_inversion
+    def _tmp_113(self) -> Optional[Any]:
+        # _tmp_113: "visible" scenic_temporal_inversion
         mark = self._mark()
         if (
             (literal := self.expect("visible"))
             and
             (scenic_temporal_inversion := self.scenic_temporal_inversion())
         ):
             return [literal, scenic_temporal_inversion];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_108(self) -> Optional[Any]:
-        # _tmp_108: scenic_temporal_prefix | scenic_temporal_inversion
+    def _tmp_114(self) -> Optional[Any]:
+        # _tmp_114: scenic_temporal_prefix | scenic_temporal_inversion
         mark = self._mark()
         if (
             (scenic_temporal_prefix := self.scenic_temporal_prefix())
         ):
             return scenic_temporal_prefix;
         self._reset(mark)
         if (
             (scenic_temporal_inversion := self.scenic_temporal_inversion())
         ):
             return scenic_temporal_inversion;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_109(self) -> Optional[Any]:
-        # _tmp_109: 'until' | 'or' | 'and' | ')' | ';' | NEWLINE
+    def _tmp_115(self) -> Optional[Any]:
+        # _tmp_115: 'until' | 'or' | 'and' | ')' | ';' | NEWLINE
         mark = self._mark()
         if (
             (literal := self.expect('until'))
         ):
             return literal;
         self._reset(mark)
         if (
@@ -11213,137 +12110,137 @@
             (_newline := self.expect('NEWLINE'))
         ):
             return _newline;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_111(self) -> Optional[Any]:
-        # _loop0_111: ',' scenic_specifier
+    def _loop0_117(self) -> Optional[Any]:
+        # _loop0_117: ',' scenic_specifier
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.scenic_specifier())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_110(self) -> Optional[Any]:
-        # _gather_110: scenic_specifier _loop0_111
+    def _gather_116(self) -> Optional[Any]:
+        # _gather_116: scenic_specifier _loop0_117
         mark = self._mark()
         if (
             (elem := self.scenic_specifier())
             is not None
             and
-            (seq := self._loop0_111())
+            (seq := self._loop0_117())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_112(self) -> Optional[Any]:
-        # _tmp_112: 'by' expression
+    def _tmp_118(self) -> Optional[Any]:
+        # _tmp_118: 'by' expression
         mark = self._mark()
         if (
             (self.expect('by'))
             and
             (e := self.expression())
         ):
             return e;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_113(self) -> Optional[Any]:
-        # _tmp_113: 'from' expression
+    def _tmp_119(self) -> Optional[Any]:
+        # _tmp_119: 'from' expression
         mark = self._mark()
         if (
             (self.expect('from'))
             and
             (a := self.expression())
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_114(self) -> Optional[Any]:
-        # _tmp_114: 'from' expression
+    def _tmp_120(self) -> Optional[Any]:
+        # _tmp_120: 'from' expression
         mark = self._mark()
         if (
             (self.expect('from'))
             and
             (r := self.expression())
         ):
             return r;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_115(self) -> Optional[Any]:
-        # _tmp_115: 'from' expression
+    def _tmp_121(self) -> Optional[Any]:
+        # _tmp_121: 'from' expression
         mark = self._mark()
         if (
             (self.expect('from'))
             and
             (r := self.expression())
         ):
             return r;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_116(self) -> Optional[Any]:
-        # _tmp_116: 'from' expression
+    def _tmp_122(self) -> Optional[Any]:
+        # _tmp_122: 'from' expression
         mark = self._mark()
         if (
             (self.expect('from'))
             and
             (e := self.expression())
         ):
             return e;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_117(self) -> Optional[Any]:
-        # _tmp_117: 'from' expression
+    def _tmp_123(self) -> Optional[Any]:
+        # _tmp_123: 'from' expression
         mark = self._mark()
         if (
             (self.expect('from'))
             and
             (a := self.expression())
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop1_118(self) -> Optional[Any]:
-        # _loop1_118: compare_op_bitwise_or_pair
+    def _loop1_124(self) -> Optional[Any]:
+        # _loop1_124: compare_op_bitwise_or_pair
         mark = self._mark()
         children = []
         while (
             (compare_op_bitwise_or_pair := self.compare_op_bitwise_or_pair())
         ):
             children.append(compare_op_bitwise_or_pair)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_119(self) -> Optional[Any]:
-        # _tmp_119: "relative" 'to' | "offset" 'by'
+    def _tmp_125(self) -> Optional[Any]:
+        # _tmp_125: "relative" 'to' | "offset" 'by'
         mark = self._mark()
         if (
             (literal := self.expect("relative"))
             and
             (literal_1 := self.expect('to'))
         ):
             return [literal, literal_1];
@@ -11354,75 +12251,91 @@
             (literal_1 := self.expect('by'))
         ):
             return [literal, literal_1];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_120(self) -> Optional[Any]:
-        # _tmp_120: 'to' | 'from'
+    def _tmp_126(self) -> Optional[Any]:
+        # _tmp_126: 'to' | 'from'
         mark = self._mark()
         if (
             (literal := self.expect('to'))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect('from'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_122(self) -> Optional[Any]:
-        # _loop0_122: ',' slice
+    def _loop0_128(self) -> Optional[Any]:
+        # _loop0_128: ',' (slice | starred_expression)
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
-            (elem := self.slice())
+            (elem := self._tmp_327())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_121(self) -> Optional[Any]:
-        # _gather_121: slice _loop0_122
+    def _gather_127(self) -> Optional[Any]:
+        # _gather_127: (slice | starred_expression) _loop0_128
         mark = self._mark()
         if (
-            (elem := self.slice())
+            (elem := self._tmp_327())
             is not None
             and
-            (seq := self._loop0_122())
+            (seq := self._loop0_128())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_123(self) -> Optional[Any]:
-        # _tmp_123: ':' expression?
+    def _tmp_129(self) -> Optional[Any]:
+        # _tmp_129: ':' expression?
         mark = self._mark()
         if (
             (self.expect(':'))
             and
             (d := self.expression(),)
         ):
             return d;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_124(self) -> Optional[Any]:
-        # _tmp_124: tuple | group | genexp
+    def _tmp_130(self) -> Optional[Any]:
+        # _tmp_130: STRING | FSTRING_START
+        mark = self._mark()
+        if (
+            (string := self.string())
+        ):
+            return string;
+        self._reset(mark)
+        if (
+            (fstring_start := self.fstring_start())
+        ):
+            return fstring_start;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_131(self) -> Optional[Any]:
+        # _tmp_131: tuple | group | genexp
         mark = self._mark()
         if (
             (tuple := self.tuple())
         ):
             return tuple;
         self._reset(mark)
         if (
@@ -11434,32 +12347,32 @@
             (genexp := self.genexp())
         ):
             return genexp;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_125(self) -> Optional[Any]:
-        # _tmp_125: list | listcomp
+    def _tmp_132(self) -> Optional[Any]:
+        # _tmp_132: list | listcomp
         mark = self._mark()
         if (
             (list := self.list())
         ):
             return list;
         self._reset(mark)
         if (
             (listcomp := self.listcomp())
         ):
             return listcomp;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_126(self) -> Optional[Any]:
-        # _tmp_126: dict | set | dictcomp | setcomp
+    def _tmp_133(self) -> Optional[Any]:
+        # _tmp_133: dict | set | dictcomp | setcomp
         mark = self._mark()
         if (
             (dict := self.dict())
         ):
             return dict;
         self._reset(mark)
         if (
@@ -11476,686 +12389,715 @@
             (setcomp := self.setcomp())
         ):
             return setcomp;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_127(self) -> Optional[Any]:
-        # _tmp_127: yield_expr | named_expression
+    def _tmp_134(self) -> Optional[Any]:
+        # _tmp_134: yield_expr | named_expression
         mark = self._mark()
         if (
             (yield_expr := self.yield_expr())
         ):
             return yield_expr;
         self._reset(mark)
         if (
             (named_expression := self.named_expression())
         ):
             return named_expression;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_128(self) -> Optional[Any]:
-        # _loop0_128: lambda_param_no_default
+    def _loop0_135(self) -> Optional[Any]:
+        # _loop0_135: lambda_param_no_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_no_default := self.lambda_param_no_default())
         ):
             children.append(lambda_param_no_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_129(self) -> Optional[Any]:
-        # _loop0_129: lambda_param_with_default
+    def _loop0_136(self) -> Optional[Any]:
+        # _loop0_136: lambda_param_with_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_with_default := self.lambda_param_with_default())
         ):
             children.append(lambda_param_with_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_130(self) -> Optional[Any]:
-        # _loop0_130: lambda_param_with_default
+    def _loop0_137(self) -> Optional[Any]:
+        # _loop0_137: lambda_param_with_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_with_default := self.lambda_param_with_default())
         ):
             children.append(lambda_param_with_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_131(self) -> Optional[Any]:
-        # _loop1_131: lambda_param_no_default
+    def _loop1_138(self) -> Optional[Any]:
+        # _loop1_138: lambda_param_no_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_no_default := self.lambda_param_no_default())
         ):
             children.append(lambda_param_no_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_132(self) -> Optional[Any]:
-        # _loop0_132: lambda_param_with_default
+    def _loop0_139(self) -> Optional[Any]:
+        # _loop0_139: lambda_param_with_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_with_default := self.lambda_param_with_default())
         ):
             children.append(lambda_param_with_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_133(self) -> Optional[Any]:
-        # _loop1_133: lambda_param_with_default
+    def _loop1_140(self) -> Optional[Any]:
+        # _loop1_140: lambda_param_with_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_with_default := self.lambda_param_with_default())
         ):
             children.append(lambda_param_with_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_134(self) -> Optional[Any]:
-        # _loop1_134: lambda_param_no_default
+    def _loop1_141(self) -> Optional[Any]:
+        # _loop1_141: lambda_param_no_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_no_default := self.lambda_param_no_default())
         ):
             children.append(lambda_param_no_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_135(self) -> Optional[Any]:
-        # _loop1_135: lambda_param_no_default
+    def _loop1_142(self) -> Optional[Any]:
+        # _loop1_142: lambda_param_no_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_no_default := self.lambda_param_no_default())
         ):
             children.append(lambda_param_no_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_136(self) -> Optional[Any]:
-        # _loop0_136: lambda_param_no_default
+    def _loop0_143(self) -> Optional[Any]:
+        # _loop0_143: lambda_param_no_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_no_default := self.lambda_param_no_default())
         ):
             children.append(lambda_param_no_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_137(self) -> Optional[Any]:
-        # _loop1_137: lambda_param_with_default
+    def _loop1_144(self) -> Optional[Any]:
+        # _loop1_144: lambda_param_with_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_with_default := self.lambda_param_with_default())
         ):
             children.append(lambda_param_with_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_138(self) -> Optional[Any]:
-        # _loop0_138: lambda_param_no_default
+    def _loop0_145(self) -> Optional[Any]:
+        # _loop0_145: lambda_param_no_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_no_default := self.lambda_param_no_default())
         ):
             children.append(lambda_param_no_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_139(self) -> Optional[Any]:
-        # _loop1_139: lambda_param_with_default
+    def _loop1_146(self) -> Optional[Any]:
+        # _loop1_146: lambda_param_with_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_with_default := self.lambda_param_with_default())
         ):
             children.append(lambda_param_with_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_140(self) -> Optional[Any]:
-        # _loop0_140: lambda_param_maybe_default
+    def _loop0_147(self) -> Optional[Any]:
+        # _loop0_147: lambda_param_maybe_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_maybe_default := self.lambda_param_maybe_default())
         ):
             children.append(lambda_param_maybe_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_141(self) -> Optional[Any]:
-        # _loop1_141: lambda_param_maybe_default
+    def _loop1_148(self) -> Optional[Any]:
+        # _loop1_148: lambda_param_maybe_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_maybe_default := self.lambda_param_maybe_default())
         ):
             children.append(lambda_param_maybe_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_143(self) -> Optional[Any]:
-        # _loop0_143: ',' scenic_param_stmt_param
+    def _loop0_150(self) -> Optional[Any]:
+        # _loop0_150: ',' scenic_param_stmt_param
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.scenic_param_stmt_param())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_142(self) -> Optional[Any]:
-        # _gather_142: scenic_param_stmt_param _loop0_143
+    def _gather_149(self) -> Optional[Any]:
+        # _gather_149: scenic_param_stmt_param _loop0_150
         mark = self._mark()
         if (
             (elem := self.scenic_param_stmt_param())
             is not None
             and
-            (seq := self._loop0_143())
+            (seq := self._loop0_150())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_144(self) -> Optional[Any]:
-        # _tmp_144: 'as' scenic_require_stmt_name
+    def _tmp_151(self) -> Optional[Any]:
+        # _tmp_151: 'as' scenic_require_stmt_name
         mark = self._mark()
         if (
             (literal := self.expect('as'))
             and
             (scenic_require_stmt_name := self.scenic_require_stmt_name())
         ):
             return [literal, scenic_require_stmt_name];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_145(self) -> Optional[Any]:
-        # _tmp_145: '[' NUMBER ']'
+    def _tmp_152(self) -> Optional[Any]:
+        # _tmp_152: '[' NUMBER ']'
         mark = self._mark()
         if (
             (self.expect('['))
             and
             (a := self.number())
             and
             (self.expect(']'))
         ):
             return float ( a . string );
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_146(self) -> Optional[Any]:
-        # _tmp_146: 'as' scenic_require_stmt_name
+    def _tmp_153(self) -> Optional[Any]:
+        # _tmp_153: 'as' scenic_require_stmt_name
         mark = self._mark()
         if (
             (self.expect('as'))
             and
             (a := self.scenic_require_stmt_name())
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_147(self) -> Optional[Any]:
-        # _tmp_147: NAME | NUMBER
+    def _tmp_154(self) -> Optional[Any]:
+        # _tmp_154: NAME | NUMBER
         mark = self._mark()
         if (
             (name := self.name())
         ):
             return name;
         self._reset(mark)
         if (
             (number := self.number())
         ):
             return number;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_148(self) -> Optional[Any]:
-        # _tmp_148: 'as' scenic_require_stmt_name
+    def _tmp_155(self) -> Optional[Any]:
+        # _tmp_155: 'as' scenic_require_stmt_name
         mark = self._mark()
         if (
             (self.expect('as'))
             and
             (a := self.scenic_require_stmt_name())
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_149(self) -> Optional[Any]:
-        # _tmp_149: 'as' scenic_require_stmt_name
+    def _tmp_156(self) -> Optional[Any]:
+        # _tmp_156: 'as' scenic_require_stmt_name
         mark = self._mark()
         if (
             (self.expect('as'))
             and
             (a := self.scenic_require_stmt_name())
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_150(self) -> Optional[Any]:
-        # _tmp_150: 'as' scenic_require_stmt_name
+    def _tmp_157(self) -> Optional[Any]:
+        # _tmp_157: 'as' scenic_require_stmt_name
         mark = self._mark()
         if (
             (self.expect('as'))
             and
             (a := self.scenic_require_stmt_name())
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_152(self) -> Optional[Any]:
-        # _loop0_152: ',' scenic_mutate_stmt_id
+    def _loop0_159(self) -> Optional[Any]:
+        # _loop0_159: ',' scenic_mutate_stmt_id
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.scenic_mutate_stmt_id())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_151(self) -> Optional[Any]:
-        # _gather_151: scenic_mutate_stmt_id _loop0_152
+    def _gather_158(self) -> Optional[Any]:
+        # _gather_158: scenic_mutate_stmt_id _loop0_159
         mark = self._mark()
         if (
             (elem := self.scenic_mutate_stmt_id())
             is not None
             and
-            (seq := self._loop0_152())
+            (seq := self._loop0_159())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_153(self) -> Optional[Any]:
-        # _tmp_153: 'by' expression
+    def _tmp_160(self) -> Optional[Any]:
+        # _tmp_160: 'by' expression
         mark = self._mark()
         if (
             (self.expect('by'))
             and
             (x := self.expression())
         ):
             return x;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_155(self) -> Optional[Any]:
-        # _loop0_155: ',' expression
+    def _loop0_162(self) -> Optional[Any]:
+        # _loop0_162: ',' expression
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.expression())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_154(self) -> Optional[Any]:
-        # _gather_154: expression _loop0_155
+    def _gather_161(self) -> Optional[Any]:
+        # _gather_161: expression _loop0_162
         mark = self._mark()
         if (
             (elem := self.expression())
             is not None
             and
-            (seq := self._loop0_155())
+            (seq := self._loop0_162())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_156(self) -> Optional[Any]:
-        # _tmp_156: 'as' scenic_require_stmt_name
+    def _tmp_163(self) -> Optional[Any]:
+        # _tmp_163: 'as' scenic_require_stmt_name
         mark = self._mark()
         if (
             (self.expect('as'))
             and
             (a := self.scenic_require_stmt_name())
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_157(self) -> Optional[Any]:
-        # _tmp_157: 'as' scenic_require_stmt_name
+    def _tmp_164(self) -> Optional[Any]:
+        # _tmp_164: 'as' scenic_require_stmt_name
         mark = self._mark()
         if (
             (self.expect('as'))
             and
             (a := self.scenic_require_stmt_name())
         ):
             return a;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_159(self) -> Optional[Any]:
-        # _loop0_159: ',' expression
+    def _loop0_166(self) -> Optional[Any]:
+        # _loop0_166: ',' expression
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.expression())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_158(self) -> Optional[Any]:
-        # _gather_158: expression _loop0_159
+    def _gather_165(self) -> Optional[Any]:
+        # _gather_165: expression _loop0_166
         mark = self._mark()
         if (
             (elem := self.expression())
             is not None
             and
-            (seq := self._loop0_159())
+            (seq := self._loop0_166())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_161(self) -> Optional[Any]:
-        # _loop0_161: ',' expression
+    def _loop0_168(self) -> Optional[Any]:
+        # _loop0_168: ',' expression
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.expression())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_160(self) -> Optional[Any]:
-        # _gather_160: expression _loop0_161
+    def _gather_167(self) -> Optional[Any]:
+        # _gather_167: expression _loop0_168
         mark = self._mark()
         if (
             (elem := self.expression())
             is not None
             and
-            (seq := self._loop0_161())
+            (seq := self._loop0_168())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_163(self) -> Optional[Any]:
-        # _loop0_163: ',' expression
+    def _loop0_170(self) -> Optional[Any]:
+        # _loop0_170: ',' expression
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.expression())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_162(self) -> Optional[Any]:
-        # _gather_162: expression _loop0_163
+    def _gather_169(self) -> Optional[Any]:
+        # _gather_169: expression _loop0_170
         mark = self._mark()
         if (
             (elem := self.expression())
             is not None
             and
-            (seq := self._loop0_163())
+            (seq := self._loop0_170())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_165(self) -> Optional[Any]:
-        # _loop0_165: ',' disjunction
+    def _loop0_172(self) -> Optional[Any]:
+        # _loop0_172: ',' disjunction
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.disjunction())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_164(self) -> Optional[Any]:
-        # _gather_164: disjunction _loop0_165
+    def _gather_171(self) -> Optional[Any]:
+        # _gather_171: disjunction _loop0_172
         mark = self._mark()
         if (
             (elem := self.disjunction())
             is not None
             and
-            (seq := self._loop0_165())
+            (seq := self._loop0_172())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_167(self) -> Optional[Any]:
-        # _loop0_167: ',' expression
+    def _loop0_174(self) -> Optional[Any]:
+        # _loop0_174: ',' expression
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.expression())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_166(self) -> Optional[Any]:
-        # _gather_166: expression _loop0_167
+    def _gather_173(self) -> Optional[Any]:
+        # _gather_173: expression _loop0_174
         mark = self._mark()
         if (
             (elem := self.expression())
             is not None
             and
-            (seq := self._loop0_167())
+            (seq := self._loop0_174())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop1_168(self) -> Optional[Any]:
-        # _loop1_168: STRING
+    def _tmp_175(self) -> Optional[Any]:
+        # _tmp_175: yield_expr | star_expressions
+        mark = self._mark()
+        if (
+            (yield_expr := self.yield_expr())
+        ):
+            return yield_expr;
+        self._reset(mark)
+        if (
+            (star_expressions := self.star_expressions())
+        ):
+            return star_expressions;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _loop0_176(self) -> Optional[Any]:
+        # _loop0_176: fstring_format_spec
         mark = self._mark()
         children = []
         while (
-            (string := self.string())
+            (fstring_format_spec := self.fstring_format_spec())
         ):
-            children.append(string)
+            children.append(fstring_format_spec)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_169(self) -> Optional[Any]:
-        # _tmp_169: star_named_expression ',' star_named_expressions?
+    def _loop1_177(self) -> Optional[Any]:
+        # _loop1_177: (fstring | STRING)
+        mark = self._mark()
+        children = []
+        while (
+            (_tmp_328 := self._tmp_328())
+        ):
+            children.append(_tmp_328)
+            mark = self._mark()
+        self._reset(mark)
+        return children;
+
+    @memoize
+    def _tmp_178(self) -> Optional[Any]:
+        # _tmp_178: star_named_expression ',' star_named_expressions?
         mark = self._mark()
         if (
             (y := self.star_named_expression())
             and
             (self.expect(','))
             and
             (z := self.star_named_expressions(),)
         ):
             return [y] + ( z or [] );
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_171(self) -> Optional[Any]:
-        # _loop0_171: ',' double_starred_kvpair
+    def _loop0_180(self) -> Optional[Any]:
+        # _loop0_180: ',' double_starred_kvpair
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.double_starred_kvpair())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_170(self) -> Optional[Any]:
-        # _gather_170: double_starred_kvpair _loop0_171
+    def _gather_179(self) -> Optional[Any]:
+        # _gather_179: double_starred_kvpair _loop0_180
         mark = self._mark()
         if (
             (elem := self.double_starred_kvpair())
             is not None
             and
-            (seq := self._loop0_171())
+            (seq := self._loop0_180())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop1_172(self) -> Optional[Any]:
-        # _loop1_172: for_if_clause
+    def _loop1_181(self) -> Optional[Any]:
+        # _loop1_181: for_if_clause
         mark = self._mark()
         children = []
         while (
             (for_if_clause := self.for_if_clause())
         ):
             children.append(for_if_clause)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_173(self) -> Optional[Any]:
-        # _loop0_173: ('if' disjunction)
+    def _loop0_182(self) -> Optional[Any]:
+        # _loop0_182: ('if' disjunction)
         mark = self._mark()
         children = []
         while (
-            (_tmp_288 := self._tmp_288())
+            (_tmp_329 := self._tmp_329())
         ):
-            children.append(_tmp_288)
+            children.append(_tmp_329)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_174(self) -> Optional[Any]:
-        # _loop0_174: ('if' disjunction)
+    def _loop0_183(self) -> Optional[Any]:
+        # _loop0_183: ('if' disjunction)
         mark = self._mark()
         children = []
         while (
-            (_tmp_289 := self._tmp_289())
+            (_tmp_330 := self._tmp_330())
         ):
-            children.append(_tmp_289)
+            children.append(_tmp_330)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_175(self) -> Optional[Any]:
-        # _tmp_175: assignment_expression | expression !':='
+    def _tmp_184(self) -> Optional[Any]:
+        # _tmp_184: assignment_expression | expression !':='
         mark = self._mark()
         if (
             (assignment_expression := self.assignment_expression())
         ):
             return assignment_expression;
         self._reset(mark)
         if (
@@ -12164,411 +13106,411 @@
             (self.negative_lookahead(self.expect, ':='))
         ):
             return expression;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_177(self) -> Optional[Any]:
-        # _loop0_177: ',' (starred_expression | (assignment_expression | expression !':=') !'=')
+    def _loop0_186(self) -> Optional[Any]:
+        # _loop0_186: ',' (starred_expression | (assignment_expression | expression !':=') !'=')
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
-            (elem := self._tmp_290())
+            (elem := self._tmp_331())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_176(self) -> Optional[Any]:
-        # _gather_176: (starred_expression | (assignment_expression | expression !':=') !'=') _loop0_177
+    def _gather_185(self) -> Optional[Any]:
+        # _gather_185: (starred_expression | (assignment_expression | expression !':=') !'=') _loop0_186
         mark = self._mark()
         if (
-            (elem := self._tmp_290())
+            (elem := self._tmp_331())
             is not None
             and
-            (seq := self._loop0_177())
+            (seq := self._loop0_186())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_178(self) -> Optional[Any]:
-        # _tmp_178: ',' kwargs
+    def _tmp_187(self) -> Optional[Any]:
+        # _tmp_187: ',' kwargs
         mark = self._mark()
         if (
             (self.expect(','))
             and
             (k := self.kwargs())
         ):
             return k;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_180(self) -> Optional[Any]:
-        # _loop0_180: ',' kwarg_or_starred
+    def _loop0_189(self) -> Optional[Any]:
+        # _loop0_189: ',' kwarg_or_starred
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.kwarg_or_starred())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_179(self) -> Optional[Any]:
-        # _gather_179: kwarg_or_starred _loop0_180
+    def _gather_188(self) -> Optional[Any]:
+        # _gather_188: kwarg_or_starred _loop0_189
         mark = self._mark()
         if (
             (elem := self.kwarg_or_starred())
             is not None
             and
-            (seq := self._loop0_180())
+            (seq := self._loop0_189())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_182(self) -> Optional[Any]:
-        # _loop0_182: ',' kwarg_or_double_starred
+    def _loop0_191(self) -> Optional[Any]:
+        # _loop0_191: ',' kwarg_or_double_starred
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.kwarg_or_double_starred())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_181(self) -> Optional[Any]:
-        # _gather_181: kwarg_or_double_starred _loop0_182
+    def _gather_190(self) -> Optional[Any]:
+        # _gather_190: kwarg_or_double_starred _loop0_191
         mark = self._mark()
         if (
             (elem := self.kwarg_or_double_starred())
             is not None
             and
-            (seq := self._loop0_182())
+            (seq := self._loop0_191())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_184(self) -> Optional[Any]:
-        # _loop0_184: ',' kwarg_or_starred
+    def _loop0_193(self) -> Optional[Any]:
+        # _loop0_193: ',' kwarg_or_starred
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.kwarg_or_starred())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_183(self) -> Optional[Any]:
-        # _gather_183: kwarg_or_starred _loop0_184
+    def _gather_192(self) -> Optional[Any]:
+        # _gather_192: kwarg_or_starred _loop0_193
         mark = self._mark()
         if (
             (elem := self.kwarg_or_starred())
             is not None
             and
-            (seq := self._loop0_184())
+            (seq := self._loop0_193())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_186(self) -> Optional[Any]:
-        # _loop0_186: ',' kwarg_or_double_starred
+    def _loop0_195(self) -> Optional[Any]:
+        # _loop0_195: ',' kwarg_or_double_starred
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.kwarg_or_double_starred())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_185(self) -> Optional[Any]:
-        # _gather_185: kwarg_or_double_starred _loop0_186
+    def _gather_194(self) -> Optional[Any]:
+        # _gather_194: kwarg_or_double_starred _loop0_195
         mark = self._mark()
         if (
             (elem := self.kwarg_or_double_starred())
             is not None
             and
-            (seq := self._loop0_186())
+            (seq := self._loop0_195())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_187(self) -> Optional[Any]:
-        # _loop0_187: (',' star_target)
+    def _loop0_196(self) -> Optional[Any]:
+        # _loop0_196: (',' star_target)
         mark = self._mark()
         children = []
         while (
-            (_tmp_291 := self._tmp_291())
+            (_tmp_332 := self._tmp_332())
         ):
-            children.append(_tmp_291)
+            children.append(_tmp_332)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_189(self) -> Optional[Any]:
-        # _loop0_189: ',' star_target
+    def _loop0_198(self) -> Optional[Any]:
+        # _loop0_198: ',' star_target
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.star_target())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_188(self) -> Optional[Any]:
-        # _gather_188: star_target _loop0_189
+    def _gather_197(self) -> Optional[Any]:
+        # _gather_197: star_target _loop0_198
         mark = self._mark()
         if (
             (elem := self.star_target())
             is not None
             and
-            (seq := self._loop0_189())
+            (seq := self._loop0_198())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop1_190(self) -> Optional[Any]:
-        # _loop1_190: (',' star_target)
+    def _loop1_199(self) -> Optional[Any]:
+        # _loop1_199: (',' star_target)
         mark = self._mark()
         children = []
         while (
-            (_tmp_292 := self._tmp_292())
+            (_tmp_333 := self._tmp_333())
         ):
-            children.append(_tmp_292)
+            children.append(_tmp_333)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_191(self) -> Optional[Any]:
-        # _tmp_191: !'*' star_target
+    def _tmp_200(self) -> Optional[Any]:
+        # _tmp_200: !'*' star_target
         mark = self._mark()
         if (
             (self.negative_lookahead(self.expect, '*'))
             and
             (star_target := self.star_target())
         ):
             return star_target;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_193(self) -> Optional[Any]:
-        # _loop0_193: ',' del_target
+    def _loop0_202(self) -> Optional[Any]:
+        # _loop0_202: ',' del_target
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.del_target())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_192(self) -> Optional[Any]:
-        # _gather_192: del_target _loop0_193
+    def _gather_201(self) -> Optional[Any]:
+        # _gather_201: del_target _loop0_202
         mark = self._mark()
         if (
             (elem := self.del_target())
             is not None
             and
-            (seq := self._loop0_193())
+            (seq := self._loop0_202())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_195(self) -> Optional[Any]:
-        # _loop0_195: ',' expression
+    def _loop0_204(self) -> Optional[Any]:
+        # _loop0_204: ',' expression
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.expression())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_194(self) -> Optional[Any]:
-        # _gather_194: expression _loop0_195
+    def _gather_203(self) -> Optional[Any]:
+        # _gather_203: expression _loop0_204
         mark = self._mark()
         if (
             (elem := self.expression())
             is not None
             and
-            (seq := self._loop0_195())
+            (seq := self._loop0_204())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_197(self) -> Optional[Any]:
-        # _loop0_197: ',' expression
+    def _loop0_206(self) -> Optional[Any]:
+        # _loop0_206: ',' expression
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.expression())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_196(self) -> Optional[Any]:
-        # _gather_196: expression _loop0_197
+    def _gather_205(self) -> Optional[Any]:
+        # _gather_205: expression _loop0_206
         mark = self._mark()
         if (
             (elem := self.expression())
             is not None
             and
-            (seq := self._loop0_197())
+            (seq := self._loop0_206())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_199(self) -> Optional[Any]:
-        # _loop0_199: ',' expression
+    def _loop0_208(self) -> Optional[Any]:
+        # _loop0_208: ',' expression
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.expression())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_198(self) -> Optional[Any]:
-        # _gather_198: expression _loop0_199
+    def _gather_207(self) -> Optional[Any]:
+        # _gather_207: expression _loop0_208
         mark = self._mark()
         if (
             (elem := self.expression())
             is not None
             and
-            (seq := self._loop0_199())
+            (seq := self._loop0_208())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_201(self) -> Optional[Any]:
-        # _loop0_201: ',' expression
+    def _loop0_210(self) -> Optional[Any]:
+        # _loop0_210: ',' expression
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.expression())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_200(self) -> Optional[Any]:
-        # _gather_200: expression _loop0_201
+    def _gather_209(self) -> Optional[Any]:
+        # _gather_209: expression _loop0_210
         mark = self._mark()
         if (
             (elem := self.expression())
             is not None
             and
-            (seq := self._loop0_201())
+            (seq := self._loop0_210())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_202(self) -> Optional[Any]:
-        # _tmp_202: NEWLINE INDENT
+    def _tmp_211(self) -> Optional[Any]:
+        # _tmp_211: NEWLINE INDENT
         mark = self._mark()
         if (
             (_newline := self.expect('NEWLINE'))
             and
             (_indent := self.expect('INDENT'))
         ):
             return [_newline, _indent];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_203(self) -> Optional[Any]:
-        # _tmp_203: args | expression for_if_clauses
+    def _tmp_212(self) -> Optional[Any]:
+        # _tmp_212: args | expression for_if_clauses
         mark = self._mark()
         if (
             (args := self.args())
         ):
             return args;
         self._reset(mark)
         if (
@@ -12577,16 +13519,45 @@
             (for_if_clauses := self.for_if_clauses())
         ):
             return [expression, for_if_clauses];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_204(self) -> Optional[Any]:
-        # _tmp_204: 'True' | 'False' | 'None'
+    def _tmp_213(self) -> Optional[Any]:
+        # _tmp_213: args ','
+        mark = self._mark()
+        if (
+            (args := self.args())
+            and
+            (literal := self.expect(','))
+        ):
+            return [args, literal];
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_214(self) -> Optional[Any]:
+        # _tmp_214: ',' | ')'
+        mark = self._mark()
+        if (
+            (literal := self.expect(','))
+        ):
+            return literal;
+        self._reset(mark)
+        if (
+            (literal := self.expect(')'))
+        ):
+            return literal;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_215(self) -> Optional[Any]:
+        # _tmp_215: 'True' | 'False' | 'None'
         mark = self._mark()
         if (
             (literal := self.expect('True'))
         ):
             return literal;
         self._reset(mark)
         if (
@@ -12598,29 +13569,29 @@
             (literal := self.expect('None'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_205(self) -> Optional[Any]:
-        # _tmp_205: NAME '='
+    def _tmp_216(self) -> Optional[Any]:
+        # _tmp_216: NAME '='
         mark = self._mark()
         if (
             (name := self.name())
             and
             (literal := self.expect('='))
         ):
             return [name, literal];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_206(self) -> Optional[Any]:
-        # _tmp_206: NAME STRING | SOFT_KEYWORD
+    def _tmp_217(self) -> Optional[Any]:
+        # _tmp_217: NAME STRING | SOFT_KEYWORD
         mark = self._mark()
         if (
             (name := self.name())
             and
             (string := self.string())
         ):
             return [name, string];
@@ -12629,48 +13600,64 @@
             (soft_keyword := self.soft_keyword())
         ):
             return soft_keyword;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_207(self) -> Optional[Any]:
-        # _tmp_207: 'else' | ':'
+    def _tmp_218(self) -> Optional[Any]:
+        # _tmp_218: 'else' | ':'
         mark = self._mark()
         if (
             (literal := self.expect('else'))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect(':'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_208(self) -> Optional[Any]:
-        # _tmp_208: '=' | ':='
+    def _tmp_219(self) -> Optional[Any]:
+        # _tmp_219: FSTRING_MIDDLE | fstring_replacement_field
+        mark = self._mark()
+        if (
+            (fstring_middle := self.fstring_middle())
+        ):
+            return fstring_middle;
+        self._reset(mark)
+        if (
+            (fstring_replacement_field := self.fstring_replacement_field())
+        ):
+            return fstring_replacement_field;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_220(self) -> Optional[Any]:
+        # _tmp_220: '=' | ':='
         mark = self._mark()
         if (
             (literal := self.expect('='))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect(':='))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_209(self) -> Optional[Any]:
-        # _tmp_209: list | tuple | genexp | 'True' | 'None' | 'False'
+    def _tmp_221(self) -> Optional[Any]:
+        # _tmp_221: list | tuple | genexp | 'True' | 'None' | 'False'
         mark = self._mark()
         if (
             (list := self.list())
         ):
             return list;
         self._reset(mark)
         if (
@@ -12697,113 +13684,113 @@
             (literal := self.expect('False'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_210(self) -> Optional[Any]:
-        # _tmp_210: '=' | ':='
+    def _tmp_222(self) -> Optional[Any]:
+        # _tmp_222: '=' | ':='
         mark = self._mark()
         if (
             (literal := self.expect('='))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect(':='))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_211(self) -> Optional[Any]:
-        # _tmp_211: NUMBER ']'
+    def _tmp_223(self) -> Optional[Any]:
+        # _tmp_223: NUMBER ']'
         mark = self._mark()
         if (
             (number := self.number())
             and
             (literal := self.expect(']'))
         ):
             return [number, literal];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_212(self) -> Optional[Any]:
-        # _tmp_212: 'as' scenic_require_stmt_name
+    def _tmp_224(self) -> Optional[Any]:
+        # _tmp_224: 'as' scenic_require_stmt_name
         mark = self._mark()
         if (
             (literal := self.expect('as'))
             and
             (scenic_require_stmt_name := self.scenic_require_stmt_name())
         ):
             return [literal, scenic_require_stmt_name];
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_213(self) -> Optional[Any]:
-        # _loop0_213: star_named_expressions
+    def _loop0_225(self) -> Optional[Any]:
+        # _loop0_225: star_named_expressions
         mark = self._mark()
         children = []
         while (
             (star_named_expressions := self.star_named_expressions())
         ):
             children.append(star_named_expressions)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_214(self) -> Optional[Any]:
-        # _loop0_214: (star_targets '=')
+    def _loop0_226(self) -> Optional[Any]:
+        # _loop0_226: (star_targets '=')
         mark = self._mark()
         children = []
         while (
-            (_tmp_293 := self._tmp_293())
+            (_tmp_334 := self._tmp_334())
         ):
-            children.append(_tmp_293)
+            children.append(_tmp_334)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_215(self) -> Optional[Any]:
-        # _loop0_215: (star_targets '=')
+    def _loop0_227(self) -> Optional[Any]:
+        # _loop0_227: (star_targets '=')
         mark = self._mark()
         children = []
         while (
-            (_tmp_294 := self._tmp_294())
+            (_tmp_335 := self._tmp_335())
         ):
-            children.append(_tmp_294)
+            children.append(_tmp_335)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_216(self) -> Optional[Any]:
-        # _tmp_216: yield_expr | star_expressions
+    def _tmp_228(self) -> Optional[Any]:
+        # _tmp_228: yield_expr | star_expressions
         mark = self._mark()
         if (
             (yield_expr := self.yield_expr())
         ):
             return yield_expr;
         self._reset(mark)
         if (
             (star_expressions := self.star_expressions())
         ):
             return star_expressions;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_217(self) -> Optional[Any]:
-        # _tmp_217: '[' | '(' | '{'
+    def _tmp_229(self) -> Optional[Any]:
+        # _tmp_229: '[' | '(' | '{'
         mark = self._mark()
         if (
             (literal := self.expect('['))
         ):
             return literal;
         self._reset(mark)
         if (
@@ -12815,266 +13802,266 @@
             (literal := self.expect('{'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_218(self) -> Optional[Any]:
-        # _tmp_218: '[' | '{'
+    def _tmp_230(self) -> Optional[Any]:
+        # _tmp_230: '[' | '{'
         mark = self._mark()
         if (
             (literal := self.expect('['))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect('{'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_219(self) -> Optional[Any]:
-        # _tmp_219: '[' | '{'
+    def _tmp_231(self) -> Optional[Any]:
+        # _tmp_231: '[' | '{'
         mark = self._mark()
         if (
             (literal := self.expect('['))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect('{'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_220(self) -> Optional[Any]:
-        # _loop0_220: param_no_default
+    def _tmp_232(self) -> Optional[Any]:
+        # _tmp_232: slash_no_default | slash_with_default
+        mark = self._mark()
+        if (
+            (slash_no_default := self.slash_no_default())
+        ):
+            return slash_no_default;
+        self._reset(mark)
+        if (
+            (slash_with_default := self.slash_with_default())
+        ):
+            return slash_with_default;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _loop0_233(self) -> Optional[Any]:
+        # _loop0_233: param_maybe_default
         mark = self._mark()
         children = []
         while (
-            (param_no_default := self.param_no_default())
+            (param_maybe_default := self.param_maybe_default())
         ):
-            children.append(param_no_default)
+            children.append(param_maybe_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_221(self) -> Optional[Any]:
-        # _loop0_221: param_no_default
+    def _loop0_234(self) -> Optional[Any]:
+        # _loop0_234: param_no_default
         mark = self._mark()
         children = []
         while (
             (param_no_default := self.param_no_default())
         ):
             children.append(param_no_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_222(self) -> Optional[Any]:
-        # _loop1_222: param_no_default
+    def _loop0_235(self) -> Optional[Any]:
+        # _loop0_235: param_no_default
         mark = self._mark()
         children = []
         while (
             (param_no_default := self.param_no_default())
         ):
             children.append(param_no_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_223(self) -> Optional[Any]:
-        # _tmp_223: slash_no_default | slash_with_default
-        mark = self._mark()
-        if (
-            (slash_no_default := self.slash_no_default())
-        ):
-            return slash_no_default;
-        self._reset(mark)
-        if (
-            (slash_with_default := self.slash_with_default())
-        ):
-            return slash_with_default;
-        self._reset(mark)
-        return None;
-
-    @memoize
-    def _loop0_224(self) -> Optional[Any]:
-        # _loop0_224: param_maybe_default
+    def _loop1_236(self) -> Optional[Any]:
+        # _loop1_236: param_no_default
         mark = self._mark()
         children = []
         while (
-            (param_maybe_default := self.param_maybe_default())
+            (param_no_default := self.param_no_default())
         ):
-            children.append(param_maybe_default)
+            children.append(param_no_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_225(self) -> Optional[Any]:
-        # _tmp_225: slash_no_default | slash_with_default
+    def _tmp_237(self) -> Optional[Any]:
+        # _tmp_237: slash_no_default | slash_with_default
         mark = self._mark()
         if (
             (slash_no_default := self.slash_no_default())
         ):
             return slash_no_default;
         self._reset(mark)
         if (
             (slash_with_default := self.slash_with_default())
         ):
             return slash_with_default;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_226(self) -> Optional[Any]:
-        # _loop0_226: param_maybe_default
+    def _loop0_238(self) -> Optional[Any]:
+        # _loop0_238: param_maybe_default
         mark = self._mark()
         children = []
         while (
             (param_maybe_default := self.param_maybe_default())
         ):
             children.append(param_maybe_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_227(self) -> Optional[Any]:
-        # _tmp_227: ',' | param_no_default
+    def _tmp_239(self) -> Optional[Any]:
+        # _tmp_239: ',' | param_no_default
         mark = self._mark()
         if (
             (literal := self.expect(','))
         ):
             return literal;
         self._reset(mark)
         if (
             (param_no_default := self.param_no_default())
         ):
             return param_no_default;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_228(self) -> Optional[Any]:
-        # _loop0_228: param_maybe_default
+    def _loop0_240(self) -> Optional[Any]:
+        # _loop0_240: param_maybe_default
         mark = self._mark()
         children = []
         while (
             (param_maybe_default := self.param_maybe_default())
         ):
             children.append(param_maybe_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_229(self) -> Optional[Any]:
-        # _loop1_229: param_maybe_default
+    def _loop1_241(self) -> Optional[Any]:
+        # _loop1_241: param_maybe_default
         mark = self._mark()
         children = []
         while (
             (param_maybe_default := self.param_maybe_default())
         ):
             children.append(param_maybe_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_230(self) -> Optional[Any]:
-        # _tmp_230: ')' | ','
+    def _tmp_242(self) -> Optional[Any]:
+        # _tmp_242: ')' | ','
         mark = self._mark()
         if (
             (literal := self.expect(')'))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect(','))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_231(self) -> Optional[Any]:
-        # _tmp_231: ')' | ',' (')' | '**')
+    def _tmp_243(self) -> Optional[Any]:
+        # _tmp_243: ')' | ',' (')' | '**')
         mark = self._mark()
         if (
             (literal := self.expect(')'))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect(','))
             and
-            (_tmp_295 := self._tmp_295())
+            (_tmp_336 := self._tmp_336())
         ):
-            return [literal, _tmp_295];
+            return [literal, _tmp_336];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_232(self) -> Optional[Any]:
-        # _tmp_232: param_no_default | ','
+    def _tmp_244(self) -> Optional[Any]:
+        # _tmp_244: param_no_default | ','
         mark = self._mark()
         if (
             (param_no_default := self.param_no_default())
         ):
             return param_no_default;
         self._reset(mark)
         if (
             (literal := self.expect(','))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_233(self) -> Optional[Any]:
-        # _loop0_233: param_maybe_default
+    def _loop0_245(self) -> Optional[Any]:
+        # _loop0_245: param_maybe_default
         mark = self._mark()
         children = []
         while (
             (param_maybe_default := self.param_maybe_default())
         ):
             children.append(param_maybe_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_234(self) -> Optional[Any]:
-        # _tmp_234: param_no_default | ','
+    def _tmp_246(self) -> Optional[Any]:
+        # _tmp_246: param_no_default | ','
         mark = self._mark()
         if (
             (param_no_default := self.param_no_default())
         ):
             return param_no_default;
         self._reset(mark)
         if (
             (literal := self.expect(','))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_235(self) -> Optional[Any]:
-        # _tmp_235: '*' | '**' | '/'
+    def _tmp_247(self) -> Optional[Any]:
+        # _tmp_247: '*' | '**' | '/'
         mark = self._mark()
         if (
             (literal := self.expect('*'))
         ):
             return literal;
         self._reset(mark)
         if (
@@ -13086,261 +14073,261 @@
             (literal := self.expect('/'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop1_236(self) -> Optional[Any]:
-        # _loop1_236: param_with_default
+    def _loop1_248(self) -> Optional[Any]:
+        # _loop1_248: param_with_default
         mark = self._mark()
         children = []
         while (
             (param_with_default := self.param_with_default())
         ):
             children.append(param_with_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_237(self) -> Optional[Any]:
-        # _loop0_237: lambda_param_no_default
+    def _tmp_249(self) -> Optional[Any]:
+        # _tmp_249: lambda_slash_no_default | lambda_slash_with_default
+        mark = self._mark()
+        if (
+            (lambda_slash_no_default := self.lambda_slash_no_default())
+        ):
+            return lambda_slash_no_default;
+        self._reset(mark)
+        if (
+            (lambda_slash_with_default := self.lambda_slash_with_default())
+        ):
+            return lambda_slash_with_default;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _loop0_250(self) -> Optional[Any]:
+        # _loop0_250: lambda_param_maybe_default
+        mark = self._mark()
+        children = []
+        while (
+            (lambda_param_maybe_default := self.lambda_param_maybe_default())
+        ):
+            children.append(lambda_param_maybe_default)
+            mark = self._mark()
+        self._reset(mark)
+        return children;
+
+    @memoize
+    def _loop0_251(self) -> Optional[Any]:
+        # _loop0_251: lambda_param_no_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_no_default := self.lambda_param_no_default())
         ):
             children.append(lambda_param_no_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_238(self) -> Optional[Any]:
-        # _loop0_238: lambda_param_no_default
+    def _loop0_252(self) -> Optional[Any]:
+        # _loop0_252: lambda_param_no_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_no_default := self.lambda_param_no_default())
         ):
             children.append(lambda_param_no_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop0_240(self) -> Optional[Any]:
-        # _loop0_240: ',' lambda_param
+    def _loop0_254(self) -> Optional[Any]:
+        # _loop0_254: ',' lambda_param
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.lambda_param())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_239(self) -> Optional[Any]:
-        # _gather_239: lambda_param _loop0_240
+    def _gather_253(self) -> Optional[Any]:
+        # _gather_253: lambda_param _loop0_254
         mark = self._mark()
         if (
             (elem := self.lambda_param())
             is not None
             and
-            (seq := self._loop0_240())
+            (seq := self._loop0_254())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_241(self) -> Optional[Any]:
-        # _tmp_241: lambda_slash_no_default | lambda_slash_with_default
+    def _tmp_255(self) -> Optional[Any]:
+        # _tmp_255: lambda_slash_no_default | lambda_slash_with_default
         mark = self._mark()
         if (
             (lambda_slash_no_default := self.lambda_slash_no_default())
         ):
             return lambda_slash_no_default;
         self._reset(mark)
         if (
             (lambda_slash_with_default := self.lambda_slash_with_default())
         ):
             return lambda_slash_with_default;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_242(self) -> Optional[Any]:
-        # _loop0_242: lambda_param_maybe_default
-        mark = self._mark()
-        children = []
-        while (
-            (lambda_param_maybe_default := self.lambda_param_maybe_default())
-        ):
-            children.append(lambda_param_maybe_default)
-            mark = self._mark()
-        self._reset(mark)
-        return children;
-
-    @memoize
-    def _tmp_243(self) -> Optional[Any]:
-        # _tmp_243: lambda_slash_no_default | lambda_slash_with_default
-        mark = self._mark()
-        if (
-            (lambda_slash_no_default := self.lambda_slash_no_default())
-        ):
-            return lambda_slash_no_default;
-        self._reset(mark)
-        if (
-            (lambda_slash_with_default := self.lambda_slash_with_default())
-        ):
-            return lambda_slash_with_default;
-        self._reset(mark)
-        return None;
-
-    @memoize
-    def _loop0_244(self) -> Optional[Any]:
-        # _loop0_244: lambda_param_maybe_default
+    def _loop0_256(self) -> Optional[Any]:
+        # _loop0_256: lambda_param_maybe_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_maybe_default := self.lambda_param_maybe_default())
         ):
             children.append(lambda_param_maybe_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_245(self) -> Optional[Any]:
-        # _tmp_245: ',' | lambda_param_no_default
+    def _tmp_257(self) -> Optional[Any]:
+        # _tmp_257: ',' | lambda_param_no_default
         mark = self._mark()
         if (
             (literal := self.expect(','))
         ):
             return literal;
         self._reset(mark)
         if (
             (lambda_param_no_default := self.lambda_param_no_default())
         ):
             return lambda_param_no_default;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_246(self) -> Optional[Any]:
-        # _loop0_246: lambda_param_maybe_default
+    def _loop0_258(self) -> Optional[Any]:
+        # _loop0_258: lambda_param_maybe_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_maybe_default := self.lambda_param_maybe_default())
         ):
             children.append(lambda_param_maybe_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_247(self) -> Optional[Any]:
-        # _loop1_247: lambda_param_maybe_default
+    def _loop1_259(self) -> Optional[Any]:
+        # _loop1_259: lambda_param_maybe_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_maybe_default := self.lambda_param_maybe_default())
         ):
             children.append(lambda_param_maybe_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _loop1_248(self) -> Optional[Any]:
-        # _loop1_248: lambda_param_with_default
+    def _loop1_260(self) -> Optional[Any]:
+        # _loop1_260: lambda_param_with_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_with_default := self.lambda_param_with_default())
         ):
             children.append(lambda_param_with_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_249(self) -> Optional[Any]:
-        # _tmp_249: ':' | ',' (':' | '**')
+    def _tmp_261(self) -> Optional[Any]:
+        # _tmp_261: ':' | ',' (':' | '**')
         mark = self._mark()
         if (
             (literal := self.expect(':'))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect(','))
             and
-            (_tmp_296 := self._tmp_296())
+            (_tmp_337 := self._tmp_337())
         ):
-            return [literal, _tmp_296];
+            return [literal, _tmp_337];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_250(self) -> Optional[Any]:
-        # _tmp_250: lambda_param_no_default | ','
+    def _tmp_262(self) -> Optional[Any]:
+        # _tmp_262: lambda_param_no_default | ','
         mark = self._mark()
         if (
             (lambda_param_no_default := self.lambda_param_no_default())
         ):
             return lambda_param_no_default;
         self._reset(mark)
         if (
             (literal := self.expect(','))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_251(self) -> Optional[Any]:
-        # _loop0_251: lambda_param_maybe_default
+    def _loop0_263(self) -> Optional[Any]:
+        # _loop0_263: lambda_param_maybe_default
         mark = self._mark()
         children = []
         while (
             (lambda_param_maybe_default := self.lambda_param_maybe_default())
         ):
             children.append(lambda_param_maybe_default)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _tmp_252(self) -> Optional[Any]:
-        # _tmp_252: lambda_param_no_default | ','
+    def _tmp_264(self) -> Optional[Any]:
+        # _tmp_264: lambda_param_no_default | ','
         mark = self._mark()
         if (
             (lambda_param_no_default := self.lambda_param_no_default())
         ):
             return lambda_param_no_default;
         self._reset(mark)
         if (
             (literal := self.expect(','))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_253(self) -> Optional[Any]:
-        # _tmp_253: '*' | '**' | '/'
+    def _tmp_265(self) -> Optional[Any]:
+        # _tmp_265: '*' | '**' | '/'
         mark = self._mark()
         if (
             (literal := self.expect('*'))
         ):
             return literal;
         self._reset(mark)
         if (
@@ -13352,16 +14339,16 @@
             (literal := self.expect('/'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_254(self) -> Optional[Any]:
-        # _tmp_254: ',' | ')' | ':'
+    def _tmp_266(self) -> Optional[Any]:
+        # _tmp_266: ',' | ')' | ':'
         mark = self._mark()
         if (
             (literal := self.expect(','))
         ):
             return literal;
         self._reset(mark)
         if (
@@ -13373,715 +14360,1171 @@
             (literal := self.expect(':'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_256(self) -> Optional[Any]:
-        # _loop0_256: ',' (expression ['as' star_target])
+    def _loop0_268(self) -> Optional[Any]:
+        # _loop0_268: ',' dotted_name
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
-            (elem := self._tmp_297())
+            (elem := self.dotted_name())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_255(self) -> Optional[Any]:
-        # _gather_255: (expression ['as' star_target]) _loop0_256
+    def _gather_267(self) -> Optional[Any]:
+        # _gather_267: dotted_name _loop0_268
         mark = self._mark()
         if (
-            (elem := self._tmp_297())
+            (elem := self.dotted_name())
             is not None
             and
-            (seq := self._loop0_256())
+            (seq := self._loop0_268())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_258(self) -> Optional[Any]:
-        # _loop0_258: ',' (expressions ['as' star_target])
+    def _loop0_270(self) -> Optional[Any]:
+        # _loop0_270: ',' (expression ['as' star_target])
+        mark = self._mark()
+        children = []
+        while (
+            (self.expect(','))
+            and
+            (elem := self._tmp_338())
+        ):
+            children.append(elem)
+            mark = self._mark()
+        self._reset(mark)
+        return children;
+
+    @memoize
+    def _gather_269(self) -> Optional[Any]:
+        # _gather_269: (expression ['as' star_target]) _loop0_270
+        mark = self._mark()
+        if (
+            (elem := self._tmp_338())
+            is not None
+            and
+            (seq := self._loop0_270())
+            is not None
+        ):
+            return [elem] + seq;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _loop0_272(self) -> Optional[Any]:
+        # _loop0_272: ',' (expressions ['as' star_target])
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
-            (elem := self._tmp_298())
+            (elem := self._tmp_339())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_257(self) -> Optional[Any]:
-        # _gather_257: (expressions ['as' star_target]) _loop0_258
+    def _gather_271(self) -> Optional[Any]:
+        # _gather_271: (expressions ['as' star_target]) _loop0_272
         mark = self._mark()
         if (
-            (elem := self._tmp_298())
+            (elem := self._tmp_339())
             is not None
             and
-            (seq := self._loop0_258())
+            (seq := self._loop0_272())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_260(self) -> Optional[Any]:
-        # _loop0_260: ',' (expression ['as' star_target])
+    def _loop0_274(self) -> Optional[Any]:
+        # _loop0_274: ',' (expression ['as' star_target])
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
-            (elem := self._tmp_299())
+            (elem := self._tmp_340())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_259(self) -> Optional[Any]:
-        # _gather_259: (expression ['as' star_target]) _loop0_260
+    def _gather_273(self) -> Optional[Any]:
+        # _gather_273: (expression ['as' star_target]) _loop0_274
         mark = self._mark()
         if (
-            (elem := self._tmp_299())
+            (elem := self._tmp_340())
             is not None
             and
-            (seq := self._loop0_260())
+            (seq := self._loop0_274())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_262(self) -> Optional[Any]:
-        # _loop0_262: ',' (expressions ['as' star_target])
+    def _loop0_276(self) -> Optional[Any]:
+        # _loop0_276: ',' (expressions ['as' star_target])
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
-            (elem := self._tmp_300())
+            (elem := self._tmp_341())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_261(self) -> Optional[Any]:
-        # _gather_261: (expressions ['as' star_target]) _loop0_262
+    def _gather_275(self) -> Optional[Any]:
+        # _gather_275: (expressions ['as' star_target]) _loop0_276
         mark = self._mark()
         if (
-            (elem := self._tmp_300())
+            (elem := self._tmp_341())
             is not None
             and
-            (seq := self._loop0_262())
+            (seq := self._loop0_276())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_263(self) -> Optional[Any]:
-        # _tmp_263: 'except' | 'finally'
+    def _tmp_277(self) -> Optional[Any]:
+        # _tmp_277: 'except' | 'finally'
         mark = self._mark()
         if (
             (literal := self.expect('except'))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect('finally'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_264(self) -> Optional[Any]:
-        # _tmp_264: 'as' NAME
+    def _loop0_278(self) -> Optional[Any]:
+        # _loop0_278: block
+        mark = self._mark()
+        children = []
+        while (
+            (block := self.block())
+        ):
+            children.append(block)
+            mark = self._mark()
+        self._reset(mark)
+        return children;
+
+    @memoize
+    def _loop1_279(self) -> Optional[Any]:
+        # _loop1_279: except_block
+        mark = self._mark()
+        children = []
+        while (
+            (except_block := self.except_block())
+        ):
+            children.append(except_block)
+            mark = self._mark()
+        self._reset(mark)
+        return children;
+
+    @memoize
+    def _tmp_280(self) -> Optional[Any]:
+        # _tmp_280: 'as' NAME
         mark = self._mark()
         if (
             (literal := self.expect('as'))
             and
             (name := self.name())
         ):
             return [literal, name];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_265(self) -> Optional[Any]:
-        # _tmp_265: 'as' NAME
+    def _loop0_281(self) -> Optional[Any]:
+        # _loop0_281: block
+        mark = self._mark()
+        children = []
+        while (
+            (block := self.block())
+        ):
+            children.append(block)
+            mark = self._mark()
+        self._reset(mark)
+        return children;
+
+    @memoize
+    def _loop1_282(self) -> Optional[Any]:
+        # _loop1_282: except_star_block
+        mark = self._mark()
+        children = []
+        while (
+            (except_star_block := self.except_star_block())
+        ):
+            children.append(except_star_block)
+            mark = self._mark()
+        self._reset(mark)
+        return children;
+
+    @memoize
+    def _tmp_283(self) -> Optional[Any]:
+        # _tmp_283: expression ['as' NAME]
+        mark = self._mark()
+        if (
+            (expression := self.expression())
+            and
+            (opt := self._tmp_342(),)
+        ):
+            return [expression, opt];
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_284(self) -> Optional[Any]:
+        # _tmp_284: 'as' NAME
         mark = self._mark()
         if (
             (literal := self.expect('as'))
             and
             (name := self.name())
         ):
             return [literal, name];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_266(self) -> Optional[Any]:
-        # _tmp_266: 'as' NAME
+    def _tmp_285(self) -> Optional[Any]:
+        # _tmp_285: 'as' NAME
+        mark = self._mark()
+        if (
+            (literal := self.expect('as'))
+            and
+            (name := self.name())
+        ):
+            return [literal, name];
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_286(self) -> Optional[Any]:
+        # _tmp_286: NEWLINE | ':'
+        mark = self._mark()
+        if (
+            (_newline := self.expect('NEWLINE'))
+        ):
+            return _newline;
+        self._reset(mark)
+        if (
+            (literal := self.expect(':'))
+        ):
+            return literal;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_287(self) -> Optional[Any]:
+        # _tmp_287: 'as' NAME
         mark = self._mark()
         if (
             (literal := self.expect('as'))
             and
             (name := self.name())
         ):
             return [literal, name];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_267(self) -> Optional[Any]:
-        # _tmp_267: positional_patterns ','
+    def _tmp_288(self) -> Optional[Any]:
+        # _tmp_288: 'as' NAME
+        mark = self._mark()
+        if (
+            (literal := self.expect('as'))
+            and
+            (name := self.name())
+        ):
+            return [literal, name];
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_289(self) -> Optional[Any]:
+        # _tmp_289: positional_patterns ','
         mark = self._mark()
         if (
             (positional_patterns := self.positional_patterns())
             and
             (literal := self.expect(','))
         ):
             return [positional_patterns, literal];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_268(self) -> Optional[Any]:
-        # _tmp_268: '->' expression
+    def _tmp_290(self) -> Optional[Any]:
+        # _tmp_290: '->' expression
         mark = self._mark()
         if (
             (literal := self.expect('->'))
             and
             (expression := self.expression())
         ):
             return [literal, expression];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_269(self) -> Optional[Any]:
-        # _tmp_269: '(' arguments? ')'
+    def _tmp_291(self) -> Optional[Any]:
+        # _tmp_291: '(' arguments? ')'
+        mark = self._mark()
+        if (
+            (literal := self.expect('('))
+            and
+            (opt := self.arguments(),)
+            and
+            (literal_1 := self.expect(')'))
+        ):
+            return [literal, opt, literal_1];
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_292(self) -> Optional[Any]:
+        # _tmp_292: '(' arguments? ')'
         mark = self._mark()
         if (
             (literal := self.expect('('))
             and
             (opt := self.arguments(),)
             and
             (literal_1 := self.expect(')'))
         ):
             return [literal, opt, literal_1];
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_271(self) -> Optional[Any]:
-        # _loop0_271: ',' double_starred_kvpair
+    def _loop0_294(self) -> Optional[Any]:
+        # _loop0_294: ',' double_starred_kvpair
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.double_starred_kvpair())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_270(self) -> Optional[Any]:
-        # _gather_270: double_starred_kvpair _loop0_271
+    def _gather_293(self) -> Optional[Any]:
+        # _gather_293: double_starred_kvpair _loop0_294
         mark = self._mark()
         if (
             (elem := self.double_starred_kvpair())
             is not None
             and
-            (seq := self._loop0_271())
+            (seq := self._loop0_294())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_272(self) -> Optional[Any]:
-        # _tmp_272: '}' | ','
+    def _tmp_295(self) -> Optional[Any]:
+        # _tmp_295: '}' | ','
         mark = self._mark()
         if (
             (literal := self.expect('}'))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect(','))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_273(self) -> Optional[Any]:
-        # _tmp_273: star_targets '='
+    def _tmp_296(self) -> Optional[Any]:
+        # _tmp_296: '}' | ','
+        mark = self._mark()
+        if (
+            (literal := self.expect('}'))
+        ):
+            return literal;
+        self._reset(mark)
+        if (
+            (literal := self.expect(','))
+        ):
+            return literal;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_297(self) -> Optional[Any]:
+        # _tmp_297: yield_expr | star_expressions
+        mark = self._mark()
+        if (
+            (yield_expr := self.yield_expr())
+        ):
+            return yield_expr;
+        self._reset(mark)
+        if (
+            (star_expressions := self.star_expressions())
+        ):
+            return star_expressions;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_298(self) -> Optional[Any]:
+        # _tmp_298: yield_expr | star_expressions
+        mark = self._mark()
+        if (
+            (yield_expr := self.yield_expr())
+        ):
+            return yield_expr;
+        self._reset(mark)
+        if (
+            (star_expressions := self.star_expressions())
+        ):
+            return star_expressions;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_299(self) -> Optional[Any]:
+        # _tmp_299: '=' | '!' | ':' | '}'
+        mark = self._mark()
+        if (
+            (literal := self.expect('='))
+        ):
+            return literal;
+        self._reset(mark)
+        if (
+            (literal := self.expect('!'))
+        ):
+            return literal;
+        self._reset(mark)
+        if (
+            (literal := self.expect(':'))
+        ):
+            return literal;
+        self._reset(mark)
+        if (
+            (literal := self.expect('}'))
+        ):
+            return literal;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_300(self) -> Optional[Any]:
+        # _tmp_300: yield_expr | star_expressions
+        mark = self._mark()
+        if (
+            (yield_expr := self.yield_expr())
+        ):
+            return yield_expr;
+        self._reset(mark)
+        if (
+            (star_expressions := self.star_expressions())
+        ):
+            return star_expressions;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_301(self) -> Optional[Any]:
+        # _tmp_301: '!' | ':' | '}'
+        mark = self._mark()
+        if (
+            (literal := self.expect('!'))
+        ):
+            return literal;
+        self._reset(mark)
+        if (
+            (literal := self.expect(':'))
+        ):
+            return literal;
+        self._reset(mark)
+        if (
+            (literal := self.expect('}'))
+        ):
+            return literal;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_302(self) -> Optional[Any]:
+        # _tmp_302: yield_expr | star_expressions
+        mark = self._mark()
+        if (
+            (yield_expr := self.yield_expr())
+        ):
+            return yield_expr;
+        self._reset(mark)
+        if (
+            (star_expressions := self.star_expressions())
+        ):
+            return star_expressions;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_303(self) -> Optional[Any]:
+        # _tmp_303: yield_expr | star_expressions
+        mark = self._mark()
+        if (
+            (yield_expr := self.yield_expr())
+        ):
+            return yield_expr;
+        self._reset(mark)
+        if (
+            (star_expressions := self.star_expressions())
+        ):
+            return star_expressions;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_304(self) -> Optional[Any]:
+        # _tmp_304: '!' NAME
+        mark = self._mark()
+        if (
+            (literal := self.expect('!'))
+            and
+            (name := self.name())
+        ):
+            return [literal, name];
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_305(self) -> Optional[Any]:
+        # _tmp_305: ':' | '}'
+        mark = self._mark()
+        if (
+            (literal := self.expect(':'))
+        ):
+            return literal;
+        self._reset(mark)
+        if (
+            (literal := self.expect('}'))
+        ):
+            return literal;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_306(self) -> Optional[Any]:
+        # _tmp_306: yield_expr | star_expressions
+        mark = self._mark()
+        if (
+            (yield_expr := self.yield_expr())
+        ):
+            return yield_expr;
+        self._reset(mark)
+        if (
+            (star_expressions := self.star_expressions())
+        ):
+            return star_expressions;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_307(self) -> Optional[Any]:
+        # _tmp_307: '!' NAME
+        mark = self._mark()
+        if (
+            (literal := self.expect('!'))
+            and
+            (name := self.name())
+        ):
+            return [literal, name];
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _loop0_308(self) -> Optional[Any]:
+        # _loop0_308: fstring_format_spec
+        mark = self._mark()
+        children = []
+        while (
+            (fstring_format_spec := self.fstring_format_spec())
+        ):
+            children.append(fstring_format_spec)
+            mark = self._mark()
+        self._reset(mark)
+        return children;
+
+    @memoize
+    def _tmp_309(self) -> Optional[Any]:
+        # _tmp_309: yield_expr | star_expressions
+        mark = self._mark()
+        if (
+            (yield_expr := self.yield_expr())
+        ):
+            return yield_expr;
+        self._reset(mark)
+        if (
+            (star_expressions := self.star_expressions())
+        ):
+            return star_expressions;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_310(self) -> Optional[Any]:
+        # _tmp_310: '!' NAME
+        mark = self._mark()
+        if (
+            (literal := self.expect('!'))
+            and
+            (name := self.name())
+        ):
+            return [literal, name];
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_311(self) -> Optional[Any]:
+        # _tmp_311: ':' | '}'
+        mark = self._mark()
+        if (
+            (literal := self.expect(':'))
+        ):
+            return literal;
+        self._reset(mark)
+        if (
+            (literal := self.expect('}'))
+        ):
+            return literal;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_312(self) -> Optional[Any]:
+        # _tmp_312: star_targets '='
         mark = self._mark()
         if (
             (z := self.star_targets())
             and
             (self.expect('='))
         ):
             return z;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_274(self) -> Optional[Any]:
-        # _tmp_274: '.' | '...'
+    def _tmp_313(self) -> Optional[Any]:
+        # _tmp_313: '.' | '...'
         mark = self._mark()
         if (
             (literal := self.expect('.'))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect('...'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_275(self) -> Optional[Any]:
-        # _tmp_275: '.' | '...'
+    def _tmp_314(self) -> Optional[Any]:
+        # _tmp_314: '.' | '...'
         mark = self._mark()
         if (
             (literal := self.expect('.'))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect('...'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _loop0_277(self) -> Optional[Any]:
-        # _loop0_277: ',' scenic_class_property_attribute
+    def _loop0_316(self) -> Optional[Any]:
+        # _loop0_316: ',' scenic_class_property_attribute
         mark = self._mark()
         children = []
         while (
             (self.expect(','))
             and
             (elem := self.scenic_class_property_attribute())
         ):
             children.append(elem)
             mark = self._mark()
         self._reset(mark)
         return children;
 
     @memoize
-    def _gather_276(self) -> Optional[Any]:
-        # _gather_276: scenic_class_property_attribute _loop0_277
+    def _gather_315(self) -> Optional[Any]:
+        # _gather_315: scenic_class_property_attribute _loop0_316
         mark = self._mark()
         if (
             (elem := self.scenic_class_property_attribute())
             is not None
             and
-            (seq := self._loop0_277())
+            (seq := self._loop0_316())
             is not None
         ):
             return [elem] + seq;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_278(self) -> Optional[Any]:
-        # _tmp_278: star_targets '='
+    def _tmp_317(self) -> Optional[Any]:
+        # _tmp_317: star_targets '='
         mark = self._mark()
         if (
             (z := self.star_targets())
             and
             (self.expect('='))
         ):
             return z;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_279(self) -> Optional[Any]:
-        # _tmp_279: scenic_specifiers ',' NEWLINE
+    def _tmp_318(self) -> Optional[Any]:
+        # _tmp_318: scenic_specifiers ',' NEWLINE
         mark = self._mark()
         if (
             (x := self.scenic_specifiers())
             and
             (self.expect(','))
             and
             (self.expect('NEWLINE'))
         ):
             return x;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_280(self) -> Optional[Any]:
-        # _tmp_280: scenic_specifiers ',' NEWLINE
+    def _tmp_319(self) -> Optional[Any]:
+        # _tmp_319: scenic_specifiers ',' NEWLINE
         mark = self._mark()
         if (
             (x := self.scenic_specifiers())
             and
             (self.expect(','))
             and
             (self.expect('NEWLINE'))
         ):
             return x;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_281(self) -> Optional[Any]:
-        # _tmp_281: (scenic_precondition_stmt | scenic_invariant_stmt) NEWLINE
+    def _tmp_320(self) -> Optional[Any]:
+        # _tmp_320: (scenic_precondition_stmt | scenic_invariant_stmt) NEWLINE
         mark = self._mark()
         if (
-            (x := self._tmp_301())
+            (x := self._tmp_343())
             and
             (self.expect('NEWLINE'))
         ):
             return x;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_282(self) -> Optional[Any]:
-        # _tmp_282: ',' expression
+    def _tmp_321(self) -> Optional[Any]:
+        # _tmp_321: ',' expression
         mark = self._mark()
         if (
             (self.expect(','))
             and
             (c := self.expression())
         ):
             return c;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_283(self) -> Optional[Any]:
-        # _tmp_283: ',' star_expression
+    def _tmp_322(self) -> Optional[Any]:
+        # _tmp_322: ',' star_expression
         mark = self._mark()
         if (
             (self.expect(','))
             and
             (c := self.star_expression())
         ):
             return c;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_284(self) -> Optional[Any]:
-        # _tmp_284: 'or' conjunction
+    def _tmp_323(self) -> Optional[Any]:
+        # _tmp_323: 'or' conjunction
         mark = self._mark()
         if (
             (self.expect('or'))
             and
             (c := self.conjunction())
         ):
             return c;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_285(self) -> Optional[Any]:
-        # _tmp_285: 'or' (scenic_temporal_prefix | scenic_temporal_conjunction)
+    def _tmp_324(self) -> Optional[Any]:
+        # _tmp_324: 'or' (scenic_temporal_prefix | scenic_temporal_conjunction)
         mark = self._mark()
         if (
             (self.expect('or'))
             and
-            (c := self._tmp_302())
+            (c := self._tmp_344())
         ):
             return c;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_286(self) -> Optional[Any]:
-        # _tmp_286: 'and' inversion
+    def _tmp_325(self) -> Optional[Any]:
+        # _tmp_325: 'and' inversion
         mark = self._mark()
         if (
             (self.expect('and'))
             and
             (c := self.inversion())
         ):
             return c;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_287(self) -> Optional[Any]:
-        # _tmp_287: 'and' (scenic_temporal_prefix | scenic_temporal_inversion)
+    def _tmp_326(self) -> Optional[Any]:
+        # _tmp_326: 'and' (scenic_temporal_prefix | scenic_temporal_inversion)
         mark = self._mark()
         if (
             (self.expect('and'))
             and
-            (c := self._tmp_303())
+            (c := self._tmp_345())
         ):
             return c;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_288(self) -> Optional[Any]:
-        # _tmp_288: 'if' disjunction
+    def _tmp_327(self) -> Optional[Any]:
+        # _tmp_327: slice | starred_expression
+        mark = self._mark()
+        if (
+            (slice := self.slice())
+        ):
+            return slice;
+        self._reset(mark)
+        if (
+            (starred_expression := self.starred_expression())
+        ):
+            return starred_expression;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_328(self) -> Optional[Any]:
+        # _tmp_328: fstring | STRING
+        mark = self._mark()
+        if (
+            (fstring := self.fstring())
+        ):
+            return fstring;
+        self._reset(mark)
+        if (
+            (string := self.string())
+        ):
+            return string;
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_329(self) -> Optional[Any]:
+        # _tmp_329: 'if' disjunction
         mark = self._mark()
         if (
             (self.expect('if'))
             and
             (z := self.disjunction())
         ):
             return z;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_289(self) -> Optional[Any]:
-        # _tmp_289: 'if' disjunction
+    def _tmp_330(self) -> Optional[Any]:
+        # _tmp_330: 'if' disjunction
         mark = self._mark()
         if (
             (self.expect('if'))
             and
             (z := self.disjunction())
         ):
             return z;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_290(self) -> Optional[Any]:
-        # _tmp_290: starred_expression | (assignment_expression | expression !':=') !'='
+    def _tmp_331(self) -> Optional[Any]:
+        # _tmp_331: starred_expression | (assignment_expression | expression !':=') !'='
         mark = self._mark()
         if (
             (starred_expression := self.starred_expression())
         ):
             return starred_expression;
         self._reset(mark)
         if (
-            (_tmp_304 := self._tmp_304())
+            (_tmp_346 := self._tmp_346())
             and
             (self.negative_lookahead(self.expect, '='))
         ):
-            return _tmp_304;
+            return _tmp_346;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_291(self) -> Optional[Any]:
-        # _tmp_291: ',' star_target
+    def _tmp_332(self) -> Optional[Any]:
+        # _tmp_332: ',' star_target
         mark = self._mark()
         if (
             (self.expect(','))
             and
             (c := self.star_target())
         ):
             return c;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_292(self) -> Optional[Any]:
-        # _tmp_292: ',' star_target
+    def _tmp_333(self) -> Optional[Any]:
+        # _tmp_333: ',' star_target
         mark = self._mark()
         if (
             (self.expect(','))
             and
             (c := self.star_target())
         ):
             return c;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_293(self) -> Optional[Any]:
-        # _tmp_293: star_targets '='
+    def _tmp_334(self) -> Optional[Any]:
+        # _tmp_334: star_targets '='
         mark = self._mark()
         if (
             (star_targets := self.star_targets())
             and
             (literal := self.expect('='))
         ):
             return [star_targets, literal];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_294(self) -> Optional[Any]:
-        # _tmp_294: star_targets '='
+    def _tmp_335(self) -> Optional[Any]:
+        # _tmp_335: star_targets '='
         mark = self._mark()
         if (
             (star_targets := self.star_targets())
             and
             (literal := self.expect('='))
         ):
             return [star_targets, literal];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_295(self) -> Optional[Any]:
-        # _tmp_295: ')' | '**'
+    def _tmp_336(self) -> Optional[Any]:
+        # _tmp_336: ')' | '**'
         mark = self._mark()
         if (
             (literal := self.expect(')'))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect('**'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_296(self) -> Optional[Any]:
-        # _tmp_296: ':' | '**'
+    def _tmp_337(self) -> Optional[Any]:
+        # _tmp_337: ':' | '**'
         mark = self._mark()
         if (
             (literal := self.expect(':'))
         ):
             return literal;
         self._reset(mark)
         if (
             (literal := self.expect('**'))
         ):
             return literal;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_297(self) -> Optional[Any]:
-        # _tmp_297: expression ['as' star_target]
+    def _tmp_338(self) -> Optional[Any]:
+        # _tmp_338: expression ['as' star_target]
         mark = self._mark()
         if (
             (expression := self.expression())
             and
-            (opt := self._tmp_305(),)
+            (opt := self._tmp_347(),)
         ):
             return [expression, opt];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_298(self) -> Optional[Any]:
-        # _tmp_298: expressions ['as' star_target]
+    def _tmp_339(self) -> Optional[Any]:
+        # _tmp_339: expressions ['as' star_target]
         mark = self._mark()
         if (
             (expressions := self.expressions())
             and
-            (opt := self._tmp_306(),)
+            (opt := self._tmp_348(),)
         ):
             return [expressions, opt];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_299(self) -> Optional[Any]:
-        # _tmp_299: expression ['as' star_target]
+    def _tmp_340(self) -> Optional[Any]:
+        # _tmp_340: expression ['as' star_target]
         mark = self._mark()
         if (
             (expression := self.expression())
             and
-            (opt := self._tmp_307(),)
+            (opt := self._tmp_349(),)
         ):
             return [expression, opt];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_300(self) -> Optional[Any]:
-        # _tmp_300: expressions ['as' star_target]
+    def _tmp_341(self) -> Optional[Any]:
+        # _tmp_341: expressions ['as' star_target]
         mark = self._mark()
         if (
             (expressions := self.expressions())
             and
-            (opt := self._tmp_308(),)
+            (opt := self._tmp_350(),)
         ):
             return [expressions, opt];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_301(self) -> Optional[Any]:
-        # _tmp_301: scenic_precondition_stmt | scenic_invariant_stmt
+    def _tmp_342(self) -> Optional[Any]:
+        # _tmp_342: 'as' NAME
+        mark = self._mark()
+        if (
+            (literal := self.expect('as'))
+            and
+            (name := self.name())
+        ):
+            return [literal, name];
+        self._reset(mark)
+        return None;
+
+    @memoize
+    def _tmp_343(self) -> Optional[Any]:
+        # _tmp_343: scenic_precondition_stmt | scenic_invariant_stmt
         mark = self._mark()
         if (
             (scenic_precondition_stmt := self.scenic_precondition_stmt())
         ):
             return scenic_precondition_stmt;
         self._reset(mark)
         if (
             (scenic_invariant_stmt := self.scenic_invariant_stmt())
         ):
             return scenic_invariant_stmt;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_302(self) -> Optional[Any]:
-        # _tmp_302: scenic_temporal_prefix | scenic_temporal_conjunction
+    def _tmp_344(self) -> Optional[Any]:
+        # _tmp_344: scenic_temporal_prefix | scenic_temporal_conjunction
         mark = self._mark()
         if (
             (scenic_temporal_prefix := self.scenic_temporal_prefix())
         ):
             return scenic_temporal_prefix;
         self._reset(mark)
         if (
             (scenic_temporal_conjunction := self.scenic_temporal_conjunction())
         ):
             return scenic_temporal_conjunction;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_303(self) -> Optional[Any]:
-        # _tmp_303: scenic_temporal_prefix | scenic_temporal_inversion
+    def _tmp_345(self) -> Optional[Any]:
+        # _tmp_345: scenic_temporal_prefix | scenic_temporal_inversion
         mark = self._mark()
         if (
             (scenic_temporal_prefix := self.scenic_temporal_prefix())
         ):
             return scenic_temporal_prefix;
         self._reset(mark)
         if (
             (scenic_temporal_inversion := self.scenic_temporal_inversion())
         ):
             return scenic_temporal_inversion;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_304(self) -> Optional[Any]:
-        # _tmp_304: assignment_expression | expression !':='
+    def _tmp_346(self) -> Optional[Any]:
+        # _tmp_346: assignment_expression | expression !':='
         mark = self._mark()
         if (
             (assignment_expression := self.assignment_expression())
         ):
             return assignment_expression;
         self._reset(mark)
         if (
@@ -14090,65 +15533,65 @@
             (self.negative_lookahead(self.expect, ':='))
         ):
             return expression;
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_305(self) -> Optional[Any]:
-        # _tmp_305: 'as' star_target
+    def _tmp_347(self) -> Optional[Any]:
+        # _tmp_347: 'as' star_target
         mark = self._mark()
         if (
             (literal := self.expect('as'))
             and
             (star_target := self.star_target())
         ):
             return [literal, star_target];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_306(self) -> Optional[Any]:
-        # _tmp_306: 'as' star_target
+    def _tmp_348(self) -> Optional[Any]:
+        # _tmp_348: 'as' star_target
         mark = self._mark()
         if (
             (literal := self.expect('as'))
             and
             (star_target := self.star_target())
         ):
             return [literal, star_target];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_307(self) -> Optional[Any]:
-        # _tmp_307: 'as' star_target
+    def _tmp_349(self) -> Optional[Any]:
+        # _tmp_349: 'as' star_target
         mark = self._mark()
         if (
             (literal := self.expect('as'))
             and
             (star_target := self.star_target())
         ):
             return [literal, star_target];
         self._reset(mark)
         return None;
 
     @memoize
-    def _tmp_308(self) -> Optional[Any]:
-        # _tmp_308: 'as' star_target
+    def _tmp_350(self) -> Optional[Any]:
+        # _tmp_350: 'as' star_target
         mark = self._mark()
         if (
             (literal := self.expect('as'))
             and
             (star_target := self.star_target())
         ):
             return [literal, star_target];
         self._reset(mark)
         return None;
 
     KEYWORDS = ('False', 'None', 'True', 'and', 'as', 'assert', 'async', 'at', 'await', 'break', 'by', 'class', 'continue', 'def', 'del', 'do', 'elif', 'else', 'except', 'finally', 'for', 'from', 'global', 'if', 'import', 'in', 'is', 'lambda', 'new', 'nonlocal', 'not', 'of', 'on', 'or', 'pass', 'raise', 'require', 'return', 'to', 'try', 'until', 'while', 'with', 'yield')
-    SOFT_KEYWORDS = ('_', 'abort', 'above', 'additive', 'after', 'ahead', 'along', 'altitude', 'always', 'angle', 'apparent', 'apparently', 'away', 'back', 'behavior', 'behind', 'below', 'beyond', 'bottom', 'can', 'case', 'choose', 'compose', 'contained', 'deg', 'directly', 'distance', 'dynamic', 'ego', 'eventually', 'facing', 'final', 'follow', 'following', 'from', 'front', 'heading', 'implies', 'initial', 'interrupt', 'invariant', 'left', 'match', 'model', 'monitor', 'mutate', 'next', 'not', 'of', 'offset', 'override', 'param', 'past', 'position', 'precondition', 'record', 'relative', 'right', 'scenario', 'seconds', 'see', 'setup', 'shuffle', 'simulation', 'simulator', 'steps', 'take', 'terminate', 'top', 'toward', 'visible', 'wait', 'when', 'workspace')
+    SOFT_KEYWORDS = ('_', 'abort', 'above', 'additive', 'after', 'ahead', 'along', 'altitude', 'always', 'angle', 'apparent', 'apparently', 'away', 'back', 'behavior', 'behind', 'below', 'beyond', 'bottom', 'can', 'case', 'choose', 'compose', 'contained', 'deg', 'directly', 'distance', 'dynamic', 'ego', 'eventually', 'facing', 'final', 'follow', 'following', 'from', 'front', 'heading', 'implies', 'initial', 'interrupt', 'intersects', 'invariant', 'left', 'match', 'model', 'monitor', 'mutate', 'next', 'not', 'of', 'offset', 'override', 'param', 'past', 'position', 'precondition', 'record', 'relative', 'right', 'scenario', 'seconds', 'see', 'setup', 'shuffle', 'simulation', 'simulator', 'steps', 'take', 'terminate', 'top', 'toward', 'type', 'visible', 'wait', 'when', 'workspace')
 
 
 if __name__ == '__main__':
     from pegen.parser import simple_parser_main
     simple_parser_main(ScenicParser)
```

### Comparing `scenic-3.0.0b2/src/scenic/syntax/pygment.py` & `scenic-3.0.0rc1/src/scenic/syntax/pygment.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/syntax/relations.py` & `scenic-3.0.0rc1/src/scenic/syntax/relations.py`

 * *Files identical despite different names*

### Comparing `scenic-3.0.0b2/src/scenic/syntax/scenic.gram` & `scenic-3.0.0rc1/src/scenic/syntax/scenic.gram`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import enum
 import io
 import itertools
 import os
 import sys
 import token
 from typing import (
-    Any, Callable, Iterator, List, Literal, Tuple, TypeVar, Union, NoReturn
+    Any, Callable, Iterator, List, Literal, NoReturn, Sequence, Tuple, TypeVar, Union
 )
 
 from pegen.tokenizer import Tokenizer
 
 import scenic.syntax.ast as s
 from scenic.core.errors import ScenicParseError
 
@@ -227,26 +227,105 @@
             return node
 
     def set_expr_context(self, node, context):
         """Set the context (Load, Store, Del) of an ast node."""
         node.ctx = context
         return node
 
-    def ensure_real(self, number: ast.Constant):
+    def ensure_real(self, number: ast.Constant) -> float:
         value = ast.literal_eval(number.string)
         if type(value) is complex:
             self.raise_syntax_error_known_location("real number required in complex literal", number)
         return value
 
-    def ensure_imaginary(self, number:  ast.Constant):
+    def ensure_imaginary(self, number: ast.Constant) -> complex:
         value = ast.literal_eval(number.string)
         if type(value) is not complex:
             self.raise_syntax_error_known_location("imaginary number required in complex literal", number)
         return value
 
+    def check_fstring_conversion(self, mark: tokenize.TokenInfo, name: tokenize.TokenInfo) -> tokenize.TokenInfo:
+        if mark.lineno != name.lineno or mark.col_offset != name.col_offset:
+            self.raise_syntax_error_known_range(
+                "f-string: conversion type must come right after the exclamanation mark",
+                mark,
+                name
+            )
+
+        s = name.string
+        if len(s) > 1 or s not in ("s", "r", "a"):
+            self.raise_syntax_error_known_location(
+                f"f-string: invalid conversion character '{s}': expected 's', 'r', or 'a'",
+                name,
+            )
+
+        return name
+
+    def _concat_strings_in_constant(self, parts) -> Union[str, bytes]:
+        s = ast.literal_eval(parts[0].string)
+        for ss in parts[1:]:
+            s += ast.literal_eval(ss.string)
+        args = dict(
+            value=s,
+            lineno=parts[0].start[0],
+            col_offset=parts[0].start[1],
+            end_lineno=parts[-1].end[0],
+            end_col_offset=parts[0].end[1],
+        )
+        if parts[0].string.startswith("u"):
+            args["kind"] = "u"
+        return ast.Constant(**args)
+
+
+    def concatenate_strings(self, parts):
+        """Concatenate multiple tokens and ast.JoinedStr"""
+        # Get proper start and stop
+        start = end = None
+        if isinstance(parts[0], ast.JoinedStr):
+            start = parts[0].lineno, parts[0].col_offset
+        if isinstance(parts[-1], ast.JoinedStr):
+            end = parts[-1].end_lineno, parts[-1].end_col_offset
+
+        # Combine the different parts
+        seen_joined = False
+        values = []
+        ss = []
+        for p in parts:
+            if isinstance(p, ast.JoinedStr):
+                seen_joined = True
+                if ss:
+                    values.append(self._concat_strings_in_constant(ss))
+                    ss.clear()
+                values.extend(p.values)
+            else:
+                ss.append(p)
+
+        if ss:
+            values.append(self._concat_strings_in_constant(ss))
+
+        consolidated = []
+        for p in values:
+            if consolidated and isinstance(consolidated[-1], ast.Constant) and isinstance(p, ast.Constant):
+                consolidated[-1].value += p.value
+                consolidated[-1].end_lineno = p.end_lineno
+                consolidated[-1].end_col_offset = p.end_col_offset
+            else:
+                consolidated.append(p)
+
+        if not seen_joined and len(values) == 1 and isinstance(values[0], ast.Constant):
+            return values[0]
+        else:
+            return ast.JoinedStr(
+                values=consolidated,
+                lineno=start[0] if start else values[0].lineno,
+                col_offset=start[1] if start else values[0].col_offset,
+                end_lineno=end[0] if end else values[-1].end_lineno,
+                end_col_offset=end[1] if end else values[-1].end_col_offset,
+            )
+
     def generate_ast_for_string(self, tokens):
         """Generate AST nodes for strings."""
         err_args = None
         line_offset = tokens[0].start[0]
         line = line_offset
         col_offset = 0
         source = "(\\n"
@@ -393,23 +472,26 @@
 
     def make_syntax_error(self, message: str) -> None:
         return self._build_syntax_error(message)
 
     def expect_forced(self, res: Any, expectation: str) -> Optional[tokenize.TokenInfo]:
         if res is None:
             last_token = self._tokenizer.diagnose()
+            end = last_token.start
+            if sys.version_info >= (3, 12) or (sys.version_info >= (3, 11) and last_token.type != 4):  # i.e. not a \n
+                end = last_token.end
             self.raise_raw_syntax_error(
-                f"expected {expectation}", last_token.start, last_token.start
+                f"expected {expectation}", last_token.start, end
             )
         return res
 
     def raise_syntax_error(self, message: str) -> NoReturn:
         """Raise a syntax error."""
         tok = self._tokenizer.diagnose()
-        raise self._build_syntax_error(message, tok.start, tok.end if tok.type != 4 else tok.start)
+        raise self._build_syntax_error(message, tok.start, tok.end if sys.version_info >= (3, 12) or tok.type != 4 else tok.start)
 
     def raise_syntax_error_known_location(
         self, message: str, node: Union[ast.AST, tokenize.TokenInfo]
     ) -> NoReturn:
         """Raise a syntax error that occured at a given AST node."""
         if isinstance(node, tokenize.TokenInfo):
             start = node.start
@@ -463,14 +545,18 @@
         if target in (Target.STAR_TARGETS, Target.FOR_TARGETS):
             msg = f"cannot assign to {self.get_expr_name(invalid_target)}"
         else:
             msg = f"cannot delete {self.get_expr_name(invalid_target)}"
 
         self.raise_syntax_error_known_location(msg, invalid_target)
 
+    def raise_syntax_error_on_next_token(self, message: str) -> NoReturn:
+        next_token = self._tokenizer.peek()
+        raise self._build_syntax_error(message, next_token.start, next_token.end)
+
     # scenic helpers
     def extend_new_specifiers(self, node: s.New, specifiers: List[ast.AST]) -> s.New:
         node.specifiers.extend(specifiers)
         return node
 '''
 
 
@@ -510,14 +596,15 @@
     | a=scenic_stmt !';' NEWLINE { [a] } # Not needed, there for speedup
     | a=';'.scenic_stmt+ [';'] NEWLINE { a }
 
 # NOTE: assignment MUST precede expression, else parsing a simple assignment
 # will throw a SyntaxError.
 simple_stmt (memo):
     | assignment
+    | &"type" type_alias
     | e=star_expressions { ast.Expr(value=e, LOCATIONS) }
     | &'return' return_stmt
     | &('import' | 'from') import_stmt
     | &'raise' raise_stmt
     | 'pass' { ast.Pass(LOCATIONS) }
     | &'del' del_stmt
     | &'yield' yield_stmt
@@ -655,15 +742,18 @@
 
 yield_stmt[ast.Expr]: y=yield_expr { ast.Expr(value=y, LOCATIONS) }
 
 assert_stmt[ast.Assert]: 'assert' a=expression b=[',' z=expression { z }] {
     ast.Assert(test=a, msg=b, LOCATIONS)
 }
 
-import_stmt[ast.Import]: import_name | import_from
+import_stmt[ast.Import]:
+    | invalid_import
+    | import_name
+    | import_from
 
 # Import statements
 # -----------------
 
 import_name[ast.Import]: 'import' a=dotted_as_names { ast.Import(names=a, LOCATIONS) }
 
 # note below: the ('.' | '...') is necessary because '...' is tokenized as ELLIPSIS
@@ -724,22 +814,34 @@
 
 class_def[ast.ClassDef]:
     | a=decorators b=class_def_raw { self.set_decorators(b, a) }
     | class_def_raw
 
 class_def_raw[ast.ClassDef]:
     | invalid_class_def_raw
-    | 'class' a=NAME b=['(' z=[arguments] ')' { z }] &&':' c=scenic_class_def_block {
-        ast.ClassDef(
-            a.string,
-            bases=b[0] if b else [],
-            keywords=b[1] if b else [],
-            body=c,
-            decorator_list=[],
-            LOCATIONS,
+    | 'class' a=NAME t=[type_params] b=['(' z=[arguments] ')' { z }] &&':' c=scenic_class_def_block {
+        (
+            ast.ClassDef(
+                a.string,
+                bases=b[0] if b else [],
+                keywords=b[1] if b else [],
+                body=c,
+                decorator_list=[],
+                type_params=t or [],
+                LOCATIONS,
+            )
+            if sys.version_info >= (3, 12) else
+            ast.ClassDef(
+                a.string,
+                bases=b[0] if b else [],
+                keywords=b[1] if b else [],
+                body=c,
+                decorator_list=[],
+                LOCATIONS,
+            )
         )
      }
 
 scenic_class_def_block:
     | NEWLINE INDENT a=scenic_class_statements DEDENT { a }
     | simple_stmts
     | invalid_block
@@ -910,38 +1012,64 @@
 
 function_def[Union[ast.FunctionDef, ast.AsyncFunctionDef]]:
     | d=decorators f=function_def_raw { self.set_decorators(f, d) }
     | f=function_def_raw {self.set_decorators(f, [])}
 
 function_def_raw[Union[ast.FunctionDef, ast.AsyncFunctionDef]]:
     | invalid_def_raw
-    | 'def' n=NAME &&'(' params=[params] ')' a=['->' z=expression { z }] &&':' tc=[func_type_comment] b=block {
-        ast.FunctionDef(
-            name=n.string,
-            args=params or self.make_arguments(None, [], None, [], None),
-            returns=a,
-            body=b,
-            type_comment=tc,
-            LOCATIONS,
-        )
-     }
-    | 'async' 'def' n=NAME &&'(' params=[params] ')' a=['->' z=expression { z }] &&':' tc=[func_type_comment] b=block {
-       self.check_version(
-            (3, 5),
-            "Async functions are",
-            ast.AsyncFunctionDef(
+    | 'def' n=NAME t=[type_params] &&'(' params=[params] ')' a=['->' z=expression { z }] &&':' tc=[func_type_comment] b=block {
+        (
+            ast.FunctionDef(
+                name=n.string,
+                args=params or self.make_arguments(None, [], None, [], None),
+                returns=a,
+                body=b,
+                type_comment=tc,
+                type_params=t or [],
+                LOCATIONS,
+            ) if sys.version_info >= (3, 12) else
+            ast.FunctionDef(
                 name=n.string,
                 args=params or self.make_arguments(None, [], None, [], None),
                 returns=a,
                 body=b,
                 type_comment=tc,
                 LOCATIONS,
             )
         )
      }
+    | 'async' 'def' n=NAME t=[type_params] &&'(' params=[params] ')' a=['->' z=expression { z }] &&':' tc=[func_type_comment] b=block {
+       (
+            self.check_version(
+                (3, 5),
+                "Async functions are",
+                ast.AsyncFunctionDef(
+                    name=n.string,
+                    args=params or self.make_arguments(None, [], None, [], None),
+                    returns=a,
+                    body=b,
+                    type_comment=tc,
+                    type_params=t or [],
+                    LOCATIONS,
+                )
+            ) if sys.version_info >= (3, 12) else
+            self.check_version(
+                (3, 5),
+                "Async functions are",
+                ast.AsyncFunctionDef(
+                    name=n.string,
+                    args=params or self.make_arguments(None, [], None, [], None),
+                    returns=a,
+                    body=b,
+                    type_comment=tc,
+                    LOCATIONS,
+                )
+            )
+       )
+     }
 
 # Function parameters
 # -------------------
 
 params:
     | invalid_parameters
     | parameters
@@ -977,14 +1105,15 @@
 slash_with_default[List[Tuple[ast.arg, Any]]]:
     | a=param_no_default* b=param_with_default+ '/' ',' { ([(p, None) for p in a] if a else []) + b }
     | a=param_no_default* b=param_with_default+ '/' &')' { ([(p, None) for p in a] if a else []) + b }
 
 star_etc[Tuple[Optional[ast.arg], List[Tuple[ast.arg, Any]], Optional[ast.arg]]]:
     | invalid_star_etc
     | '*' a=param_no_default b=param_maybe_default* c=[kwds] { (a, b, c) }
+    | '*' a=param_no_default_star_annotation b=param_maybe_default* c=[kwds] { (a, b, c) }
     | '*' ',' b=param_maybe_default+ c=[kwds] { (None, b, c) }
     | a=kwds { (None, [], a) }
 
 kwds[ast.arg]:
     | invalid_kwds
     | '**' a=param_no_default { a }
 
@@ -1000,22 +1129,29 @@
 # - No comma, optional type comment, must be followed by close paren
 # The latter form is for a final parameter without trailing comma.
 #
 
 param_no_default[ast.arg]:
     | a=param ',' tc=TYPE_COMMENT? { self.set_arg_type_comment(a, tc) }
     | a=param tc=TYPE_COMMENT? &')' { self.set_arg_type_comment(a, tc) }
+param_no_default_star_annotation[ast.arg]:
+    | a=param_star_annotation ',' tc=TYPE_COMMENT? { self.set_arg_type_comment(a, tc) }
+    | a=param_star_annotation tc=TYPE_COMMENT? &')' { self.set_arg_type_comment(a, tc) }
 param_with_default[Tuple[ast.arg, Any]]:
     | a=param c=default ',' tc=TYPE_COMMENT? { (self.set_arg_type_comment(a, tc), c) }
     | a=param c=default tc=TYPE_COMMENT? &')' { (self.set_arg_type_comment(a, tc), c) }
 param_maybe_default[Tuple[ast.arg, Any]]:
     | a=param c=default? ',' tc=TYPE_COMMENT? { (self.set_arg_type_comment(a, tc), c) }
     | a=param c=default? tc=TYPE_COMMENT? &')' { (self.set_arg_type_comment(a, tc), c) }
 param: a=NAME b=annotation? { ast.arg(arg=a.string, annotation=b, LOCATIONS) }
+param_star_annotation: a=NAME b=star_annotation {
+    ast.arg(arg=a.string, annotations=b, LOCATIONS)
+ }
 annotation: ':' a=expression { a }
+star_annotation: ':' a=star_expression { a }
 default: '=' a=expression { a } | invalid_default
 
 # If statement
 # ------------
 
 if_stmt[ast.If]:
     | invalid_if_stmt
@@ -1097,14 +1233,25 @@
     | invalid_try_stmt
     | 'try' &&':' b=block f=finally_block {
         ast.Try(body=b, handlers=[], orelse=[], finalbody=f, LOCATIONS)
      }
     | 'try' &&':' b=block ex=except_block+ el=[else_block] f=[finally_block] {
         ast.Try(body=b, handlers=ex, orelse=el or [], finalbody=f or [], LOCATIONS)
      }
+    | 'try' &&':' b=block ex=except_star_block+ el=[else_block] f=[finally_block] {
+        self.check_version(
+            (3, 11),
+            "Exception groups are",
+            (
+                ast.TryStar(body=b, handlers=ex, orelse=el or [], finalbody=f or [], LOCATIONS)
+                if sys.version_info >= (3, 11)
+                else None
+            )
+        )
+     }
 
 scenic_try_interrupt_stmt[s.TryInterrupt]:
     | 'try' &&':' b=block iw=interrupt_when_block+ ex=except_block* el=[else_block] f=[finally_block] {
         s.TryInterrupt(
             body=b,
             interrupt_when_handlers=iw,
             except_handlers=ex,
@@ -1125,14 +1272,20 @@
 
 except_block[ast.ExceptHandler]:
     | invalid_except_stmt_indent
     | 'except' e=expression t=['as' z=NAME { z.string }] ':' b=block {
         ast.ExceptHandler(type=e, name=t, body=b, LOCATIONS) }
     | 'except' ':' b=block { ast.ExceptHandler(type=None, name=None, body=b, LOCATIONS) }
     | invalid_except_stmt
+except_star_block[ast.ExceptHandler]:
+    | invalid_except_star_stmt_indent
+    | 'except' '*' e=expression t=['as' z=NAME { z.string }] ':' b=block {
+        ast.ExceptHandler(type=e, name=t, body=b, LOCATIONS)
+     }
+    | invalid_except_stmt
 finally_block[list]:
     | invalid_finally_stmt
     | 'finally' &&':' a=block { a }
 
 # Match statement
 # ---------------
 
@@ -1354,14 +1507,90 @@
 
 keyword_patterns:
     | ','.keyword_pattern+
 
 keyword_pattern:
     | arg=NAME '=' value=pattern { (arg.string, value) }
 
+# Type statement
+# ---------------
+
+type_alias["ast.TypeAlias"]:
+    | "type" n=NAME t=[type_params] '=' b=expression {
+        self.check_version(
+            (3, 12),
+            "Type statement is",
+            (
+                ast.TypeAlias(
+                    name=ast.Name(
+                        id=n.string,
+                        ctx=Store,
+                        lineno=n.start[0],
+                        col_offset=n.start[1],
+                        end_lineno=n.end[0],
+                        end_col_offset=n.end[1],
+                    ),
+                    type_params=t or [],
+                    value=b,
+                    LOCATIONS
+                )
+                if sys.version_info >= (3, 12)
+                else None
+            )
+        )
+     }
+
+# Type parameter declaration
+# --------------------------
+
+type_params[list]: '[' t=type_param_seq  ']' {
+    self.check_version(
+        (3, 12),
+        "Type parameter lists are",
+        t
+    )
+ }
+
+type_param_seq: a=','.type_param+ [','] { a }
+
+type_param (memo):
+    | a=NAME b=[type_param_bound] {
+        ast.TypeVar(name=a.string, bound=b, LOCATIONS)
+        if sys.version_info >= (3, 12)
+        else object()
+     }
+    | '*' a=NAME colon=":" e=expression {
+        self.raise_syntax_error_starting_from(
+            "cannot use constraints with TypeVarTuple"
+            if isinstance(e, ast.Tuple)
+            else "cannot use bound with TypeVarTuple",
+            colon
+        )
+     }
+    | '*' a=NAME {
+        ast.TypeVarTuple(name=a.string, LOCATIONS)
+        if sys.version_info >= (3, 12)
+        else object()
+     }
+    | '**' a=NAME colon=":" e=expression {
+        self.raise_syntax_error_starting_from(
+            "cannot use constraints with ParamSpec"
+            if isinstance(e, ast.Tuple)
+            else "cannot use bound with ParamSpec",
+            colon
+        )
+     }
+    | '**' a=NAME {
+        ast.ParamSpec(name=a.string, LOCATIONS)
+        if sys.version_info >= (3, 12)
+        else object()
+     }
+
+type_param_bound: ":" e=expression { e }
+
 # EXPRESSIONS
 # -----------
 
 expressions:
     | a=expression b=(',' c=expression { c })+ [','] {
         ast.Tuple(elts=[a] + b, ctx=Load, LOCATIONS) }
     | a=expression ',' { ast.Tuple(elts=[a], ctx=Load, LOCATIONS) }
@@ -1569,23 +1798,26 @@
 # Logical operators
 # -----------------
 
 bitwise_or:
     | scenic_visible_from
     | scenic_not_visible_from
     | scenic_can_see
+    | scenic_intersects
     | a=bitwise_or '|' b=bitwise_xor { ast.BinOp(left=a, op=ast.BitOr(), right=b, LOCATIONS) }
     | bitwise_xor
 
 scenic_visible_from: a=bitwise_or "visible" 'from' b=bitwise_xor { s.VisibleFromOp(region=a, base=b, LOCATIONS) }
 
 scenic_not_visible_from: a=bitwise_or "not" "visible" 'from' b=bitwise_xor { s.NotVisibleFromOp(region=a, base=b, LOCATIONS) }
 
 scenic_can_see: a=bitwise_or "can" "see" b=bitwise_xor { s.CanSeeOp(left=a, right=b, LOCATIONS) }
 
+scenic_intersects: a=bitwise_or "intersects" b=bitwise_xor { s.IntersectsOp(left=a, right=b, LOCATIONS) }
+
 bitwise_xor:
     | scenic_offset_along
     | a=bitwise_xor '^' b=bitwise_and { ast.BinOp(left=a, op=ast.BitXor(), right=b, LOCATIONS) }
     | bitwise_and
 
 scenic_offset_along: a=bitwise_xor "offset" "along" b=bitwise_xor 'by' c=bitwise_and { s.OffsetAlongOp(base=a, direction=b, offset=c, LOCATIONS) }
 
@@ -1726,15 +1958,15 @@
         )
      }
     | a=primary '[' b=slices ']' { ast.Subscript(value=a, slice=b, ctx=Load, LOCATIONS) }
     | atom
 
 slices:
     | a=slice !',' { a }
-    | a=','.slice+ [','] {
+    | a=','.(slice | starred_expression)+ [','] {
         ast.Tuple(elts=a, ctx=Load, LOCATIONS)
         if sys.version_info >= (3, 9) else
         (
             ast.ExtSlice(dims=a, LOCATIONS)
             if any(isinstance(e, ast.Slice) for e in a) else
             ast.Index(value=ast.Tuple(elts=[e.value for e in a], ctx=Load, LOCATIONS), LOCATIONS)
         )
@@ -1770,15 +2002,15 @@
         ast.Constant(value=False, kind=None, LOCATIONS)
      }
     | 'None' {
         ast.Constant(value=None, LOCATIONS)
         if sys.version_info >= (3, 9) else
         ast.Constant(value=None, kind=None, LOCATIONS)
      }
-    | &STRING strings
+    | &(STRING|FSTRING_START) strings
     | a=NUMBER {
         ast.Constant(value=ast.literal_eval(a.string), LOCATIONS)
         if sys.version_info >= (3, 9) else
         ast.Constant(value=ast.literal_eval(a.string), kind=None, LOCATIONS)
      }
     | &'(' (tuple | group | genexp)
     | &'[' (list | listcomp)
@@ -1945,18 +2177,61 @@
 scenic_do_stmt: 'do' e=(','.expression+) { s.Do(elts=e, LOCATIONS) }
 
 scenic_simulator_stmt: "simulator" e=expression { s.Simulator(value=e, LOCATIONS) }
 
 # LITERALS
 # ========
 
-strings[ast.Str] (memo): a=STRING+ { self.generate_ast_for_string(a) }
+fstring_mid:
+    | fstring_replacement_field
+    | t=FSTRING_MIDDLE { ast.Constant(value=t.string, LOCATIONS) }
+fstring_replacement_field:
+    | '{' a=(yield_expr | star_expressions) debug_expr="="? conversion=[fstring_conversion] format=[fstring_full_format_spec] rbrace='}' {
+        ast.FormattedValue(
+            value=a,
+            conversion=(
+                conversion.decode()[0]
+                if conversion else
+                (b'r'[0] if debug_expr else -1)
+            ),
+            format_spec=format,
+            LOCATIONS
+        )
+     }
+    | invalid_replacement_field
+fstring_conversion[int]:
+    | conv_token="!" conv=NAME { self.check_fstring_conversion(conv_token, conv) }
+fstring_full_format_spec:
+    | ':' spec=fstring_format_spec* {
+        ast.JoinedStr(
+            values=spec if spec and (len(spec) > 1 or spec[0].value) else [],
+            LOCATIONS,
+        )
+     }
+fstring_format_spec:
+    | t=FSTRING_MIDDLE { ast.Constant(value=t.string, LOCATIONS) }
+    | fstring_replacement_field
+fstring:
+    | a=FSTRING_START b=fstring_mid* c=FSTRING_END {
+        ast.JoinedStr(values=b, LOCATIONS)
+     }
+
+strings (memo): a=(fstring|STRING)+ {
+    self.concatenate_strings(a) if sys.version_info >= (3, 12) else self.generate_ast_for_string(a)
+ }
+
 
 list[ast.List]:
     | '[' a=[star_named_expressions] ']' { ast.List(elts=a or [], ctx=Load, LOCATIONS) }
+    | a='**' expression '=' b=expression {
+        self.raise_syntax_error_known_range(
+            "cannot assign to keyword argument unpacking", a, b
+        )
+     }
+
 
 tuple[ast.Tuple]:
     | '(' a=[y=star_named_expression ',' z=[star_named_expressions] { [y] + (z or []) } ] ')' {
         ast.Tuple(elts=a or [], ctx=Load, LOCATIONS)
      }
 
 set[ast.Set]: '{' a=star_named_expressions '}' { ast.Set(elts=a, LOCATIONS) }
@@ -2034,14 +2309,15 @@
 
 kwargs[list]:
     | a=','.kwarg_or_starred+ ',' b=','.kwarg_or_double_starred+ { a + b }
     | ','.kwarg_or_starred+
     | ','.kwarg_or_double_starred+
 
 starred_expression:
+    | invalid_starred_expression
     | '*' a=expression { ast.Starred(value=a, ctx=Load, LOCATIONS) }
 
 kwarg_or_starred:
     | invalid_kwarg
     | a=NAME '=' b=expression { ast.keyword(arg=a.string, value=b, LOCATIONS) }
     | a=starred_expression { a }
 
@@ -2169,14 +2445,17 @@
         )
      }
     | a=NAME b='=' expression for_if_clauses {
         self.raise_syntax_error_known_range(
             "invalid syntax. Maybe you meant '==' or ':=' instead of '='?", a, b
         )
      }
+    | (args ',')? a=NAME b='=' &(',' | ')') {
+        self.raise_syntax_error_known_range("expected argument value expression", a, b)
+     }
     | a=args b=for_if_clauses {
         self.raise_syntax_error_known_range(
             "Generator expression must be parenthesized",
             a[0][-1],
             (b[-1].ifs[-1] if b[-1].ifs else b[-1].iter),
         ) if len(a[0]) > 1 else None
      }
@@ -2219,15 +2498,15 @@
     }
 
 expression_without_invalid[ast.AST]:
     | a=disjunction 'if' b=disjunction 'else' c=expression { ast.IfExp(body=b, test=a, orelse=c, LOCATIONS) }
     | disjunction
     | lambdef
 invalid_legacy_expression:
-    | a=NAME !'(' b=expression_without_invalid {
+    | a=NAME !'(' b=star_expressions {
         self.raise_syntax_error_known_range(
             f"Missing parentheses in call to '{a.string}' . Did you mean {a.string}(...)?", a, b,
         ) if a.string in ("exec", "print") else
         None
      }
 invalid_expression[NoReturn]:
     # !(NAME STRING) is not matched so we don't show this error with some invalid string prefixes like: kf"dsfsdf"
@@ -2239,14 +2518,19 @@
             if not isinstance(a, ast.Name) or a.id not in ("print", "exec")
             else None
         )
      }
     | a=disjunction 'if' b=disjunction !('else'|':') {
         self.raise_syntax_error_known_range("expected 'else' after 'if' expression", a, b)
      }
+    | a='lambda' [lambda_params] b=':' &(FSTRING_MIDDLE | fstring_replacement_field)  {
+        self.raise_syntax_error_known_range(
+            "f-string: lambda expressions are not allowed without parentheses", a, b
+        )
+     }
 invalid_named_expression[NoReturn]:
     | a=expression ':=' expression {
         self.raise_syntax_error_known_location(
             f"cannot use assignment expressions with {self.get_expr_name(a)}", a
         )
      }
     # Use in_raw_rule
@@ -2342,26 +2626,30 @@
         )
      }
 invalid_dict_comprehension[NoReturn]:
     | '{' a='**' bitwise_or for_if_clauses '}' {
         self.raise_syntax_error_known_location("dict unpacking cannot be used in dict comprehension", a)
      }
 invalid_parameters[NoReturn]:
-    | param_no_default* invalid_parameters_helper a=param_no_default {
-        self.raise_syntax_error_known_location("non-default argument follows default argument", a)
-     }
-    | param_no_default* a='(' param_no_default+ ','? b=')' {
-        self.raise_syntax_error_known_range("Function parameters cannot be parenthesized", a, b)
-     }
     | a="/" ',' {
         self.raise_syntax_error_known_location("at least one argument must precede /", a)
      }
     | (slash_no_default | slash_with_default) param_maybe_default* a='/' {
         self.raise_syntax_error_known_location("/ may appear only once", a)
      }
+    | slash_no_default? param_no_default* invalid_parameters_helper a=param_no_default {
+        self.raise_syntax_error_known_location(
+            "parameter without a default follows parameter with a default", a
+        )
+     }
+    | param_no_default* a='(' param_no_default+ ','? b=')' {
+        self.raise_syntax_error_known_range(
+            "Function parameters cannot be parenthesized", a, b
+        )
+     }
     | (slash_no_default | slash_with_default)? param_maybe_default* '*' (',' | param_no_default) param_maybe_default* a='/' {
         self.raise_syntax_error_known_location("/ must be ahead of *", a)
      }
     | param_maybe_default+ '/' a='*' {
         self.raise_syntax_error_known_location("expected comma between / and *", a)
      }
 invalid_default:
@@ -2389,26 +2677,30 @@
     | '**' param ',' a=('*'|'**'|'/') {
         self.raise_syntax_error_known_location("arguments cannot follow var-keyword argument", a)
      }
 invalid_parameters_helper: # This is only there to avoid type errors
     | a=slash_with_default { [a] }
     | a=param_with_default+
 invalid_lambda_parameters[NoReturn]:
-    | lambda_param_no_default* invalid_lambda_parameters_helper a=lambda_param_no_default {
-        self.raise_syntax_error_known_location("non-default argument follows default argument", a)
-     }
-    | lambda_param_no_default* a='(' ','.lambda_param+ ','? b=')' {
-        self.raise_syntax_error_known_range("Lambda expression parameters cannot be parenthesized", a, b)
-     }
     | a="/" ',' {
         self.raise_syntax_error_known_location("at least one argument must precede /", a)
      }
     | (lambda_slash_no_default | lambda_slash_with_default) lambda_param_maybe_default* a='/' {
         self.raise_syntax_error_known_location("/ may appear only once", a)
      }
+    | lambda_slash_no_default? lambda_param_no_default* invalid_lambda_parameters_helper a=lambda_param_no_default {
+        self.raise_syntax_error_known_location(
+            "parameter without a default follows parameter with a default", a
+        )
+     }
+    | lambda_param_no_default* a='(' ','.lambda_param+ ','? b=')' {
+        self.raise_syntax_error_known_range(
+            "Lambda expression parameters cannot be parenthesized", a, b
+        )
+     }
     | (lambda_slash_no_default | lambda_slash_with_default)? lambda_param_maybe_default* '*' (',' | lambda_param_no_default) lambda_param_maybe_default* a='/' {
         self.raise_syntax_error_known_location("/ must be ahead of *", a)
      }
     | lambda_param_maybe_default+ '/' a='*' {
         self.raise_syntax_error_known_location("expected comma between / and *", a)
      }
 invalid_lambda_parameters_helper[NoReturn]:
@@ -2451,14 +2743,20 @@
 invalid_group[NoReturn]:
     | '(' a=starred_expression ')' {
         self.raise_syntax_error_known_location("cannot use starred expression here", a)
      }
     | '(' a='**' expression ')' {
         self.raise_syntax_error_known_location("cannot use double starred expression here", a)
      }
+invalid_import:
+    | a='import' ','.dotted_name+ 'from' dotted_name {
+        self.raise_syntax_error_starting_from(
+            "Did you mean to use 'from ... import ...' instead?", a
+        )
+     }
 invalid_import_from_targets[NoReturn]:
     | import_from_as_names ',' NEWLINE {
         self.raise_syntax_error("trailing comma not allowed without surrounding parentheses")
      }
 
 invalid_with_stmt[None]:
     | ['async'] 'with' ','.(expression ['as' star_target])+ &&':' { UNREACHABLE }
@@ -2480,20 +2778,33 @@
         self.raise_indentation_error(
             f"expected an indented block after 'try' statement on line {a.start[0]}",
         )
      }
     | 'try' ':' block !('except' | 'finally') {
         self.raise_syntax_error("expected 'except' or 'finally' block")
      }
+    | 'try' ':' block* except_block+ a='except' b='*' expression ['as' NAME] ':' {
+        self.raise_syntax_error_known_range(
+            "cannot have both 'except' and 'except*' on the same 'try'", a, b
+        )
+     }
+    | 'try' ':' block* except_star_block+ a='except' [expression ['as' NAME]] ':' {
+        self.raise_syntax_error_known_location(
+            "cannot have both 'except' and 'except*' on the same 'try'", a
+        )
+     }
 invalid_except_stmt[None]:
-    | 'except' a=expression ',' expressions ['as' NAME ] ':' {
+    | 'except' '*'? a=expression ',' expressions ['as' NAME ] ':' {
         self.raise_syntax_error_starting_from("multiple exception types must be parenthesized", a)
      }
-    | a='except' expression ['as' NAME ] NEWLINE { self.raise_syntax_error("expected ':'") }
-    | a='except' NEWLINE { self.raise_syntax_error("expected ':'") }
+    | a='except' '*'? expression ['as' NAME ] NEWLINE { self.raise_syntax_error("expected ':'") }
+    | a='except' '*'? NEWLINE { self.raise_syntax_error("expected ':'") }
+    | a='except' '*' (NEWLINE | ':') {
+        self.raise_syntax_error("expected one or more exception types")
+     }
 invalid_finally_stmt[NoReturn]:
     | a='finally' ':' NEWLINE !INDENT {
         self.raise_indentation_error(
             f"expected an indented block after 'finally' statement on line {a.start[0]}"
         )
      }
 invalid_except_stmt_indent[NoReturn]:
@@ -2503,14 +2814,20 @@
         )
      }
     | a='except' ':' NEWLINE !INDENT {
         self.raise_indentation_error(
             f"expected an indented block after 'except' statement on line {a.start[0]}"
         )
      }
+invalid_except_star_stmt_indent:
+    | a='except' '*' expression ['as' NAME ] ':' NEWLINE !INDENT {
+        self.raise_indentation_error(
+            f"expected an indented block after 'except*' statement on line {a.start[0]}"
+        )
+     }
 invalid_match_stmt[NoReturn]:
     | "match" subject_expr !':' {
         self.check_version(
             (3, 10),
             "Pattern matching is",
             self.raise_syntax_error("expected ':'")
         )
@@ -2570,27 +2887,29 @@
     | 'while' named_expression NEWLINE { self.raise_syntax_error("expected ':'") }
     | a='while' named_expression ':' NEWLINE !INDENT {
         self.raise_indentation_error(
             f"expected an indented block after 'while' statement on line {a.start[0]}"
         )
      }
 invalid_for_stmt[NoReturn]:
+    | [ASYNC] 'for' star_targets 'in' star_expressions NEWLINE { self.raise_syntax_error("expected ':'") }
     | ['async'] a='for' star_targets 'in' star_expressions ':' NEWLINE !INDENT {
         self.raise_indentation_error(
             f"expected an indented block after 'for' statement on line {a.start[0]}"
         )
      }
 invalid_def_raw[NoReturn]:
-    | ['async'] a='def' NAME '(' [params] ')' ['->' expression] ':' NEWLINE !INDENT {
+    | ['async'] a='def' NAME  [type_params] '(' [params] ')' ['->' expression] ':' NEWLINE !INDENT {
         self.raise_indentation_error(
             f"expected an indented block after function definition on line {a.start[0]}"
         )
      }
 invalid_class_def_raw[NoReturn]:
-    | a='class' NAME ['(' [arguments] ')'] ':' NEWLINE !INDENT {
+    | 'class' NAME [type_params] ['(' [arguments] ')'] NEWLINE { self.raise_syntax_error("expected ':'") }
+    | a='class' NAME  [type_params] ['(' [arguments] ')'] ':' NEWLINE !INDENT {
         self.raise_indentation_error(
             f"expected an indented block after class definition on line {a.start[0]}"
         )
      }
 
 invalid_double_starred_kvpairs[None]:
     | ','.double_starred_kvpair+ ',' invalid_kvpair
@@ -2607,10 +2926,50 @@
             (a.lineno, a.col_offset),
             (a.end_lineno, a.end_col_offset)
         )
      }
     | expression ':' a='*' bitwise_or {
         self.raise_syntax_error_starting_from("cannot use a starred expression in a dictionary value", a)
      }
+    | expression a=':' &('}'|',') {
+        self.raise_syntax_error_known_location(
+            "expression expected after dictionary key and ':'", a
+        )
+     }
     | expression a=':' {
         self.raise_syntax_error_known_location("expression expected after dictionary key and ':'", a)
-     }
+     }
+invalid_starred_expression:
+    | a='*' expression '=' b=expression {
+        self.raise_syntax_error_known_range(
+            "cannot assign to iterable argument unpacking", a, b
+        )
+     }
+invalid_replacement_field:
+    | '{' a='=' { self.raise_syntax_error_known_location("f-string: valid expression required before '='", a) }
+    | '{' a='!' { self.raise_syntax_error_known_location("f-string: valid expression required before '!'", a) }
+    | '{' a=':' { self.raise_syntax_error_known_location("f-string: valid expression required before ':'", a) }
+    | '{' a='}' { self.raise_syntax_error_known_location("f-string: valid expression required before '}'", a) }
+    | '{' !(yield_expr | star_expressions) {
+        self.raise_syntax_error_on_next_token(
+            "f-string: expecting a valid expression after '{'"
+        )
+     }
+    | '{' (yield_expr | star_expressions) !('=' | '!' | ':' | '}') {
+        self.raise_syntax_error_on_next_token("f-string: expecting '=', or '!', or ':', or '}'") }
+    | '{' (yield_expr | star_expressions) '=' !('!' | ':' | '}') {
+       self.raise_syntax_error_on_next_token("f-string: expecting '!', or ':', or '}'")
+     }
+    | '{' (yield_expr | star_expressions) '='? invalid_conversion_character
+    | '{' (yield_expr | star_expressions) '='? ['!' NAME] !(':' | '}') {
+        self.raise_syntax_error_on_next_token("f-string: expecting ':' or '}'")
+     }
+    | '{' (yield_expr | star_expressions) '='? ['!' NAME] ':' fstring_format_spec* !'}' {
+        self.raise_syntax_error_on_next_token("f-string: expecting '}', or format specs")
+     }
+    | '{' (yield_expr | star_expressions) '='? ['!' NAME] !'}' {
+        self.raise_syntax_error_on_next_token("f-string: expecting '}'")
+     }
+
+invalid_conversion_character:
+    | '!' &(':' | '}') { self.raise_syntax_error_on_next_token("f-string: missing conversion character") }
+    | '!' !NAME { self.raise_syntax_error_on_next_token("f-string: invalid conversion character") }
```

### Comparing `scenic-3.0.0b2/src/scenic/syntax/translator.py` & `scenic-3.0.0rc1/src/scenic/syntax/translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import os
 import sys
 import time
 import types
 from typing import Optional
 
 from scenic.core.distributions import RejectionException, toDistribution
-import scenic.core.dynamics as dynamics
+from scenic.core.dynamics.scenarios import DynamicScenario
 import scenic.core.errors as errors
 from scenic.core.errors import InvalidScenarioError, PythonCompileError
 from scenic.core.lazy_eval import needsLazyEvaluation
 import scenic.core.pruning as pruning
 from scenic.core.utils import cached_property
 from scenic.syntax.compiler import compileScenicAST
 from scenic.syntax.parser import parse_string
@@ -649,15 +649,15 @@
 
 
 def constructScenarioFrom(namespace, scenarioName=None):
     """Build a Scenario object from an executed Scenic module."""
     modularScenarios = namespace["_scenarios"]
 
     def isModularScenario(thing):
-        return isinstance(thing, type) and issubclass(thing, dynamics.DynamicScenario)
+        return isinstance(thing, type) and issubclass(thing, DynamicScenario)
 
     if not scenarioName and isModularScenario(namespace.get("Main", None)):
         scenarioName = "Main"
     if scenarioName:
         ty = namespace.get(scenarioName, None)
         if not isModularScenario(ty):
             raise RuntimeError(f'no scenario "{scenarioName}" found')
@@ -683,8 +683,11 @@
         dynScenario._prepare(delayPreconditionCheck=True)
     scenario = dynScenario._toScenario(namespace)
 
     # Prune infeasible parts of the space
     if usePruning:
         pruning.prune(scenario, verbosity=errors.verbosityLevel)
 
+    # Validate scenario
+    scenario.validate()
+
     return scenario
```

### Comparing `scenic-3.0.0b2/src/scenic/syntax/veneer.py` & `scenic-3.0.0rc1/src/scenic/syntax/veneer.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     "AltitudeTo",
     "AltitudeFrom",
     # Infix operators
     "FieldAt",
     "RelativeTo",
     "OffsetAlong",
     "CanSee",
+    "Intersects",
     "Until",
     "Implies",
     "VisibleFromOp",
     "NotVisibleFromOp",
     # Primitive types
     "Vector",
     "Orientation",
@@ -185,26 +186,22 @@
     Normal,
     Options,
     RandomControlFlowError,
     Range,
     TruncatedNormal,
     Uniform,
 )
-from scenic.core.dynamics import (
-    Behavior,
-    BlockConclusion,
-    DynamicScenario,
+from scenic.core.dynamics.behaviors import Behavior, Monitor
+from scenic.core.dynamics.guards import (
     GuardViolation,
     InvariantViolation,
-    Monitor,
     PreconditionViolation,
-    _makeSimulationTerminationAction,
-    _makeTerminationAction,
-    runTryInterrupt,
 )
+from scenic.core.dynamics.invocables import BlockConclusion, runTryInterrupt
+from scenic.core.dynamics.scenarios import DynamicScenario
 from scenic.core.external_params import (
     VerifaiDiscreteRange,
     VerifaiOptions,
     VerifaiParameter,
     VerifaiRange,
 )
 from scenic.core.geometry import cos, hypot, max, min, sin
@@ -260,14 +257,15 @@
     StarredDistribution,
     TupleDistribution,
     canUnpackDistributions,
     distributionFunction,
     needsSampling,
     toDistribution,
 )
+from scenic.core.dynamics.actions import _EndScenarioAction, _EndSimulationAction
 import scenic.core.errors as errors
 from scenic.core.errors import InvalidScenarioError, ScenicSyntaxError
 from scenic.core.external_params import ExternalParameter
 from scenic.core.geometry import apparentHeadingAtPoint, normalizeAngle
 from scenic.core.lazy_eval import (
     DelayedArgument,
     isLazy,
@@ -313,14 +311,15 @@
 inInitialScenario = True
 runningScenarios = []  # in order, oldest first
 currentBehavior = None
 simulatorFactory = None
 evaluatingGuard = False
 mode2D = False
 _originalConstructibles = (Point, OrientedPoint, Object)
+BUFFERING_PITCH = 0.1
 
 ## APIs used internally by the rest of Scenic
 
 # Scenic compilation
 
 
 def isActive():
@@ -392,14 +391,16 @@
             scenic.core.object_types.OrientedPoint = OrientedPoint
             scenic.core.object_types.Object = Object
     else:
         currentScenario = scenarioStack[-1]
 
 
 # Instance/Object creation
+
+
 def registerInstance(inst):
     """Add a Scenic instance to the global list of created objects.
 
     This is called by the Point/OrientedPoint constructor.
     """
     if currentScenario:
         assert isinstance(inst, Constructible)
@@ -627,14 +628,29 @@
     evaluatingGuard = True
     try:
         yield
     finally:
         evaluatingGuard = False
 
 
+def _makeTerminationAction(agent, line):
+    assert activity == 0
+    if agent:
+        scenario = agent._parentScenario()
+        assert scenario is not None
+    else:
+        scenario = None
+    return _EndScenarioAction(scenario, line)
+
+
+def _makeSimulationTerminationAction(line):
+    assert activity == 0
+    return _EndSimulationAction(line)
+
+
 ### Parsing support
 
 
 class Modifier(typing.NamedTuple):
     name: str
     value: typing.Any
     terminator: typing.Optional[str] = None
@@ -656,15 +672,20 @@
     value for stores.
     """
     egoObject = currentScenario._ego
     if obj is None:
         if egoObject is None:
             raise InvalidScenarioError("referred to ego object not yet assigned")
     elif not isinstance(obj, Object):
-        raise TypeError("tried to make non-object the ego object")
+        if isinstance(obj, type) and issubclass(obj, Object):
+            suffix = " (perhaps you forgot 'new'?)"
+        else:
+            suffix = ""
+        ty = type(obj).__name__
+        raise TypeError(f"tried to make non-object (of type {ty}) the ego object{suffix}")
     else:
         currentScenario._ego = obj
         for scenario in runningScenarios:
             if scenario._ego is None:
                 scenario._ego = obj
     return egoObject
 
@@ -1344,14 +1365,23 @@
         )
 
         return X.canSee(Y, occludingObjects=occludingObjects)
 
     return canSeeHelper(X, Y, objects)
 
 
+@distributionFunction
+def Intersects(X, Y):
+    """The :scenic:`{X} intersects {Y}` operator."""
+    if isA(X, Object):
+        return X.intersects(Y)
+    else:
+        return Y.intersects(X)
+
+
 ### Specifiers
 
 
 def With(prop, val):
     """The :grammar:`with <property> <value>` specifier.
 
     Specifies the given property, with no dependencies.
@@ -1416,23 +1446,23 @@
         on <region>
         on <object>
         on <vector>
     """
     if isA(thing, Object):
         # Target is an Object: use its onSurface.
         target = thing.onSurface
+    elif canCoerce(thing, Vector, exact=True):
+        # Target is a vector
+        target = toVector(thing)
     elif canCoerce(thing, Region):
         # Target is a region (or could theoretically be coerced to one),
         # so we can use it as a target.
-        target = thing
+        target = toType(thing, Region)
     else:
-        # Target is a vector, so we can use it as a target.
-        target = toType(
-            thing, Vector, 'specifier "on R" with R not a Region, Object, or Vector'
-        )
+        raise TypeError('specifier "on R" with R not a Region, Object, or Vector')
 
     props = {"position": 1}
 
     if isA(target, Region) and alwaysProvidesOrientation(target):
         props["parentOrientation"] = 2
 
     def helper(context):
@@ -1579,18 +1609,36 @@
     """The :grammar:`visible from <point>` specifier.
 
     Specifies :prop:`_observingEntity` and :prop:`position`, with no dependencies.
     """
     if not isA(base, Point):
         raise TypeError('specifier "visible from O" with O not a Point')
 
+    def helper(self):
+        if mode2D:
+            position = Region.uniformPointIn(base.visibleRegion)
+        else:
+            containing_region = (
+                currentScenario._workspace.region
+                if self.regionContainedIn is None
+                and currentScenario._workspace is not None
+                else self.regionContainedIn
+            )
+            position = (
+                Region.uniformPointIn(everywhere, tag="visible")
+                if containing_region is None
+                else Region.uniformPointIn(containing_region)
+            )
+
+        return {"position": position, "_observingEntity": base}
+
     return Specifier(
         "Visible/VisibleFrom",
         {"position": 3, "_observingEntity": 1},
-        {"position": Region.uniformPointIn(base.visibleRegion), "_observingEntity": base},
+        DelayedArgument({"regionContainedIn"}, helper),
     )
 
 
 def VisibleSpec():
     """The :specifier:`visible` specifier (equivalent to :specifier:`visible from ego`).
 
     Specifies :prop:`_observingEntity` and :prop:`position`, with no dependencies.
@@ -1616,17 +1664,16 @@
                     '"not visible" specifier with no workspace or containing region defined'
                 )
             region = currentScenario._workspace.region
 
         if mode2D:
             position = Region.uniformPointIn(region.difference(base.visibleRegion))
         else:
-            position = Region.uniformPointIn(
-                convertToFootprint(region).difference(base.visibleRegion)
-            )
+            # We can't limit the available region since any spot could potentially be occluded.
+            position = Region.uniformPointIn(convertToFootprint(region))
 
         return {"position": position, "_nonObservingEntity": base}
 
     return Specifier(
         "NotVisible/NotVisibleFrom",
         {"position": 3, "_nonObservingEntity": 1},
         DelayedArgument({"regionContainedIn"}, helper),
```

### Comparing `scenic-3.0.0b2/PKG-INFO` & `scenic-3.0.0rc1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,90 @@
 Metadata-Version: 2.1
 Name: scenic
-Version: 3.0.0b2
+Version: 3.0.0rc1
 Summary: The Scenic scenario description language.
-Author: Daniel Fremont, Eric Vin, Edward Kim, Tommaso Dreossi, Shromona Ghosh, Xiangyu Yue, Alberto L. Sangiovanni-Vincentelli, Sanjit A. Seshia
+Author: Daniel Fremont, Eric Vin, Shun Kashiwa, Edward Kim, Tommaso Dreossi, Shromona Ghosh, Xiangyu Yue, Alberto L. Sangiovanni-Vincentelli, Sanjit A. Seshia
 Maintainer-email: Daniel Fremont <dfremont@ucsc.edu>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: antlr4-python3-runtime ~= 4.11
 Requires-Dist: attrs >= 19.3.0
 Requires-Dist: dotmap ~= 1.3
 Requires-Dist: mapbox_earcut >= 0.12.10
 Requires-Dist: matplotlib ~= 3.2
+Requires-Dist: manifold3d == 2.3.0
 Requires-Dist: networkx >= 2.6
 Requires-Dist: numpy ~= 1.24
 Requires-Dist: opencv-python ~= 4.5
-Requires-Dist: pegen >= 0.2
-Requires-Dist: pillow ~= 9.1
+Requires-Dist: pegen >= 0.3.0
+Requires-Dist: pillow >= 9.1
 Requires-Dist: pygame >= 2.1.3.dev8, <3; python_version >= "3.11"
 Requires-Dist: pygame ~= 2.0; python_version < "3.11"
 Requires-Dist: pyglet ~= 1.5
 Requires-Dist: python-fcl >= 0.7
 Requires-Dist: Rtree ~= 1.0
 Requires-Dist: rv-ltl ~= 0.1
+Requires-Dist: scikit-image ~= 0.21
 Requires-Dist: scipy ~= 1.7
 Requires-Dist: shapely ~= 2.0
-Requires-Dist: trimesh >=3.22.2, <4
-Requires-Dist: scenic[test] ; extra == "dev"
-Requires-Dist: scenic[guideways] ; extra == "dev"
-Requires-Dist: astor >= 0.8.1 ; extra == "dev"
-Requires-Dist: black ~= 23.0 ; extra == "dev"
-Requires-Dist: inflect ~= 5.5 ; extra == "dev"
+Requires-Dist: trimesh >=4.0.9, <5
+Requires-Dist: scenic[test-full] ; extra == "dev"
+Requires-Dist: black ~= 24.0 ; extra == "dev"
 Requires-Dist: isort ~= 5.11 ; extra == "dev"
 Requires-Dist: pre-commit ~= 3.0 ; extra == "dev"
-Requires-Dist: pygments ~= 2.11 ; extra == "dev"
 Requires-Dist: pytest-cov >= 3.0.0 ; extra == "dev"
-Requires-Dist: sphinx >= 5.0.0, <6 ; extra == "dev"
-Requires-Dist: sphinx_rtd_theme >= 0.5.2 ; extra == "dev"
-Requires-Dist: sphinx-tabs ~= 3.4.1 ; extra == "dev"
-Requires-Dist: tox ~= 3.14 ; extra == "dev"
+Requires-Dist: tox ~= 4.0 ; extra == "dev"
 Requires-Dist: pyproj ~= 3.0 ; extra == "guideways" and ( python_version < "3.10")
 Requires-Dist: pyproj ~= 3.3 ; extra == "guideways" and ( python_version >= "3.10")
 Requires-Dist: pytest >= 7.0.0, <8 ; extra == "test"
+Requires-Dist: pytest-cov >= 3.0.0 ; extra == "test"
 Requires-Dist: pytest-randomly ~= 3.2 ; extra == "test"
+Requires-Dist: scenic[test] ; extra == "test-full"
+Requires-Dist: scenic[guideways] ; extra == "test-full"
+Requires-Dist: astor >= 0.8.1 ; extra == "test-full"
+Requires-Dist: carla >= 0.9.12 ; extra == "test-full" and ( python_version <= "3.8" and (platform_system == "Linux" or platform_system == "Windows"))
+Requires-Dist: dill ; extra == "test-full"
+Requires-Dist: exceptiongroup ; extra == "test-full"
+Requires-Dist: inflect ~= 5.5 ; extra == "test-full"
+Requires-Dist: pygments ~= 2.11 ; extra == "test-full"
+Requires-Dist: sphinx >= 5.0.0, <6 ; extra == "test-full"
+Requires-Dist: sphinx_rtd_theme >= 0.5.2 ; extra == "test-full"
+Requires-Dist: sphinx-tabs ~= 3.4.1 ; extra == "test-full"
+Requires-Dist: verifai >= 2.1.0b1 ; extra == "test-full"
 Project-URL: Documentation, https://scenic-lang.readthedocs.io
 Project-URL: Repository, https://github.com/BerkeleyLearnVerify/Scenic
 Provides-Extra: dev
 Provides-Extra: guideways
 Provides-Extra: test
+Provides-Extra: test-full
 
 # Scenic
 
 [![Documentation Status](https://readthedocs.org/projects/scenic-lang/badge/?version=latest)](https://scenic-lang.readthedocs.io/en/latest/?badge=latest)
 [![Tests Status](https://github.com/BerkeleyLearnVerify/Scenic/actions/workflows/run-tests.yml/badge.svg)](https://github.com/BerkeleyLearnVerify/Scenic/actions/workflows/run-tests.yml)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
-A compiler and scenario generator for the Scenic scenario description language.
+A compiler and scenario generator for Scenic, a domain-specific probabilistic programming language for modeling the environments of cyber-physical systems.
 Please see the [documentation](https://scenic-lang.readthedocs.io/) for installation instructions, as well as tutorials and other information about the Scenic language, its implementation, and its interfaces to various simulators.
 
-For a description of the language and some of its applications, see [our journal paper](https://link.springer.com/article/10.1007/s10994-021-06120-5), which extends our [PLDI 2019 paper](https://arxiv.org/abs/1809.09310) (*note:* the syntax of Scenic has changed slightly since the PLDI paper, and many features such as support for dynamic scenarios have been added; these are described in the journal paper).
-Scenic was designed and implemented by Daniel J. Fremont, Edward Kim, Tommaso Dreossi, Shromona Ghosh, Xiangyu Yue, Alberto L. Sangiovanni-Vincentelli, and Sanjit A. Seshia.
+For an overview of the language and some of its applications, see our [2022 journal paper](https://link.springer.com/article/10.1007/s10994-021-06120-5) on Scenic 2, which extends our [PLDI 2019 paper](https://arxiv.org/abs/1809.09310) on Scenic 1.
+The new syntax and features of Scenic 3 are described in our [CAV 2023 paper](https://arxiv.org/abs/2307.03325).
+Our [Publications](https://scenic-lang.readthedocs.io/en/latest/publications.html) page lists additional relevant publications.
+
+Scenic was initially designed and implemented by Daniel J. Fremont, Tommaso Dreossi, Shromona Ghosh, Xiangyu Yue, Alberto L. Sangiovanni-Vincentelli, and Sanjit A. Seshia.
+Additionally, Edward Kim made major contributions to Scenic 2, and Eric Vin, Shun Kashiwa, Matthew Rhea, and Ellen Kalvan to Scenic 3.
+Please see our [Credits](https://scenic-lang.readthedocs.io/en/latest/credits.html) page for details and more contributors.
 
-If you have any problems using Scenic, please submit an issue to [our GitHub repository](https://github.com/BerkeleyLearnVerify/Scenic) or contact Daniel at <dfremont@ucsc.edu>.
+If you have any problems using Scenic, please submit an issue to [our GitHub repository](https://github.com/BerkeleyLearnVerify/Scenic).
 
 The repository is organized as follows:
 
 * the _src/scenic_ directory contains the package proper;
 * the _examples_ directory has many examples of Scenic programs;
+* the _assets_ directory contains meshes and other resources used by the examples and tests;
 * the _docs_ directory contains the sources for the documentation;
-* the _tests_ directory contains tests for the Scenic compiler.
+* the _tests_ directory contains tests for the Scenic tool.
```

