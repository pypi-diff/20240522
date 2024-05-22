# Comparing `tmp/janim-1.0.3.tar.gz` & `tmp/janim-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janim-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "janim-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `janim-1.0.3.tar` & `janim-1.0.4.tar`

### file list

```diff
@@ -1,97 +1,98 @@
--rw-r--r--   0        0        0      165 2024-05-15 13:12:47.689581 janim-1.0.3/.gitignore
--rw-r--r--   0        0        0     1053 2024-05-15 13:12:47.693570 janim-1.0.3/.readthedocs.yaml
--rw-r--r--   0        0        0     1085 2023-08-02 08:54:33.983910 janim-1.0.3/LICENSE
--rw-r--r--   0        0        0      966 2024-05-15 13:12:47.702546 janim-1.0.3/README.md
--rw-r--r--   0        0        0       71 2024-05-20 03:02:24.964401 janim-1.0.3/janim/__init__.py
--rw-r--r--   0        0        0     3147 2024-05-15 13:12:48.880157 janim-1.0.3/janim/__main__.py
--rw-r--r--   0        0        0     4233 2024-05-15 13:12:48.880157 janim-1.0.3/janim/anims/animation.py
--rw-r--r--   0        0        0     6347 2024-05-18 15:41:45.486818 janim-1.0.3/janim/anims/composition.py
--rw-r--r--   0        0        0     6034 2024-05-15 13:12:48.882153 janim-1.0.3/janim/anims/creation.py
--rw-r--r--   0        0        0      815 2024-05-15 13:12:48.882153 janim-1.0.3/janim/anims/display.py
--rw-r--r--   0        0        0     3454 2024-05-15 13:12:48.883149 janim-1.0.3/janim/anims/fading.py
--rw-r--r--   0        0        0     3954 2024-05-15 13:12:48.884148 janim-1.0.3/janim/anims/growing.py
--rw-r--r--   0        0        0    10342 2024-05-15 13:12:48.884148 janim-1.0.3/janim/anims/indication.py
--rw-r--r--   0        0        0     1547 2024-05-15 13:12:48.885147 janim-1.0.3/janim/anims/rotation.py
--rw-r--r--   0        0        0    26783 2024-05-19 14:28:07.770496 janim-1.0.3/janim/anims/timeline.py
--rw-r--r--   0        0        0     9210 2024-05-15 13:12:48.887139 janim-1.0.3/janim/anims/transform.py
--rw-r--r--   0        0        0     9946 2024-05-19 14:26:49.275303 janim-1.0.3/janim/anims/updater.py
--rw-r--r--   0        0        0     4505 2024-05-15 13:12:48.896116 janim-1.0.3/janim/camera/camera.py
--rw-r--r--   0        0        0     2744 2024-05-15 13:12:48.903096 janim-1.0.3/janim/camera/camera_info.py
--rw-r--r--   0        0        0     6808 2024-05-15 13:12:48.913071 janim-1.0.3/janim/cli.py
--rw-r--r--   0        0        0     9221 2024-05-15 13:12:48.913071 janim-1.0.3/janim/components/component.py
--rw-r--r--   0        0        0     2408 2024-05-15 13:12:48.919053 janim-1.0.3/janim/components/data.py
--rw-r--r--   0        0        0     2609 2024-05-15 13:12:48.919053 janim-1.0.3/janim/components/depth.py
--rw-r--r--   0        0        0     1284 2024-05-15 13:12:48.926037 janim-1.0.3/janim/components/image.py
--rw-r--r--   0        0        0    31079 2024-05-19 05:52:00.253534 janim-1.0.3/janim/components/points.py
--rw-r--r--   0        0        0     2833 2024-05-15 13:12:48.933016 janim-1.0.3/janim/components/radius.py
--rw-r--r--   0        0        0     7922 2024-05-15 13:12:48.941993 janim-1.0.3/janim/components/rgbas.py
--rw-r--r--   0        0        0    22599 2024-05-15 13:12:48.941993 janim-1.0.3/janim/components/vpoints.py
--rw-r--r--   0        0        0      245 2024-05-15 13:12:48.942989 janim-1.0.3/janim/constants/__init__.py
--rw-r--r--   0        0        0      169 2024-05-15 13:12:48.948973 janim-1.0.3/janim/constants/alignment.py
--rw-r--r--   0        0        0     1542 2024-05-15 13:12:48.948973 janim-1.0.3/janim/constants/colors.py
--rw-r--r--   0        0        0      639 2024-05-19 23:59:21.996726 janim-1.0.3/janim/constants/coord.py
--rw-r--r--   0        0        0      179 2024-05-15 13:12:48.961939 janim-1.0.3/janim/constants/degrees.py
--rw-r--r--   0        0        0     4900 2024-05-15 13:12:48.962938 janim-1.0.3/janim/examples.py
--rw-r--r--   0        0        0     1723 2024-05-15 13:12:49.008814 janim-1.0.3/janim/exception.py
--rw-r--r--   0        0        0    41710 2024-05-20 02:25:11.810501 janim-1.0.3/janim/gui/anim_viewer.py
--rw-r--r--   0        0        0      330 2024-05-15 13:12:49.015794 janim-1.0.3/janim/gui/application.py
--rw-r--r--   0        0        0      797 2024-05-15 13:12:49.024773 janim-1.0.3/janim/gui/audio_player.py
--rw-r--r--   0        0        0     3181 2024-05-15 13:12:49.034744 janim-1.0.3/janim/gui/export.png
--rw-r--r--   0        0        0     1534 2024-05-15 13:12:49.035741 janim-1.0.3/janim/gui/fixed_ratio_widget.py
--rw-r--r--   0        0        0     1465 2024-05-20 02:25:45.947783 janim-1.0.3/janim/gui/glwidget.py
--rw-r--r--   0        0        0      903 2024-05-15 13:12:49.048708 janim-1.0.3/janim/gui/precise_timer.py
--rw-r--r--   0        0        0     5278 2024-05-15 13:12:49.058683 janim-1.0.3/janim/gui/richtext_editor.py
--rw-r--r--   0        0        0     8331 2024-05-15 13:12:49.074245 janim-1.0.3/janim/gui/selector.py
--rw-r--r--   0        0        0     1710 2024-05-18 05:33:18.266011 janim-1.0.3/janim/imports.py
--rw-r--r--   0        0        0     5727 2024-05-15 13:12:49.077235 janim-1.0.3/janim/items/audio.py
--rw-r--r--   0        0        0     5362 2024-05-15 13:12:49.077235 janim-1.0.3/janim/items/boolean_ops.py
--rw-r--r--   0        0        0     8745 2024-05-15 13:12:49.078232 janim-1.0.3/janim/items/coordinate/coordinate_systems.py
--rw-r--r--   0        0        0     2165 2024-05-15 13:12:49.088209 janim-1.0.3/janim/items/coordinate/functions.py
--rw-r--r--   0        0        0     8330 2024-05-15 13:12:49.097183 janim-1.0.3/janim/items/coordinate/number_line.py
--rw-r--r--   0        0        0     8784 2024-05-15 13:12:49.108152 janim-1.0.3/janim/items/geometry/arc.py
--rw-r--r--   0        0        0     6729 2024-05-15 13:12:49.109152 janim-1.0.3/janim/items/geometry/arrow.py
--rw-r--r--   0        0        0     7917 2024-05-15 13:12:49.118125 janim-1.0.3/janim/items/geometry/line.py
--rw-r--r--   0        0        0     5239 2024-05-15 13:12:49.119124 janim-1.0.3/janim/items/geometry/polygon.py
--rw-r--r--   0        0        0     5242 2024-05-20 00:46:08.126552 janim-1.0.3/janim/items/image_item.py
--rw-r--r--   0        0        0    19084 2024-05-15 13:12:49.121117 janim-1.0.3/janim/items/item.py
--rw-r--r--   0        0        0     3262 2024-05-15 13:12:49.122116 janim-1.0.3/janim/items/points.py
--rw-r--r--   0        0        0     7660 2024-05-15 13:12:49.123112 janim-1.0.3/janim/items/relation.py
--rw-r--r--   0        0        0     2071 2024-05-15 13:12:49.131090 janim-1.0.3/janim/items/shape_matchers.py
--rw-r--r--   0        0        0     5955 2024-05-15 13:12:49.140067 janim-1.0.3/janim/items/svg/brace.py
--rw-r--r--   0        0        0     1736 2024-05-15 13:12:49.148045 janim-1.0.3/janim/items/svg/brace.svg
--rw-r--r--   0        0        0     4377 2024-05-15 13:12:49.149042 janim-1.0.3/janim/items/svg/svg_item.py
--rw-r--r--   0        0        0     3090 2024-05-15 13:12:49.158019 janim-1.0.3/janim/items/svg/typst.py
--rw-r--r--   0        0        0       40 2024-05-15 13:12:49.165001 janim-1.0.3/janim/items/svg/typst_template.typ
--rw-r--r--   0        0        0    16153 2024-05-15 13:12:49.165997 janim-1.0.3/janim/items/text/text.py
--rw-r--r--   0        0        0     1094 2024-05-15 13:12:49.174974 janim-1.0.3/janim/items/value_tracker.py
--rw-r--r--   0        0        0     5357 2024-05-15 13:12:49.174974 janim-1.0.3/janim/items/vitem.py
--rw-r--r--   0        0        0      271 2024-05-15 13:12:49.182953 janim-1.0.3/janim/logger.py
--rw-r--r--   0        0        0     3054 2024-05-15 13:12:49.192927 janim-1.0.3/janim/render/base.py
--rw-r--r--   0        0        0     8857 2024-05-20 01:47:59.633622 janim-1.0.3/janim/render/impl.py
--rw-r--r--   0        0        0      448 2024-05-15 13:12:49.208887 janim-1.0.3/janim/render/shaders/dotcloud.frag.glsl
--rw-r--r--   0        0        0     1250 2024-05-15 13:12:49.216861 janim-1.0.3/janim/render/shaders/dotcloud.geom.glsl
--rw-r--r--   0        0        0      325 2024-05-15 13:12:49.225837 janim-1.0.3/janim/render/shaders/dotcloud.vert.glsl
--rw-r--r--   0        0        0      180 2024-05-20 01:53:43.325091 janim-1.0.3/janim/render/shaders/image.frag.glsl
--rw-r--r--   0        0        0      350 2024-05-15 13:12:49.247780 janim-1.0.3/janim/render/shaders/image.vert.glsl
--rw-r--r--   0        0        0     6950 2024-05-15 13:12:49.259747 janim-1.0.3/janim/render/shaders/vitem.frag.glsl
--rw-r--r--   0        0        0      203 2024-05-15 13:12:49.269436 janim-1.0.3/janim/render/shaders/vitem.vert.glsl
--rw-r--r--   0        0        0     1073 2024-05-19 06:01:17.272817 janim-1.0.3/janim/render/texture.py
--rw-r--r--   0        0        0     6971 2024-05-16 13:52:55.279071 janim-1.0.3/janim/render/writer.py
--rw-r--r--   0        0        0      964 2024-05-15 13:12:49.278412 janim-1.0.3/janim/typing.py
--rw-r--r--   0        0        0    17207 2024-05-15 13:12:49.289382 janim-1.0.3/janim/utils/bezier.py
--rw-r--r--   0        0        0     5515 2024-05-15 13:12:49.297361 janim-1.0.3/janim/utils/config.py
--rw-r--r--   0        0        0     5786 2024-05-19 13:34:44.597026 janim-1.0.3/janim/utils/data.py
--rw-r--r--   0        0        0      637 2024-05-15 13:12:49.317308 janim-1.0.3/janim/utils/dict_ops.py
--rw-r--r--   0        0        0     2483 2024-05-15 13:12:49.330273 janim-1.0.3/janim/utils/file_ops.py
--rw-r--r--   0        0        0     2995 2024-05-15 13:12:49.331270 janim-1.0.3/janim/utils/font.py
--rw-r--r--   0        0        0     6369 2024-05-15 13:12:49.392575 janim-1.0.3/janim/utils/font_manager.py
--rw-r--r--   0        0        0     5973 2024-05-15 13:12:49.403546 janim-1.0.3/janim/utils/iterables.py
--rw-r--r--   0        0        0     1870 2024-05-15 13:12:49.428480 janim-1.0.3/janim/utils/paths.py
--rw-r--r--   0        0        0     2705 2024-05-15 13:12:49.435461 janim-1.0.3/janim/utils/rate_functions.py
--rw-r--r--   0        0        0     2651 2024-05-15 13:12:49.435461 janim-1.0.3/janim/utils/refresh.py
--rw-r--r--   0        0        0     8342 2024-05-15 13:12:49.436460 janim-1.0.3/janim/utils/signal.py
--rw-r--r--   0        0        0     2000 2024-05-15 13:12:49.446431 janim-1.0.3/janim/utils/simple_functions.py
--rw-r--r--   0        0        0    10068 2024-05-15 13:12:49.456405 janim-1.0.3/janim/utils/space_ops.py
--rw-r--r--   0        0        0    18504 2024-05-15 13:12:49.457404 janim-1.0.3/logo.png
--rw-r--r--   0        0        0     1030 2024-05-19 13:23:23.085515 janim-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 janim-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      165 2024-05-15 13:12:47.689581 janim-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1053 2024-05-15 13:12:47.693570 janim-1.0.4/.readthedocs.yaml
+-rw-r--r--   0        0        0     1085 2023-08-02 08:54:33.983910 janim-1.0.4/LICENSE
+-rw-r--r--   0        0        0      966 2024-05-15 13:12:47.702546 janim-1.0.4/README.md
+-rw-r--r--   0        0        0       71 2024-05-22 00:25:29.846729 janim-1.0.4/janim/__init__.py
+-rw-r--r--   0        0        0     3147 2024-05-15 13:12:48.880157 janim-1.0.4/janim/__main__.py
+-rw-r--r--   0        0        0     4233 2024-05-15 13:12:48.880157 janim-1.0.4/janim/anims/animation.py
+-rw-r--r--   0        0        0     6347 2024-05-20 08:38:15.611875 janim-1.0.4/janim/anims/composition.py
+-rw-r--r--   0        0        0     6034 2024-05-15 13:12:48.882153 janim-1.0.4/janim/anims/creation.py
+-rw-r--r--   0        0        0      815 2024-05-15 13:12:48.882153 janim-1.0.4/janim/anims/display.py
+-rw-r--r--   0        0        0     3454 2024-05-15 13:12:48.883149 janim-1.0.4/janim/anims/fading.py
+-rw-r--r--   0        0        0     3954 2024-05-15 13:12:48.884148 janim-1.0.4/janim/anims/growing.py
+-rw-r--r--   0        0        0    10342 2024-05-15 13:12:48.884148 janim-1.0.4/janim/anims/indication.py
+-rw-r--r--   0        0        0     1547 2024-05-15 13:12:48.885147 janim-1.0.4/janim/anims/rotation.py
+-rw-r--r--   0        0        0    26783 2024-05-20 08:38:15.615866 janim-1.0.4/janim/anims/timeline.py
+-rw-r--r--   0        0        0     9210 2024-05-15 13:12:48.887139 janim-1.0.4/janim/anims/transform.py
+-rw-r--r--   0        0        0     9946 2024-05-19 14:26:49.275303 janim-1.0.4/janim/anims/updater.py
+-rw-r--r--   0        0        0     4505 2024-05-15 13:12:48.896116 janim-1.0.4/janim/camera/camera.py
+-rw-r--r--   0        0        0     2744 2024-05-15 13:12:48.903096 janim-1.0.4/janim/camera/camera_info.py
+-rw-r--r--   0        0        0     6808 2024-05-15 13:12:48.913071 janim-1.0.4/janim/cli.py
+-rw-r--r--   0        0        0     9221 2024-05-15 13:12:48.913071 janim-1.0.4/janim/components/component.py
+-rw-r--r--   0        0        0     2408 2024-05-15 13:12:48.919053 janim-1.0.4/janim/components/data.py
+-rw-r--r--   0        0        0     2609 2024-05-15 13:12:48.919053 janim-1.0.4/janim/components/depth.py
+-rw-r--r--   0        0        0     1284 2024-05-15 13:12:48.926037 janim-1.0.4/janim/components/image.py
+-rw-r--r--   0        0        0    31079 2024-05-20 08:38:15.620882 janim-1.0.4/janim/components/points.py
+-rw-r--r--   0        0        0     2833 2024-05-15 13:12:48.933016 janim-1.0.4/janim/components/radius.py
+-rw-r--r--   0        0        0     7927 2024-05-21 15:04:02.417208 janim-1.0.4/janim/components/rgbas.py
+-rw-r--r--   0        0        0    22599 2024-05-15 13:12:48.941993 janim-1.0.4/janim/components/vpoints.py
+-rw-r--r--   0        0        0      245 2024-05-15 13:12:48.942989 janim-1.0.4/janim/constants/__init__.py
+-rw-r--r--   0        0        0      169 2024-05-15 13:12:48.948973 janim-1.0.4/janim/constants/alignment.py
+-rw-r--r--   0        0        0     1542 2024-05-15 13:12:48.948973 janim-1.0.4/janim/constants/colors.py
+-rw-r--r--   0        0        0      639 2024-05-20 08:38:15.623876 janim-1.0.4/janim/constants/coord.py
+-rw-r--r--   0        0        0      179 2024-05-15 13:12:48.961939 janim-1.0.4/janim/constants/degrees.py
+-rw-r--r--   0        0        0     4900 2024-05-15 13:12:48.962938 janim-1.0.4/janim/examples.py
+-rw-r--r--   0        0        0     1723 2024-05-15 13:12:49.008814 janim-1.0.4/janim/exception.py
+-rw-r--r--   0        0        0    41800 2024-05-20 08:38:15.624840 janim-1.0.4/janim/gui/anim_viewer.py
+-rw-r--r--   0        0        0      330 2024-05-15 13:12:49.015794 janim-1.0.4/janim/gui/application.py
+-rw-r--r--   0        0        0      797 2024-05-21 00:09:53.460651 janim-1.0.4/janim/gui/audio_player.py
+-rw-r--r--   0        0        0     3181 2024-05-15 13:12:49.034744 janim-1.0.4/janim/gui/export.png
+-rw-r--r--   0        0        0    16958 2024-05-20 08:38:15.625840 janim-1.0.4/janim/gui/favicon.ico
+-rw-r--r--   0        0        0     1534 2024-05-20 08:38:15.630824 janim-1.0.4/janim/gui/fixed_ratio_widget.py
+-rw-r--r--   0        0        0     1465 2024-05-20 08:38:15.634815 janim-1.0.4/janim/gui/glwidget.py
+-rw-r--r--   0        0        0      903 2024-05-15 13:12:49.048708 janim-1.0.4/janim/gui/precise_timer.py
+-rw-r--r--   0        0        0     5278 2024-05-15 13:12:49.058683 janim-1.0.4/janim/gui/richtext_editor.py
+-rw-r--r--   0        0        0     8331 2024-05-15 13:12:49.074245 janim-1.0.4/janim/gui/selector.py
+-rw-r--r--   0        0        0     1710 2024-05-20 08:38:15.638834 janim-1.0.4/janim/imports.py
+-rw-r--r--   0        0        0     5727 2024-05-15 13:12:49.077235 janim-1.0.4/janim/items/audio.py
+-rw-r--r--   0        0        0     5362 2024-05-20 08:38:15.643789 janim-1.0.4/janim/items/boolean_ops.py
+-rw-r--r--   0        0        0     8745 2024-05-15 13:12:49.078232 janim-1.0.4/janim/items/coordinate/coordinate_systems.py
+-rw-r--r--   0        0        0     2165 2024-05-15 13:12:49.088209 janim-1.0.4/janim/items/coordinate/functions.py
+-rw-r--r--   0        0        0     8330 2024-05-15 13:12:49.097183 janim-1.0.4/janim/items/coordinate/number_line.py
+-rw-r--r--   0        0        0     8784 2024-05-15 13:12:49.108152 janim-1.0.4/janim/items/geometry/arc.py
+-rw-r--r--   0        0        0     6729 2024-05-15 13:12:49.109152 janim-1.0.4/janim/items/geometry/arrow.py
+-rw-r--r--   0        0        0     7917 2024-05-15 13:12:49.118125 janim-1.0.4/janim/items/geometry/line.py
+-rw-r--r--   0        0        0     5239 2024-05-15 13:12:49.119124 janim-1.0.4/janim/items/geometry/polygon.py
+-rw-r--r--   0        0        0     5242 2024-05-20 08:38:15.648777 janim-1.0.4/janim/items/image_item.py
+-rw-r--r--   0        0        0    18981 2024-05-21 05:58:39.571823 janim-1.0.4/janim/items/item.py
+-rw-r--r--   0        0        0     3262 2024-05-15 13:12:49.122116 janim-1.0.4/janim/items/points.py
+-rw-r--r--   0        0        0     7660 2024-05-15 13:12:49.123112 janim-1.0.4/janim/items/relation.py
+-rw-r--r--   0        0        0     2071 2024-05-15 13:12:49.131090 janim-1.0.4/janim/items/shape_matchers.py
+-rw-r--r--   0        0        0     5955 2024-05-15 13:12:49.140067 janim-1.0.4/janim/items/svg/brace.py
+-rw-r--r--   0        0        0     1736 2024-05-15 13:12:49.148045 janim-1.0.4/janim/items/svg/brace.svg
+-rw-r--r--   0        0        0     4432 2024-05-21 15:03:01.842591 janim-1.0.4/janim/items/svg/svg_item.py
+-rw-r--r--   0        0        0     3090 2024-05-15 13:12:49.158019 janim-1.0.4/janim/items/svg/typst.py
+-rw-r--r--   0        0        0       40 2024-05-15 13:12:49.165001 janim-1.0.4/janim/items/svg/typst_template.typ
+-rw-r--r--   0        0        0    16286 2024-05-21 05:45:52.964782 janim-1.0.4/janim/items/text/text.py
+-rw-r--r--   0        0        0     1094 2024-05-15 13:12:49.174974 janim-1.0.4/janim/items/value_tracker.py
+-rw-r--r--   0        0        0     5357 2024-05-21 05:46:36.179638 janim-1.0.4/janim/items/vitem.py
+-rw-r--r--   0        0        0      271 2024-05-15 13:12:49.182953 janim-1.0.4/janim/logger.py
+-rw-r--r--   0        0        0     3054 2024-05-15 13:12:49.192927 janim-1.0.4/janim/render/base.py
+-rw-r--r--   0        0        0     8857 2024-05-20 08:38:15.653763 janim-1.0.4/janim/render/impl.py
+-rw-r--r--   0        0        0      448 2024-05-15 13:12:49.208887 janim-1.0.4/janim/render/shaders/dotcloud.frag.glsl
+-rw-r--r--   0        0        0     1250 2024-05-15 13:12:49.216861 janim-1.0.4/janim/render/shaders/dotcloud.geom.glsl
+-rw-r--r--   0        0        0      325 2024-05-15 13:12:49.225837 janim-1.0.4/janim/render/shaders/dotcloud.vert.glsl
+-rw-r--r--   0        0        0      180 2024-05-20 01:53:43.325091 janim-1.0.4/janim/render/shaders/image.frag.glsl
+-rw-r--r--   0        0        0      350 2024-05-15 13:12:49.247780 janim-1.0.4/janim/render/shaders/image.vert.glsl
+-rw-r--r--   0        0        0     6950 2024-05-15 13:12:49.259747 janim-1.0.4/janim/render/shaders/vitem.frag.glsl
+-rw-r--r--   0        0        0      203 2024-05-15 13:12:49.269436 janim-1.0.4/janim/render/shaders/vitem.vert.glsl
+-rw-r--r--   0        0        0     1091 2024-05-21 13:06:43.084360 janim-1.0.4/janim/render/texture.py
+-rw-r--r--   0        0        0     6971 2024-05-20 08:38:15.661774 janim-1.0.4/janim/render/writer.py
+-rw-r--r--   0        0        0      964 2024-05-15 13:12:49.278412 janim-1.0.4/janim/typing.py
+-rw-r--r--   0        0        0    17207 2024-05-15 13:12:49.289382 janim-1.0.4/janim/utils/bezier.py
+-rw-r--r--   0        0        0     5515 2024-05-15 13:12:49.297361 janim-1.0.4/janim/utils/config.py
+-rw-r--r--   0        0        0     5786 2024-05-19 13:34:44.597026 janim-1.0.4/janim/utils/data.py
+-rw-r--r--   0        0        0      637 2024-05-15 13:12:49.317308 janim-1.0.4/janim/utils/dict_ops.py
+-rw-r--r--   0        0        0     2483 2024-05-15 13:12:49.330273 janim-1.0.4/janim/utils/file_ops.py
+-rw-r--r--   0        0        0     2995 2024-05-15 13:12:49.331270 janim-1.0.4/janim/utils/font.py
+-rw-r--r--   0        0        0     6369 2024-05-15 13:12:49.392575 janim-1.0.4/janim/utils/font_manager.py
+-rw-r--r--   0        0        0     5973 2024-05-15 13:12:49.403546 janim-1.0.4/janim/utils/iterables.py
+-rw-r--r--   0        0        0     1870 2024-05-15 13:12:49.428480 janim-1.0.4/janim/utils/paths.py
+-rw-r--r--   0        0        0     2712 2024-05-21 01:50:12.474122 janim-1.0.4/janim/utils/rate_functions.py
+-rw-r--r--   0        0        0     2651 2024-05-15 13:12:49.435461 janim-1.0.4/janim/utils/refresh.py
+-rw-r--r--   0        0        0     8342 2024-05-15 13:12:49.436460 janim-1.0.4/janim/utils/signal.py
+-rw-r--r--   0        0        0     2000 2024-05-15 13:12:49.446431 janim-1.0.4/janim/utils/simple_functions.py
+-rw-r--r--   0        0        0    10068 2024-05-15 13:12:49.456405 janim-1.0.4/janim/utils/space_ops.py
+-rw-r--r--   0        0        0    18504 2024-05-20 08:38:15.667725 janim-1.0.4/logo.png
+-rw-r--r--   0        0        0     1030 2024-05-20 08:38:15.671747 janim-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 janim-1.0.4/PKG-INFO
```

### Comparing `janim-1.0.3/.readthedocs.yaml` & `janim-1.0.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/LICENSE` & `janim-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/README.md` & `janim-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/__main__.py` & `janim-1.0.4/janim/__main__.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/anims/animation.py` & `janim-1.0.4/janim/anims/animation.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/anims/composition.py` & `janim-1.0.4/janim/anims/composition.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/anims/creation.py` & `janim-1.0.4/janim/anims/creation.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/anims/display.py` & `janim-1.0.4/janim/anims/display.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/anims/fading.py` & `janim-1.0.4/janim/anims/fading.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/anims/growing.py` & `janim-1.0.4/janim/anims/growing.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/anims/indication.py` & `janim-1.0.4/janim/anims/indication.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/anims/rotation.py` & `janim-1.0.4/janim/anims/rotation.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/anims/timeline.py` & `janim-1.0.4/janim/anims/timeline.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/anims/transform.py` & `janim-1.0.4/janim/anims/transform.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/anims/updater.py` & `janim-1.0.4/janim/anims/updater.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/camera/camera.py` & `janim-1.0.4/janim/camera/camera.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/camera/camera_info.py` & `janim-1.0.4/janim/camera/camera_info.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/cli.py` & `janim-1.0.4/janim/cli.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/components/component.py` & `janim-1.0.4/janim/components/component.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/components/data.py` & `janim-1.0.4/janim/components/data.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/components/depth.py` & `janim-1.0.4/janim/components/depth.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/components/image.py` & `janim-1.0.4/janim/components/image.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/components/points.py` & `janim-1.0.4/janim/components/points.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/components/radius.py` & `janim-1.0.4/janim/components/radius.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/components/rgbas.py` & `janim-1.0.4/janim/components/rgbas.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
         特殊传参：
 
         - 当 ``colors`` 为四分量 ``RGBA`` 颜色数据时，
           则同时表示了 ``colors`` 和 ``alphas`` 二者，因此不能再传入 ``alphas`` 参数
         '''
         if color is None and alpha is None:
-            return
+            return self
 
         def is_single_color(value: Iterable) -> bool:
             if isinstance(value, str):
                 return True
             if isinstance(value[0], str):
                 return False
             return not isinstance(value[0], Iterable)
```

### Comparing `janim-1.0.3/janim/components/vpoints.py` & `janim-1.0.4/janim/components/vpoints.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/constants/colors.py` & `janim-1.0.4/janim/constants/colors.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/constants/coord.py` & `janim-1.0.4/janim/constants/coord.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/examples.py` & `janim-1.0.4/janim/examples.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/exception.py` & `janim-1.0.4/janim/exception.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/gui/anim_viewer.py` & `janim-1.0.4/janim/gui/anim_viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,16 @@
         interact: bool = False,
         parent: QWidget | None = None
     ) -> None:
         super().__init__(parent)
         self.anim = anim
         self.interact = interact
 
+        self.setWindowIcon(QIcon(os.path.join(get_janim_dir(), 'gui', 'favicon.ico')))
+
         self.setup_ui()
         self.move_to_position()
         self.socket = None
         if interact:
             self.setup_socket()
 
         self.timeline_view.value_changed.connect(self.on_value_changed)
```

### Comparing `janim-1.0.3/janim/gui/audio_player.py` & `janim-1.0.4/janim/gui/audio_player.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/gui/export.png` & `janim-1.0.4/janim/gui/export.png`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/gui/fixed_ratio_widget.py` & `janim-1.0.4/janim/gui/fixed_ratio_widget.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/gui/glwidget.py` & `janim-1.0.4/janim/gui/glwidget.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/gui/precise_timer.py` & `janim-1.0.4/janim/gui/precise_timer.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/gui/richtext_editor.py` & `janim-1.0.4/janim/gui/richtext_editor.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/gui/selector.py` & `janim-1.0.4/janim/gui/selector.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/imports.py` & `janim-1.0.4/janim/imports.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/items/audio.py` & `janim-1.0.4/janim/items/audio.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/items/boolean_ops.py` & `janim-1.0.4/janim/items/boolean_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/items/coordinate/coordinate_systems.py` & `janim-1.0.4/janim/items/coordinate/coordinate_systems.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/items/coordinate/functions.py` & `janim-1.0.4/janim/items/coordinate/functions.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/items/coordinate/number_line.py` & `janim-1.0.4/janim/items/coordinate/number_line.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/items/geometry/arc.py` & `janim-1.0.4/janim/items/geometry/arc.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/items/geometry/arrow.py` & `janim-1.0.4/janim/items/geometry/arrow.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/items/geometry/line.py` & `janim-1.0.4/janim/items/geometry/line.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/items/geometry/polygon.py` & `janim-1.0.4/janim/items/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/items/image_item.py` & `janim-1.0.4/janim/items/image_item.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/items/item.py` & `janim-1.0.4/janim/items/item.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,14 @@
     '''
 
     depth = CmptInfo(Cmpt_Depth[Self], 0)
 
     def __init__(
         self,
         *args,
-        depth: float | None = None,
         children: list[Item] | None = None,
         **kwargs
     ):
         super().__init__(*args)
 
         self.stored: bool = False
         self.stored_parents: list[Item] | None = None
@@ -93,16 +92,14 @@
         # 如果 is_temporary 为 True，则不会另外创建渲染器，而是使用共用的渲染器
         self.is_temporary: bool = False
 
         from janim.anims.timeline import Timeline
         self.timeline = Timeline.get_context(raise_exc=False)
 
         self._init_components()
-        if depth is not None:
-            self.depth.set(depth)
 
         self._astype: type[Item] | None = None
         self._astype_mock_cmpt: dict[str, Component] = {}
 
         self.renderer: Renderer | None = None
 
         if children is not None:
```

### Comparing `janim-1.0.3/janim/items/points.py` & `janim-1.0.4/janim/items/points.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/items/relation.py` & `janim-1.0.4/janim/items/relation.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/items/shape_matchers.py` & `janim-1.0.4/janim/items/shape_matchers.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/items/svg/brace.py` & `janim-1.0.4/janim/items/svg/brace.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/items/svg/brace.svg` & `janim-1.0.4/janim/items/svg/brace.svg`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/items/svg/svg_item.py` & `janim-1.0.4/janim/items/svg/svg_item.py`

 * *Files 19% similar despite different names*

```diff
@@ -36,239 +36,242 @@
 00000230: 0d0a 6465 6620 5f63 6f6e 7665 7274 5f70  ..def _convert_p
 00000240: 6f69 6e74 5f74 6f5f 3364 2878 3a20 666c  oint_to_3d(x: fl
 00000250: 6f61 742c 2079 3a20 666c 6f61 7429 202d  oat, y: float) -
 00000260: 3e20 6e70 2e6e 6461 7272 6179 3a0d 0a20  > np.ndarray:.. 
 00000270: 2020 2072 6574 7572 6e20 6e70 2e61 7272     return np.arr
 00000280: 6179 285b 782c 2079 2c20 305d 290d 0a0d  ay([x, y, 0])...
 00000290: 0a0d 0a64 6566 205f 636f 6e76 6572 745f  ...def _convert_
-000002a0: 616c 7068 615f 746f 5f66 6c6f 6174 2878  alpha_to_float(x
-000002b0: 3a20 696e 7420 7c20 4e6f 6e65 2920 2d3e  : int | None) ->
-000002c0: 2066 6c6f 6174 3a0d 0a20 2020 2072 6574   float:..    ret
-000002d0: 7572 6e20 4e6f 6e65 2069 6620 7820 6973  urn None if x is
-000002e0: 204e 6f6e 6520 656c 7365 2078 202f 2032   None else x / 2
-000002f0: 3535 0d0a 0d0a 0d0a 636c 6173 7320 5356  55......class SV
-00000300: 4749 7465 6d28 4772 6f75 705b 5649 7465  GItem(Group[VIte
-00000310: 6d5d 293a 0d0a 2020 2020 2727 270d 0a20  m]):..    '''.. 
-00000320: 2020 20e4 bca0 e585 a520 5356 4720 e696     ...... SVG ..
-00000330: 87e4 bbb6 e8b7 afe5 be84 efbc 8ce8 a7a3  ................
-00000340: e69e 90e4 b8ba e789 a9e4 bbb6 0d0a 2020  ..............  
-00000350: 2020 2727 270d 0a20 2020 2073 7667 5f70    '''..    svg_p
-00000360: 6172 745f 6465 6661 756c 745f 6b77 6172  art_default_kwar
-00000370: 6773 203d 2064 6963 7428 0d0a 2020 2020  gs = dict(..    
-00000380: 2020 2020 7374 726f 6b65 5f72 6164 6975      stroke_radiu
-00000390: 733d 312e 3020 2a20 5354 524f 4b45 5f57  s=1.0 * STROKE_W
-000003a0: 4944 5448 5f43 4f4e 5645 5253 494f 4e20  IDTH_CONVERSION 
-000003b0: 2f20 322c 0d0a 2020 2020 2020 2020 7374  / 2,..        st
-000003c0: 726f 6b65 5f63 6f6c 6f72 3d4e 6f6e 652c  roke_color=None,
-000003d0: 0d0a 2020 2020 2020 2020 7374 726f 6b65  ..        stroke
-000003e0: 5f61 6c70 6861 3d30 2c0d 0a20 2020 2020  _alpha=0,..     
-000003f0: 2020 2066 696c 6c5f 636f 6c6f 723d 4e6f     fill_color=No
-00000400: 6e65 2c0d 0a20 2020 2020 2020 2066 696c  ne,..        fil
-00000410: 6c5f 616c 7068 613d 300d 0a20 2020 2029  l_alpha=0..    )
-00000420: 0d0a 2020 2020 7669 7465 6d5f 6275 696c  ..    vitem_buil
-00000430: 6465 7273 5f6d 6170 3a20 6469 6374 5b74  ders_map: dict[t
-00000440: 7570 6c65 2c20 6c69 7374 5b56 4974 656d  uple, list[VItem
-00000450: 4275 696c 6465 725d 5d20 3d20 7b7d 0d0a  Builder]] = {}..
-00000460: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-00000470: 5f5f 2873 656c 662c 2066 696c 655f 7061  __(self, file_pa
-00000480: 7468 3a20 7374 722c 202a 2a6b 7761 7267  th: str, **kwarg
-00000490: 7329 3a0d 0a20 2020 2020 2020 2069 7465  s):..        ite
-000004a0: 6d73 203d 2073 656c 662e 6765 745f 6974  ms = self.get_it
-000004b0: 656d 735f 6672 6f6d 5f66 696c 6528 6669  ems_from_file(fi
-000004c0: 6c65 5f70 6174 6829 0d0a 0d0a 2020 2020  le_path)....    
-000004d0: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-000004e0: 6974 5f5f 282a 6974 656d 732c 202a 2a6b  it__(*items, **k
-000004f0: 7761 7267 7329 0d0a 0d0a 2020 2020 2020  wargs)....      
-00000500: 2020 7365 6c66 2856 4974 656d 292e 706f    self(VItem).po
-00000510: 696e 7473 2e73 6361 6c65 280d 0a20 2020  ints.scale(..   
-00000520: 2020 2020 2020 2020 2043 6f6e 6669 672e           Config.
-00000530: 6765 742e 7069 7865 6c5f 746f 5f66 7261  get.pixel_to_fra
-00000540: 6d65 5f72 6174 696f 202a 2044 4546 4155  me_ratio * DEFAU
-00000550: 4c54 5f53 5647 4954 454d 5f53 4341 4c45  LT_SVGITEM_SCALE
-00000560: 5f46 4143 544f 522c 0d0a 2020 2020 2020  _FACTOR,..      
-00000570: 2020 2020 2020 6162 6f75 745f 706f 696e        about_poin
-00000580: 743d 4f52 4947 494e 0d0a 2020 2020 2020  t=ORIGIN..      
-00000590: 2020 292e 666c 6970 2852 4947 4854 290d    ).flip(RIGHT).
-000005a0: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-000005b0: 6d6f 7665 5f69 6e74 6f5f 706f 7369 7469  move_into_positi
-000005c0: 6f6e 2829 0d0a 0d0a 2020 2020 6465 6620  on()....    def 
-000005d0: 6d6f 7665 5f69 6e74 6f5f 706f 7369 7469  move_into_positi
-000005e0: 6f6e 2873 656c 6629 202d 3e20 4e6f 6e65  on(self) -> None
-000005f0: 3a0d 0a20 2020 2020 2020 2070 6173 730d  :..        pass.
-00000600: 0a0d 0a20 2020 2040 7374 6174 6963 6d65  ...    @staticme
-00000610: 7468 6f64 0d0a 2020 2020 6465 6620 6765  thod..    def ge
-00000620: 745f 6974 656d 735f 6672 6f6d 5f66 696c  t_items_from_fil
-00000630: 6528 6669 6c65 5f70 6174 683a 2073 7472  e(file_path: str
-00000640: 2920 2d3e 206c 6973 745b 4974 656d 5d3a  ) -> list[Item]:
-00000650: 0d0a 2020 2020 2020 2020 2727 270d 0a20  ..        '''.. 
-00000660: 2020 2020 2020 20e8 a7a3 e69e 90e6 9687         .........
-00000670: e4bb b6e5 b9b6 e5be 97e5 88b0 e789 a9e4  ................
-00000680: bbb6 e588 97e8 a1a8 0d0a 2020 2020 2020  ..........      
-00000690: 2020 2727 270d 0a20 2020 2020 2020 2066    '''..        f
-000006a0: 696c 655f 7061 7468 203d 2066 696e 645f  ile_path = find_
-000006b0: 6669 6c65 2866 696c 655f 7061 7468 290d  file(file_path).
-000006c0: 0a20 2020 2020 2020 206d 7469 6d65 203d  .        mtime =
-000006d0: 206f 732e 7061 7468 2e67 6574 6d74 696d   os.path.getmtim
-000006e0: 6528 6669 6c65 5f70 6174 6829 0d0a 2020  e(file_path)..  
-000006f0: 2020 2020 2020 6e61 6d65 203d 206f 732e        name = os.
-00000700: 7061 7468 2e73 706c 6974 6578 7428 6f73  path.splitext(os
-00000710: 2e70 6174 682e 6261 7365 6e61 6d65 2866  .path.basename(f
-00000720: 696c 655f 7061 7468 2929 5b30 5d0d 0a20  ile_path))[0].. 
-00000730: 2020 2020 2020 206b 6579 203d 2028 6e61         key = (na
-00000740: 6d65 2c20 6d74 696d 6529 0d0a 0d0a 2020  me, mtime)....  
-00000750: 2020 2020 2020 6361 6368 6564 203d 2053        cached = S
-00000760: 5647 4974 656d 2e76 6974 656d 5f62 7569  VGItem.vitem_bui
-00000770: 6c64 6572 735f 6d61 702e 6765 7428 6b65  lders_map.get(ke
-00000780: 792c 204e 6f6e 6529 0d0a 2020 2020 2020  y, None)..      
-00000790: 2020 6966 2063 6163 6865 6420 6973 206e    if cached is n
-000007a0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-000007b0: 2020 2020 2020 7265 7475 726e 205b 6275        return [bu
-000007c0: 696c 6465 7228 2920 666f 7220 6275 696c  ilder() for buil
-000007d0: 6465 7220 696e 2063 6163 6865 645d 0d0a  der in cached]..
-000007e0: 0d0a 2020 2020 2020 2020 7376 673a 2073  ..        svg: s
-000007f0: 652e 5356 4720 3d20 7365 2e53 5647 2e70  e.SVG = se.SVG.p
-00000800: 6172 7365 2866 696c 655f 7061 7468 290d  arse(file_path).
-00000810: 0a0d 0a20 2020 2020 2020 206f 6666 7365  ...        offse
-00000820: 7420 3d20 6e70 2e61 7272 6179 285b 7376  t = np.array([sv
-00000830: 672e 7769 6474 6820 2f20 2d32 2c20 7376  g.width / -2, sv
-00000840: 672e 6865 6967 6874 202f 202d 325d 290d  g.height / -2]).
-00000850: 0a0d 0a20 2020 2020 2020 2062 7569 6c64  ...        build
-00000860: 6572 733a 206c 6973 745b 5649 7465 6d42  ers: list[VItemB
-00000870: 7569 6c64 6572 5d20 3d20 5b5d 0d0a 2020  uilder] = []..  
-00000880: 2020 2020 2020 666f 7220 7368 6170 6520        for shape 
-00000890: 696e 2073 7667 2e65 6c65 6d65 6e74 7328  in svg.elements(
-000008a0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000008b0: 6966 2069 7369 6e73 7461 6e63 6528 7368  if isinstance(sh
-000008c0: 6170 652c 2028 7365 2e47 726f 7570 2c20  ape, (se.Group, 
-000008d0: 7365 2e55 7365 2929 3a0d 0a20 2020 2020  se.Use)):..     
-000008e0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-000008f0: 6e75 650d 0a20 2020 2020 2020 2020 2020  nue..           
-00000900: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-00000910: 2873 6861 7065 2c20 7365 2e50 6174 6829  (shape, se.Path)
-00000920: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00000930: 2020 2062 7569 6c64 6572 732e 6170 7065     builders.appe
-00000940: 6e64 2853 5647 4974 656d 2e63 6f6e 7665  nd(SVGItem.conve
-00000950: 7274 5f70 6174 6828 7368 6170 652c 206f  rt_path(shape, o
-00000960: 6666 7365 7429 290d 0a20 2020 2020 2020  ffset))..       
-00000970: 2020 2020 2065 6c69 6620 7479 7065 2873       elif type(s
-00000980: 6861 7065 2920 6973 2073 652e 5356 4745  hape) is se.SVGE
-00000990: 6c65 6d65 6e74 3a0d 0a20 2020 2020 2020  lement:..       
-000009a0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-000009b0: 650d 0a20 2020 2020 2020 2020 2020 2065  e..            e
-000009c0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-000009d0: 2020 2020 2020 6c6f 672e 7761 726e 696e        log.warnin
-000009e0: 6728 6627 556e 7375 7070 6f72 7465 6420  g(f'Unsupported 
-000009f0: 656c 656d 656e 7420 7479 7065 3a20 7b74  element type: {t
-00000a00: 7970 6528 7368 6170 6529 7d27 290d 0a0d  ype(shape)}')...
-00000a10: 0a20 2020 2020 2020 2053 5647 4974 656d  .        SVGItem
-00000a20: 2e76 6974 656d 5f62 7569 6c64 6572 735f  .vitem_builders_
-00000a30: 6d61 705b 6b65 795d 203d 2062 7569 6c64  map[key] = build
-00000a40: 6572 730d 0a20 2020 2020 2020 2072 6574  ers..        ret
-00000a50: 7572 6e20 5b62 7569 6c64 6572 2829 2066  urn [builder() f
-00000a60: 6f72 2062 7569 6c64 6572 2069 6e20 6275  or builder in bu
-00000a70: 696c 6465 7273 5d0d 0a0d 0a20 2020 2040  ilders]....    @
-00000a80: 7374 6174 6963 6d65 7468 6f64 0d0a 2020  staticmethod..  
-00000a90: 2020 6465 6620 636f 6e76 6572 745f 7061    def convert_pa
-00000aa0: 7468 2870 6174 683a 2073 652e 5061 7468  th(path: se.Path
-00000ab0: 2c20 6f66 6673 6574 3a20 6e70 2e6e 6461  , offset: np.nda
-00000ac0: 7272 6179 2920 2d3e 2056 4974 656d 4275  rray) -> VItemBu
-00000ad0: 696c 6465 723a 0d0a 2020 2020 2020 2020  ilder:..        
-00000ae0: 6275 696c 6465 7220 3d20 5061 7468 4275  builder = PathBu
-00000af0: 696c 6465 7228 290d 0a20 2020 2020 2020  ilder()..       
-00000b00: 2073 6567 6d65 6e74 5f63 6c61 7373 5f74   segment_class_t
-00000b10: 6f5f 6675 6e63 5f6d 6170 203d 207b 0d0a  o_func_map = {..
-00000b20: 2020 2020 2020 2020 2020 2020 7365 2e4d              se.M
-00000b30: 6f76 653a 2028 6275 696c 6465 722e 6d6f  ove: (builder.mo
-00000b40: 7665 5f74 6f2c 2028 2765 6e64 272c 2929  ve_to, ('end',))
-00000b50: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
-00000b60: 652e 436c 6f73 653a 2028 6275 696c 6465  e.Close: (builde
-00000b70: 722e 636c 6f73 655f 7061 7468 2c20 2829  r.close_path, ()
-00000b80: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-00000b90: 7365 2e4c 696e 653a 2028 6275 696c 6465  se.Line: (builde
-00000ba0: 722e 6c69 6e65 5f74 6f2c 2028 2765 6e64  r.line_to, ('end
-00000bb0: 272c 2929 2c0d 0a20 2020 2020 2020 2020  ',)),..         
-00000bc0: 2020 2073 652e 5175 6164 7261 7469 6342     se.QuadraticB
-00000bd0: 657a 6965 723a 2028 6275 696c 6465 722e  ezier: (builder.
-00000be0: 636f 6e69 635f 746f 2c20 2827 636f 6e74  conic_to, ('cont
-00000bf0: 726f 6c27 2c20 2765 6e64 2729 292c 0d0a  rol', 'end')),..
-00000c00: 2020 2020 2020 2020 2020 2020 7365 2e43              se.C
-00000c10: 7562 6963 4265 7a69 6572 3a20 2862 7569  ubicBezier: (bui
-00000c20: 6c64 6572 2e63 7562 6963 5f74 6f2c 2028  lder.cubic_to, (
-00000c30: 2763 6f6e 7472 6f6c 3127 2c20 2763 6f6e  'control1', 'con
-00000c40: 7472 6f6c 3227 2c20 2765 6e64 2729 292c  trol2', 'end')),
-00000c50: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00000c60: 2e41 7263 3a20 286c 616d 6264 6120 7365  .Arc: (lambda se
-00000c70: 676d 656e 743a 2062 7569 6c64 6572 2e61  gment: builder.a
-00000c80: 7263 5f74 6f28 5f63 6f6e 7665 7274 5f70  rc_to(_convert_p
-00000c90: 6f69 6e74 5f74 6f5f 3364 282a 7365 676d  oint_to_3d(*segm
-00000ca0: 656e 742e 656e 6429 2c20 7365 676d 656e  ent.end), segmen
-00000cb0: 742e 7377 6565 7029 2c20 4e6f 6e65 292c  t.sweep), None),
-00000cc0: 0d0a 2020 2020 2020 2020 7d0d 0a0d 0a20  ..        }.... 
-00000cd0: 2020 2020 2020 2066 6f72 2073 6567 6d65         for segme
-00000ce0: 6e74 2069 6e20 7061 7468 3a0d 0a20 2020  nt in path:..   
-00000cf0: 2020 2020 2020 2020 2073 6567 6d65 6e74           segment
-00000d00: 5f63 6c61 7373 203d 2073 6567 6d65 6e74  _class = segment
-00000d10: 2e5f 5f63 6c61 7373 5f5f 0d0a 2020 2020  .__class__..    
-00000d20: 2020 2020 2020 2020 6675 6e63 2c20 6174          func, at
-00000d30: 7472 5f6e 616d 6573 203d 2073 6567 6d65  tr_names = segme
-00000d40: 6e74 5f63 6c61 7373 5f74 6f5f 6675 6e63  nt_class_to_func
-00000d50: 5f6d 6170 5b73 6567 6d65 6e74 5f63 6c61  _map[segment_cla
-00000d60: 7373 5d0d 0a20 2020 2020 2020 2020 2020  ss]..           
-00000d70: 2069 6620 6174 7472 5f6e 616d 6573 2069   if attr_names i
-00000d80: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-00000d90: 2020 2020 2020 2020 2066 756e 6328 7365           func(se
-00000da0: 676d 656e 7429 0d0a 2020 2020 2020 2020  gment)..        
-00000db0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00000dc0: 2020 2020 2020 2020 2020 2070 6f69 6e74             point
-00000dd0: 7320 3d20 5b0d 0a20 2020 2020 2020 2020  s = [..         
-00000de0: 2020 2020 2020 2020 2020 205f 636f 6e76             _conv
-00000df0: 6572 745f 706f 696e 745f 746f 5f33 6428  ert_point_to_3d(
-00000e00: 2a67 6574 6174 7472 2873 6567 6d65 6e74  *getattr(segment
-00000e10: 2c20 6174 7472 5f6e 616d 6529 290d 0a20  , attr_name)).. 
-00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e30: 2020 2066 6f72 2061 7474 725f 6e61 6d65     for attr_name
-00000e40: 2069 6e20 6174 7472 5f6e 616d 6573 0d0a   in attr_names..
-00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e60: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00000e70: 2020 2066 756e 6328 2a70 6f69 6e74 7329     func(*points)
-00000e80: 0d0a 0d0a 2020 2020 2020 2020 7669 7465  ....        vite
-00000e90: 6d5f 7374 796c 6573 203d 2064 6963 7428  m_styles = dict(
-00000ea0: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-00000eb0: 726f 6b65 5f72 6164 6975 733d 7061 7468  roke_radius=path
-00000ec0: 2e73 7472 6f6b 655f 7769 6474 6820 2a20  .stroke_width * 
-00000ed0: 5354 524f 4b45 5f57 4944 5448 5f43 4f4e  STROKE_WIDTH_CON
-00000ee0: 5645 5253 494f 4e20 2f20 322c 0d0a 2020  VERSION / 2,..  
-00000ef0: 2020 2020 2020 2020 2020 7374 726f 6b65            stroke
-00000f00: 5f63 6f6c 6f72 3d70 6174 682e 7374 726f  _color=path.stro
-00000f10: 6b65 2e68 6578 2c0d 0a20 2020 2020 2020  ke.hex,..       
-00000f20: 2020 2020 2073 7472 6f6b 655f 616c 7068       stroke_alph
-00000f30: 613d 5f63 6f6e 7665 7274 5f61 6c70 6861  a=_convert_alpha
-00000f40: 5f74 6f5f 666c 6f61 7428 7061 7468 2e73  _to_float(path.s
-00000f50: 7472 6f6b 652e 616c 7068 6129 2c0d 0a20  troke.alpha),.. 
-00000f60: 2020 2020 2020 2020 2020 2066 696c 6c5f             fill_
-00000f70: 636f 6c6f 723d 7061 7468 2e66 696c 6c2e  color=path.fill.
-00000f80: 6865 782c 0d0a 2020 2020 2020 2020 2020  hex,..          
-00000f90: 2020 6669 6c6c 5f61 6c70 6861 3d5f 636f    fill_alpha=_co
-00000fa0: 6e76 6572 745f 616c 7068 615f 746f 5f66  nvert_alpha_to_f
-00000fb0: 6c6f 6174 2870 6174 682e 6669 6c6c 2e61  loat(path.fill.a
-00000fc0: 6c70 6861 290d 0a20 2020 2020 2020 2029  lpha)..        )
-00000fd0: 0d0a 2020 2020 2020 2020 7669 7465 6d5f  ..        vitem_
-00000fe0: 706f 696e 7473 203d 2062 7569 6c64 6572  points = builder
-00000ff0: 2e67 6574 2829 0d0a 2020 2020 2020 2020  .get()..        
-00001000: 7669 7465 6d5f 706f 696e 7473 5b3a 2c20  vitem_points[:, 
-00001010: 3a32 5d20 2b3d 206f 6666 7365 740d 0a0d  :2] += offset...
-00001020: 0a20 2020 2020 2020 2064 6566 2076 6974  .        def vit
-00001030: 656d 5f62 7569 6c64 6572 2829 202d 3e20  em_builder() -> 
-00001040: 5649 7465 6d3a 0d0a 2020 2020 2020 2020  VItem:..        
-00001050: 2020 2020 7669 7465 6d20 3d20 5649 7465      vitem = VIte
-00001060: 6d28 2a2a 5356 4749 7465 6d2e 7376 675f  m(**SVGItem.svg_
-00001070: 7061 7274 5f64 6566 6175 6c74 5f6b 7761  part_default_kwa
-00001080: 7267 7329 0d0a 2020 2020 2020 2020 2020  rgs)..          
-00001090: 2020 7669 7465 6d2e 7365 745f 7374 796c    vitem.set_styl
-000010a0: 6528 2a2a 7669 7465 6d5f 7374 796c 6573  e(**vitem_styles
-000010b0: 290d 0a20 2020 2020 2020 2020 2020 2076  )..            v
-000010c0: 6974 656d 2e70 6f69 6e74 732e 7365 7428  item.points.set(
-000010d0: 7669 7465 6d5f 706f 696e 7473 290d 0a20  vitem_points).. 
-000010e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000010f0: 6e20 7669 7465 6d0d 0a0d 0a20 2020 2020  n vitem....     
-00001100: 2020 2072 6574 7572 6e20 7669 7465 6d5f     return vitem_
-00001110: 6275 696c 6465 720d 0a                   builder..
+000002a0: 6f70 6163 6974 7928 783a 2066 6c6f 6174  opacity(x: float
+000002b0: 207c 204e 6f6e 6529 202d 3e20 666c 6f61   | None) -> floa
+000002c0: 743a 0d0a 2020 2020 7265 7475 726e 2030  t:..    return 0
+000002d0: 2e20 6966 2078 2069 7320 4e6f 6e65 2065  . if x is None e
+000002e0: 6c73 6520 780d 0a0d 0a0d 0a63 6c61 7373  lse x......class
+000002f0: 2053 5647 4974 656d 2847 726f 7570 5b56   SVGItem(Group[V
+00000300: 4974 656d 5d29 3a0d 0a20 2020 2027 2727  Item]):..    '''
+00000310: 0d0a 2020 2020 e4bc a0e5 85a5 2053 5647  ..    ...... SVG
+00000320: 20e6 9687 e4bb b6e8 b7af e5be 84ef bc8c   ...............
+00000330: e8a7 a3e6 9e90 e4b8 bae7 89a9 e4bb b60d  ................
+00000340: 0a20 2020 2027 2727 0d0a 2020 2020 7376  .    '''..    sv
+00000350: 675f 7061 7274 5f64 6566 6175 6c74 5f6b  g_part_default_k
+00000360: 7761 7267 7320 3d20 6469 6374 280d 0a20  wargs = dict(.. 
+00000370: 2020 2020 2020 2073 7472 6f6b 655f 7261         stroke_ra
+00000380: 6469 7573 3d31 2e30 202a 2053 5452 4f4b  dius=1.0 * STROK
+00000390: 455f 5749 4454 485f 434f 4e56 4552 5349  E_WIDTH_CONVERSI
+000003a0: 4f4e 202f 2032 2c0d 0a20 2020 2020 2020  ON / 2,..       
+000003b0: 2073 7472 6f6b 655f 636f 6c6f 723d 4e6f   stroke_color=No
+000003c0: 6e65 2c0d 0a20 2020 2020 2020 2073 7472  ne,..        str
+000003d0: 6f6b 655f 616c 7068 613d 302c 0d0a 2020  oke_alpha=0,..  
+000003e0: 2020 2020 2020 6669 6c6c 5f63 6f6c 6f72        fill_color
+000003f0: 3d4e 6f6e 652c 0d0a 2020 2020 2020 2020  =None,..        
+00000400: 6669 6c6c 5f61 6c70 6861 3d30 0d0a 2020  fill_alpha=0..  
+00000410: 2020 290d 0a20 2020 2076 6974 656d 5f62    )..    vitem_b
+00000420: 7569 6c64 6572 735f 6d61 703a 2064 6963  uilders_map: dic
+00000430: 745b 7475 706c 652c 206c 6973 745b 5649  t[tuple, list[VI
+00000440: 7465 6d42 7569 6c64 6572 5d5d 203d 207b  temBuilder]] = {
+00000450: 7d0d 0a0d 0a20 2020 2064 6566 205f 5f69  }....    def __i
+00000460: 6e69 745f 5f28 7365 6c66 2c20 6669 6c65  nit__(self, file
+00000470: 5f70 6174 683a 2073 7472 2c20 2a2a 6b77  _path: str, **kw
+00000480: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
+00000490: 6974 656d 7320 3d20 7365 6c66 2e67 6574  items = self.get
+000004a0: 5f69 7465 6d73 5f66 726f 6d5f 6669 6c65  _items_from_file
+000004b0: 2866 696c 655f 7061 7468 290d 0a0d 0a20  (file_path).... 
+000004c0: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
+000004d0: 5f69 6e69 745f 5f28 2a69 7465 6d73 2c20  _init__(*items, 
+000004e0: 2a2a 6b77 6172 6773 290d 0a0d 0a20 2020  **kwargs)....   
+000004f0: 2020 2020 2073 656c 6628 5649 7465 6d29       self(VItem)
+00000500: 2e70 6f69 6e74 732e 7363 616c 6528 0d0a  .points.scale(..
+00000510: 2020 2020 2020 2020 2020 2020 436f 6e66              Conf
+00000520: 6967 2e67 6574 2e70 6978 656c 5f74 6f5f  ig.get.pixel_to_
+00000530: 6672 616d 655f 7261 7469 6f20 2a20 4445  frame_ratio * DE
+00000540: 4641 554c 545f 5356 4749 5445 4d5f 5343  FAULT_SVGITEM_SC
+00000550: 414c 455f 4641 4354 4f52 2c0d 0a20 2020  ALE_FACTOR,..   
+00000560: 2020 2020 2020 2020 2061 626f 7574 5f70           about_p
+00000570: 6f69 6e74 3d4f 5249 4749 4e0d 0a20 2020  oint=ORIGIN..   
+00000580: 2020 2020 2029 2e66 6c69 7028 5249 4748       ).flip(RIGH
+00000590: 5429 0d0a 0d0a 2020 2020 2020 2020 7365  T)....        se
+000005a0: 6c66 2e6d 6f76 655f 696e 746f 5f70 6f73  lf.move_into_pos
+000005b0: 6974 696f 6e28 290d 0a0d 0a20 2020 2064  ition()....    d
+000005c0: 6566 206d 6f76 655f 696e 746f 5f70 6f73  ef move_into_pos
+000005d0: 6974 696f 6e28 7365 6c66 2920 2d3e 204e  ition(self) -> N
+000005e0: 6f6e 653a 0d0a 2020 2020 2020 2020 7061  one:..        pa
+000005f0: 7373 0d0a 0d0a 2020 2020 4073 7461 7469  ss....    @stati
+00000600: 636d 6574 686f 640d 0a20 2020 2064 6566  cmethod..    def
+00000610: 2067 6574 5f69 7465 6d73 5f66 726f 6d5f   get_items_from_
+00000620: 6669 6c65 2866 696c 655f 7061 7468 3a20  file(file_path: 
+00000630: 7374 7229 202d 3e20 6c69 7374 5b49 7465  str) -> list[Ite
+00000640: 6d5d 3a0d 0a20 2020 2020 2020 2027 2727  m]:..        '''
+00000650: 0d0a 2020 2020 2020 2020 e8a7 a3e6 9e90  ..        ......
+00000660: e696 87e4 bbb6 e5b9 b6e5 be97 e588 b0e7  ................
+00000670: 89a9 e4bb b6e5 8897 e8a1 a80d 0a20 2020  .............   
+00000680: 2020 2020 2027 2727 0d0a 2020 2020 2020       '''..      
+00000690: 2020 6669 6c65 5f70 6174 6820 3d20 6669    file_path = fi
+000006a0: 6e64 5f66 696c 6528 6669 6c65 5f70 6174  nd_file(file_pat
+000006b0: 6829 0d0a 2020 2020 2020 2020 6d74 696d  h)..        mtim
+000006c0: 6520 3d20 6f73 2e70 6174 682e 6765 746d  e = os.path.getm
+000006d0: 7469 6d65 2866 696c 655f 7061 7468 290d  time(file_path).
+000006e0: 0a20 2020 2020 2020 206e 616d 6520 3d20  .        name = 
+000006f0: 6f73 2e70 6174 682e 7370 6c69 7465 7874  os.path.splitext
+00000700: 286f 732e 7061 7468 2e62 6173 656e 616d  (os.path.basenam
+00000710: 6528 6669 6c65 5f70 6174 6829 295b 305d  e(file_path))[0]
+00000720: 0d0a 2020 2020 2020 2020 6b65 7920 3d20  ..        key = 
+00000730: 286e 616d 652c 206d 7469 6d65 290d 0a0d  (name, mtime)...
+00000740: 0a20 2020 2020 2020 2063 6163 6865 6420  .        cached 
+00000750: 3d20 5356 4749 7465 6d2e 7669 7465 6d5f  = SVGItem.vitem_
+00000760: 6275 696c 6465 7273 5f6d 6170 2e67 6574  builders_map.get
+00000770: 286b 6579 2c20 4e6f 6e65 290d 0a20 2020  (key, None)..   
+00000780: 2020 2020 2069 6620 6361 6368 6564 2069       if cached i
+00000790: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+000007a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000007b0: 5b62 7569 6c64 6572 2829 2066 6f72 2062  [builder() for b
+000007c0: 7569 6c64 6572 2069 6e20 6361 6368 6564  uilder in cached
+000007d0: 5d0d 0a0d 0a20 2020 2020 2020 2073 7667  ]....        svg
+000007e0: 3a20 7365 2e53 5647 203d 2073 652e 5356  : se.SVG = se.SV
+000007f0: 472e 7061 7273 6528 6669 6c65 5f70 6174  G.parse(file_pat
+00000800: 6829 0d0a 0d0a 2020 2020 2020 2020 6f66  h)....        of
+00000810: 6673 6574 203d 206e 702e 6172 7261 7928  fset = np.array(
+00000820: 5b73 7667 2e77 6964 7468 202f 202d 322c  [svg.width / -2,
+00000830: 2073 7667 2e68 6569 6768 7420 2f20 2d32   svg.height / -2
+00000840: 5d29 0d0a 0d0a 2020 2020 2020 2020 6275  ])....        bu
+00000850: 696c 6465 7273 3a20 6c69 7374 5b56 4974  ilders: list[VIt
+00000860: 656d 4275 696c 6465 725d 203d 205b 5d0d  emBuilder] = [].
+00000870: 0a20 2020 2020 2020 2066 6f72 2073 6861  .        for sha
+00000880: 7065 2069 6e20 7376 672e 656c 656d 656e  pe in svg.elemen
+00000890: 7473 2829 3a0d 0a20 2020 2020 2020 2020  ts():..         
+000008a0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+000008b0: 2873 6861 7065 2c20 2873 652e 4772 6f75  (shape, (se.Grou
+000008c0: 702c 2073 652e 5573 6529 293a 0d0a 2020  p, se.Use)):..  
+000008d0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000008e0: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
+000008f0: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+00000900: 6e63 6528 7368 6170 652c 2073 652e 5061  nce(shape, se.Pa
+00000910: 7468 293a 0d0a 2020 2020 2020 2020 2020  th):..          
+00000920: 2020 2020 2020 6275 696c 6465 7273 2e61        builders.a
+00000930: 7070 656e 6428 5356 4749 7465 6d2e 636f  ppend(SVGItem.co
+00000940: 6e76 6572 745f 7061 7468 2873 6861 7065  nvert_path(shape
+00000950: 2c20 6f66 6673 6574 2929 0d0a 2020 2020  , offset))..    
+00000960: 2020 2020 2020 2020 656c 6966 2074 7970          elif typ
+00000970: 6528 7368 6170 6529 2069 7320 7365 2e53  e(shape) is se.S
+00000980: 5647 456c 656d 656e 743a 0d0a 2020 2020  VGElement:..    
+00000990: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+000009a0: 696e 7565 0d0a 2020 2020 2020 2020 2020  inue..          
+000009b0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+000009c0: 2020 2020 2020 2020 206c 6f67 2e77 6172           log.war
+000009d0: 6e69 6e67 2866 2755 6e73 7570 706f 7274  ning(f'Unsupport
+000009e0: 6564 2065 6c65 6d65 6e74 2074 7970 653a  ed element type:
+000009f0: 207b 7479 7065 2873 6861 7065 297d 2729   {type(shape)}')
+00000a00: 0d0a 0d0a 2020 2020 2020 2020 5356 4749  ....        SVGI
+00000a10: 7465 6d2e 7669 7465 6d5f 6275 696c 6465  tem.vitem_builde
+00000a20: 7273 5f6d 6170 5b6b 6579 5d20 3d20 6275  rs_map[key] = bu
+00000a30: 696c 6465 7273 0d0a 2020 2020 2020 2020  ilders..        
+00000a40: 7265 7475 726e 205b 6275 696c 6465 7228  return [builder(
+00000a50: 2920 666f 7220 6275 696c 6465 7220 696e  ) for builder in
+00000a60: 2062 7569 6c64 6572 735d 0d0a 0d0a 2020   builders]....  
+00000a70: 2020 4073 7461 7469 636d 6574 686f 640d    @staticmethod.
+00000a80: 0a20 2020 2064 6566 2063 6f6e 7665 7274  .    def convert
+00000a90: 5f70 6174 6828 7061 7468 3a20 7365 2e50  _path(path: se.P
+00000aa0: 6174 682c 206f 6666 7365 743a 206e 702e  ath, offset: np.
+00000ab0: 6e64 6172 7261 7929 202d 3e20 5649 7465  ndarray) -> VIte
+00000ac0: 6d42 7569 6c64 6572 3a0d 0a20 2020 2020  mBuilder:..     
+00000ad0: 2020 2062 7569 6c64 6572 203d 2050 6174     builder = Pat
+00000ae0: 6842 7569 6c64 6572 2829 0d0a 2020 2020  hBuilder()..    
+00000af0: 2020 2020 7365 676d 656e 745f 636c 6173      segment_clas
+00000b00: 735f 746f 5f66 756e 635f 6d61 7020 3d20  s_to_func_map = 
+00000b10: 7b0d 0a20 2020 2020 2020 2020 2020 2073  {..            s
+00000b20: 652e 4d6f 7665 3a20 2862 7569 6c64 6572  e.Move: (builder
+00000b30: 2e6d 6f76 655f 746f 2c20 2827 656e 6427  .move_to, ('end'
+00000b40: 2c29 292c 0d0a 2020 2020 2020 2020 2020  ,)),..          
+00000b50: 2020 7365 2e43 6c6f 7365 3a20 2862 7569    se.Close: (bui
+00000b60: 6c64 6572 2e63 6c6f 7365 5f70 6174 682c  lder.close_path,
+00000b70: 2028 2929 2c0d 0a20 2020 2020 2020 2020   ()),..         
+00000b80: 2020 2073 652e 4c69 6e65 3a20 2862 7569     se.Line: (bui
+00000b90: 6c64 6572 2e6c 696e 655f 746f 2c20 2827  lder.line_to, ('
+00000ba0: 656e 6427 2c29 292c 0d0a 2020 2020 2020  end',)),..      
+00000bb0: 2020 2020 2020 7365 2e51 7561 6472 6174        se.Quadrat
+00000bc0: 6963 4265 7a69 6572 3a20 2862 7569 6c64  icBezier: (build
+00000bd0: 6572 2e63 6f6e 6963 5f74 6f2c 2028 2763  er.conic_to, ('c
+00000be0: 6f6e 7472 6f6c 272c 2027 656e 6427 2929  ontrol', 'end'))
+00000bf0: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
+00000c00: 652e 4375 6269 6342 657a 6965 723a 2028  e.CubicBezier: (
+00000c10: 6275 696c 6465 722e 6375 6269 635f 746f  builder.cubic_to
+00000c20: 2c20 2827 636f 6e74 726f 6c31 272c 2027  , ('control1', '
+00000c30: 636f 6e74 726f 6c32 272c 2027 656e 6427  control2', 'end'
+00000c40: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+00000c50: 2073 652e 4172 633a 2028 6c61 6d62 6461   se.Arc: (lambda
+00000c60: 2073 6567 6d65 6e74 3a20 6275 696c 6465   segment: builde
+00000c70: 722e 6172 635f 746f 285f 636f 6e76 6572  r.arc_to(_conver
+00000c80: 745f 706f 696e 745f 746f 5f33 6428 2a73  t_point_to_3d(*s
+00000c90: 6567 6d65 6e74 2e65 6e64 292c 2073 6567  egment.end), seg
+00000ca0: 6d65 6e74 2e73 7765 6570 292c 204e 6f6e  ment.sweep), Non
+00000cb0: 6529 2c0d 0a20 2020 2020 2020 207d 0d0a  e),..        }..
+00000cc0: 0d0a 2020 2020 2020 2020 666f 7220 7365  ..        for se
+00000cd0: 676d 656e 7420 696e 2070 6174 683a 0d0a  gment in path:..
+00000ce0: 2020 2020 2020 2020 2020 2020 7365 676d              segm
+00000cf0: 656e 745f 636c 6173 7320 3d20 7365 676d  ent_class = segm
+00000d00: 656e 742e 5f5f 636c 6173 735f 5f0d 0a20  ent.__class__.. 
+00000d10: 2020 2020 2020 2020 2020 2066 756e 632c             func,
+00000d20: 2061 7474 725f 6e61 6d65 7320 3d20 7365   attr_names = se
+00000d30: 676d 656e 745f 636c 6173 735f 746f 5f66  gment_class_to_f
+00000d40: 756e 635f 6d61 705b 7365 676d 656e 745f  unc_map[segment_
+00000d50: 636c 6173 735d 0d0a 2020 2020 2020 2020  class]..        
+00000d60: 2020 2020 6966 2061 7474 725f 6e61 6d65      if attr_name
+00000d70: 7320 6973 204e 6f6e 653a 0d0a 2020 2020  s is None:..    
+00000d80: 2020 2020 2020 2020 2020 2020 6675 6e63              func
+00000d90: 2873 6567 6d65 6e74 290d 0a20 2020 2020  (segment)..     
+00000da0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00000db0: 2020 2020 2020 2020 2020 2020 2020 706f                po
+00000dc0: 696e 7473 203d 205b 0d0a 2020 2020 2020  ints = [..      
+00000dd0: 2020 2020 2020 2020 2020 2020 2020 5f63                _c
+00000de0: 6f6e 7665 7274 5f70 6f69 6e74 5f74 6f5f  onvert_point_to_
+00000df0: 3364 282a 6765 7461 7474 7228 7365 676d  3d(*getattr(segm
+00000e00: 656e 742c 2061 7474 725f 6e61 6d65 2929  ent, attr_name))
+00000e10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000e20: 2020 2020 2020 666f 7220 6174 7472 5f6e        for attr_n
+00000e30: 616d 6520 696e 2061 7474 725f 6e61 6d65  ame in attr_name
+00000e40: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00000e50: 2020 205d 0d0a 2020 2020 2020 2020 2020     ]..          
+00000e60: 2020 2020 2020 6675 6e63 282a 706f 696e        func(*poin
+00000e70: 7473 290d 0a0d 0a20 2020 2020 2020 206f  ts)....        o
+00000e80: 7061 6369 7479 203d 2066 6c6f 6174 2870  pacity = float(p
+00000e90: 6174 682e 7661 6c75 6573 2e67 6574 2827  ath.values.get('
+00000ea0: 6f70 6163 6974 7927 2c20 3129 290d 0a0d  opacity', 1))...
+00000eb0: 0a20 2020 2020 2020 2076 6974 656d 5f73  .        vitem_s
+00000ec0: 7479 6c65 7320 3d20 6469 6374 280d 0a20  tyles = dict(.. 
+00000ed0: 2020 2020 2020 2020 2020 2073 7472 6f6b             strok
+00000ee0: 655f 7261 6469 7573 3d70 6174 682e 7374  e_radius=path.st
+00000ef0: 726f 6b65 5f77 6964 7468 202a 2053 5452  roke_width * STR
+00000f00: 4f4b 455f 5749 4454 485f 434f 4e56 4552  OKE_WIDTH_CONVER
+00000f10: 5349 4f4e 202f 2032 2c0d 0a20 2020 2020  SION / 2,..     
+00000f20: 2020 2020 2020 2073 7472 6f6b 655f 636f         stroke_co
+00000f30: 6c6f 723d 7061 7468 2e73 7472 6f6b 652e  lor=path.stroke.
+00000f40: 6865 782c 0d0a 2020 2020 2020 2020 2020  hex,..          
+00000f50: 2020 7374 726f 6b65 5f61 6c70 6861 3d5f    stroke_alpha=_
+00000f60: 636f 6e76 6572 745f 6f70 6163 6974 7928  convert_opacity(
+00000f70: 7061 7468 2e73 7472 6f6b 652e 6f70 6163  path.stroke.opac
+00000f80: 6974 7929 202a 206f 7061 6369 7479 2c0d  ity) * opacity,.
+00000f90: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+00000fa0: 6c5f 636f 6c6f 723d 7061 7468 2e66 696c  l_color=path.fil
+00000fb0: 6c2e 6865 782c 0d0a 2020 2020 2020 2020  l.hex,..        
+00000fc0: 2020 2020 6669 6c6c 5f61 6c70 6861 3d5f      fill_alpha=_
+00000fd0: 636f 6e76 6572 745f 6f70 6163 6974 7928  convert_opacity(
+00000fe0: 7061 7468 2e66 696c 6c2e 6f70 6163 6974  path.fill.opacit
+00000ff0: 7929 202a 206f 7061 6369 7479 0d0a 2020  y) * opacity..  
+00001000: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00001010: 2076 6974 656d 5f70 6f69 6e74 7320 3d20   vitem_points = 
+00001020: 6275 696c 6465 722e 6765 7428 290d 0a20  builder.get().. 
+00001030: 2020 2020 2020 2076 6974 656d 5f70 6f69         vitem_poi
+00001040: 6e74 735b 3a2c 203a 325d 202b 3d20 6f66  nts[:, :2] += of
+00001050: 6673 6574 0d0a 0d0a 2020 2020 2020 2020  fset....        
+00001060: 6465 6620 7669 7465 6d5f 6275 696c 6465  def vitem_builde
+00001070: 7228 2920 2d3e 2056 4974 656d 3a0d 0a20  r() -> VItem:.. 
+00001080: 2020 2020 2020 2020 2020 2076 6974 656d             vitem
+00001090: 203d 2056 4974 656d 282a 2a53 5647 4974   = VItem(**SVGIt
+000010a0: 656d 2e73 7667 5f70 6172 745f 6465 6661  em.svg_part_defa
+000010b0: 756c 745f 6b77 6172 6773 290d 0a20 2020  ult_kwargs)..   
+000010c0: 2020 2020 2020 2020 2076 6974 656d 2e73           vitem.s
+000010d0: 6574 5f73 7479 6c65 282a 2a76 6974 656d  et_style(**vitem
+000010e0: 5f73 7479 6c65 7329 0d0a 2020 2020 2020  _styles)..      
+000010f0: 2020 2020 2020 7669 7465 6d2e 706f 696e        vitem.poin
+00001100: 7473 2e73 6574 2876 6974 656d 5f70 6f69  ts.set(vitem_poi
+00001110: 6e74 7329 0d0a 2020 2020 2020 2020 2020  nts)..          
+00001120: 2020 7265 7475 726e 2076 6974 656d 0d0a    return vitem..
+00001130: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00001140: 2076 6974 656d 5f62 7569 6c64 6572 0d0a   vitem_builder..
```

### Comparing `janim-1.0.3/janim/items/svg/typst.py` & `janim-1.0.4/janim/items/svg/typst.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/items/text/text.py` & `janim-1.0.4/janim/items/text/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -426,15 +426,15 @@
 
                 char.apply_act_list(act_params_map)
                 text_at += 1
 
             text_at += 1
 
 
-class Title(Text):
+class Title(Group):
     '''
     标题
 
     - ``include_underline=True`` 会添加下划线（默认添加）
     - ``underline_width`` 下划线的长度（默认屏幕宽 - 2 个单位）
     - ``match_underline_width_to_text=True`` 时将下划线的长度和文字匹配（默认为 ``False``）
     '''
@@ -443,32 +443,39 @@
         text: str,
         font: str | Iterable[str] = [],
         font_size: float = DEFAULT_FONT_SIZE,
         include_underline: bool = True,
         underline_width: float | None = None,
         underline_buff: float = MED_SMALL_BUFF,
         match_underline_width_to_text: bool = False,
+        depth: float | None = None,
         **kwargs
     ):
-        super().__init__(text, font=font, font_size=font_size, **kwargs)
-        self.points.to_border(UP)
+        txt = Text(text, font=font, font_size=font_size, **kwargs)
+        txt.points.to_border(UP)
 
-        if underline_width is None and not match_underline_width_to_text:
-            underline_width = Config.get.frame_width - 2
+        super().__init__(txt)
+        self.txt = txt
 
         if include_underline:
+            if underline_width is None and not match_underline_width_to_text:
+                underline_width = Config.get.frame_width - 2
+
             underline = Line(LEFT, RIGHT)
-            underline.points.next_to(self, DOWN, buff=underline_buff)
+            underline.points.next_to(txt, DOWN, buff=underline_buff)
             if match_underline_width_to_text:
-                underline.points.set_width(self.points.box.width)
+                underline.points.set_width(txt.points.box.width)
             else:
                 underline.points.set_width(underline_width)
+
             self.add(underline)
             self.underline = underline
 
+        self.depth.arrange(depth)
+
 
 class SourceDisplayer(Text):
     '''
     显示 ``obj`` 的源代码
     '''
     def __init__(
         self,
```

### Comparing `janim-1.0.3/janim/items/value_tracker.py` & `janim-1.0.4/janim/items/value_tracker.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/items/vitem.py` & `janim-1.0.4/janim/items/vitem.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/render/base.py` & `janim-1.0.4/janim/render/base.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/render/impl.py` & `janim-1.0.4/janim/render/impl.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/render/shaders/dotcloud.geom.glsl` & `janim-1.0.4/janim/render/shaders/dotcloud.geom.glsl`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/render/shaders/vitem.frag.glsl` & `janim-1.0.4/janim/render/shaders/vitem.frag.glsl`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/render/texture.py` & `janim-1.0.4/janim/render/texture.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,20 +22,21 @@
     return img
 
 
 img_to_texture_map: dict[int, mgl.Texture] = {}
 
 
 def get_texture_from_img(img: Image.Image) -> mgl.Texture:
-    texture = img_to_texture_map.get(id(img), None)
+    ctx = Renderer.data_ctx.get().ctx
+    key = (ctx, id(img))
+    texture = img_to_texture_map.get(key, None)
     if texture is not None:
         return texture
-    ctx = Renderer.data_ctx.get().ctx
     texture = ctx.texture(
         size=img.size,
         components=len(img.getbands()),
         data=img.tobytes()
     )
     texture.repeat_x = False
     texture.repeat_y = False
-    img_to_texture_map[id(img)] = texture
+    img_to_texture_map[key] = texture
     return texture
```

### Comparing `janim-1.0.3/janim/render/writer.py` & `janim-1.0.4/janim/render/writer.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/typing.py` & `janim-1.0.4/janim/typing.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/utils/bezier.py` & `janim-1.0.4/janim/utils/bezier.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/utils/config.py` & `janim-1.0.4/janim/utils/config.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/utils/data.py` & `janim-1.0.4/janim/utils/data.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/utils/dict_ops.py` & `janim-1.0.4/janim/utils/dict_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/utils/file_ops.py` & `janim-1.0.4/janim/utils/file_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/utils/font.py` & `janim-1.0.4/janim/utils/font.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/utils/font_manager.py` & `janim-1.0.4/janim/utils/font_manager.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/utils/iterables.py` & `janim-1.0.4/janim/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/utils/paths.py` & `janim-1.0.4/janim/utils/paths.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/utils/rate_functions.py` & `janim-1.0.4/janim/utils/rate_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 def there_and_back(t: float) -> float:
     new_t = 2 * t if t < 0.5 else 2 * (1 - t)
     return smooth(new_t)
 
 
 def there_and_back_with_pause(t: float, pause_ratio: float = 1. / 3) -> float:
-    a = 1. / pause_ratio
+    a = 2. / (1. - pause_ratio)
     if t < 0.5 - pause_ratio / 2:
         return smooth(a * t)
     elif t < 0.5 + pause_ratio / 2:
         return 1
     else:
         return smooth(a - a * t)
```

### Comparing `janim-1.0.3/janim/utils/refresh.py` & `janim-1.0.4/janim/utils/refresh.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/utils/signal.py` & `janim-1.0.4/janim/utils/signal.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/utils/simple_functions.py` & `janim-1.0.4/janim/utils/simple_functions.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/janim/utils/space_ops.py` & `janim-1.0.4/janim/utils/space_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/logo.png` & `janim-1.0.4/logo.png`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/pyproject.toml` & `janim-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `janim-1.0.3/PKG-INFO` & `janim-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janim
-Version: 1.0.3
+Version: 1.0.4
 Summary: a library for simple animation effects
 Author: jkjkil4
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Requires-Dist: numpy
 Requires-Dist: scipy
```

