# Comparing `tmp/magpylib-5.0.1.tar.gz` & `tmp/magpylib-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magpylib-5.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "magpylib-5.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `magpylib-5.0.1.tar` & `magpylib-5.0.2.tar`

### file list

```diff
@@ -1,248 +1,248 @@
--rw-r--r--   0        0        0       20 2024-04-12 06:52:54.515146 magpylib-5.0.1/.binder/apt.txt
--rw-r--r--   0        0        0      171 2024-04-12 06:52:54.515146 magpylib-5.0.1/.binder/labconfig/default_setting_overrides.json
--rw-r--r--   0        0        0      207 2024-04-12 06:52:54.515146 magpylib-5.0.1/.binder/postBuild
--rw-r--r--   0        0        0        8 2024-04-12 06:52:54.515146 magpylib-5.0.1/.binder/requirements.txt
--rw-r--r--   0        0        0      187 2024-04-12 06:52:54.515146 magpylib-5.0.1/.binder/start
--rw-r--r--   0        0        0     1562 2024-04-12 06:52:54.515146 magpylib-5.0.1/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0        0        0      910 2024-04-12 06:52:54.515146 magpylib-5.0.1/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0        0        0      573 2024-04-12 06:52:54.515146 magpylib-5.0.1/.github/ISSUE_TEMPLATE/question_magnetics.yaml
--rw-r--r--   0        0        0       27 2024-04-12 06:52:54.515146 magpylib-5.0.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0       59 2024-04-12 06:52:54.515146 magpylib-5.0.1/.github/codeql/codeql-config.yml
--rw-r--r--   0        0        0     1000 2024-04-12 06:52:54.515146 magpylib-5.0.1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     2145 2024-04-12 06:52:54.515146 magpylib-5.0.1/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1690 2024-04-12 06:52:54.515146 magpylib-5.0.1/.gitignore
--rw-r--r--   0        0        0     1116 2024-04-12 06:52:54.515146 magpylib-5.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    16348 2024-04-12 06:52:54.515146 magpylib-5.0.1/.pylintrc
--rw-r--r--   0        0        0      806 2024-04-12 06:52:54.515146 magpylib-5.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0    33573 2024-04-12 06:52:54.515146 magpylib-5.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     4790 2024-04-12 06:52:54.515146 magpylib-5.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3287 2024-04-12 06:52:54.515146 magpylib-5.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1332 2024-04-12 06:52:54.515146 magpylib-5.0.1/LICENSE
--rw-r--r--   0        0        0       68 2024-04-12 06:52:54.515146 magpylib-5.0.1/MANIFEST.in
--rw-r--r--   0        0        0     6947 2024-04-12 06:52:54.519146 magpylib-5.0.1/README.md
--rw-r--r--   0        0        0      602 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/Makefile
--rw-r--r--   0        0        0     1720 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/README.md
--rw-r--r--   0        0        0    40241 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/docu/docu_graphics.md
--rw-r--r--   0        0        0      733 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/docu/docu_index.md
--rw-r--r--   0        0        0    39553 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/docu/docu_magpylib_api.md
--rw-r--r--   0        0        0    10878 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/docu/docu_physics.md
--rw-r--r--   0        0        0     2687 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_app_end_of_shaft.md
--rw-r--r--   0        0        0      477 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_app_halbach.md
--rw-r--r--   0        0        0     4757 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_app_helmholtz.md
--rw-r--r--   0        0        0      426 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_app_scales.md
--rw-r--r--   0        0        0     5029 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_index.md
--rw-r--r--   0        0        0     5938 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_misc_compound.md
--rw-r--r--   0        0        0     5283 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_misc_field_interpolation.md
--rw-r--r--   0        0        0      372 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_misc_inhom.md
--rw-r--r--   0        0        0      367 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_shapes_3d_models.md
--rw-r--r--   0        0        0     1297 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_shapes_convex_hull.md
--rw-r--r--   0        0        0     3878 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_shapes_pyvista.md
--rw-r--r--   0        0        0     6628 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_shapes_superpos.md
--rw-r--r--   0        0        0     8369 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_shapes_triangle.md
--rw-r--r--   0        0        0     8058 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_collection.md
--rw-r--r--   0        0        0     7509 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_custom.md
--rw-r--r--   0        0        0     7845 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_field_computation.md
--rw-r--r--   0        0        0    10548 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_modelling_magnets.md
--rw-r--r--   0        0        0     6804 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_paths.md
--rw-r--r--   0        0        0     1313 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_vis_animations.md
--rw-r--r--   0        0        0     4091 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_vis_mpl_streamplot.md
--rw-r--r--   0        0        0     1657 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_vis_pv_streamlines.md
--rw-r--r--   0        0        0      545 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/gallery/gallery_vis_subplots.md
--rw-r--r--   0        0        0       89 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/reso_changelog.md
--rw-r--r--   0        0        0      102 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/reso_code_of_conduct.md
--rw-r--r--   0        0        0       95 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/reso_contributing.md
--rw-r--r--   0        0        0     7718 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/reso_get_started.md
--rw-r--r--   0        0        0      383 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/reso_license.md
--rw-r--r--   0        0        0      279 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_pages/reso_site_notice.md
--rw-r--r--   0        0        0      252 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/custom.css
--rw-r--r--   0        0        0    21562 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_collection.png
--rw-r--r--   0        0        0    17761 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_cuboid.png
--rw-r--r--   0        0        0    20351 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_custom.png
--rw-r--r--   0        0        0    19925 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_cylinder.png
--rw-r--r--   0        0        0    26491 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_cylindersegment.png
--rw-r--r--   0        0        0    16339 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_dipole.png
--rw-r--r--   0        0        0    13734 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_global_local.png
--rw-r--r--   0        0        0    21266 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_line.png
--rw-r--r--   0        0        0    18823 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_loop.png
--rw-r--r--   0        0        0    20182 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_sensor.png
--rw-r--r--   0        0        0    19936 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_sphere.png
--rw-r--r--   0        0        0    23461 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_tetra.png
--rw-r--r--   0        0        0    21231 2024-04-12 06:52:54.519146 magpylib-5.0.1/docs/_static/images/docu_classes_init_triangle.png
--rw-r--r--   0        0        0    27786 2024-04-12 06:52:54.523146 magpylib-5.0.1/docs/_static/images/docu_classes_init_trimesh.png
--rw-r--r--   0        0        0   249417 2024-04-12 06:52:54.523146 magpylib-5.0.1/docs/_static/images/docu_field_comp_flow.png
--rw-r--r--   0        0        0    18560 2024-04-12 06:52:54.523146 magpylib-5.0.1/docs/_static/images/docu_field_superpos_cutout.png
--rw-r--r--   0        0        0    18079 2024-04-12 06:52:54.523146 magpylib-5.0.1/docs/_static/images/docu_field_superpos_union.png
--rw-r--r--   0        0        0   236681 2024-04-12 06:52:54.523146 magpylib-5.0.1/docs/_static/images/docu_index_icon_magpylib.png
--rw-r--r--   0        0        0    91437 2024-04-12 06:52:54.523146 magpylib-5.0.1/docs/_static/images/docu_index_icon_magpylib_show.png
--rw-r--r--   0        0        0   319986 2024-04-12 06:52:54.523146 magpylib-5.0.1/docs/_static/images/docu_index_icon_physics.png
--rw-r--r--   0        0        0    49387 2024-04-12 06:52:54.523146 magpylib-5.0.1/docs/_static/images/docu_position_sketch.png
--rw-r--r--   0        0        0    13848 2024-04-12 06:52:54.523146 magpylib-5.0.1/docs/_static/images/favicons/android-chrome-192x192.png
--rw-r--r--   0        0        0    59132 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/favicons/android-chrome-512x512.png
--rw-r--r--   0        0        0    12328 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/favicons/apple-touch-icon.png
--rw-r--r--   0        0        0      708 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/favicons/favicon-16x16.png
--rw-r--r--   0        0        0     1470 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/favicons/favicon-32x32.png
--rw-r--r--   0        0        0    15406 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/favicons/favicon.ico
--rw-r--r--   0        0        0    29951 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_WIP.png
--rw-r--r--   0        0        0    36788 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_app_end_of_shaft.png
--rw-r--r--   0        0        0   142838 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_app_helmholtz.png
--rw-r--r--   0        0        0   126489 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_ext_custom_quadrupole.png
--rw-r--r--   0        0        0    52664 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_misc_compound.png
--rw-r--r--   0        0        0    19393 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_misc_field_interpolation.png
--rw-r--r--   0        0        0    28378 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_shapes_convex_hull.png
--rw-r--r--   0        0        0    26107 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_shapes_pyvista.png
--rw-r--r--   0        0        0    16589 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_shapes_superpos.png
--rw-r--r--   0        0        0    31361 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_shapes_triangle.png
--rw-r--r--   0        0        0    49507 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_collection.png
--rw-r--r--   0        0        0   270663 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_custom.png
--rw-r--r--   0        0        0    37618 2024-04-12 06:52:54.527146 magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_field_computation.png
--rw-r--r--   0        0        0    58417 2024-04-12 06:52:54.531146 magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_modelling_magnets.png
--rw-r--r--   0        0        0    32221 2024-04-12 06:52:54.531146 magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_paths.png
--rw-r--r--   0        0        0    29154 2024-04-12 06:52:54.531146 magpylib-5.0.1/docs/_static/images/gallery_icon_viz_animations.png
--rw-r--r--   0        0        0   133213 2024-04-12 06:52:54.531146 magpylib-5.0.1/docs/_static/images/gallery_icon_viz_mpl_streamplot.png
--rw-r--r--   0        0        0   101122 2024-04-12 06:52:54.531146 magpylib-5.0.1/docs/_static/images/gallery_icon_viz_pv_streamlines.png
--rw-r--r--   0        0        0   125215 2024-04-12 06:52:54.531146 magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_LDratio.png
--rw-r--r--   0        0        0   192104 2024-04-12 06:52:54.531146 magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_datasheet.png
--rw-r--r--   0        0        0   115449 2024-04-12 06:52:54.531146 magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_datasheet2.png
--rw-r--r--   0        0        0   105716 2024-04-12 06:52:54.531146 magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_fieldcomparison.png
--rw-r--r--   0        0        0    82273 2024-04-12 06:52:54.535146 magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_hysteresis.png
--rw-r--r--   0        0        0    60218 2024-04-12 06:52:54.535146 magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_table.png
--rw-r--r--   0        0        0    42153 2024-04-12 06:52:54.535146 magpylib-5.0.1/docs/_static/images/getting_started_animation.png
--rw-r--r--   0        0        0   107905 2024-04-12 06:52:54.535146 magpylib-5.0.1/docs/_static/images/getting_started_complex_shapes.png
--rw-r--r--   0        0        0   101291 2024-04-12 06:52:54.535146 magpylib-5.0.1/docs/_static/images/getting_started_fundamentals1.png
--rw-r--r--   0        0        0   114836 2024-04-12 06:52:54.535146 magpylib-5.0.1/docs/_static/images/getting_started_styles.png
--rw-r--r--   0        0        0   240757 2024-04-12 06:52:54.535146 magpylib-5.0.1/docs/_static/images/index_flowchart.png
--rw-r--r--   0        0        0   323052 2024-04-12 06:52:54.539146 magpylib-5.0.1/docs/_static/images/index_head.png
--rw-r--r--   0        0        0     7837 2024-04-12 06:52:54.539146 magpylib-5.0.1/docs/_static/images/index_icon_academic.png
--rw-r--r--   0        0        0     5281 2024-04-12 06:52:54.539146 magpylib-5.0.1/docs/_static/images/index_icon_contributing.png
--rw-r--r--   0        0        0     8741 2024-04-12 06:52:54.539146 magpylib-5.0.1/docs/_static/images/index_icon_docu.png
--rw-r--r--   0        0        0    12683 2024-04-12 06:52:54.539146 magpylib-5.0.1/docs/_static/images/index_icon_gallery.png
--rw-r--r--   0        0        0     9752 2024-04-12 06:52:54.539146 magpylib-5.0.1/docs/_static/images/index_icon_getting_started.png
--rw-r--r--   0        0        0     7864 2024-04-12 06:52:54.539146 magpylib-5.0.1/docs/_static/images/index_icon_github.png
--rw-r--r--   0        0        0   167515 2024-04-12 06:52:54.539146 magpylib-5.0.1/docs/_static/images/magpylib_flag.png
--rw-r--r--   0        0        0    22705 2024-04-12 06:52:54.539146 magpylib-5.0.1/docs/_static/images/magpylib_logo.png
--rw-r--r--   0        0        0   526695 2024-04-12 06:52:54.543146 magpylib-5.0.1/docs/_static/videos/axis.mp4
--rw-r--r--   0        0        0     2970 2024-04-12 06:52:54.543146 magpylib-5.0.1/docs/_static/webcode/copybutton.js
--rw-r--r--   0        0        0      447 2024-04-12 06:52:54.543146 magpylib-5.0.1/docs/_static/webcode/summaryOpen.js
--rw-r--r--   0        0        0    10243 2024-04-12 06:52:54.543146 magpylib-5.0.1/docs/conf.py
--rw-r--r--   0        0        0     2316 2024-04-12 06:52:54.543146 magpylib-5.0.1/docs/index.md
--rw-r--r--   0        0        0     6715 2024-04-12 06:52:54.543146 magpylib-5.0.1/docs/make.bat
--rw-r--r--   0        0        0     1916 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/__init__.py
--rw-r--r--   0        0        0       11 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/__init__.py
--rw-r--r--   0        0        0       22 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/defaults/__init__.py
--rw-r--r--   0        0        0     9448 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/defaults/defaults_classes.py
--rw-r--r--   0        0        0    13989 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/defaults/defaults_utility.py
--rw-r--r--   0        0        0     5981 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/defaults/defaults_values.py
--rw-r--r--   0        0        0       22 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/__init__.py
--rw-r--r--   0        0        0    14530 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/backend_matplotlib.py
--rw-r--r--   0        0        0    10746 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/backend_plotly.py
--rw-r--r--   0        0        0    12228 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/backend_pyvista.py
--rw-r--r--   0        0        0    17456 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/display.py
--rw-r--r--   0        0        0    11170 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/sensor_mesh.py
--rw-r--r--   0        0        0    21819 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/traces_base.py
--rw-r--r--   0        0        0    22486 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/traces_core.py
--rw-r--r--   0        0        0    33281 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/traces_generic.py
--rw-r--r--   0        0        0    26175 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/display/traces_utility.py
--rw-r--r--   0        0        0      458 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/exceptions.py
--rw-r--r--   0        0        0      312 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/__init__.py
--rw-r--r--   0        0        0     3696 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_circle.py
--rw-r--r--   0        0        0     8994 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_cuboid.py
--rw-r--r--   0        0        0    11016 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_cylinder.py
--rw-r--r--   0        0        0    77680 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_cylinder_segment.py
--rw-r--r--   0        0        0     2360 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_dipole.py
--rw-r--r--   0        0        0     7223 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_polyline.py
--rw-r--r--   0        0        0     2762 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_sphere.py
--rw-r--r--   0        0        0     3775 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_tetrahedron.py
--rw-r--r--   0        0        0     6453 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_triangle.py
--rw-r--r--   0        0        0    19051 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_BH_triangularmesh.py
--rw-r--r--   0        0        0    48296 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/field_wrap_BH.py
--rw-r--r--   0        0        0     4396 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/special_cel.py
--rw-r--r--   0        0        0    17650 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/fields/special_el3.py
--rw-r--r--   0        0        0    20724 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/input_checks.py
--rw-r--r--   0        0        0       23 2024-04-12 06:52:54.543146 magpylib-5.0.1/magpylib/_src/obj_classes/__init__.py
--rw-r--r--   0        0        0     4090 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_BaseDisplayRepr.py
--rw-r--r--   0        0        0    19372 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_BaseExcitations.py
--rw-r--r--   0        0        0    12717 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_BaseGeo.py
--rw-r--r--   0        0        0    34491 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_BaseTransform.py
--rw-r--r--   0        0        0    36312 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_Collection.py
--rw-r--r--   0        0        0    18854 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_Sensor.py
--rw-r--r--   0        0        0     5043 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_current_Circle.py
--rw-r--r--   0        0        0     5456 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_current_Polyline.py
--rw-r--r--   0        0        0     4421 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_Cuboid.py
--rw-r--r--   0        0        0     5006 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_Cylinder.py
--rw-r--r--   0        0        0     6828 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py
--rw-r--r--   0        0        0     4681 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_Sphere.py
--rw-r--r--   0        0        0     6030 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py
--rw-r--r--   0        0        0    36933 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_TriangularMesh.py
--rw-r--r--   0        0        0     3520 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_misc_CustomSource.py
--rw-r--r--   0        0        0     4530 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_misc_Dipole.py
--rw-r--r--   0        0        0     5934 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/obj_classes/class_misc_Triangle.py
--rw-r--r--   0        0        0    77585 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/style.py
--rw-r--r--   0        0        0    12334 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/_src/utility.py
--rw-r--r--   0        0        0     1048 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/core/__init__.py
--rw-r--r--   0        0        0      398 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/current/__init__.py
--rw-r--r--   0        0        0      260 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/graphics/__init__.py
--rw-r--r--   0        0        0      835 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/graphics/model3d/__init__.py
--rw-r--r--   0        0        0      353 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/graphics/style/__init__.py
--rw-r--r--   0        0        0      632 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/magnet/__init__.py
--rw-r--r--   0        0        0      335 2024-04-12 06:52:54.547146 magpylib-5.0.1/magpylib/misc/__init__.py
--rw-r--r--   0        0        0     2332 2024-04-12 06:52:54.547146 magpylib-5.0.1/pyproject.toml
--rw-r--r--   0        0        0       14 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/__init__.py
--rw-r--r--   0        0        0    25344 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_BHMJ_level.py
--rw-r--r--   0        0        0     7672 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_BaseTransform.py
--rw-r--r--   0        0        0     5503 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_Coumpound_setters.py
--rw-r--r--   0        0        0     2035 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_CustomSource.py
--rw-r--r--   0        0        0      760 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test__missing_optional_modules.py
--rw-r--r--   0        0        0      465 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_core.py
--rw-r--r--   0        0        0    17752 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_core_physics_consistency.py
--rw-r--r--   0        0        0     7060 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_default_utils.py
--rw-r--r--   0        0        0    10824 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_defaults.py
--rw-r--r--   0        0        0    21282 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_display_matplotlib.py
--rw-r--r--   0        0        0    13771 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_display_plotly.py
--rw-r--r--   0        0        0     4507 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_display_pyvista.py
--rw-r--r--   0        0        0     3181 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_display_utility.py
--rw-r--r--   0        0        0     3453 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_elliptics.py
--rw-r--r--   0        0        0     8864 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_exceptions.py
--rw-r--r--   0        0        0    15385 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_field_cylinder.py
--rw-r--r--   0        0        0    13402 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_getBH_dict.py
--rw-r--r--   0        0        0    12196 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_getBH_interfaces.py
--rw-r--r--   0        0        0    19579 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_getBH_level2.py
--rw-r--r--   0        0        0    25249 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_input_checks.py
--rw-r--r--   0        0        0      346 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_misc.py
--rw-r--r--   0        0        0      737 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_numerical_stability.py
--rw-r--r--   0        0        0    20450 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_obj_BaseGeo.py
--rw-r--r--   0        0        0    12300 2024-04-12 06:52:54.547146 magpylib-5.0.1/tests/test_obj_BaseGeo_v4motion.py
--rw-r--r--   0        0        0     2208 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Circle.py
--rw-r--r--   0        0        0    15913 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Collection.py
--rw-r--r--   0        0        0    10301 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Collection_child_parent.py
--rw-r--r--   0        0        0    25232 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Collection_v4motion.py
--rw-r--r--   0        0        0     4516 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Cuboid.py
--rw-r--r--   0        0        0     4140 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Cylinder.py
--rw-r--r--   0        0        0     1087 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_CylinderSegment.py
--rw-r--r--   0        0        0     1038 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Dipole.py
--rw-r--r--   0        0        0     3787 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Polyline.py
--rw-r--r--   0        0        0     3719 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Sensor.py
--rw-r--r--   0        0        0     3105 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Sphere.py
--rw-r--r--   0        0        0     2467 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Tetrahedron.py
--rw-r--r--   0        0        0     2446 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_Triangle.py
--rw-r--r--   0        0        0    16212 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_obj_TriangularMesh.py
--rw-r--r--   0        0        0     1654 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_path.py
--rw-r--r--   0        0        0    10338 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_physics_consistency.py
--rw-r--r--   0        0        0      661 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_scaling.py
--rw-r--r--   0        0        0     2633 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_utility.py
--rw-r--r--   0        0        0     2966 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/test_vs_mag2.py
--rw-r--r--   0        0        0    14641 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/testdata/testdata_Collection.p
--rw-r--r--   0        0        0     1568 2024-04-12 06:52:54.551146 magpylib-5.0.1/tests/testdata/testdata_Collection_setter.npy
--rw-r--r--   0        0        0  1747640 2024-04-12 06:52:54.559146 magpylib-5.0.1/tests/testdata/testdata_Cuboid.p
--rw-r--r--   0        0        0  1746038 2024-04-12 06:52:54.571146 magpylib-5.0.1/tests/testdata/testdata_Sphere.p
--rw-r--r--   0        0        0    17225 2024-04-12 06:52:54.571146 magpylib-5.0.1/tests/testdata/testdata_compound_setter_cases.npy
--rw-r--r--   0        0        0  1095577 2024-04-12 06:52:54.575146 magpylib-5.0.1/tests/testdata/testdata_cy_cases.npy
--rw-r--r--   0        0        0   320128 2024-04-12 06:52:54.575146 magpylib-5.0.1/tests/testdata/testdata_el3.npy
--rw-r--r--   0        0        0  1534592 2024-04-12 06:52:54.583146 magpylib-5.0.1/tests/testdata/testdata_el3_angle.npy
--rw-r--r--   0        0        0    13056 2024-04-12 06:52:54.583146 magpylib-5.0.1/tests/testdata/testdata_femDat_cylinder_tile2.npy
--rw-r--r--   0        0        0   102475 2024-04-12 06:52:54.583146 magpylib-5.0.1/tests/testdata/testdata_field_BH_cuboid.p
--rw-r--r--   0        0        0   240606 2024-04-12 06:52:54.583146 magpylib-5.0.1/tests/testdata/testdata_field_BH_cylinder.p
--rw-r--r--   0        0        0     9728 2024-04-12 06:52:54.583146 magpylib-5.0.1/tests/testdata/testdata_full_cyl.npy
--rw-r--r--   0        0        0     1022 2024-04-12 06:52:54.583146 magpylib-5.0.1/tests/testdata/testdata_path_BaseGeo.p
--rw-r--r--   0        0        0     7362 2024-04-12 06:52:54.583146 magpylib-5.0.1/tests/testdata/testdata_vs_mag2.p
--rw-r--r--   0        0        0      606 2024-04-12 06:52:54.583146 magpylib-5.0.1/tox.ini
--rw-r--r--   0        0        0     9404 1970-01-01 00:00:00.000000 magpylib-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0       20 2024-05-22 07:39:06.741836 magpylib-5.0.2/.binder/apt.txt
+-rw-r--r--   0        0        0      171 2024-05-22 07:39:06.741836 magpylib-5.0.2/.binder/labconfig/default_setting_overrides.json
+-rw-r--r--   0        0        0      207 2024-05-22 07:39:06.741836 magpylib-5.0.2/.binder/postBuild
+-rw-r--r--   0        0        0        8 2024-05-22 07:39:06.741836 magpylib-5.0.2/.binder/requirements.txt
+-rw-r--r--   0        0        0      187 2024-05-22 07:39:06.741836 magpylib-5.0.2/.binder/start
+-rw-r--r--   0        0        0     1562 2024-05-22 07:39:06.741836 magpylib-5.0.2/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0        0        0      910 2024-05-22 07:39:06.741836 magpylib-5.0.2/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0        0        0      573 2024-05-22 07:39:06.741836 magpylib-5.0.2/.github/ISSUE_TEMPLATE/question_magnetics.yaml
+-rw-r--r--   0        0        0       27 2024-05-22 07:39:06.741836 magpylib-5.0.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0       59 2024-05-22 07:39:06.741836 magpylib-5.0.2/.github/codeql/codeql-config.yml
+-rw-r--r--   0        0        0     1000 2024-05-22 07:39:06.741836 magpylib-5.0.2/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     2113 2024-05-22 07:39:06.741836 magpylib-5.0.2/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1690 2024-05-22 07:39:06.741836 magpylib-5.0.2/.gitignore
+-rw-r--r--   0        0        0     1116 2024-05-22 07:39:06.741836 magpylib-5.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    16348 2024-05-22 07:39:06.741836 magpylib-5.0.2/.pylintrc
+-rw-r--r--   0        0        0      807 2024-05-22 07:39:06.741836 magpylib-5.0.2/.readthedocs.yaml
+-rw-r--r--   0        0        0    34350 2024-05-22 07:39:06.741836 magpylib-5.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     4790 2024-05-22 07:39:06.741836 magpylib-5.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3287 2024-05-22 07:39:06.741836 magpylib-5.0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1332 2024-05-22 07:39:06.741836 magpylib-5.0.2/LICENSE
+-rw-r--r--   0        0        0       68 2024-05-22 07:39:06.741836 magpylib-5.0.2/MANIFEST.in
+-rw-r--r--   0        0        0     6948 2024-05-22 07:39:06.745836 magpylib-5.0.2/README.md
+-rw-r--r--   0        0        0      602 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/Makefile
+-rw-r--r--   0        0        0     1720 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/README.md
+-rw-r--r--   0        0        0    40241 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/docu/docu_graphics.md
+-rw-r--r--   0        0        0      733 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/docu/docu_index.md
+-rw-r--r--   0        0        0    39553 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/docu/docu_magpylib_api.md
+-rw-r--r--   0        0        0    10878 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/docu/docu_physics.md
+-rw-r--r--   0        0        0     2687 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_app_end_of_shaft.md
+-rw-r--r--   0        0        0      477 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_app_halbach.md
+-rw-r--r--   0        0        0     4757 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_app_helmholtz.md
+-rw-r--r--   0        0        0      426 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_app_scales.md
+-rw-r--r--   0        0        0     5029 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_index.md
+-rw-r--r--   0        0        0     5938 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_misc_compound.md
+-rw-r--r--   0        0        0     5283 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_misc_field_interpolation.md
+-rw-r--r--   0        0        0      372 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_misc_inhom.md
+-rw-r--r--   0        0        0      367 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_shapes_3d_models.md
+-rw-r--r--   0        0        0     1297 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_shapes_convex_hull.md
+-rw-r--r--   0        0        0     3878 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_shapes_pyvista.md
+-rw-r--r--   0        0        0     6628 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_shapes_superpos.md
+-rw-r--r--   0        0        0     8369 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_shapes_triangle.md
+-rw-r--r--   0        0        0     8058 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_collection.md
+-rw-r--r--   0        0        0     7509 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_custom.md
+-rw-r--r--   0        0        0     7845 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_field_computation.md
+-rw-r--r--   0        0        0    10548 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_modelling_magnets.md
+-rw-r--r--   0        0        0     6804 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_paths.md
+-rw-r--r--   0        0        0     1313 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_vis_animations.md
+-rw-r--r--   0        0        0     4091 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_vis_mpl_streamplot.md
+-rw-r--r--   0        0        0     1657 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_vis_pv_streamlines.md
+-rw-r--r--   0        0        0      545 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_vis_subplots.md
+-rw-r--r--   0        0        0       89 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/reso_changelog.md
+-rw-r--r--   0        0        0      102 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/reso_code_of_conduct.md
+-rw-r--r--   0        0        0       95 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/reso_contributing.md
+-rw-r--r--   0        0        0     7719 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/reso_get_started.md
+-rw-r--r--   0        0        0      383 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/reso_license.md
+-rw-r--r--   0        0        0      357 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/reso_site_notice.md
+-rw-r--r--   0        0        0      252 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/custom.css
+-rw-r--r--   0        0        0    21562 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_collection.png
+-rw-r--r--   0        0        0    17761 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_cuboid.png
+-rw-r--r--   0        0        0    20351 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_custom.png
+-rw-r--r--   0        0        0    19925 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_cylinder.png
+-rw-r--r--   0        0        0    26491 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_cylindersegment.png
+-rw-r--r--   0        0        0    16339 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_dipole.png
+-rw-r--r--   0        0        0    13734 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_global_local.png
+-rw-r--r--   0        0        0    21266 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_line.png
+-rw-r--r--   0        0        0    18823 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_loop.png
+-rw-r--r--   0        0        0    20182 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_sensor.png
+-rw-r--r--   0        0        0    19936 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_sphere.png
+-rw-r--r--   0        0        0    23461 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_tetra.png
+-rw-r--r--   0        0        0    21231 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_triangle.png
+-rw-r--r--   0        0        0    27786 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_trimesh.png
+-rw-r--r--   0        0        0   249417 2024-05-22 07:39:06.749836 magpylib-5.0.2/docs/_static/images/docu_field_comp_flow.png
+-rw-r--r--   0        0        0    18560 2024-05-22 07:39:06.749836 magpylib-5.0.2/docs/_static/images/docu_field_superpos_cutout.png
+-rw-r--r--   0        0        0    18079 2024-05-22 07:39:06.749836 magpylib-5.0.2/docs/_static/images/docu_field_superpos_union.png
+-rw-r--r--   0        0        0   236681 2024-05-22 07:39:06.749836 magpylib-5.0.2/docs/_static/images/docu_index_icon_magpylib.png
+-rw-r--r--   0        0        0    91437 2024-05-22 07:39:06.749836 magpylib-5.0.2/docs/_static/images/docu_index_icon_magpylib_show.png
+-rw-r--r--   0        0        0   319986 2024-05-22 07:39:06.749836 magpylib-5.0.2/docs/_static/images/docu_index_icon_physics.png
+-rw-r--r--   0        0        0    49387 2024-05-22 07:39:06.749836 magpylib-5.0.2/docs/_static/images/docu_position_sketch.png
+-rw-r--r--   0        0        0    13848 2024-05-22 07:39:06.749836 magpylib-5.0.2/docs/_static/images/favicons/android-chrome-192x192.png
+-rw-r--r--   0        0        0    59132 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/favicons/android-chrome-512x512.png
+-rw-r--r--   0        0        0    12328 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/favicons/apple-touch-icon.png
+-rw-r--r--   0        0        0      708 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/favicons/favicon-16x16.png
+-rw-r--r--   0        0        0     1470 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/favicons/favicon-32x32.png
+-rw-r--r--   0        0        0    15406 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/favicons/favicon.ico
+-rw-r--r--   0        0        0    29951 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_WIP.png
+-rw-r--r--   0        0        0    36788 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_app_end_of_shaft.png
+-rw-r--r--   0        0        0   142838 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_app_helmholtz.png
+-rw-r--r--   0        0        0   126489 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_ext_custom_quadrupole.png
+-rw-r--r--   0        0        0    52664 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_misc_compound.png
+-rw-r--r--   0        0        0    19393 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_misc_field_interpolation.png
+-rw-r--r--   0        0        0    28378 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_shapes_convex_hull.png
+-rw-r--r--   0        0        0    26107 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_shapes_pyvista.png
+-rw-r--r--   0        0        0    16589 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_shapes_superpos.png
+-rw-r--r--   0        0        0    31361 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_shapes_triangle.png
+-rw-r--r--   0        0        0    49507 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_collection.png
+-rw-r--r--   0        0        0   270663 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_custom.png
+-rw-r--r--   0        0        0    37618 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_field_computation.png
+-rw-r--r--   0        0        0    58417 2024-05-22 07:39:06.757836 magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_modelling_magnets.png
+-rw-r--r--   0        0        0    32221 2024-05-22 07:39:06.757836 magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_paths.png
+-rw-r--r--   0        0        0    29154 2024-05-22 07:39:06.757836 magpylib-5.0.2/docs/_static/images/gallery_icon_viz_animations.png
+-rw-r--r--   0        0        0   133213 2024-05-22 07:39:06.757836 magpylib-5.0.2/docs/_static/images/gallery_icon_viz_mpl_streamplot.png
+-rw-r--r--   0        0        0   101122 2024-05-22 07:39:06.757836 magpylib-5.0.2/docs/_static/images/gallery_icon_viz_pv_streamlines.png
+-rw-r--r--   0        0        0   125215 2024-05-22 07:39:06.757836 magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_LDratio.png
+-rw-r--r--   0        0        0   192104 2024-05-22 07:39:06.757836 magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_datasheet.png
+-rw-r--r--   0        0        0   115449 2024-05-22 07:39:06.757836 magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_datasheet2.png
+-rw-r--r--   0        0        0   105716 2024-05-22 07:39:06.757836 magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_fieldcomparison.png
+-rw-r--r--   0        0        0    82273 2024-05-22 07:39:06.761836 magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_hysteresis.png
+-rw-r--r--   0        0        0    60218 2024-05-22 07:39:06.761836 magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_table.png
+-rw-r--r--   0        0        0    42153 2024-05-22 07:39:06.761836 magpylib-5.0.2/docs/_static/images/getting_started_animation.png
+-rw-r--r--   0        0        0   107905 2024-05-22 07:39:06.761836 magpylib-5.0.2/docs/_static/images/getting_started_complex_shapes.png
+-rw-r--r--   0        0        0   101291 2024-05-22 07:39:06.761836 magpylib-5.0.2/docs/_static/images/getting_started_fundamentals1.png
+-rw-r--r--   0        0        0   114836 2024-05-22 07:39:06.761836 magpylib-5.0.2/docs/_static/images/getting_started_styles.png
+-rw-r--r--   0        0        0   240757 2024-05-22 07:39:06.761836 magpylib-5.0.2/docs/_static/images/index_flowchart.png
+-rw-r--r--   0        0        0   323052 2024-05-22 07:39:06.765836 magpylib-5.0.2/docs/_static/images/index_head.png
+-rw-r--r--   0        0        0     7837 2024-05-22 07:39:06.765836 magpylib-5.0.2/docs/_static/images/index_icon_academic.png
+-rw-r--r--   0        0        0     5281 2024-05-22 07:39:06.765836 magpylib-5.0.2/docs/_static/images/index_icon_contributing.png
+-rw-r--r--   0        0        0     8741 2024-05-22 07:39:06.765836 magpylib-5.0.2/docs/_static/images/index_icon_docu.png
+-rw-r--r--   0        0        0    12683 2024-05-22 07:39:06.765836 magpylib-5.0.2/docs/_static/images/index_icon_gallery.png
+-rw-r--r--   0        0        0     9752 2024-05-22 07:39:06.765836 magpylib-5.0.2/docs/_static/images/index_icon_getting_started.png
+-rw-r--r--   0        0        0     7864 2024-05-22 07:39:06.765836 magpylib-5.0.2/docs/_static/images/index_icon_github.png
+-rw-r--r--   0        0        0   167515 2024-05-22 07:39:06.765836 magpylib-5.0.2/docs/_static/images/magpylib_flag.png
+-rw-r--r--   0        0        0    22705 2024-05-22 07:39:06.765836 magpylib-5.0.2/docs/_static/images/magpylib_logo.png
+-rw-r--r--   0        0        0   526695 2024-05-22 07:39:06.769836 magpylib-5.0.2/docs/_static/videos/axis.mp4
+-rw-r--r--   0        0        0     2970 2024-05-22 07:39:06.769836 magpylib-5.0.2/docs/_static/webcode/copybutton.js
+-rw-r--r--   0        0        0      447 2024-05-22 07:39:06.769836 magpylib-5.0.2/docs/_static/webcode/summaryOpen.js
+-rw-r--r--   0        0        0    10243 2024-05-22 07:39:06.769836 magpylib-5.0.2/docs/conf.py
+-rw-r--r--   0        0        0     2316 2024-05-22 07:39:06.769836 magpylib-5.0.2/docs/index.md
+-rw-r--r--   0        0        0     6715 2024-05-22 07:39:06.769836 magpylib-5.0.2/docs/make.bat
+-rw-r--r--   0        0        0     1916 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/__init__.py
+-rw-r--r--   0        0        0       11 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/defaults/__init__.py
+-rw-r--r--   0        0        0     9448 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/defaults/defaults_classes.py
+-rw-r--r--   0        0        0    13989 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/defaults/defaults_utility.py
+-rw-r--r--   0        0        0     5981 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/defaults/defaults_values.py
+-rw-r--r--   0        0        0       22 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/__init__.py
+-rw-r--r--   0        0        0    14530 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/backend_matplotlib.py
+-rw-r--r--   0        0        0    10746 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/backend_plotly.py
+-rw-r--r--   0        0        0    12228 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/backend_pyvista.py
+-rw-r--r--   0        0        0    17456 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/display.py
+-rw-r--r--   0        0        0    11170 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/sensor_mesh.py
+-rw-r--r--   0        0        0    21819 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/traces_base.py
+-rw-r--r--   0        0        0    22531 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/traces_core.py
+-rw-r--r--   0        0        0    33281 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/traces_generic.py
+-rw-r--r--   0        0        0    26263 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/traces_utility.py
+-rw-r--r--   0        0        0      458 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/exceptions.py
+-rw-r--r--   0        0        0      312 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/__init__.py
+-rw-r--r--   0        0        0     3696 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/field_BH_circle.py
+-rw-r--r--   0        0        0     8994 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/field_BH_cuboid.py
+-rw-r--r--   0        0        0    11016 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/field_BH_cylinder.py
+-rw-r--r--   0        0        0    77680 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/field_BH_cylinder_segment.py
+-rw-r--r--   0        0        0     2360 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/field_BH_dipole.py
+-rw-r--r--   0        0        0     7223 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/field_BH_polyline.py
+-rw-r--r--   0        0        0     2762 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/field_BH_sphere.py
+-rw-r--r--   0        0        0     3775 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/field_BH_tetrahedron.py
+-rw-r--r--   0        0        0     6453 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/field_BH_triangle.py
+-rw-r--r--   0        0        0    19051 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/fields/field_BH_triangularmesh.py
+-rw-r--r--   0        0        0    48296 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/fields/field_wrap_BH.py
+-rw-r--r--   0        0        0     4396 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/fields/special_cel.py
+-rw-r--r--   0        0        0    17650 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/fields/special_el3.py
+-rw-r--r--   0        0        0    20731 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/input_checks.py
+-rw-r--r--   0        0        0       23 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/__init__.py
+-rw-r--r--   0        0        0     4090 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_BaseDisplayRepr.py
+-rw-r--r--   0        0        0    19372 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_BaseExcitations.py
+-rw-r--r--   0        0        0    12717 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_BaseGeo.py
+-rw-r--r--   0        0        0    34491 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_BaseTransform.py
+-rw-r--r--   0        0        0    36370 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_Collection.py
+-rw-r--r--   0        0        0    18854 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_Sensor.py
+-rw-r--r--   0        0        0     4535 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_current_Circle.py
+-rw-r--r--   0        0        0     4946 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_current_Polyline.py
+-rw-r--r--   0        0        0     4421 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_Cuboid.py
+-rw-r--r--   0        0        0     5006 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_Cylinder.py
+-rw-r--r--   0        0        0     6828 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py
+-rw-r--r--   0        0        0     4681 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_Sphere.py
+-rw-r--r--   0        0        0     6030 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py
+-rw-r--r--   0        0        0    36933 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_TriangularMesh.py
+-rw-r--r--   0        0        0     3520 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_misc_CustomSource.py
+-rw-r--r--   0        0        0     4530 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_misc_Dipole.py
+-rw-r--r--   0        0        0     5934 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_misc_Triangle.py
+-rw-r--r--   0        0        0    77585 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/style.py
+-rw-r--r--   0        0        0    12334 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/utility.py
+-rw-r--r--   0        0        0     1048 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/core/__init__.py
+-rw-r--r--   0        0        0      398 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/current/__init__.py
+-rw-r--r--   0        0        0      260 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/graphics/__init__.py
+-rw-r--r--   0        0        0      835 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/graphics/model3d/__init__.py
+-rw-r--r--   0        0        0      353 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/graphics/style/__init__.py
+-rw-r--r--   0        0        0      632 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/magnet/__init__.py
+-rw-r--r--   0        0        0      335 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/misc/__init__.py
+-rw-r--r--   0        0        0     2290 2024-05-22 07:39:06.773836 magpylib-5.0.2/pyproject.toml
+-rw-r--r--   0        0        0       14 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/__init__.py
+-rw-r--r--   0        0        0    25344 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_BHMJ_level.py
+-rw-r--r--   0        0        0     7672 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_BaseTransform.py
+-rw-r--r--   0        0        0     5503 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_Coumpound_setters.py
+-rw-r--r--   0        0        0     2035 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_CustomSource.py
+-rw-r--r--   0        0        0      760 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test__missing_optional_modules.py
+-rw-r--r--   0        0        0      465 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_core.py
+-rw-r--r--   0        0        0    18105 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_core_physics_consistency.py
+-rw-r--r--   0        0        0     7060 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_default_utils.py
+-rw-r--r--   0        0        0    10878 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_defaults.py
+-rw-r--r--   0        0        0    21282 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_display_matplotlib.py
+-rw-r--r--   0        0        0    13771 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_display_plotly.py
+-rw-r--r--   0        0        0     4507 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_display_pyvista.py
+-rw-r--r--   0        0        0     3181 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_display_utility.py
+-rw-r--r--   0        0        0     3453 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_elliptics.py
+-rw-r--r--   0        0        0     8864 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_exceptions.py
+-rw-r--r--   0        0        0    15385 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_field_cylinder.py
+-rw-r--r--   0        0        0    13402 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_getBH_dict.py
+-rw-r--r--   0        0        0    12196 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_getBH_interfaces.py
+-rw-r--r--   0        0        0    19639 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_getBH_level2.py
+-rw-r--r--   0        0        0    25249 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_input_checks.py
+-rw-r--r--   0        0        0      346 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_misc.py
+-rw-r--r--   0        0        0      737 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_numerical_stability.py
+-rw-r--r--   0        0        0    20619 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_BaseGeo.py
+-rw-r--r--   0        0        0    12300 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_BaseGeo_v4motion.py
+-rw-r--r--   0        0        0     2208 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Circle.py
+-rw-r--r--   0        0        0    15913 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Collection.py
+-rw-r--r--   0        0        0    10301 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Collection_child_parent.py
+-rw-r--r--   0        0        0    25232 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Collection_v4motion.py
+-rw-r--r--   0        0        0     4516 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Cuboid.py
+-rw-r--r--   0        0        0     4140 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Cylinder.py
+-rw-r--r--   0        0        0     1087 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_CylinderSegment.py
+-rw-r--r--   0        0        0     1038 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Dipole.py
+-rw-r--r--   0        0        0     3787 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Polyline.py
+-rw-r--r--   0        0        0     3719 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Sensor.py
+-rw-r--r--   0        0        0     3105 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Sphere.py
+-rw-r--r--   0        0        0     2467 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Tetrahedron.py
+-rw-r--r--   0        0        0     2446 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Triangle.py
+-rw-r--r--   0        0        0    16212 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_TriangularMesh.py
+-rw-r--r--   0        0        0     1654 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_path.py
+-rw-r--r--   0        0        0    10338 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_physics_consistency.py
+-rw-r--r--   0        0        0      661 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_scaling.py
+-rw-r--r--   0        0        0     2633 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_utility.py
+-rw-r--r--   0        0        0     2966 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_vs_mag2.py
+-rw-r--r--   0        0        0    14641 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/testdata/testdata_Collection.p
+-rw-r--r--   0        0        0     1568 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/testdata/testdata_Collection_setter.npy
+-rw-r--r--   0        0        0  1747640 2024-05-22 07:39:06.785836 magpylib-5.0.2/tests/testdata/testdata_Cuboid.p
+-rw-r--r--   0        0        0  1746038 2024-05-22 07:39:06.797836 magpylib-5.0.2/tests/testdata/testdata_Sphere.p
+-rw-r--r--   0        0        0    17225 2024-05-22 07:39:06.797836 magpylib-5.0.2/tests/testdata/testdata_compound_setter_cases.npy
+-rw-r--r--   0        0        0  1095577 2024-05-22 07:39:06.801836 magpylib-5.0.2/tests/testdata/testdata_cy_cases.npy
+-rw-r--r--   0        0        0   320128 2024-05-22 07:39:06.801836 magpylib-5.0.2/tests/testdata/testdata_el3.npy
+-rw-r--r--   0        0        0  1534592 2024-05-22 07:39:06.809836 magpylib-5.0.2/tests/testdata/testdata_el3_angle.npy
+-rw-r--r--   0        0        0    13056 2024-05-22 07:39:06.809836 magpylib-5.0.2/tests/testdata/testdata_femDat_cylinder_tile2.npy
+-rw-r--r--   0        0        0   102475 2024-05-22 07:39:06.809836 magpylib-5.0.2/tests/testdata/testdata_field_BH_cuboid.p
+-rw-r--r--   0        0        0   240606 2024-05-22 07:39:06.809836 magpylib-5.0.2/tests/testdata/testdata_field_BH_cylinder.p
+-rw-r--r--   0        0        0     9728 2024-05-22 07:39:06.809836 magpylib-5.0.2/tests/testdata/testdata_full_cyl.npy
+-rw-r--r--   0        0        0     1022 2024-05-22 07:39:06.809836 magpylib-5.0.2/tests/testdata/testdata_path_BaseGeo.p
+-rw-r--r--   0        0        0     7362 2024-05-22 07:39:06.809836 magpylib-5.0.2/tests/testdata/testdata_vs_mag2.p
+-rw-r--r--   0        0        0      576 2024-05-22 07:39:06.809836 magpylib-5.0.2/tox.ini
+-rw-r--r--   0        0        0     9358 1970-01-01 00:00:00.000000 magpylib-5.0.2/PKG-INFO
```

### Comparing `magpylib-5.0.1/.github/ISSUE_TEMPLATE/bug_report.yaml` & `magpylib-5.0.2/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/.github/ISSUE_TEMPLATE/feature_request.yaml` & `magpylib-5.0.2/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/.github/ISSUE_TEMPLATE/question_magnetics.yaml` & `magpylib-5.0.2/.github/ISSUE_TEMPLATE/question_magnetics.yaml`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/.github/workflows/codeql.yml` & `magpylib-5.0.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/.github/workflows/python-app.yml` & `magpylib-5.0.2/.github/workflows/python-app.yml`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,14 @@
     strategy:
       fail-fast: false
       matrix:
         py:
           - "3.12"
           - "3.11"
           - "3.10"
-          - "3.9"
-          - "3.8"
         os:
           - ubuntu-latest
           - macos-latest
           - windows-latest
     steps:
       - name: Setup headless display
         uses: pyvista/setup-headless-display-action@v2
@@ -68,17 +66,17 @@
     runs-on: ubuntu-latest
     permissions:
       # IMPORTANT: this permission is mandatory for trusted publishing
       id-token: write
     steps:
       - name: Checkout source
         uses: actions/checkout@v4
-      - name: Set up Python 3.9
+      - name: Set up Python 3.10
         uses: actions/setup-python@v4
         with:
-          python-version: 3.9
+          python-version: "3.10"
       - name: Install flit
         run: pip install flit
       - name: Build package
         run: flit build
       - name: Publish
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `magpylib-5.0.1/.gitignore` & `magpylib-5.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/.pre-commit-config.yaml` & `magpylib-5.0.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     rev: v3.15.2
     hooks:
       - id: pyupgrade
         args: [--py38-plus]
 
 
   - repo: https://github.com/psf/black
-    rev: "24.3.0"
+    rev: "24.4.0"
     hooks:
       - id: black
 
 
   # - repo: local
   #   hooks:
   #     - id: pylint
```

### Comparing `magpylib-5.0.1/.pylintrc` & `magpylib-5.0.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/.readthedocs.yaml` & `magpylib-5.0.2/.readthedocs.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Required
 version: 2
 
 # Set the version of Python and other tools you might need
 build:
   os: ubuntu-20.04
   tools:
-    python: "3.9"
+    python: "3.10"
     # You can also specify other tool versions:
     # nodejs: "16"
     # rust: "1.55"
     # golang: "1.17"
   apt_packages:
     # for pyvista
     - libgl1-mesa-dev
```

### Comparing `magpylib-5.0.1/CHANGELOG.md` & `magpylib-5.0.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 All notable changes to magpylib are documented here.
 
 
 # Changelog
 
+## [5.0.2] - 2024-05-21
+- Fixed a display issue causing incorrect calculation of viewbox limits ([#772](https://github.com/magpylib/magpylib/pull/772))
+- Removed support for python 3.8 and 3.9 by now following the scientific-python.org support timelines ([#773](https://github.com/magpylib/magpylib/pull/773))
+- Fixed CI testing with newer backend versions ([#774](https://github.com/magpylib/magpylib/pull/774))
+- Updated site notice to mention the awarded "small development grant" by NumFocus. ([#758](https://github.com/magpylib/magpylib/pull/758))
+- Fix inaccurate citation year for Yang publication ([#764](https://github.com/magpylib/magpylib/pull/764), with thanks to @feldnerd for the contribution!)
+
 ## [5.0.1] - 2024-04-12
 - Fixed a bug where `getBHJM` of a Collection would produce one extra dimension ([#753](https://github.com/magpylib/magpylib/issues/753))
 - Fixed a bug where the legend of a deeply nested Collection would be wrong ([#756](https://github.com/magpylib/magpylib/issues/756))
 
 ## [5.0.0] - 2024-03-13
 ### ⚠️ Breaking Changes ⚠️
 - The Magpylib inputs and outputs are now in **SI Units**.
@@ -452,15 +459,16 @@
    - Loop Current
    - Current Line
    - Dipole
 - Collection class
 
 ---
 
-[5.0.1]:https://github.com/magpylib/magpylib/compare/5.0.0...HEAD
+[5.0.2]:https://github.com/magpylib/magpylib/compare/5.0.1...HEAD
+[5.0.1]:https://github.com/magpylib/magpylib/compare/5.0.0...5.0.1
 [5.0.0]:https://github.com/magpylib/magpylib/compare/4.5.1...5.0.0
 [4.5.1]:https://github.com/magpylib/magpylib/compare/4.5.0...4.5.1
 [4.5.0]:https://github.com/magpylib/magpylib/compare/4.4.0...4.5.0
 [4.4.1]:https://github.com/magpylib/magpylib/compare/4.4.0...4.4.1
 [4.4.0]:https://github.com/magpylib/magpylib/compare/4.3.0...4.4.0
 [4.3.0]:https://github.com/magpylib/magpylib/compare/4.2.0...4.3.0
 [4.2.0]:https://github.com/magpylib/magpylib/compare/4.1.2...4.2.0
```

### Comparing `magpylib-5.0.1/CODE_OF_CONDUCT.md` & `magpylib-5.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/CONTRIBUTING.md` & `magpylib-5.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/LICENSE` & `magpylib-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/README.md` & `magpylib-5.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 </a>
 <a href="https://codecov.io/gh/magpylib/magpylib"> <img src="https://codecov.io/gh/magpylib/magpylib/branch/main/graph/badge.svg">
 </a>
 <a href="https://pypi.org/project/magpylib/"> <img src="https://badge.fury.io/py/magpylib.svg" alt="PyPI version" height="18">
 </a>
 <a href="https://anaconda.org/conda-forge/magpylib"> <img src="https://anaconda.org/conda-forge/magpylib/badges/version.svg" alt="Conda Cloud" height="18">
 </a>
-<a href="https://mybinder.org/v2/gh/magpylib/magpylib/5.0.0?filepath=docs%2Fexamples"> <img src="https://mybinder.org/badge_logo.svg" alt="MyBinder link" height="18">
+<a href="https://mybinder.org/v2/gh/magpylib/magpylib/5.0.2?filepath=docs%2Fexamples"> <img src="https://mybinder.org/badge_logo.svg" alt="MyBinder link" height="18">
 </a>
 <a href="https://github.com/psf/black"> <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="black" height="18">
 </a>
 </div>
 
 Magpylib is a Python package for calculating **3D static magnetic fields** of magnets, line currents and other sources. The computation is based on explicit expressions and is therefore **extremely fast**. A **user friendly API** enables convenient positioning of sources and observers.
 
@@ -34,15 +34,15 @@
 ```
 pip install magpylib
 ```
 Install from conda forge using **conda**
 ```
 conda install -c conda-forge magpylib
 ```
-Magpylib supports _Python3.8+_ and relies on common scientific computation libraries _Numpy_, _Scipy_, _Matplotlib_ and _Plotly_. Optionally, _Pyvista_ is recommended as graphical backend.
+Magpylib supports _Python3.10+_ and relies on common scientific computation libraries _Numpy_, _Scipy_, _Matplotlib_ and _Plotly_. Optionally, _Pyvista_ is recommended as graphical backend.
 
 # Resources
 
  - Check out our **[Documentation](https://magpylib.readthedocs.io/en/latest)** for detailed information.
  - Please abide by our **[Code of Conduct](https://github.com/magpylib/magpylib/blob/main/CODE_OF_CONDUCT.md)**.
  - Contribute through **[Discussions](https://github.com/magpylib/magpylib/discussions)** and coding by following the **[Contribution Guide](https://github.com/magpylib/magpylib/blob/main/CONTRIBUTING.md)**. The Git project **[Issues](https://github.com/magpylib/magpylib/issues)** give an up-to-date list of potential enhancements and planned milestones. Propose new ones.
  - A **[Youtube video](https://www.youtube.com/watch?v=LeUx6cM1vcs)** introduction to Magpylib v4.0.0 within the **[GSC network](https://www.internationalcollaboration.org/).**
@@ -132,11 +132,11 @@
 A valid software citation could be
 
 ```
 @software{magpylib,
     author = {{Michael-Ortner et al.}},
     title = {magpylib},
     url = {https://magpylib.readthedocs.io/en/latest/},
-    version = {5.0.1},
+    version = {5.0.2},
     date = {2023-06-25},
 }
 ```
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 _[_M_y_B_i_n_d_e_r_ _l_i_n_k_]_[_b_l_a_c_k_]
 Magpylib is a Python package for calculating **3D static magnetic fields** of
 magnets, line currents and other sources. The computation is based on explicit
 expressions and is therefore **extremely fast**. A **user friendly API**
 enables convenient positioning of sources and observers. # Installation Install
 from PyPI using **pip** ``` pip install magpylib ``` Install from conda forge
 using **conda** ``` conda install -c conda-forge magpylib ``` Magpylib supports
-_Python3.8+_ and relies on common scientific computation libraries _Numpy_,
+_Python3.10+_ and relies on common scientific computation libraries _Numpy_,
 _Scipy_, _Matplotlib_ and _Plotly_. Optionally, _Pyvista_ is recommended as
 graphical backend. # Resources - Check out our **[Documentation](https://
 magpylib.readthedocs.io/en/latest)** for detailed information. - Please abide
 by our **[Code of Conduct](https://github.com/magpylib/magpylib/blob/main/
 CODE_OF_CONDUCT.md)**. - Contribute through **[Discussions](https://github.com/
 magpylib/magpylib/discussions)** and coding by following the **[Contribution
 Guide](https://github.com/magpylib/magpylib/blob/main/CONTRIBUTING.md)**. The
@@ -72,9 +72,9 @@
 bibtex entry for the [2020 open-access paper](https://www.sciencedirect.com/
 science/article/pii/S2352711020300170) would be ``` @article
 {ortner2020magpylib, title={Magpylib: A free Python package for magnetic field
 computation}, author={Ortner, Michael and Bandeira, Lucas Gabriel Coliado},
 journal={SoftwareX}, volume={11}, pages={100466}, year={2020}, publisher=
 {Elsevier} } ``` A valid software citation could be ``` @software{magpylib,
 author = {{Michael-Ortner et al.}}, title = {magpylib}, url = {https://
-magpylib.readthedocs.io/en/latest/}, version = {5.0.1}, date = {2023-06-25}, }
+magpylib.readthedocs.io/en/latest/}, version = {5.0.2}, date = {2023-06-25}, }
 ```
```

### Comparing `magpylib-5.0.1/docs/Makefile` & `magpylib-5.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/README.md` & `magpylib-5.0.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/docu/docu_graphics.md` & `magpylib-5.0.2/docs/_pages/docu/docu_graphics.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/docu/docu_index.md` & `magpylib-5.0.2/docs/_pages/docu/docu_index.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/docu/docu_magpylib_api.md` & `magpylib-5.0.2/docs/_pages/docu/docu_magpylib_api.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/docu/docu_physics.md` & `magpylib-5.0.2/docs/_pages/docu/docu_physics.md`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 The expressions used in Magpylib describe perfectly homogeneous magnets, surface charges, and line currents with natural boundary conditions. Magpylib is at its best when dealing with static air-coils (no eddy currents, no soft-magnetic cores) and high grade permanent magnets (Ferrite, NdFeB, SmCo or similar materials). When **magnet** permeabilities are below $\mu_r < 1.1$ the error typically undercuts few %. Demagnetization factors are not included. The line **current** solutions give the exact same field as outside of a wire that carries a homogeneous current.
 
 ## The analytical solutions
 
 Magnetic field computations in Magpylib are based on known analytical solutions (closed form expressions) to permanent magnet and current problems. The Magpylib implementations are based on the following literature references:
 
-- Field of cuboid magnets: \[Yang1999, Engel-Herbert2005, Camacho2013, Cichon2019\]
+- Field of cuboid magnets: \[Yang1990, Engel-Herbert2005, Camacho2013, Cichon2019\]
 - Field of cylindrical magnets: \[Furlani1994, Derby2009, Caciagli2018, Slanovc2021\]
 - Field of triangular surfaces: \[Guptasarma1999, Janssen2009, Rubeck2013\]
 - Field of the current loop: \[Ortner2022\]
 - all others derived by hand
 
 A short reflection on how these formulas can be achieved: In magnetostatics the magnetic field becomes conservative (Maxwell: $\nabla \times {\bf H} = 0$) and can thus be expressed through the magnetic scalar potential $\Phi_m$:
 
@@ -101,15 +101,15 @@
 
 ## Numerical stability
 
 Many expressions provided in the literature have very questionable numerical stability. Many of these problems are fixed in Magpylib, but one should be aware that accuracy can be a problem very close to objects, close the z-axis in cylindrical symmetries, at edge extensions, and at large distances. We are working on fixing these problems. Some details can be found in \[Ortner2022\].
 
 **References**
 
-- \[Yang1999\] Z. J. Yang et al., "Potential and force between a magnet and a bulk Y1Ba2Cu3O7-d superconductor studied by a mechanical pendulum", Superconductor Science and Technology 3(12):591, 1999
+- \[Yang1990\] Z. J. Yang et al., "Potential and force between a magnet and a bulk Y1Ba2Cu3O7-d superconductor studied by a mechanical pendulum", Superconductor Science and Technology 3(12):591, 1990
 - \[Engel-Herbert2005\] R. Engel-Herbert et al., Journal of Applied Physics 97(7):074504 - 074504-4 (2005)
 - \[Camacho2013\] J.M. Camacho and V. Sosa, "Alternative method to calculate the magnetic field of permanent magnets with azimuthal symmetry", Revista Mexicana de Fisica E 59 8–17, 2013
 - \[Cichon2019\] D. Cichon, R. Psiuk and H. Brauer, "A Hall-Sensor-Based Localization Method With Six Degrees of Freedom Using Unscented Kalman Filter", IEEE Sensors Journal, Vol. 19, No. 7, April 1, 2019.
 - \[Furlani1994\] E. P. Furlani, S. Reanik and W. Janson, "A Three-Dimensional Field Solution for Bipolar Cylinders", IEEE Transaction on Magnetics, VOL. 30, NO. 5, 1994
 - \[Derby2009\] N. Derby, "Cylindrical Magnets and Ideal Solenoids", arXiv:0909.3880v1, 2009
 - \[Caciagli2018\] A. Caciagli, R. J. Baars, A. P. Philipse and B. W. M. Kuipers, "Exact expression for the magnetic field of a finite cylinder with arbitrary uniform magnetization", Journal of Magnetism and Magnetic Materials 456 (2018) 423–432.
 - \[Slanovc2022\] F. Slanovc, M. Ortner, M. Moridi, C. Abert and D. Suess, "Full analytical solution for the magnetic field of uniformly magnetized cylinder tiles", submitted to Journal of Magnetism and Magnetic Materials.
```

### Comparing `magpylib-5.0.1/docs/_pages/gallery/gallery_app_end_of_shaft.md` & `magpylib-5.0.2/docs/_pages/gallery/gallery_app_end_of_shaft.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/gallery/gallery_app_helmholtz.md` & `magpylib-5.0.2/docs/_pages/gallery/gallery_app_helmholtz.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/gallery/gallery_index.md` & `magpylib-5.0.2/docs/_pages/gallery/gallery_index.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/gallery/gallery_misc_compound.md` & `magpylib-5.0.2/docs/_pages/gallery/gallery_misc_compound.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/gallery/gallery_misc_field_interpolation.md` & `magpylib-5.0.2/docs/_pages/gallery/gallery_misc_field_interpolation.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/gallery/gallery_shapes_convex_hull.md` & `magpylib-5.0.2/docs/_pages/gallery/gallery_shapes_convex_hull.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/gallery/gallery_shapes_pyvista.md` & `magpylib-5.0.2/docs/_pages/gallery/gallery_shapes_pyvista.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/gallery/gallery_shapes_superpos.md` & `magpylib-5.0.2/docs/_pages/gallery/gallery_shapes_superpos.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/gallery/gallery_shapes_triangle.md` & `magpylib-5.0.2/docs/_pages/gallery/gallery_shapes_triangle.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_collection.md` & `magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_collection.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_custom.md` & `magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_custom.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_field_computation.md` & `magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_field_computation.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_modelling_magnets.md` & `magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_modelling_magnets.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/gallery/gallery_tutorial_paths.md` & `magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_paths.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/gallery/gallery_vis_animations.md` & `magpylib-5.0.2/docs/_pages/gallery/gallery_vis_animations.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/gallery/gallery_vis_mpl_streamplot.md` & `magpylib-5.0.2/docs/_pages/gallery/gallery_vis_mpl_streamplot.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/gallery/gallery_vis_pv_streamlines.md` & `magpylib-5.0.2/docs/_pages/gallery/gallery_vis_pv_streamlines.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/gallery/gallery_vis_subplots.md` & `magpylib-5.0.2/docs/_pages/gallery/gallery_vis_subplots.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_pages/reso_get_started.md` & `magpylib-5.0.2/docs/_pages/reso_get_started.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 (get-started)=
 
 # Get Started
 
 ## Installation and Dependencies
 
-Magpylib supports *Python3.8+* and relies on common scientific computation libraries *Numpy*, *Scipy*, *Matplotlib* and *Plotly*. Optionally, *Pyvista* is recommended as graphical backend.
+Magpylib supports *Python3.10+* and relies on common scientific computation libraries *Numpy*, *Scipy*, *Matplotlib* and *Plotly*. Optionally, *Pyvista* is recommended as graphical backend.
 
 ::::{grid} 1 1 2 2
 :margin: 4 4 0 0
 :gutter: 4
 
 :::{grid-item-card} Install with pip:
 :text-align: center
```

### Comparing `magpylib-5.0.1/docs/_static/images/docu_classes_init_collection.png` & `magpylib-5.0.2/docs/_static/images/docu_classes_init_collection.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_classes_init_cuboid.png` & `magpylib-5.0.2/docs/_static/images/docu_classes_init_cuboid.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_classes_init_custom.png` & `magpylib-5.0.2/docs/_static/images/docu_classes_init_custom.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_classes_init_cylinder.png` & `magpylib-5.0.2/docs/_static/images/docu_classes_init_cylinder.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_classes_init_cylindersegment.png` & `magpylib-5.0.2/docs/_static/images/docu_classes_init_cylindersegment.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_classes_init_dipole.png` & `magpylib-5.0.2/docs/_static/images/docu_classes_init_dipole.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_classes_init_global_local.png` & `magpylib-5.0.2/docs/_static/images/docu_classes_init_global_local.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_classes_init_line.png` & `magpylib-5.0.2/docs/_static/images/docu_classes_init_line.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_classes_init_loop.png` & `magpylib-5.0.2/docs/_static/images/docu_classes_init_loop.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_classes_init_sensor.png` & `magpylib-5.0.2/docs/_static/images/docu_classes_init_sensor.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_classes_init_sphere.png` & `magpylib-5.0.2/docs/_static/images/docu_classes_init_sphere.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_classes_init_tetra.png` & `magpylib-5.0.2/docs/_static/images/docu_classes_init_tetra.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_classes_init_triangle.png` & `magpylib-5.0.2/docs/_static/images/docu_classes_init_triangle.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_classes_init_trimesh.png` & `magpylib-5.0.2/docs/_static/images/docu_classes_init_trimesh.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_field_comp_flow.png` & `magpylib-5.0.2/docs/_static/images/docu_field_comp_flow.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_field_superpos_cutout.png` & `magpylib-5.0.2/docs/_static/images/docu_field_superpos_cutout.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_field_superpos_union.png` & `magpylib-5.0.2/docs/_static/images/docu_field_superpos_union.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_index_icon_magpylib.png` & `magpylib-5.0.2/docs/_static/images/docu_index_icon_magpylib.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_index_icon_magpylib_show.png` & `magpylib-5.0.2/docs/_static/images/docu_index_icon_magpylib_show.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_index_icon_physics.png` & `magpylib-5.0.2/docs/_static/images/docu_index_icon_physics.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/docu_position_sketch.png` & `magpylib-5.0.2/docs/_static/images/docu_position_sketch.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/favicons/android-chrome-192x192.png` & `magpylib-5.0.2/docs/_static/images/favicons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/favicons/android-chrome-512x512.png` & `magpylib-5.0.2/docs/_static/images/favicons/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/favicons/apple-touch-icon.png` & `magpylib-5.0.2/docs/_static/images/favicons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/favicons/favicon-16x16.png` & `magpylib-5.0.2/docs/_static/images/favicons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/favicons/favicon-32x32.png` & `magpylib-5.0.2/docs/_static/images/favicons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/favicons/favicon.ico` & `magpylib-5.0.2/docs/_static/images/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_icon_WIP.png` & `magpylib-5.0.2/docs/_static/images/gallery_icon_WIP.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_icon_app_end_of_shaft.png` & `magpylib-5.0.2/docs/_static/images/gallery_icon_app_end_of_shaft.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_icon_app_helmholtz.png` & `magpylib-5.0.2/docs/_static/images/gallery_icon_app_helmholtz.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_icon_ext_custom_quadrupole.png` & `magpylib-5.0.2/docs/_static/images/gallery_icon_ext_custom_quadrupole.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_icon_misc_compound.png` & `magpylib-5.0.2/docs/_static/images/gallery_icon_misc_compound.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_icon_misc_field_interpolation.png` & `magpylib-5.0.2/docs/_static/images/gallery_icon_misc_field_interpolation.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_icon_shapes_convex_hull.png` & `magpylib-5.0.2/docs/_static/images/gallery_icon_shapes_convex_hull.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_icon_shapes_pyvista.png` & `magpylib-5.0.2/docs/_static/images/gallery_icon_shapes_pyvista.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_icon_shapes_superpos.png` & `magpylib-5.0.2/docs/_static/images/gallery_icon_shapes_superpos.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_icon_shapes_triangle.png` & `magpylib-5.0.2/docs/_static/images/gallery_icon_shapes_triangle.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_collection.png` & `magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_collection.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_custom.png` & `magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_custom.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_field_computation.png` & `magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_field_computation.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_modelling_magnets.png` & `magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_modelling_magnets.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_icon_tutorial_paths.png` & `magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_paths.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_icon_viz_animations.png` & `magpylib-5.0.2/docs/_static/images/gallery_icon_viz_animations.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_icon_viz_mpl_streamplot.png` & `magpylib-5.0.2/docs/_static/images/gallery_icon_viz_mpl_streamplot.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_icon_viz_pv_streamlines.png` & `magpylib-5.0.2/docs/_static/images/gallery_icon_viz_pv_streamlines.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_LDratio.png` & `magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_LDratio.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_datasheet.png` & `magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_datasheet.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_datasheet2.png` & `magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_datasheet2.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_fieldcomparison.png` & `magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_fieldcomparison.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_hysteresis.png` & `magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_hysteresis.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/gallery_tutorial_magnet_table.png` & `magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_table.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/getting_started_animation.png` & `magpylib-5.0.2/docs/_static/images/getting_started_animation.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/getting_started_complex_shapes.png` & `magpylib-5.0.2/docs/_static/images/getting_started_complex_shapes.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/getting_started_fundamentals1.png` & `magpylib-5.0.2/docs/_static/images/getting_started_fundamentals1.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/getting_started_styles.png` & `magpylib-5.0.2/docs/_static/images/getting_started_styles.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/index_flowchart.png` & `magpylib-5.0.2/docs/_static/images/index_flowchart.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/index_head.png` & `magpylib-5.0.2/docs/_static/images/index_head.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/index_icon_academic.png` & `magpylib-5.0.2/docs/_static/images/index_icon_academic.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/index_icon_contributing.png` & `magpylib-5.0.2/docs/_static/images/index_icon_contributing.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/index_icon_docu.png` & `magpylib-5.0.2/docs/_static/images/index_icon_docu.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/index_icon_gallery.png` & `magpylib-5.0.2/docs/_static/images/index_icon_gallery.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/index_icon_getting_started.png` & `magpylib-5.0.2/docs/_static/images/index_icon_getting_started.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/index_icon_github.png` & `magpylib-5.0.2/docs/_static/images/index_icon_github.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/magpylib_flag.png` & `magpylib-5.0.2/docs/_static/images/magpylib_flag.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/images/magpylib_logo.png` & `magpylib-5.0.2/docs/_static/images/magpylib_logo.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/videos/axis.mp4` & `magpylib-5.0.2/docs/_static/videos/axis.mp4`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/_static/webcode/copybutton.js` & `magpylib-5.0.2/docs/_static/webcode/copybutton.js`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/conf.py` & `magpylib-5.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/index.md` & `magpylib-5.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/docs/make.bat` & `magpylib-5.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/__init__.py` & `magpylib-5.0.2/magpylib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 The original software publication (version 2):
 
 https://www.sciencedirect.com/science/article/pii/S2352711020300170
 
 """
 # module level dunders
-__version__ = "5.0.1"
+__version__ = "5.0.2"
 __author__ = "Michael Ortner & Alexandre Boisselet"
 __credits__ = "The Magpylib community"
 __all__ = [
     "magnet",
     "current",
     "misc",
     "getB",
```

### Comparing `magpylib-5.0.1/magpylib/_src/defaults/defaults_classes.py` & `magpylib-5.0.2/magpylib/_src/defaults/defaults_classes.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/defaults/defaults_utility.py` & `magpylib-5.0.2/magpylib/_src/defaults/defaults_utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/defaults/defaults_values.py` & `magpylib-5.0.2/magpylib/_src/defaults/defaults_values.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/display/backend_matplotlib.py` & `magpylib-5.0.2/magpylib/_src/display/backend_matplotlib.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/display/backend_plotly.py` & `magpylib-5.0.2/magpylib/_src/display/backend_plotly.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/display/backend_pyvista.py` & `magpylib-5.0.2/magpylib/_src/display/backend_pyvista.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/display/display.py` & `magpylib-5.0.2/magpylib/_src/display/display.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/display/sensor_mesh.py` & `magpylib-5.0.2/magpylib/_src/display/sensor_mesh.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/display/traces_base.py` & `magpylib-5.0.2/magpylib/_src/display/traces_base.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/display/traces_core.py` & `magpylib-5.0.2/magpylib/_src/display/traces_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,14 +314,15 @@
     trace = merge_mesh3d(*traces)
     trace["ismagnet"] = False  # neede to avoid updating mag mesh
     return trace
 
 
 def get_closest_vertices(faces_subsets, vertices):
     """Get closest pairs of points between disconnected subsets of faces indices"""
+    # pylint: disable=used-before-assignment
     nparts = len(faces_subsets)
     inds_subsets = [np.unique(v) for v in faces_subsets]
     closest_verts_list = []
     if nparts > 1:
         connected = [np.min(inds_subsets[0])]
         while len(connected) < nparts:
             prev_min = float("inf")
```

### Comparing `magpylib-5.0.1/magpylib/_src/display/traces_generic.py` & `magpylib-5.0.2/magpylib/_src/display/traces_generic.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/display/traces_utility.py` & `magpylib-5.0.2/magpylib/_src/display/traces_utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -495,18 +495,20 @@
                     pass
                 pts = pts.reshape(-1, 3)
                 if pts.size != 0:
                     min_max = np.nanmin(pts, axis=0), np.nanmax(pts, axis=0)
                     for v, min_, max_ in zip(ranges.values(), *min_max):
                         v.extend([min_, max_])
         if trace3d_found:
+            # SET 3D PLOT BOUNDARIES
+            # collect min/max from all elements
             r = np.array([[np.nanmin(v), np.nanmax(v)] for v in ranges.values()])
             size = np.diff(r, axis=1)
-            size[size == 0] = 1
             m = size.max() / 2
+            m = 1 if m == 0 else m
             center = r.mean(axis=1)
             ranges = np.array([center - m * (1 + zoom), center + m * (1 + zoom)]).T
     if not traces or not trace3d_found:
         ranges = np.array([[-1.0, 1.0]] * 3)
     return ranges
```

### Comparing `magpylib-5.0.1/magpylib/_src/fields/field_BH_circle.py` & `magpylib-5.0.2/magpylib/_src/fields/field_BH_circle.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/fields/field_BH_cuboid.py` & `magpylib-5.0.2/magpylib/_src/fields/field_BH_cuboid.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         B-field generated by Cuboids at observer positions.
 
     Notes
     -----
     Field computations via magnetic surface charge density. Published
     several times with similar expressions:
 
-    Yang: Superconductor Science and Technology 3(12):591 (1999)
+    Yang: Superconductor Science and Technology 3(12):591 (1990)
 
     Engel-Herbert: Journal of Applied Physics 97(7):074504 - 074504-4 (2005)
 
     Camacho: Revista Mexicana de Fisica E 59 (2013) 8-17
 
     Avoiding indeterminate forms:
```

### Comparing `magpylib-5.0.1/magpylib/_src/fields/field_BH_cylinder.py` & `magpylib-5.0.2/magpylib/_src/fields/field_BH_cylinder.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/fields/field_BH_cylinder_segment.py` & `magpylib-5.0.2/magpylib/_src/fields/field_BH_cylinder_segment.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/fields/field_BH_dipole.py` & `magpylib-5.0.2/magpylib/_src/fields/field_BH_dipole.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/fields/field_BH_polyline.py` & `magpylib-5.0.2/magpylib/_src/fields/field_BH_polyline.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/fields/field_BH_sphere.py` & `magpylib-5.0.2/magpylib/_src/fields/field_BH_sphere.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/fields/field_BH_tetrahedron.py` & `magpylib-5.0.2/magpylib/_src/fields/field_BH_tetrahedron.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/fields/field_BH_triangle.py` & `magpylib-5.0.2/magpylib/_src/fields/field_BH_triangle.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/fields/field_BH_triangularmesh.py` & `magpylib-5.0.2/magpylib/_src/fields/field_BH_triangularmesh.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/fields/field_wrap_BH.py` & `magpylib-5.0.2/magpylib/_src/fields/field_wrap_BH.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/fields/special_cel.py` & `magpylib-5.0.2/magpylib/_src/fields/special_cel.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/fields/special_el3.py` & `magpylib-5.0.2/magpylib/_src/fields/special_el3.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/input_checks.py` & `magpylib-5.0.2/magpylib/_src/input_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -541,17 +541,14 @@
     if "sources" in allow.split("+"):
         wanted_types += (BaseSource,)
     if "sensors" in allow.split("+"):
         wanted_types += (Sensor,)
     if "collections" in allow.split("+"):
         wanted_types += (Collection,)
 
-    if typechecks:
-        all_types = (BaseSource, Sensor, Collection)
-
     obj_list = []
     for obj in inp:
         # add to list if wanted type
         if isinstance(obj, wanted_types):
             obj_list.append(obj)
 
         # recursion
@@ -560,15 +557,16 @@
                 obj,
                 allow=allow,
                 recursive=recursive,
                 typechecks=typechecks,
             )
 
         # typechecks
-        if typechecks and not isinstance(obj, all_types):
+        # pylint disable possibly-used-before-assignment
+        if typechecks and not isinstance(obj, (BaseSource, Sensor, Collection)):
             raise MagpylibBadUserInput(
                 f"Input objects must be {allow} or a flat list thereof.\n"
                 f"Instead received {type(obj)}."
             )
 
     return obj_list
```

### Comparing `magpylib-5.0.1/magpylib/_src/obj_classes/class_BaseDisplayRepr.py` & `magpylib-5.0.2/magpylib/_src/obj_classes/class_BaseDisplayRepr.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/obj_classes/class_BaseExcitations.py` & `magpylib-5.0.2/magpylib/_src/obj_classes/class_BaseExcitations.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/obj_classes/class_BaseGeo.py` & `magpylib-5.0.2/magpylib/_src/obj_classes/class_BaseGeo.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/obj_classes/class_BaseTransform.py` & `magpylib-5.0.2/magpylib/_src/obj_classes/class_BaseTransform.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/obj_classes/class_Collection.py` & `magpylib-5.0.2/magpylib/_src/obj_classes/class_Collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -502,14 +502,15 @@
 
     def _validate_getBH_inputs(self, *inputs):
         """
         select correct sources and observers for getBHJM_level2
         """
         # pylint: disable=protected-access
         # pylint: disable=too-many-branches
+        # pylint: disable=possibly-used-before-assignment
         current_sources = format_obj_input(self, allow="sources")
         current_sensors = format_obj_input(self, allow="sensors")
 
         # if collection includes source and observer objects, select itself as
         #   source and observer in gethBH
         if current_sensors and current_sources:
             sources, sensors = self, self
```

### Comparing `magpylib-5.0.1/magpylib/_src/obj_classes/class_Sensor.py` & `magpylib-5.0.2/magpylib/_src/obj_classes/class_Sensor.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/obj_classes/class_current_Circle.py` & `magpylib-5.0.2/magpylib/_src/obj_classes/class_current_Circle.py`

 * *Files 11% similar despite different names*

```diff
@@ -59,33 +59,21 @@
     >>> src = magpy.current.Circle(current=100, diameter=2)
     >>> H = src.getH((.01,.01,.01))
     >>> print(H)
     [7.50093701e-03 7.50093701e-03 4.99999967e+01]
 
     We rotate the source object, and compute the B-field, this time at a set of observer positions:
 
-    >>> src.rotate_from_angax(45, 'x')
+    >>> src.rotate_from_angax(90, 'x')
     Circle(id=...)
     >>> B = src.getB([(.01,.01,.01), (.02,.02,.02), (.03,.03,.03)])
     >>> print(B)
-    [[-1.63585841e-24 -4.44388287e-05  4.44388287e-05]
-     [-6.55449367e-24 -4.44688604e-05  4.44688604e-05]
-     [-9.85948765e-24 -4.45190261e-05  4.45190261e-05]]
-
-    The same result is obtained when the rotated source moves along a path away from an
-    observer at position (1,1,1). This time we use a `Sensor` object as observer.
-
-    >>> src.move([(-.01,-.01,-.01), (-.02,-.02,-.02)])
-    Circle(id=...)
-    >>> sens = magpy.Sensor(position=(.01,.01,.01))
-    >>> B = src.getB(sens)
-    >>> print(B)
-    [[-1.63585841e-24 -4.44388287e-05  4.44388287e-05]
-     [-6.55449367e-24 -4.44688604e-05  4.44688604e-05]
-     [-9.85948765e-24 -4.45190261e-05  4.45190261e-05]]
+    [[-9.42595544e-09 -6.28318490e-05 -9.42595544e-09]
+     [-3.77179218e-08 -6.28317871e-05 -3.77179218e-08]
+     [-8.49179752e-08 -6.28315185e-05 -8.49179752e-08]]
     """
 
     _field_func = staticmethod(BHJM_circle)
     _field_func_kwargs_ndim = {"current": 1, "diameter": 1}
     get_trace = make_Circle
 
     def __init__(
```

### Comparing `magpylib-5.0.1/magpylib/_src/obj_classes/class_current_Polyline.py` & `magpylib-5.0.2/magpylib/_src/obj_classes/class_current_Polyline.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,33 +63,21 @@
     ... )
     >>> H = src.getH((.01,.01,.01))
     >>> print(H)
     [3.16063859 3.16063859 0.76687556]
 
     We rotate the source object, and compute the B-field, this time at a set of observer positions:
 
-    >>> src.rotate_from_angax(45, 'x')
+    >>> src.rotate_from_angax(90, 'x')
     Polyline(id=...)
     >>> B = src.getB([(.01,.01,.01), (.02,.02,.02), (.03,.03,.03)])
     >>> print(B)
-    [[-1.04529728e-21  3.50341393e-06 -3.50341393e-06]
-     [-9.28140349e-23  3.62181325e-07 -3.62181325e-07]
-     [-1.72744075e-23  1.03643004e-07 -1.03643004e-07]]
-
-    The same result is obtained when the rotated source moves along a path away from an
-    observer at position (1,1,1). This time we use a `Sensor` object as observer.
-
-    >>> src.move([(-.01,-.01,-.01), (-.02,-.02,-.02)])
-    Polyline(id=...)
-    >>> sens = magpy.Sensor(position=(.01,.01,.01))
-    >>> B = src.getB(sens)
-    >>> print(B)
-    [[-1.04529728e-21  3.50341393e-06 -3.50341393e-06]
-     [-9.28140349e-23  3.62181325e-07 -3.62181325e-07]
-     [-1.72744075e-23  1.03643004e-07 -1.03643004e-07]]
+    [[-3.97177559e-06 -9.63684251e-07 -3.97177559e-06]
+     [-4.90331150e-07 -3.11039072e-08 -4.90331150e-07]
+     [-1.43908549e-07 -4.10438492e-09 -1.43908549e-07]]
     """
 
     # pylint: disable=dangerous-default-value
     _field_func = staticmethod(current_vertices_field)
     _field_func_kwargs_ndim = {
         "current": 1,
         "vertices": 3,
```

### Comparing `magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_Cuboid.py` & `magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_Cuboid.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_Cylinder.py` & `magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_Cylinder.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py` & `magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_Sphere.py` & `magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_Sphere.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py` & `magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/obj_classes/class_magnet_TriangularMesh.py` & `magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_TriangularMesh.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/obj_classes/class_misc_CustomSource.py` & `magpylib-5.0.2/magpylib/_src/obj_classes/class_misc_CustomSource.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/obj_classes/class_misc_Dipole.py` & `magpylib-5.0.2/magpylib/_src/obj_classes/class_misc_Dipole.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/obj_classes/class_misc_Triangle.py` & `magpylib-5.0.2/magpylib/_src/obj_classes/class_misc_Triangle.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/style.py` & `magpylib-5.0.2/magpylib/_src/style.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/_src/utility.py` & `magpylib-5.0.2/magpylib/_src/utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/core/__init__.py` & `magpylib-5.0.2/magpylib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/graphics/model3d/__init__.py` & `magpylib-5.0.2/magpylib/graphics/model3d/__init__.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/magpylib/magnet/__init__.py` & `magpylib-5.0.2/magpylib/magnet/__init__.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/pyproject.toml` & `magpylib-5.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,37 +2,36 @@
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "magpylib"
 dynamic = ["version"]
 dependencies = [
-    "numpy>=1.20",
-    "scipy>=1.7",
-    "matplotlib>=3.3",
-    "plotly>=5.3",
+    "numpy>=1.23",
+    "scipy>=1.8",
+    "matplotlib>=3.6",
+    "plotly>=5.16",
     ]
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 authors = [
     {name = "Michael Ortner", email = "magpylib@gmail.com"},
 ]
 maintainers = [
     {name = "Alexandre Boisselet", email = "alexabois+magpylib@gmail.com"}
 ]
 description = "Free Python3 package to compute magnetic fields."
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["magnetism", "physics", "analytical", "electromagnetic", "magnetic-field", "B-field"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Education",
     "Operating System :: OS Independent",
 ]
 
 [project.optional-dependencies]
```

### Comparing `magpylib-5.0.1/tests/test_BHMJ_level.py` & `magpylib-5.0.2/tests/test_BHMJ_level.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_BaseTransform.py` & `magpylib-5.0.2/tests/test_BaseTransform.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_Coumpound_setters.py` & `magpylib-5.0.2/tests/test_Coumpound_setters.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_CustomSource.py` & `magpylib-5.0.2/tests/test_CustomSource.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test__missing_optional_modules.py` & `magpylib-5.0.2/tests/test__missing_optional_modules.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_core_physics_consistency.py` & `magpylib-5.0.2/tests/test_core_physics_consistency.py`

 * *Files 4% similar despite different names*

```diff
@@ -351,48 +351,56 @@
     pol = mom / vol * MU0
     Bcub = BHJM_magnet_cuboid(
         field="H",
         observers=obs,
         dimension=dim,
         polarization=pol,
     )
-    np.testing.assert_allclose(Bdip, Bcub)
+    # np.testing.assert_allclose(Bdip, Bcub)
+    err = np.linalg.norm(Bdip - Bcub) / np.linalg.norm(Bdip)
+    assert err < 1e-6
 
     dim = np.array([(0.5, 0.5)] * 2)
     vol = 0.25**2 * np.pi * 0.5
     pol = mom / vol * MU0
     Bcyl = BHJM_magnet_cylinder(
         field="H",
         observers=obs,
         dimension=dim,
         polarization=pol,
     )
-    np.testing.assert_allclose(Bdip, Bcyl)
+    # np.testing.assert_allclose(Bdip, Bcyl, rtol=1e-6)
+    err = np.linalg.norm(Bdip - Bcyl) / np.linalg.norm(Bdip)
+    assert err < 1e-6
 
     vert = np.array([[(0, 0, 0), (0, 0, 0.1), (0.1, 0, 0), (0, 0.1, 0)]] * 2)
     vol = 1 / 6 * 1e-3
     pol = mom / vol * MU0
     Btetra = BHJM_magnet_tetrahedron(
         field="H",
         observers=obs,
         vertices=vert,
         polarization=pol,
     )
-    np.testing.assert_allclose(Bdip, Btetra, rtol=1e-3)
+    # np.testing.assert_allclose(Bdip, Btetra, rtol=1e-3)
+    err = np.linalg.norm(Bdip - Btetra) / np.linalg.norm(Bdip)
+    assert err < 1e-3
 
     dim = np.array([(0.1, 0.2, 0.1, -25, 25)] * 2)
     vol = 3 * np.pi * (50 / 360) * 1e-3
     pol = mom / vol * MU0
     Bcys = BHJM_cylinder_segment(
         field="H",
         observers=obs + np.array((0.15, 0, 0)),
         dimension=dim,
         polarization=pol,
     )
-    np.testing.assert_allclose(Bdip, Bcys, rtol=1e-4)
+    # np.testing.assert_allclose(Bdip, Bcys, rtol=1e-4)
+    err = np.linalg.norm(Bdip - Bcys) / np.linalg.norm(Bdip)
+    assert err < 1e-4
 
 
 # --> Circle
 def test_core_physics_circle_VS_webpage_numbers():
     """
     Compare Circle on-axis field vs e-magnetica & hyperphysics
     """
```

### Comparing `magpylib-5.0.1/tests/test_default_utils.py` & `magpylib-5.0.2/tests/test_default_utils.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_defaults.py` & `magpylib-5.0.2/tests/test_defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     "display_style_markers_marker_color": ("wrongcolor",),
     "display_style_markers_marker_symbol": ("wrongsymbol",),
 }
 
 
 def get_bad_test_data():
     """create parametrized bad style test data"""
+    # pylint: disable=possibly-used-before-assignment
     bad_test_data = []
     for k, tup in bad_inputs.items():
         for v in tup:
             if "description_text" not in k:
                 if "color" in k and "transition" not in k and "mode" not in k:
                     # color attributes use a the color validator, which raises a ValueError
                     errortype = ValueError
```

### Comparing `magpylib-5.0.1/tests/test_display_matplotlib.py` & `magpylib-5.0.2/tests/test_display_matplotlib.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_display_plotly.py` & `magpylib-5.0.2/tests/test_display_plotly.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_display_pyvista.py` & `magpylib-5.0.2/tests/test_display_pyvista.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_display_utility.py` & `magpylib-5.0.2/tests/test_display_utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_elliptics.py` & `magpylib-5.0.2/tests/test_elliptics.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_exceptions.py` & `magpylib-5.0.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_field_cylinder.py` & `magpylib-5.0.2/tests/test_field_cylinder.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_getBH_dict.py` & `magpylib-5.0.2/tests/test_getBH_dict.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_getBH_interfaces.py` & `magpylib-5.0.2/tests/test_getBH_interfaces.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_getBH_level2.py` & `magpylib-5.0.2/tests/test_getBH_level2.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,42 +240,50 @@
     x1b = np.array([-19.64, 0, 0]) * 1e-3
     x2b = np.array([-13.89, 13.89, 0]) * 1e-3
     x3b = np.array([0, 19.64, 0]) * 1e-3
 
     B = magpy.getB(src, poss, squeeze=True)
     Btest = x1
     np.testing.assert_allclose(
-        np.around(B, decimals=5),
+        B,
         Btest,
+        rtol=1e-4,
+        atol=1e-5,
         err_msg="FAIL: mag  +  pos",
     )
 
     B = magpy.getB([src], [sens], squeeze=True)
     Btest = np.array([x1, x2, x3])
     np.testing.assert_allclose(
-        np.around(B, decimals=5),
+        B,
         Btest,
+        rtol=1e-4,
+        atol=1e-5,
         err_msg="FAIL: mag  +  sens_rot_path",
     )
 
     B = magpy.getB([src], [sens, poss], squeeze=True)
     Btest = np.array([[x1, x1], [x2, x1], [x3, x1]])
     np.testing.assert_allclose(
-        np.around(B, decimals=5),
+        B,
         Btest,
+        rtol=1e-4,
+        atol=1e-5,
         err_msg="FAIL: mag  +  sens_rot_path, pos",
     )
 
     B = magpy.getB([src, col], [sens, poss], squeeze=True)
     Btest = np.array(
         [[[x1, x1], [x2, x1], [x3, x1]], [[x1b, x1b], [x2b, x1b], [x3b, x1b]]]
     )
     np.testing.assert_allclose(
-        np.around(B, decimals=5),
+        B,
         Btest,
+        rtol=1e-4,
+        atol=1e-5,
         err_msg="FAIL: mag,col  +  sens_rot_path, pos",
     )
 
 
 def test_sensor_rotation3():
     """testing rotated static sensor path"""
     # case static sensor rot
```

### Comparing `magpylib-5.0.1/tests/test_input_checks.py` & `magpylib-5.0.2/tests/test_input_checks.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_numerical_stability.py` & `magpylib-5.0.2/tests/test_numerical_stability.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_obj_BaseGeo.py` & `magpylib-5.0.2/tests/test_obj_BaseGeo.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,27 @@
     bgeo.rotate_from_angax(33, (3, 2, 1), anchor=0, start=-1)
     poss += [bgeo.position.copy()]
     rots += [bgeo.orientation.as_rotvec()]
 
     poss = np.array(poss)
     rots = np.array(rots)
 
-    np.testing.assert_allclose(poss, ptest, err_msg="test_BaseGeo bad position")
-    np.testing.assert_allclose(rots, otest, err_msg="test_BaseGeo bad orientation")
+    # avoid generating different zeros in macos CI tests (atol=1e-6)
+    np.testing.assert_allclose(
+        poss,
+        ptest,
+        atol=1e-6,
+        err_msg="test_BaseGeo bad position",
+    )
+    np.testing.assert_allclose(
+        rots,
+        otest,
+        atol=1e-6,
+        err_msg="test_BaseGeo bad orientation",
+    )
 
 
 def test_rotate_vs_rotate_from():
     """testing rotate vs rotate_from_angax"""
     roz = [
         (0.1, 0.2, 0.3),
         (-0.1, -0.1, -0.1),
```

### Comparing `magpylib-5.0.1/tests/test_obj_BaseGeo_v4motion.py` & `magpylib-5.0.2/tests/test_obj_BaseGeo_v4motion.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_obj_Circle.py` & `magpylib-5.0.2/tests/test_obj_Circle.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_obj_Collection.py` & `magpylib-5.0.2/tests/test_obj_Collection.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_obj_Collection_child_parent.py` & `magpylib-5.0.2/tests/test_obj_Collection_child_parent.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_obj_Collection_v4motion.py` & `magpylib-5.0.2/tests/test_obj_Collection_v4motion.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_obj_Cuboid.py` & `magpylib-5.0.2/tests/test_obj_Cuboid.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_obj_Cylinder.py` & `magpylib-5.0.2/tests/test_obj_Cylinder.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_obj_CylinderSegment.py` & `magpylib-5.0.2/tests/test_obj_CylinderSegment.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_obj_Dipole.py` & `magpylib-5.0.2/tests/test_obj_Dipole.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_obj_Polyline.py` & `magpylib-5.0.2/tests/test_obj_Polyline.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_obj_Sensor.py` & `magpylib-5.0.2/tests/test_obj_Sensor.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_obj_Sphere.py` & `magpylib-5.0.2/tests/test_obj_Sphere.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_obj_Tetrahedron.py` & `magpylib-5.0.2/tests/test_obj_Tetrahedron.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_obj_Triangle.py` & `magpylib-5.0.2/tests/test_obj_Triangle.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_obj_TriangularMesh.py` & `magpylib-5.0.2/tests/test_obj_TriangularMesh.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_path.py` & `magpylib-5.0.2/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_physics_consistency.py` & `magpylib-5.0.2/tests/test_physics_consistency.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_scaling.py` & `magpylib-5.0.2/tests/test_scaling.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_utility.py` & `magpylib-5.0.2/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/test_vs_mag2.py` & `magpylib-5.0.2/tests/test_vs_mag2.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/testdata/testdata_Collection.p` & `magpylib-5.0.2/tests/testdata/testdata_Collection.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/testdata/testdata_Collection_setter.npy` & `magpylib-5.0.2/tests/testdata/testdata_Collection_setter.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/testdata/testdata_Cuboid.p` & `magpylib-5.0.2/tests/testdata/testdata_Cuboid.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/testdata/testdata_Sphere.p` & `magpylib-5.0.2/tests/testdata/testdata_Sphere.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/testdata/testdata_compound_setter_cases.npy` & `magpylib-5.0.2/tests/testdata/testdata_compound_setter_cases.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/testdata/testdata_cy_cases.npy` & `magpylib-5.0.2/tests/testdata/testdata_cy_cases.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/testdata/testdata_el3.npy` & `magpylib-5.0.2/tests/testdata/testdata_el3.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/testdata/testdata_el3_angle.npy` & `magpylib-5.0.2/tests/testdata/testdata_el3_angle.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/testdata/testdata_femDat_cylinder_tile2.npy` & `magpylib-5.0.2/tests/testdata/testdata_femDat_cylinder_tile2.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/testdata/testdata_field_BH_cuboid.p` & `magpylib-5.0.2/tests/testdata/testdata_field_BH_cuboid.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/testdata/testdata_field_BH_cylinder.p` & `magpylib-5.0.2/tests/testdata/testdata_field_BH_cylinder.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/testdata/testdata_full_cyl.npy` & `magpylib-5.0.2/tests/testdata/testdata_full_cyl.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/testdata/testdata_path_BaseGeo.p` & `magpylib-5.0.2/tests/testdata/testdata_path_BaseGeo.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tests/testdata/testdata_vs_mag2.p` & `magpylib-5.0.2/tests/testdata/testdata_vs_mag2.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.1/tox.ini` & `magpylib-5.0.2/tox.ini`

 * *Files 21% similar despite different names*

```diff
@@ -4,16 +4,14 @@
     py311
 
 [gh]
 python =
     3.12 = py312
     3.11 = py311 #, type
     3.10 = py310
-    3.9 = py39
-    3.8 = py38
 
 [testenv]
 description = run the tests with pytest
 package = wheel
 wheel_build_env = .pkg
 deps =
     pytest>=7
```

### Comparing `magpylib-5.0.1/PKG-INFO` & `magpylib-5.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: magpylib
-Version: 5.0.1
+Version: 5.0.2
 Summary: Free Python3 package to compute magnetic fields.
 Keywords: magnetism,physics,analytical,electromagnetic,magnetic-field,B-field
 Author-email: Michael Ortner <magpylib@gmail.com>
 Maintainer-email: Alexandre Boisselet <alexabois+magpylib@gmail.com>
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: OS Independent
-Requires-Dist: numpy>=1.20
-Requires-Dist: scipy>=1.7
-Requires-Dist: matplotlib>=3.3
-Requires-Dist: plotly>=5.3
+Requires-Dist: numpy>=1.23
+Requires-Dist: scipy>=1.8
+Requires-Dist: matplotlib>=3.6
+Requires-Dist: plotly>=5.16
 Requires-Dist: jupytext ; extra == "binder"
 Requires-Dist: jupyterlab>=3.2 ; extra == "binder"
 Requires-Dist: jupyterlab-myst ; extra == "binder"
 Requires-Dist: pre-commit ; extra == "code_style"
 Requires-Dist: sphinx==7.2 ; extra == "docs"
 Requires-Dist: sphinx-design ; extra == "docs"
 Requires-Dist: sphinx-thebe ; extra == "docs"
@@ -72,15 +71,15 @@
 </a>
 <a href="https://codecov.io/gh/magpylib/magpylib"> <img src="https://codecov.io/gh/magpylib/magpylib/branch/main/graph/badge.svg">
 </a>
 <a href="https://pypi.org/project/magpylib/"> <img src="https://badge.fury.io/py/magpylib.svg" alt="PyPI version" height="18">
 </a>
 <a href="https://anaconda.org/conda-forge/magpylib"> <img src="https://anaconda.org/conda-forge/magpylib/badges/version.svg" alt="Conda Cloud" height="18">
 </a>
-<a href="https://mybinder.org/v2/gh/magpylib/magpylib/5.0.0?filepath=docs%2Fexamples"> <img src="https://mybinder.org/badge_logo.svg" alt="MyBinder link" height="18">
+<a href="https://mybinder.org/v2/gh/magpylib/magpylib/5.0.2?filepath=docs%2Fexamples"> <img src="https://mybinder.org/badge_logo.svg" alt="MyBinder link" height="18">
 </a>
 <a href="https://github.com/psf/black"> <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="black" height="18">
 </a>
 </div>
 
 Magpylib is a Python package for calculating **3D static magnetic fields** of magnets, line currents and other sources. The computation is based on explicit expressions and is therefore **extremely fast**. A **user friendly API** enables convenient positioning of sources and observers.
 
@@ -90,15 +89,15 @@
 ```
 pip install magpylib
 ```
 Install from conda forge using **conda**
 ```
 conda install -c conda-forge magpylib
 ```
-Magpylib supports _Python3.8+_ and relies on common scientific computation libraries _Numpy_, _Scipy_, _Matplotlib_ and _Plotly_. Optionally, _Pyvista_ is recommended as graphical backend.
+Magpylib supports _Python3.10+_ and relies on common scientific computation libraries _Numpy_, _Scipy_, _Matplotlib_ and _Plotly_. Optionally, _Pyvista_ is recommended as graphical backend.
 
 # Resources
 
  - Check out our **[Documentation](https://magpylib.readthedocs.io/en/latest)** for detailed information.
  - Please abide by our **[Code of Conduct](https://github.com/magpylib/magpylib/blob/main/CODE_OF_CONDUCT.md)**.
  - Contribute through **[Discussions](https://github.com/magpylib/magpylib/discussions)** and coding by following the **[Contribution Guide](https://github.com/magpylib/magpylib/blob/main/CONTRIBUTING.md)**. The Git project **[Issues](https://github.com/magpylib/magpylib/issues)** give an up-to-date list of potential enhancements and planned milestones. Propose new ones.
  - A **[Youtube video](https://www.youtube.com/watch?v=LeUx6cM1vcs)** introduction to Magpylib v4.0.0 within the **[GSC network](https://www.internationalcollaboration.org/).**
@@ -188,12 +187,12 @@
 A valid software citation could be
 
 ```
 @software{magpylib,
     author = {{Michael-Ortner et al.}},
     title = {magpylib},
     url = {https://magpylib.readthedocs.io/en/latest/},
-    version = {5.0.1},
+    version = {5.0.2},
     date = {2023-06-25},
 }
 ```
```

#### html2text {}

```diff
@@ -1,59 +1,58 @@
-Metadata-Version: 2.1 Name: magpylib Version: 5.0.1 Summary: Free Python3
+Metadata-Version: 2.1 Name: magpylib Version: 5.0.2 Summary: Free Python3
 package to compute magnetic fields. Keywords:
 magnetism,physics,analytical,electromagnetic,magnetic-field,B-field Author-
 email: Michael Ortner
 gmail.com> Maintainer-email: Alexandre Boisselet
-magpylib@gmail.com> Requires-Python: >=3.8 Description-Content-Type: text/
+magpylib@gmail.com> Requires-Python: >=3.10 Description-Content-Type: text/
 markdown Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Science/Research Classifier: Intended Audience :: Education
-Classifier: Operating System :: OS Independent Requires-Dist: numpy>=1.20
-Requires-Dist: scipy>=1.7 Requires-Dist: matplotlib>=3.3 Requires-Dist:
-plotly>=5.3 Requires-Dist: jupytext ; extra == "binder" Requires-Dist:
-jupyterlab>=3.2 ; extra == "binder" Requires-Dist: jupyterlab-myst ; extra ==
-"binder" Requires-Dist: pre-commit ; extra == "code_style" Requires-Dist:
-sphinx==7.2 ; extra == "docs" Requires-Dist: sphinx-design ; extra == "docs"
-Requires-Dist: sphinx-thebe ; extra == "docs" Requires-Dist: sphinx-favicon ;
-extra == "docs" Requires-Dist: sphinx-gallery ; extra == "docs" Requires-Dist:
-sphinx-copybutton ; extra == "docs" Requires-Dist: sphinx-book-theme ; extra ==
-"docs" Requires-Dist: myst-nb ; extra == "docs" Requires-Dist: pandas ; extra
-== "docs" Requires-Dist: numpy-stl ; extra == "docs" Requires-Dist: pyvista ;
-extra == "docs" Requires-Dist: tox>=4.11 ; extra == "test" Requires-Dist:
-pytest>=7.4 ; extra == "test" Requires-Dist: pylint>3.0 ; extra == "test"
-Requires-Dist: coverage ; extra == "test" Requires-Dist: pandas ; extra ==
-"test" Requires-Dist: pyvista ; extra == "test" Requires-Dist: ipywidgets ;
-extra == "test" Requires-Dist: imageio[tifffile, ffmpeg] ; extra == "test"
-Requires-Dist: jupyterlab ; extra == "test" Project-URL: Bug Tracker, https://
-github.com/magpylib/magpylib/issues Project-URL: Changelog, https://github.com/
-magpylib/magpylib/blob/master/CHANGELOG.md Project-URL: Documentation, https://
-magpylib.readthedocs.io/en/latest/ Project-URL: Repository, https://github.com/
-magpylib/magpylib.git Provides-Extra: binder Provides-Extra: code_style
-Provides-Extra: docs Provides-Extra: test > [!WARNING] > Version 5 introduces
-critical breaking changes with, among others, the _move to SI units_. We
-recommended to pin your dependencies to `magpylib>=4.5<5` until you are ready
-to migrate to the latest version! ([see details](https://github.com/magpylib/
-magpylib/discussions/647))
+:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Science/Research Classifier:
+Intended Audience :: Education Classifier: Operating System :: OS Independent
+Requires-Dist: numpy>=1.23 Requires-Dist: scipy>=1.8 Requires-Dist:
+matplotlib>=3.6 Requires-Dist: plotly>=5.16 Requires-Dist: jupytext ; extra ==
+"binder" Requires-Dist: jupyterlab>=3.2 ; extra == "binder" Requires-Dist:
+jupyterlab-myst ; extra == "binder" Requires-Dist: pre-commit ; extra ==
+"code_style" Requires-Dist: sphinx==7.2 ; extra == "docs" Requires-Dist:
+sphinx-design ; extra == "docs" Requires-Dist: sphinx-thebe ; extra == "docs"
+Requires-Dist: sphinx-favicon ; extra == "docs" Requires-Dist: sphinx-gallery ;
+extra == "docs" Requires-Dist: sphinx-copybutton ; extra == "docs" Requires-
+Dist: sphinx-book-theme ; extra == "docs" Requires-Dist: myst-nb ; extra ==
+"docs" Requires-Dist: pandas ; extra == "docs" Requires-Dist: numpy-stl ; extra
+== "docs" Requires-Dist: pyvista ; extra == "docs" Requires-Dist: tox>=4.11 ;
+extra == "test" Requires-Dist: pytest>=7.4 ; extra == "test" Requires-Dist:
+pylint>3.0 ; extra == "test" Requires-Dist: coverage ; extra == "test"
+Requires-Dist: pandas ; extra == "test" Requires-Dist: pyvista ; extra ==
+"test" Requires-Dist: ipywidgets ; extra == "test" Requires-Dist: imageio
+[tifffile, ffmpeg] ; extra == "test" Requires-Dist: jupyterlab ; extra ==
+"test" Project-URL: Bug Tracker, https://github.com/magpylib/magpylib/issues
+Project-URL: Changelog, https://github.com/magpylib/magpylib/blob/master/
+CHANGELOG.md Project-URL: Documentation, https://magpylib.readthedocs.io/en/
+latest/ Project-URL: Repository, https://github.com/magpylib/magpylib.git
+Provides-Extra: binder Provides-Extra: code_style Provides-Extra: docs
+Provides-Extra: test > [!WARNING] > Version 5 introduces critical breaking
+changes with, among others, the _move to SI units_. We recommended to pin your
+dependencies to `magpylib>=4.5<5` until you are ready to migrate to the latest
+version! ([see details](https://github.com/magpylib/magpylib/discussions/647))
 [docs/_static/images/magpylib_flag.png]
 ---
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_B_S_D___2_-_-_C_l_a_u_s_e_-_o_r_a_n_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
 _g_i_t_h_u_b_._c_o_m_/_m_a_g_p_y_l_i_b_/_m_a_g_p_y_l_i_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_p_y_t_h_o_n_-_a_p_p_._y_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:
 _/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/_m_a_g_p_y_l_i_b_/_b_a_d_g_e_/_?_v_e_r_s_i_o_n_=_l_a_t_e_s_t_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/
 _g_h_/_m_a_g_p_y_l_i_b_/_m_a_g_p_y_l_i_b_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_C_o_n_d_a_ _C_l_o_u_d_]
 _[_M_y_B_i_n_d_e_r_ _l_i_n_k_]_[_b_l_a_c_k_]
 Magpylib is a Python package for calculating **3D static magnetic fields** of
 magnets, line currents and other sources. The computation is based on explicit
 expressions and is therefore **extremely fast**. A **user friendly API**
 enables convenient positioning of sources and observers. # Installation Install
 from PyPI using **pip** ``` pip install magpylib ``` Install from conda forge
 using **conda** ``` conda install -c conda-forge magpylib ``` Magpylib supports
-_Python3.8+_ and relies on common scientific computation libraries _Numpy_,
+_Python3.10+_ and relies on common scientific computation libraries _Numpy_,
 _Scipy_, _Matplotlib_ and _Plotly_. Optionally, _Pyvista_ is recommended as
 graphical backend. # Resources - Check out our **[Documentation](https://
 magpylib.readthedocs.io/en/latest)** for detailed information. - Please abide
 by our **[Code of Conduct](https://github.com/magpylib/magpylib/blob/main/
 CODE_OF_CONDUCT.md)**. - Contribute through **[Discussions](https://github.com/
 magpylib/magpylib/discussions)** and coding by following the **[Contribution
 Guide](https://github.com/magpylib/magpylib/blob/main/CONTRIBUTING.md)**. The
@@ -106,9 +105,9 @@
 bibtex entry for the [2020 open-access paper](https://www.sciencedirect.com/
 science/article/pii/S2352711020300170) would be ``` @article
 {ortner2020magpylib, title={Magpylib: A free Python package for magnetic field
 computation}, author={Ortner, Michael and Bandeira, Lucas Gabriel Coliado},
 journal={SoftwareX}, volume={11}, pages={100466}, year={2020}, publisher=
 {Elsevier} } ``` A valid software citation could be ``` @software{magpylib,
 author = {{Michael-Ortner et al.}}, title = {magpylib}, url = {https://
-magpylib.readthedocs.io/en/latest/}, version = {5.0.1}, date = {2023-06-25}, }
+magpylib.readthedocs.io/en/latest/}, version = {5.0.2}, date = {2023-06-25}, }
 ```
```

