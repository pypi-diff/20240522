# Comparing `tmp/ipyanimlab-1.0.0.tar.gz` & `tmp/ipyanimlab-1.0.1.tar.gz`

## Comparing `ipyanimlab-1.0.0.tar` & `ipyanimlab-1.0.1.tar`

### file list

```diff
@@ -1,73 +1,74 @@
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/MANIFEST.in
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/readthedocs.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/docs/Makefile
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/docs/api.rst
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/docs/conf.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/docs/index.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/docs/make.bat
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/docs/requirements.in
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/docs/requirements.txt
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/docs/usage.rst
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/docs/examples/01_simple_sphere.nblink
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/docs/examples/02_rigid_usd.nblink
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/docs/examples/03_character_usd.nblink
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/docs/examples/04_animation.nblink
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/docs/examples/05_multiple_character.nblink
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/docs/examples/10_time_of_day.nblink
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/docs/examples/11_edit_material.nblink
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/docs/examples/index.rst
--rw-r--r--   0        0        0   485129 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/docs/images/screen_001.png
--rw-r--r--   0        0        0   436456 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/docs/images/screen_002.png
--rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/examples/animation.ipynb
--rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/examples/character_usd.ipynb
--rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/examples/edit_material.ipynb
--rw-r--r--   0        0        0   382933 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/examples/example_animation.usd
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/examples/multiple_characters.ipynb
--rw-r--r--   0        0        0  2144059 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/examples/push1_subject2.bvh
--rw-r--r--   0        0        0     7808 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/examples/rigid_usd.ipynb
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/examples/simple_sphere.ipynb
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/examples/time_of_day.ipynb
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/__init__.py
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/animation.py
--rw-r--r--   0        0        0     9896 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/asset.py
--rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/bvh.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/procedural_asset.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/timeline.py
--rw-r--r--   0        0        0    19953 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/utils.py
--rw-r--r--   0        0        0    16678 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/viewer.py
--rw-r--r--   0        0        0  2628081 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/assets/AnimLabSimpleMale.usd
--rw-r--r--   0        0        0  1493537 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/assets/ShaderBall.usd
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/assets/__init__.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/assets/cube.usd
--rw-r--r--   0        0        0    19675 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/assets/sphere.usd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/render/__init__.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/render/axis.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/render/background.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/render/frustum.py
--rw-r--r--   0        0        0    12010 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/render/gbuffer.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/render/ground.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/render/line.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/render/material.py
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/render/mesh.py
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/render/mesh_render.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/render/screen_vbo.py
--rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/render/shadow.py
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/render/show_texture.py
--rw-r--r--   0        0        0    37949 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/render/sky.py
--rw-r--r--   0        0        0     7592 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/render/ssao.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/usd/__init__.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/usd/import_animation.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/usd/import_asset.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/usd/material_prim.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/usd/reading_accessors.py
--rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/usd/reading_buffers.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/usd/reading_mesh.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/usd/rigid_asset.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/usd/skeleton_prim.py
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/src/ipyanimlab/usd/skinned_asset.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/.gitignore
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/README.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 ipyanimlab-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/MANIFEST.in
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/readthedocs.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/docs/api.rst
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/docs/conf.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/docs/index.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/docs/requirements.in
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/docs/requirements.txt
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/docs/usage.rst
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/docs/examples/01_simple_sphere.nblink
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/docs/examples/02_rigid_usd.nblink
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/docs/examples/03_character_usd.nblink
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/docs/examples/04_animation.nblink
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/docs/examples/05_multiple_character.nblink
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/docs/examples/10_time_of_day.nblink
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/docs/examples/11_edit_material.nblink
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/docs/examples/index.rst
+-rw-r--r--   0        0        0   485129 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/docs/images/screen_001.png
+-rw-r--r--   0        0        0   436456 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/docs/images/screen_002.png
+-rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/examples/add_bone.ipynb
+-rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/examples/animation.ipynb
+-rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/examples/character_usd.ipynb
+-rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/examples/edit_material.ipynb
+-rw-r--r--   0        0        0   382933 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/examples/example_animation.usd
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/examples/multiple_characters.ipynb
+-rw-r--r--   0        0        0  2144059 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/examples/push1_subject2.bvh
+-rw-r--r--   0        0        0     7808 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/examples/rigid_usd.ipynb
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/examples/simple_sphere.ipynb
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/examples/time_of_day.ipynb
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/__init__.py
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/animation.py
+-rw-r--r--   0        0        0    10264 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/asset.py
+-rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/bvh.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/procedural_asset.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/timeline.py
+-rw-r--r--   0        0        0    19953 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/utils.py
+-rw-r--r--   0        0        0    16678 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/viewer.py
+-rw-r--r--   0        0        0  2628081 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/assets/AnimLabSimpleMale.usd
+-rw-r--r--   0        0        0  1493537 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/assets/ShaderBall.usd
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/assets/__init__.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/assets/cube.usd
+-rw-r--r--   0        0        0    19675 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/assets/sphere.usd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/render/__init__.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/render/axis.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/render/background.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/render/frustum.py
+-rw-r--r--   0        0        0    12010 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/render/gbuffer.py
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/render/ground.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/render/line.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/render/material.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/render/mesh.py
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/render/mesh_render.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/render/screen_vbo.py
+-rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/render/shadow.py
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/render/show_texture.py
+-rw-r--r--   0        0        0    37949 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/render/sky.py
+-rw-r--r--   0        0        0     7592 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/render/ssao.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/usd/__init__.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/usd/import_animation.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/usd/import_asset.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/usd/material_prim.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/usd/reading_accessors.py
+-rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/usd/reading_buffers.py
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/usd/reading_mesh.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/usd/rigid_asset.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/usd/skeleton_prim.py
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/src/ipyanimlab/usd/skinned_asset.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/README.md
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 ipyanimlab-1.0.1/PKG-INFO
```

### Comparing `ipyanimlab-1.0.0/MANIFEST.in` & `ipyanimlab-1.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/readthedocs.yml` & `ipyanimlab-1.0.1/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/.github/workflows/python-publish.yml` & `ipyanimlab-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/docs/Makefile` & `ipyanimlab-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/docs/conf.py` & `ipyanimlab-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/docs/make.bat` & `ipyanimlab-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/docs/requirements.txt` & `ipyanimlab-1.0.1/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/docs/images/screen_001.png` & `ipyanimlab-1.0.1/docs/images/screen_001.png`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/docs/images/screen_002.png` & `ipyanimlab-1.0.1/docs/images/screen_002.png`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/examples/animation.ipynb` & `ipyanimlab-1.0.1/examples/animation.ipynb`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/examples/character_usd.ipynb` & `ipyanimlab-1.0.1/examples/character_usd.ipynb`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/examples/edit_material.ipynb` & `ipyanimlab-1.0.1/examples/edit_material.ipynb`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/examples/example_animation.usd` & `ipyanimlab-1.0.1/examples/example_animation.usd`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/examples/multiple_characters.ipynb` & `ipyanimlab-1.0.1/examples/multiple_characters.ipynb`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/examples/push1_subject2.bvh` & `ipyanimlab-1.0.1/examples/push1_subject2.bvh`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/examples/rigid_usd.ipynb` & `ipyanimlab-1.0.1/examples/rigid_usd.ipynb`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/examples/simple_sphere.ipynb` & `ipyanimlab-1.0.1/examples/simple_sphere.ipynb`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/examples/time_of_day.ipynb` & `ipyanimlab-1.0.1/examples/time_of_day.ipynb`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/animation.py` & `ipyanimlab-1.0.1/src/ipyanimlab/animation.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/asset.py` & `ipyanimlab-1.0.1/src/ipyanimlab/asset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 from copy import deepcopy
 import itertools
 
 from .render.material import Material
+from . import utils
 
 class Asset:
     """An asset in the viewer that can be rendered.
     An asset represent a mesh in webgl.
     Several asset can share the same mesh for a smaller memory footprint on the GPU
     """
 
@@ -213,17 +214,26 @@
         Args:
             :name: (str): the name of the skeleton
             :q: (np.array([4], dtype=np.float32)): the quaternion of the bone to add
             :p: (np.array([3], dtype=np.float32)): the position of the bone to add
             :parent_name: (str, optional): the name of the parent bone. Defaults to None.
             :global_space: (bool, optional): is the quaternion and position in localspace or worldspace. Defaults to True.
         """
-        self._mesh.add_bone(name, q, p, parent_name, global_space)
+        matrix = utils.quat_to_mat(q, p)
+        parent_id = -1
+        if parent_name in self.bone_names():
+            parent_id = self.bone_names().index(parent_name)
+            
+        if parent_id > -1 and global_space:
+            self.world_skeleton_xforms()
+            matrix = np.dot(np.linalg.inv(self._scratch_skeleton_[parent_id, :, :]), matrix)
+
+        self._mesh.add_bone(name, parent_id, matrix)
         self._skeleton_xforms = np.zeros_like(self._mesh.initialpose, dtype=np.float32)
-        self._skeleton_xforms[:,:,:] = self._compute_local_to_global()
+        self._skeleton_xforms[:,:,:] = self._compute_skeleton_xforms()
 
     def _compute_skeleton_xforms(self, local_matrices=None, names=None):
         if local_matrices is not None:
             if names:
                 self._scratch_skeleton_[:self._skeleton_xforms.shape[0], :, :] = self._mesh.initialpose[:, :, :]
                 for i, name in enumerate(names):
                     if name in self._mesh.bone_names:
```

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/bvh.py` & `ipyanimlab-1.0.1/src/ipyanimlab/bvh.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/procedural_asset.py` & `ipyanimlab-1.0.1/src/ipyanimlab/procedural_asset.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/timeline.py` & `ipyanimlab-1.0.1/src/ipyanimlab/timeline.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/utils.py` & `ipyanimlab-1.0.1/src/ipyanimlab/utils.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/viewer.py` & `ipyanimlab-1.0.1/src/ipyanimlab/viewer.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/assets/AnimLabSimpleMale.usd` & `ipyanimlab-1.0.1/src/ipyanimlab/assets/AnimLabSimpleMale.usd`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/assets/ShaderBall.usd` & `ipyanimlab-1.0.1/src/ipyanimlab/assets/ShaderBall.usd`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/assets/cube.usd` & `ipyanimlab-1.0.1/src/ipyanimlab/assets/cube.usd`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/assets/sphere.usd` & `ipyanimlab-1.0.1/src/ipyanimlab/assets/sphere.usd`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/render/axis.py` & `ipyanimlab-1.0.1/src/ipyanimlab/render/axis.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/render/background.py` & `ipyanimlab-1.0.1/src/ipyanimlab/render/background.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/render/frustum.py` & `ipyanimlab-1.0.1/src/ipyanimlab/render/frustum.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/render/gbuffer.py` & `ipyanimlab-1.0.1/src/ipyanimlab/render/gbuffer.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/render/ground.py` & `ipyanimlab-1.0.1/src/ipyanimlab/render/ground.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/render/line.py` & `ipyanimlab-1.0.1/src/ipyanimlab/render/line.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/render/material.py` & `ipyanimlab-1.0.1/src/ipyanimlab/render/material.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/render/mesh.py` & `ipyanimlab-1.0.1/src/ipyanimlab/render/mesh.py`

 * *Files 13% similar despite different names*

```diff
@@ -72,28 +72,23 @@
         return len(self.bone_names)
 
 
     def bone_index(self, name):
         return self.bone_names.index(name)
 
 
-    def add_bone(self, name, q, p, parent_name=None, global_space=True):
+    def add_bone(self, name, parent_id, matrix):
         if name in self.bone_names:
             raise Exception(name + " already in skeleton")
 
-        m = utils.quat_to_mat(q, p)
-        parent_id = -1
-        if parent_name in self.bone_names:
-            parent_id = self.bone_names.index(parent_name)
-            
-        if parent_id > -1 and global_space:
-            self.global_bones()
-            m = np.dot(np.linalg.inv(self.scratch_buffer[parent_id, :, :]), m)
-
-        self.bone_names.append(name)
         self.bone_names.append(name)
         self.bone_parents = np.append(self.bone_parents, parent_id)
         initial = np.zeros([self.bone_count(), 4, 4], dtype=np.float32)
         initial[:self.bone_count()-1,:, :] = self.initialpose
-        initial[-1, :, :] = m
+        initial[-1, :, :] = matrix
         self.initialpose = initial
+        
+        initial = np.zeros([self.bone_count(), 4, 4], dtype=np.float32)
+        initial[:self.bone_count()-1,:, :] = self.bindpose
+        initial[-1, :, :] = matrix
+        self.bindpose = initial
```

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/render/mesh_render.py` & `ipyanimlab-1.0.1/src/ipyanimlab/render/mesh_render.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/render/screen_vbo.py` & `ipyanimlab-1.0.1/src/ipyanimlab/render/screen_vbo.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/render/shadow.py` & `ipyanimlab-1.0.1/src/ipyanimlab/render/shadow.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/render/show_texture.py` & `ipyanimlab-1.0.1/src/ipyanimlab/render/show_texture.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/render/sky.py` & `ipyanimlab-1.0.1/src/ipyanimlab/render/sky.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/render/ssao.py` & `ipyanimlab-1.0.1/src/ipyanimlab/render/ssao.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/usd/import_animation.py` & `ipyanimlab-1.0.1/src/ipyanimlab/usd/import_animation.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/usd/import_asset.py` & `ipyanimlab-1.0.1/src/ipyanimlab/usd/import_asset.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/usd/material_prim.py` & `ipyanimlab-1.0.1/src/ipyanimlab/usd/material_prim.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/usd/reading_accessors.py` & `ipyanimlab-1.0.1/src/ipyanimlab/usd/reading_accessors.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/usd/reading_buffers.py` & `ipyanimlab-1.0.1/src/ipyanimlab/usd/reading_buffers.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/usd/reading_mesh.py` & `ipyanimlab-1.0.1/src/ipyanimlab/usd/reading_mesh.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/usd/rigid_asset.py` & `ipyanimlab-1.0.1/src/ipyanimlab/usd/rigid_asset.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/src/ipyanimlab/usd/skinned_asset.py` & `ipyanimlab-1.0.1/src/ipyanimlab/usd/skinned_asset.py`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/.gitignore` & `ipyanimlab-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/LICENSE.txt` & `ipyanimlab-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipyanimlab-1.0.0/README.md` & `ipyanimlab-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # ipyanimlab
 
 <p align="center">
 <img src="docs/images/screen_001.png"/><br>
 A character animation widget for Jupyter Lab
 </p>
 
+[![Documentation Status](https://readthedocs.org/projects/ipyanimlab/badge/?version=latest)](https://ipyanimlab.readthedocs.io/en/latest/?badge=latest)
 
 ## Introduction
 
 **ipyanimlab** is jupyter lab library to quickly display character animation when doing animation research.
 
 **OpenUSD** file format to import assets and animations.
 * Assets can be rigid or skinned
```

### Comparing `ipyanimlab-1.0.0/pyproject.toml` & `ipyanimlab-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,12 +26,12 @@
     "Programming Language :: Python :: 3"
 ]
 dependencies = [
     "numpy",
 	"ipywebgl",
 	"usd-core"
 ]
-version = "1.0.0"
+version = "1.0.1"
 
 [project.urls]
 Homepage = "https://github.com/JeromeEippers/ipywebgl"
 Documentation = "https://ipywebgl.readthedocs.io/en/latest/index.html"
```

### Comparing `ipyanimlab-1.0.0/PKG-INFO` & `ipyanimlab-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ipyanimlab
-Version: 1.0.0
+Version: 1.0.1
 Summary: An Animation R&D jupyter Lab, build on top of ipywebgl
 Project-URL: Homepage, https://github.com/JeromeEippers/ipywebgl
 Project-URL: Documentation, https://ipywebgl.readthedocs.io/en/latest/index.html
 Author-email: Jerome Eippers <jerome@eippers.be>
 License: Copyright (c) 2024 Jerome Eippers
         All rights reserved.
         
@@ -48,14 +48,15 @@
 # ipyanimlab
 
 <p align="center">
 <img src="docs/images/screen_001.png"/><br>
 A character animation widget for Jupyter Lab
 </p>
 
+[![Documentation Status](https://readthedocs.org/projects/ipyanimlab/badge/?version=latest)](https://ipyanimlab.readthedocs.io/en/latest/?badge=latest)
 
 ## Introduction
 
 **ipyanimlab** is jupyter lab library to quickly display character animation when doing animation research.
 
 **OpenUSD** file format to import assets and animations.
 * Assets can be rigid or skinned
```

