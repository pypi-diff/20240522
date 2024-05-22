# Comparing `tmp/sleplet-1.4.7.tar.gz` & `tmp/sleplet-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleplet-1.4.7.tar", last modified: Tue Apr 23 13:49:48 2024, max compression
+gzip compressed data, was "sleplet-1.4.8.tar", last modified: Wed May 22 15:42:41 2024, max compression
```

## Comparing `sleplet-1.4.7.tar` & `sleplet-1.4.8.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.612817 sleplet-1.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-23 13:49:43.000000 sleplet-1.4.7/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-23 13:49:43.000000 sleplet-1.4.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-23 13:49:43.000000 sleplet-1.4.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-23 13:49:43.000000 sleplet-1.4.7/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9856 2024-04-23 13:49:48.612817 sleplet-1.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-04-23 13:49:43.000000 sleplet-1.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-23 13:49:43.000000 sleplet-1.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:49:48.612817 sleplet-1.4.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.588817 sleplet-1.4.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.596817 sleplet-1.4.7/src/sleplet/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_array_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_bool_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_class_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_convolution_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.600817 sleplet-1.4.7/src/sleplet/_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/create_earth_flm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/create_wmap_flm.py
--rw-r--r--   0 runner    (1001) docker     (127)    39339 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_polygons_bird.off
--rw-r--r--   0 runner    (1001) docker     (127)   111621 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_polygons_cheetah.off
--rw-r--r--   0 runner    (1001) docker     (127)   321932 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_polygons_cube.off
--rw-r--r--   0 runner    (1001) docker     (127)    65194 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_polygons_dragon.off
--rw-r--r--   0 runner    (1001) docker     (127)   329591 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_polygons_homer.off
--rw-r--r--   0 runner    (1001) docker     (127)    36961 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_polygons_teapot.off
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_regions_bird.toml
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_regions_cheetah.toml
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_regions_cube.toml
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_regions_dragon.toml
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_regions_homer.toml
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_regions_teapot.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/setup_pooch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_integration_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_mask_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_mesh_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_parallel_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_plotly_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.600817 sleplet-1.4.7/src/sleplet/_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_scripts/plotting_on_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    11063 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_scripts/plotting_on_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_slepian_arbitrary_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_string_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-23 13:49:48.000000 sleplet-1.4.7/src/sleplet/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.604817 sleplet-1.4.7/src/sleplet/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/africa.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/axisymmetric_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/dirac_delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/earth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/elongated_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/flm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/fp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/harmonic_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/noise_earth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/ridgelets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian_africa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian_dirac_delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian_noise_africa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian_noise_south_america.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian_south_america.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian_wavelet_coefficients_africa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/south_america.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/spherical_harmonic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/squashed_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/wmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/harmonic_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.608817 sleplet-1.4.7/src/sleplet/meshes/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/_mesh_slepian_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_basis_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_harmonic_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_noise_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_slepian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_noise_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/plot_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.608817 sleplet-1.4.7/src/sleplet/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/plotting/_create_plot_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/plotting/_create_plot_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.608817 sleplet-1.4.7/src/sleplet/slepian/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/slepian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/slepian/_slepian_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/slepian/region.py
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/slepian/slepian_arbitrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/slepian/slepian_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/slepian/slepian_limit_lat_lon.py
--rw-r--r--   0 runner    (1001) docker     (127)    14615 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/slepian/slepian_polar_cap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/slepian_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/wavelet_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.612817 sleplet-1.4.7/src/sleplet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9856 2024-04-23 13:49:48.000000 sleplet-1.4.7/src/sleplet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-23 13:49:48.000000 sleplet-1.4.7/src/sleplet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:49:48.000000 sleplet-1.4.7/src/sleplet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-23 13:49:48.000000 sleplet-1.4.7/src/sleplet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-23 13:49:48.000000 sleplet-1.4.7/src/sleplet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 13:49:48.000000 sleplet-1.4.7/src/sleplet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.632697 sleplet-1.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-22 15:42:36.000000 sleplet-1.4.8/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-05-22 15:42:36.000000 sleplet-1.4.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-05-22 15:42:36.000000 sleplet-1.4.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-22 15:42:36.000000 sleplet-1.4.8/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-05-22 15:42:41.632697 sleplet-1.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-22 15:42:36.000000 sleplet-1.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-22 15:42:36.000000 sleplet-1.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:42:41.632697 sleplet-1.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.612697 sleplet-1.4.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.616697 sleplet-1.4.8/src/sleplet/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_array_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_bool_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_class_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_convolution_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.620697 sleplet-1.4.8/src/sleplet/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/create_earth_flm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/create_wmap_flm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39339 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_polygons_bird.off
+-rw-r--r--   0 runner    (1001) docker     (127)   111621 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_polygons_cheetah.off
+-rw-r--r--   0 runner    (1001) docker     (127)   321932 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_polygons_cube.off
+-rw-r--r--   0 runner    (1001) docker     (127)    65194 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_polygons_dragon.off
+-rw-r--r--   0 runner    (1001) docker     (127)   329591 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_polygons_homer.off
+-rw-r--r--   0 runner    (1001) docker     (127)    36961 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_polygons_teapot.off
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_regions_bird.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_regions_cheetah.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_regions_cube.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_regions_dragon.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_regions_homer.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_regions_teapot.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/setup_pooch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_integration_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_mask_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_mesh_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_parallel_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_plotly_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.620697 sleplet-1.4.8/src/sleplet/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_scripts/plotting_on_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11063 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_scripts/plotting_on_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_slepian_arbitrary_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_string_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 15:42:41.000000 sleplet-1.4.8/src/sleplet/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.628697 sleplet-1.4.8/src/sleplet/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/africa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/axisymmetric_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/dirac_delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/earth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/elongated_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/flm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/fp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/harmonic_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/noise_earth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/ridgelets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian_africa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian_dirac_delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian_noise_africa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian_noise_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian_wavelet_coefficients_africa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/south_america.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/spherical_harmonic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/squashed_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/wmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/harmonic_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.628697 sleplet-1.4.8/src/sleplet/meshes/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/_mesh_slepian_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_basis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_harmonic_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_noise_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_slepian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_noise_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/plot_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.628697 sleplet-1.4.8/src/sleplet/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/plotting/_create_plot_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/plotting/_create_plot_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.632697 sleplet-1.4.8/src/sleplet/slepian/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/slepian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/slepian/_slepian_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/slepian/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/slepian/slepian_arbitrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/slepian/slepian_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/slepian/slepian_limit_lat_lon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14615 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/slepian/slepian_polar_cap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/slepian_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/wavelet_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.632697 sleplet-1.4.8/src/sleplet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-05-22 15:42:41.000000 sleplet-1.4.8/src/sleplet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-22 15:42:41.000000 sleplet-1.4.8/src/sleplet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:42:41.000000 sleplet-1.4.8/src/sleplet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-22 15:42:41.000000 sleplet-1.4.8/src/sleplet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-22 15:42:41.000000 sleplet-1.4.8/src/sleplet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 15:42:41.000000 sleplet-1.4.8/src/sleplet.egg-info/top_level.txt
```

### Comparing `sleplet-1.4.7/CITATION.cff` & `sleplet-1.4.8/CITATION.cff`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 cff-version: 1.2.0
 authors:
   - family-names: Roddy
     given-names: Patrick J.
     orcid: https://orcid.org/0000-0002-6271-1700
 doi: 10.5281/zenodo.7268074
 message: >-
-  If you use this software, please cite our article in the
-  Journal of Open Source Software.
+  If you use this software, please cite our article in the Journal of Open
+  Source Software.
 preferred-citation:
   authors:
     - family-names: Roddy
       given-names: Patrick J.
       orcid: https://orcid.org/0000-0002-6271-1700
   date-published: 2023-04-20
   doi: 10.21105/joss.05221
```

### Comparing `sleplet-1.4.7/CODE_OF_CONDUCT.md` & `sleplet-1.4.8/CODE_OF_CONDUCT.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 
 ## Our Pledge
 
 We as members, contributors, and leaders pledge to make participation in our
 community a harassment-free experience for everyone, regardless of age, body
 size, visible or invisible disability, ethnicity, sex characteristics, gender
 identity and expression, level of experience, education, socio-economic status,
-nationality, personal appearance, race, religion, or sexual identity
-and orientation.
+nationality, personal appearance, race, religion, or sexual identity and
+orientation.
 
 We pledge to act and interact in ways that contribute to an open, welcoming,
 diverse, inclusive, and healthy community.
 
 ## Our Standards
 
 Examples of behavior that contributes to a positive environment for our
 community include:
 
 - Demonstrating empathy and kindness toward other people
 - Being respectful of differing opinions, viewpoints, and experiences
 - Giving and gracefully accepting constructive feedback
 - Accepting responsibility and apologizing to those affected by our mistakes,
   and learning from the experience
-- Focusing on what is best not just for us as individuals, but for the
-  overall community
+- Focusing on what is best not just for us as individuals, but for the overall
+  community
 
 Examples of unacceptable behavior include:
 
-- The use of sexualized language or imagery, and sexual attention or
-  advances of any kind
+- The use of sexualized language or imagery, and sexual attention or advances of
+  any kind
 - Trolling, insulting or derogatory comments, and personal or political attacks
 - Public or private harassment
-- Publishing others' private information, such as a physical or email
-  address, without their explicit permission
+- Publishing others' private information, such as a physical or email address,
+  without their explicit permission
 - Other conduct which could reasonably be considered inappropriate in a
   professional setting
 
 ## Enforcement Responsibilities
 
 Community leaders are responsible for clarifying and enforcing our standards of
 acceptable behavior and will take appropriate and fair corrective action in
@@ -56,16 +56,16 @@
 posting via an official social media account, or acting as an appointed
 representative at an online or offline event.
 
 ## Enforcement
 
 Instances of abusive, harassing, or otherwise unacceptable behavior may be
 reported to the community leaders responsible for enforcement at
-<patrickjamesroddy@gmail.com>.
-All complaints will be reviewed and investigated promptly and fairly.
+<patrickjamesroddy@gmail.com>. All complaints will be reviewed and investigated
+promptly and fairly.
 
 All community leaders are obligated to respect the privacy and security of the
 reporter of any incident.
 
 ## Enforcement Guidelines
 
 Community leaders will follow these Community Impact Guidelines in determining
@@ -78,23 +78,23 @@
 
 **Consequence**: A private, written warning from community leaders, providing
 clarity around the nature of the violation and an explanation of why the
 behavior was inappropriate. A public apology may be requested.
 
 ### 2. Warning
 
-**Community Impact**: A violation through a single incident or series
-of actions.
+**Community Impact**: A violation through a single incident or series of
+actions.
 
 **Consequence**: A warning with consequences for continued behavior. No
 interaction with the people involved, including unsolicited interaction with
 those enforcing the Code of Conduct, for a specified period of time. This
 includes avoiding interactions in community spaces as well as external channels
-like social media. Violating these terms may lead to a temporary or
-permanent ban.
+like social media. Violating these terms may lead to a temporary or permanent
+ban.
 
 ### 3. Temporary Ban
 
 **Community Impact**: A serious violation of community standards, including
 sustained inappropriate behavior.
 
 **Consequence**: A temporary ban from any sort of interaction or public
@@ -105,24 +105,24 @@
 
 ### 4. Permanent Ban
 
 **Community Impact**: Demonstrating a pattern of violation of community
 standards, including sustained inappropriate behavior, harassment of an
 individual, or aggression toward or disparagement of classes of individuals.
 
-**Consequence**: A permanent ban from any sort of public interaction within
-the community.
+**Consequence**: A permanent ban from any sort of public interaction within the
+community.
 
 ## Attribution
 
 This Code of Conduct is adapted from the [Contributor Covenant][homepage],
 version 2.0, available at
 <https://www.contributor-covenant.org/version/2/0/code_of_conduct.html>.
 
-Community Impact Guidelines were inspired by [Mozilla's code of conduct
-enforcement ladder](https://github.com/mozilla/diversity).
+Community Impact Guidelines were inspired by
+[Mozilla's code of conduct enforcement ladder](https://github.com/mozilla/diversity).
 
 [homepage]: https://www.contributor-covenant.org
 
 For answers to common questions about this code of conduct, see the FAQ at
 <https://www.contributor-covenant.org/faq>. Translations are available at
 <https://www.contributor-covenant.org/translations>.
```

### Comparing `sleplet-1.4.7/CONTRIBUTING.md` & `sleplet-1.4.8/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,16 @@
 and describe the issue in detail in your report. Please complete the following
 steps in advance to help us fix any potential bug as fast as possible.
 
 - Make sure that you are using the latest version.
 - Determine if your bug is really a bug and not an error on your side e.g. using
   incompatible environment components/versions (Make sure that you have read the
   [documentation](https://astro-informatics.github.io/sleplet). If you are
-  looking for support, you might want to check [this section](#i-have-a-question)).
+  looking for support, you might want to check
+  [this section](#i-have-a-question)).
 - To see if other users have experienced (and potentially already solved) the
   same issue you are having, check if there is not already a bug report existing
   for your bug or error in the
   [bug tracker](https://github.com/astro-informatics/sleplet/issues?q=label%3Abug).
 - Also make sure to search the internet (including Stack Overflow) to see if
   users outside the GitHub community have discussed the issue.
 - Collect information about the bug:
@@ -83,46 +84,47 @@
   - Can you reliably reproduce the issue? And can you also reproduce it with
     older versions?
 
 #### How Do I Submit a Good Bug Report?
 
 > You must never report security related issues, vulnerabilities or bugs
 > including sensitive information to the issue tracker, or elsewhere in public.
-> Instead, sensitive bugs must be sent by email to <patrickjamesroddy@gmail.com>.
+> Instead, sensitive bugs must be sent by email to
+> <patrickjamesroddy@gmail.com>.
 
 We use GitHub issues to track bugs and errors. If you run into an issue with the
 project:
 
 - Open an [Issue](https://github.com/astro-informatics/sleplet/issues/new).
-  (Since we can't be sure at this point whether it is a bug or not, we ask you not
-  to talk about a bug yet and not to label the issue.)
+  (Since we can't be sure at this point whether it is a bug or not, we ask you
+  not to talk about a bug yet and not to label the issue.)
 - Explain the behaviour you would expect and the actual behaviour.
 - Please provide as much context as possible and describe the _reproduction_
   _steps_ that someone else can follow to recreate the issue on their own. This
-  usually includes your code. For good bug reports you should isolate the problem
-  and create a reduced test case.
+  usually includes your code. For good bug reports you should isolate the
+  problem and create a reduced test case.
 - Provide the information you collected in the previous section.
 
 Once it's filed:
 
 - The project team will label the issue accordingly.
 - A team member will try to reproduce the issue with your provided steps. If
   there are no reproduction steps or no obvious way to reproduce the issue, the
-  team will ask you for those steps and mark the issue as `needs-repro`. Bugs with
-  the `needs-repro` tag will not be addressed until they are reproduced.
+  team will ask you for those steps and mark the issue as `needs-repro`. Bugs
+  with the `needs-repro` tag will not be addressed until they are reproduced.
 - If the team is able to reproduce the issue, it will be marked `needs-fix`, as
-  well as possibly other tags (such as `critical`), and the issue will be left to
-  be implemented by someone.
+  well as possibly other tags (such as `critical`), and the issue will be left
+  to be implemented by someone.
 
 ### Suggesting Enhancements
 
-This section guides you through submitting an enhancement suggestion for `SLEPLET`,
-**including completely new features and minor improvements to existing**
-**functionality**. Following these guidelines will help maintainers and the
-community to understand your suggestion and find related suggestions.
+This section guides you through submitting an enhancement suggestion for
+`SLEPLET`, **including completely new features and minor improvements to
+existing** **functionality**. Following these guidelines will help maintainers
+and the community to understand your suggestion and find related suggestions.
 
 #### Before Submitting an Enhancement
 
 - Make sure that you are using the latest version.
 - Read the [documentation](https://astro-informatics.github.io/sleplet)
   carefully and find out if the functionality is already covered, maybe by an
   individual configuration.
@@ -136,16 +138,17 @@
   targeting a minority of users, consider writing an add-on/plugin library.
 
 #### How Do I Submit a Good Enhancement Suggestion?
 
 Enhancement suggestions are tracked as
 [GitHub issues](https://github.com/astro-informatics/sleplet/issues).
 
-- Use a **clear and descriptive title** for the issue to identify the suggestion.
+- Use a **clear and descriptive title** for the issue to identify the
+  suggestion.
 - Provide a **step-by-step description of the suggested enhancement** in as many
   details as possible.
-- **Describe the current behaviour** and **explain which behaviour you expected**
-  **to see instead** and why. At this point you can also tell which alternatives
-  do not work for you.
+- **Describe the current behaviour** and **explain which behaviour you
+  expected** **to see instead** and why. At this point you can also tell which
+  alternatives do not work for you.
 - **Explain why this enhancement would be useful** to most `SLEPLET` users. You
   may also want to point out the other projects that solved it better and which
   could serve as inspiration.
```

### Comparing `sleplet-1.4.7/LICENCE.txt` & `sleplet-1.4.8/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/PKG-INFO` & `sleplet-1.4.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleplet
-Version: 1.4.7
+Version: 1.4.8
 Summary: Slepian Scale-Discretised Wavelets in Python
 Author-email: "Patrick J. Roddy" <patrickjamesroddy@gmail.com>
 License: BSD 3-Clause Licence
         
         Copyright (c) 2017-2024, Patrick Roddy
         All rights reserved.
         
@@ -49,15 +49,15 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
-Requires-Dist: cmocean~=3.0
+Requires-Dist: cmocean~=4.0
 Requires-Dist: gmpy2~=2.0
 Requires-Dist: hypothesis~=6.0
 Requires-Dist: libigl~=2.0
 Requires-Dist: matplotlib~=3.0
 Requires-Dist: multiprocess~=0.0
 Requires-Dist: numba~=0.0
 Requires-Dist: numpy~=1.0
@@ -85,24 +85,29 @@
 Requires-Dist: pdoc3; extra == "docs"
 Provides-Extra: readme
 Requires-Dist: pytest-codeblocks; extra == "readme"
 
 # SLEPLET
 
 [![PyPI](https://badge.fury.io/py/sleplet.svg)](https://pypi.org/project/sleplet)
-[![Python](https://img.shields.io/pypi/pyversions/sleplet)](https://www.python.org)
-[![Licence](https://img.shields.io/github/license/astro-informatics/sleplet)](https://github.com/astro-informatics/sleplet/blob/main/LICENCE.txt)
-[![JOSS](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2/status.svg)](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2)
 [![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.7268074.svg)](https://doi.org/10.5281/zenodo.7268074)
 [![Documentation](https://img.shields.io/badge/Documentation-SLEPLET-blueviolet.svg)](https://astro-informatics.github.io/sleplet)
+[![Licence](https://img.shields.io/github/license/astro-informatics/sleplet)](https://github.com/astro-informatics/sleplet/blob/main/LICENCE.txt)
+
+[![Python](https://img.shields.io/pypi/pyversions/sleplet)](https://www.python.org)
+[![repostatus](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![Test](https://github.com/astro-informatics/sleplet/actions/workflows/test.yaml/badge.svg)](https://github.com/astro-informatics/sleplet/actions/workflows/test.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/astro-informatics/sleplet/badge.svg?branch=main)](https://coveralls.io/github/astro-informatics/sleplet?branch=main)
+
+[![JOSS](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2/status.svg)](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2)
+[![PyOpenSci](https://tinyurl.com/y22nb8up)](https://github.com/pyOpenSci/software-submission/issues/148)
+[![Citation](https://img.shields.io/badge/cite-SLEPLET-yellow)](#citing)
+
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Renovate](https://img.shields.io/badge/renovate-enabled-orange?logo=renovatebot)](https://renovatebot.com)
-[![repostatus](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 
 `SLEPLET` is a Python package for the construction of Slepian wavelets in the
 spherical and manifold (via meshes) settings. The API of `SLEPLET` has been
 designed in an object-orientated manner and is easily extendible. Upon
 installation, `SLEPLET` comes with two command line interfaces - `sphere` and
 `mesh` - which allows one to easily generate plots on the sphere and a set of
 meshes using `plotly`.
@@ -119,16 +124,16 @@
 The recommended way to install `SLEPLET` is via
 [pip](https://pypi.org/project/pip)
 
 ```sh
 pip install sleplet
 ```
 
-To install the latest development version of `SLEPLET` clone this repository
-and run
+To install the latest development version of `SLEPLET` clone this repository and
+run
 
 ```sh
 pip install -e .
 ```
 
 This will install two scripts `sphere` and `mesh` which can be used to generate
 the figures in
@@ -136,19 +141,19 @@
 
 ### Supported Platforms
 
 `SLEPLET` has been tested with
 [![Python](https://img.shields.io/pypi/pyversions/sleplet)](https://www.python.org).
 Windows is not currently supported as `SLEPLET` relies on
 [pyssht](https://pypi.org/project/pyssht) and
-[pys2let](https://pypi.org/project/pys2let) which do not work on Windows.
-These can hopefully be replaced with
+[pys2let](https://pypi.org/project/pys2let) which do not work on Windows. These
+can hopefully be replaced with
 [s2fft](https://github.com/astro-informatics/s2fft) and
-[s2wav](https://github.com/astro-informatics/s2wav) in the future when they
-are available on [PyPI](https://pypi.org).
+[s2wav](https://github.com/astro-informatics/s2wav) in the future when they are
+available on [PyPI](https://pypi.org).
 
 ## Example Usage
 
 `SLEPLET` may be interacted with via the API or the CLIs.
 
 ### API Usage
 
@@ -212,9 +217,9 @@
   pages   = 5221,
   doi     = {10.21105/joss.05221},
 }
 ```
 
 Please also cite [S2LET](https://doi.org/10.1051/0004-6361/201220729) upon which
 `SLEPLET` is built, along with [SSHT](https://doi.org/10.1109/TSP.2011.2166394)
-in the spherical setting or [libigl](https://doi.org/10.1145/3134472.3134497)
-in the mesh setting.
+in the spherical setting or [libigl](https://doi.org/10.1145/3134472.3134497) in
+the mesh setting.
```

### Comparing `sleplet-1.4.7/README.md` & `sleplet-1.4.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # SLEPLET
 
 [![PyPI](https://badge.fury.io/py/sleplet.svg)](https://pypi.org/project/sleplet)
-[![Python](https://img.shields.io/pypi/pyversions/sleplet)](https://www.python.org)
-[![Licence](https://img.shields.io/github/license/astro-informatics/sleplet)](https://github.com/astro-informatics/sleplet/blob/main/LICENCE.txt)
-[![JOSS](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2/status.svg)](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2)
 [![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.7268074.svg)](https://doi.org/10.5281/zenodo.7268074)
 [![Documentation](https://img.shields.io/badge/Documentation-SLEPLET-blueviolet.svg)](https://astro-informatics.github.io/sleplet)
+[![Licence](https://img.shields.io/github/license/astro-informatics/sleplet)](https://github.com/astro-informatics/sleplet/blob/main/LICENCE.txt)
+
+[![Python](https://img.shields.io/pypi/pyversions/sleplet)](https://www.python.org)
+[![repostatus](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![Test](https://github.com/astro-informatics/sleplet/actions/workflows/test.yaml/badge.svg)](https://github.com/astro-informatics/sleplet/actions/workflows/test.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/astro-informatics/sleplet/badge.svg?branch=main)](https://coveralls.io/github/astro-informatics/sleplet?branch=main)
+
+[![JOSS](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2/status.svg)](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2)
+[![PyOpenSci](https://tinyurl.com/y22nb8up)](https://github.com/pyOpenSci/software-submission/issues/148)
+[![Citation](https://img.shields.io/badge/cite-SLEPLET-yellow)](#citing)
+
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Renovate](https://img.shields.io/badge/renovate-enabled-orange?logo=renovatebot)](https://renovatebot.com)
-[![repostatus](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 
 `SLEPLET` is a Python package for the construction of Slepian wavelets in the
 spherical and manifold (via meshes) settings. The API of `SLEPLET` has been
 designed in an object-orientated manner and is easily extendible. Upon
 installation, `SLEPLET` comes with two command line interfaces - `sphere` and
 `mesh` - which allows one to easily generate plots on the sphere and a set of
 meshes using `plotly`.
@@ -31,16 +36,16 @@
 The recommended way to install `SLEPLET` is via
 [pip](https://pypi.org/project/pip)
 
 ```sh
 pip install sleplet
 ```
 
-To install the latest development version of `SLEPLET` clone this repository
-and run
+To install the latest development version of `SLEPLET` clone this repository and
+run
 
 ```sh
 pip install -e .
 ```
 
 This will install two scripts `sphere` and `mesh` which can be used to generate
 the figures in
@@ -48,19 +53,19 @@
 
 ### Supported Platforms
 
 `SLEPLET` has been tested with
 [![Python](https://img.shields.io/pypi/pyversions/sleplet)](https://www.python.org).
 Windows is not currently supported as `SLEPLET` relies on
 [pyssht](https://pypi.org/project/pyssht) and
-[pys2let](https://pypi.org/project/pys2let) which do not work on Windows.
-These can hopefully be replaced with
+[pys2let](https://pypi.org/project/pys2let) which do not work on Windows. These
+can hopefully be replaced with
 [s2fft](https://github.com/astro-informatics/s2fft) and
-[s2wav](https://github.com/astro-informatics/s2wav) in the future when they
-are available on [PyPI](https://pypi.org).
+[s2wav](https://github.com/astro-informatics/s2wav) in the future when they are
+available on [PyPI](https://pypi.org).
 
 ## Example Usage
 
 `SLEPLET` may be interacted with via the API or the CLIs.
 
 ### API Usage
 
@@ -124,9 +129,9 @@
   pages   = 5221,
   doi     = {10.21105/joss.05221},
 }
 ```
 
 Please also cite [S2LET](https://doi.org/10.1051/0004-6361/201220729) upon which
 `SLEPLET` is built, along with [SSHT](https://doi.org/10.1109/TSP.2011.2166394)
-in the spherical setting or [libigl](https://doi.org/10.1145/3134472.3134497)
-in the mesh setting.
+in the spherical setting or [libigl](https://doi.org/10.1145/3134472.3134497) in
+the mesh setting.
```

### Comparing `sleplet-1.4.7/pyproject.toml` & `sleplet-1.4.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "Topic :: Scientific/Engineering :: Image Processing",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Scientific/Engineering :: Visualization",
     "Typing :: Typed",
 ]
 dependencies = [
-    "cmocean~=3.0",
+    "cmocean~=4.0",
     "gmpy2~=2.0",
     "hypothesis~=6.0",
     "libigl~=2.0",
     "matplotlib~=3.0",
     "multiprocess~=0.0",
     "numba~=0.0",
     "numpy~=1.0",
```

### Comparing `sleplet-1.4.7/src/sleplet/__init__.py` & `sleplet-1.4.8/src/sleplet/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_bool_methods.py` & `sleplet-1.4.8/src/sleplet/_bool_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_class_lists.py` & `sleplet-1.4.8/src/sleplet/_class_lists.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_convolution_methods.py` & `sleplet-1.4.8/src/sleplet/_convolution_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_data/create_earth_flm.py` & `sleplet-1.4.8/src/sleplet/_data/create_earth_flm.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_data/create_wmap_flm.py` & `sleplet-1.4.8/src/sleplet/_data/create_wmap_flm.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_data/meshes_polygons_bird.off` & `sleplet-1.4.8/src/sleplet/_data/meshes_polygons_bird.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_data/meshes_polygons_cheetah.off` & `sleplet-1.4.8/src/sleplet/_data/meshes_polygons_cheetah.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_data/meshes_polygons_cube.off` & `sleplet-1.4.8/src/sleplet/_data/meshes_polygons_cube.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_data/meshes_polygons_dragon.off` & `sleplet-1.4.8/src/sleplet/_data/meshes_polygons_dragon.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_data/meshes_polygons_homer.off` & `sleplet-1.4.8/src/sleplet/_data/meshes_polygons_homer.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_data/meshes_polygons_teapot.off` & `sleplet-1.4.8/src/sleplet/_data/meshes_polygons_teapot.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_data/setup_pooch.py` & `sleplet-1.4.8/src/sleplet/_data/setup_pooch.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_integration_methods.py` & `sleplet-1.4.8/src/sleplet/_integration_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_mask_methods.py` & `sleplet-1.4.8/src/sleplet/_mask_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_mesh_methods.py` & `sleplet-1.4.8/src/sleplet/_mesh_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_parallel_methods.py` & `sleplet-1.4.8/src/sleplet/_parallel_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_plotly_methods.py` & `sleplet-1.4.8/src/sleplet/_plotly_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_scripts/plotting_on_mesh.py` & `sleplet-1.4.8/src/sleplet/_scripts/plotting_on_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_scripts/plotting_on_sphere.py` & `sleplet-1.4.8/src/sleplet/_scripts/plotting_on_sphere.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_slepian_arbitrary_methods.py` & `sleplet-1.4.8/src/sleplet/_slepian_arbitrary_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_smoothing.py` & `sleplet-1.4.8/src/sleplet/_smoothing.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/_string_methods.py` & `sleplet-1.4.8/src/sleplet/_string_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/__init__.py` & `sleplet-1.4.8/src/sleplet/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/africa.py` & `sleplet-1.4.8/src/sleplet/functions/africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py` & `sleplet-1.4.8/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py` & `sleplet-1.4.8/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py` & `sleplet-1.4.8/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/axisymmetric_wavelets.py` & `sleplet-1.4.8/src/sleplet/functions/axisymmetric_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/coefficients.py` & `sleplet-1.4.8/src/sleplet/functions/coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/dirac_delta.py` & `sleplet-1.4.8/src/sleplet/functions/dirac_delta.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/earth.py` & `sleplet-1.4.8/src/sleplet/functions/earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/elongated_gaussian.py` & `sleplet-1.4.8/src/sleplet/functions/elongated_gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/flm.py` & `sleplet-1.4.8/src/sleplet/functions/flm.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/fp.py` & `sleplet-1.4.8/src/sleplet/functions/fp.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/gaussian.py` & `sleplet-1.4.8/src/sleplet/functions/gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/harmonic_gaussian.py` & `sleplet-1.4.8/src/sleplet/functions/harmonic_gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/identity.py` & `sleplet-1.4.8/src/sleplet/functions/identity.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/noise_earth.py` & `sleplet-1.4.8/src/sleplet/functions/noise_earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/ridgelets.py` & `sleplet-1.4.8/src/sleplet/functions/ridgelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/slepian.py` & `sleplet-1.4.8/src/sleplet/functions/slepian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/slepian_africa.py` & `sleplet-1.4.8/src/sleplet/functions/slepian_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/slepian_dirac_delta.py` & `sleplet-1.4.8/src/sleplet/functions/slepian_dirac_delta.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/slepian_identity.py` & `sleplet-1.4.8/src/sleplet/functions/slepian_identity.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/slepian_noise_africa.py` & `sleplet-1.4.8/src/sleplet/functions/slepian_noise_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/slepian_noise_south_america.py` & `sleplet-1.4.8/src/sleplet/functions/slepian_noise_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/slepian_south_america.py` & `sleplet-1.4.8/src/sleplet/functions/slepian_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/slepian_wavelet_coefficients_africa.py` & `sleplet-1.4.8/src/sleplet/functions/slepian_wavelet_coefficients_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py` & `sleplet-1.4.8/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/slepian_wavelets.py` & `sleplet-1.4.8/src/sleplet/functions/slepian_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/south_america.py` & `sleplet-1.4.8/src/sleplet/functions/south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/spherical_harmonic.py` & `sleplet-1.4.8/src/sleplet/functions/spherical_harmonic.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/squashed_gaussian.py` & `sleplet-1.4.8/src/sleplet/functions/squashed_gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/functions/wmap.py` & `sleplet-1.4.8/src/sleplet/functions/wmap.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/harmonic_methods.py` & `sleplet-1.4.8/src/sleplet/harmonic_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/meshes/__init__.py` & `sleplet-1.4.8/src/sleplet/meshes/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/meshes/_mesh_slepian_decomposition.py` & `sleplet-1.4.8/src/sleplet/meshes/_mesh_slepian_decomposition.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/meshes/mesh.py` & `sleplet-1.4.8/src/sleplet/meshes/mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/meshes/mesh_basis_functions.py` & `sleplet-1.4.8/src/sleplet/meshes/mesh_basis_functions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/meshes/mesh_coefficients.py` & `sleplet-1.4.8/src/sleplet/meshes/mesh_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/meshes/mesh_field.py` & `sleplet-1.4.8/src/sleplet/meshes/mesh_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/meshes/mesh_harmonic_coefficients.py` & `sleplet-1.4.8/src/sleplet/meshes/mesh_harmonic_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/meshes/mesh_noise_field.py` & `sleplet-1.4.8/src/sleplet/meshes/mesh_noise_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/meshes/mesh_slepian.py` & `sleplet-1.4.8/src/sleplet/meshes/mesh_slepian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_coefficients.py` & `sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_field.py` & `sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_functions.py` & `sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_functions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_noise_field.py` & `sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_noise_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py` & `sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_wavelets.py` & `sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/noise.py` & `sleplet-1.4.8/src/sleplet/noise.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/plot_methods.py` & `sleplet-1.4.8/src/sleplet/plot_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/plotting/_create_plot_mesh.py` & `sleplet-1.4.8/src/sleplet/plotting/_create_plot_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/plotting/_create_plot_sphere.py` & `sleplet-1.4.8/src/sleplet/plotting/_create_plot_sphere.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/slepian/_slepian_decomposition.py` & `sleplet-1.4.8/src/sleplet/slepian/_slepian_decomposition.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/slepian/region.py` & `sleplet-1.4.8/src/sleplet/slepian/region.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/slepian/slepian_arbitrary.py` & `sleplet-1.4.8/src/sleplet/slepian/slepian_arbitrary.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/slepian/slepian_functions.py` & `sleplet-1.4.8/src/sleplet/slepian/slepian_functions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/slepian/slepian_limit_lat_lon.py` & `sleplet-1.4.8/src/sleplet/slepian/slepian_limit_lat_lon.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/slepian/slepian_polar_cap.py` & `sleplet-1.4.8/src/sleplet/slepian/slepian_polar_cap.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/slepian_methods.py` & `sleplet-1.4.8/src/sleplet/slepian_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet/wavelet_methods.py` & `sleplet-1.4.8/src/sleplet/wavelet_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.7/src/sleplet.egg-info/PKG-INFO` & `sleplet-1.4.8/src/sleplet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleplet
-Version: 1.4.7
+Version: 1.4.8
 Summary: Slepian Scale-Discretised Wavelets in Python
 Author-email: "Patrick J. Roddy" <patrickjamesroddy@gmail.com>
 License: BSD 3-Clause Licence
         
         Copyright (c) 2017-2024, Patrick Roddy
         All rights reserved.
         
@@ -49,15 +49,15 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
-Requires-Dist: cmocean~=3.0
+Requires-Dist: cmocean~=4.0
 Requires-Dist: gmpy2~=2.0
 Requires-Dist: hypothesis~=6.0
 Requires-Dist: libigl~=2.0
 Requires-Dist: matplotlib~=3.0
 Requires-Dist: multiprocess~=0.0
 Requires-Dist: numba~=0.0
 Requires-Dist: numpy~=1.0
@@ -85,24 +85,29 @@
 Requires-Dist: pdoc3; extra == "docs"
 Provides-Extra: readme
 Requires-Dist: pytest-codeblocks; extra == "readme"
 
 # SLEPLET
 
 [![PyPI](https://badge.fury.io/py/sleplet.svg)](https://pypi.org/project/sleplet)
-[![Python](https://img.shields.io/pypi/pyversions/sleplet)](https://www.python.org)
-[![Licence](https://img.shields.io/github/license/astro-informatics/sleplet)](https://github.com/astro-informatics/sleplet/blob/main/LICENCE.txt)
-[![JOSS](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2/status.svg)](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2)
 [![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.7268074.svg)](https://doi.org/10.5281/zenodo.7268074)
 [![Documentation](https://img.shields.io/badge/Documentation-SLEPLET-blueviolet.svg)](https://astro-informatics.github.io/sleplet)
+[![Licence](https://img.shields.io/github/license/astro-informatics/sleplet)](https://github.com/astro-informatics/sleplet/blob/main/LICENCE.txt)
+
+[![Python](https://img.shields.io/pypi/pyversions/sleplet)](https://www.python.org)
+[![repostatus](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![Test](https://github.com/astro-informatics/sleplet/actions/workflows/test.yaml/badge.svg)](https://github.com/astro-informatics/sleplet/actions/workflows/test.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/astro-informatics/sleplet/badge.svg?branch=main)](https://coveralls.io/github/astro-informatics/sleplet?branch=main)
+
+[![JOSS](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2/status.svg)](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2)
+[![PyOpenSci](https://tinyurl.com/y22nb8up)](https://github.com/pyOpenSci/software-submission/issues/148)
+[![Citation](https://img.shields.io/badge/cite-SLEPLET-yellow)](#citing)
+
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Renovate](https://img.shields.io/badge/renovate-enabled-orange?logo=renovatebot)](https://renovatebot.com)
-[![repostatus](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 
 `SLEPLET` is a Python package for the construction of Slepian wavelets in the
 spherical and manifold (via meshes) settings. The API of `SLEPLET` has been
 designed in an object-orientated manner and is easily extendible. Upon
 installation, `SLEPLET` comes with two command line interfaces - `sphere` and
 `mesh` - which allows one to easily generate plots on the sphere and a set of
 meshes using `plotly`.
@@ -119,16 +124,16 @@
 The recommended way to install `SLEPLET` is via
 [pip](https://pypi.org/project/pip)
 
 ```sh
 pip install sleplet
 ```
 
-To install the latest development version of `SLEPLET` clone this repository
-and run
+To install the latest development version of `SLEPLET` clone this repository and
+run
 
 ```sh
 pip install -e .
 ```
 
 This will install two scripts `sphere` and `mesh` which can be used to generate
 the figures in
@@ -136,19 +141,19 @@
 
 ### Supported Platforms
 
 `SLEPLET` has been tested with
 [![Python](https://img.shields.io/pypi/pyversions/sleplet)](https://www.python.org).
 Windows is not currently supported as `SLEPLET` relies on
 [pyssht](https://pypi.org/project/pyssht) and
-[pys2let](https://pypi.org/project/pys2let) which do not work on Windows.
-These can hopefully be replaced with
+[pys2let](https://pypi.org/project/pys2let) which do not work on Windows. These
+can hopefully be replaced with
 [s2fft](https://github.com/astro-informatics/s2fft) and
-[s2wav](https://github.com/astro-informatics/s2wav) in the future when they
-are available on [PyPI](https://pypi.org).
+[s2wav](https://github.com/astro-informatics/s2wav) in the future when they are
+available on [PyPI](https://pypi.org).
 
 ## Example Usage
 
 `SLEPLET` may be interacted with via the API or the CLIs.
 
 ### API Usage
 
@@ -212,9 +217,9 @@
   pages   = 5221,
   doi     = {10.21105/joss.05221},
 }
 ```
 
 Please also cite [S2LET](https://doi.org/10.1051/0004-6361/201220729) upon which
 `SLEPLET` is built, along with [SSHT](https://doi.org/10.1109/TSP.2011.2166394)
-in the spherical setting or [libigl](https://doi.org/10.1145/3134472.3134497)
-in the mesh setting.
+in the spherical setting or [libigl](https://doi.org/10.1145/3134472.3134497) in
+the mesh setting.
```

### Comparing `sleplet-1.4.7/src/sleplet.egg-info/SOURCES.txt` & `sleplet-1.4.8/src/sleplet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

