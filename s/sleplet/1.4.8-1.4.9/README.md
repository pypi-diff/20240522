# Comparing `tmp/sleplet-1.4.8.tar.gz` & `tmp/sleplet-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleplet-1.4.8.tar", last modified: Wed May 22 15:42:41 2024, max compression
+gzip compressed data, was "sleplet-1.4.9.tar", last modified: Wed May 22 15:53:26 2024, max compression
```

## Comparing `sleplet-1.4.8.tar` & `sleplet-1.4.9.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.632697 sleplet-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-22 15:42:36.000000 sleplet-1.4.8/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-05-22 15:42:36.000000 sleplet-1.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-05-22 15:42:36.000000 sleplet-1.4.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-22 15:42:36.000000 sleplet-1.4.8/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-05-22 15:42:41.632697 sleplet-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-22 15:42:36.000000 sleplet-1.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-22 15:42:36.000000 sleplet-1.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:42:41.632697 sleplet-1.4.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.612697 sleplet-1.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.616697 sleplet-1.4.8/src/sleplet/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_array_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_bool_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_class_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_convolution_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.620697 sleplet-1.4.8/src/sleplet/_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/create_earth_flm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/create_wmap_flm.py
--rw-r--r--   0 runner    (1001) docker     (127)    39339 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_polygons_bird.off
--rw-r--r--   0 runner    (1001) docker     (127)   111621 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_polygons_cheetah.off
--rw-r--r--   0 runner    (1001) docker     (127)   321932 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_polygons_cube.off
--rw-r--r--   0 runner    (1001) docker     (127)    65194 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_polygons_dragon.off
--rw-r--r--   0 runner    (1001) docker     (127)   329591 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_polygons_homer.off
--rw-r--r--   0 runner    (1001) docker     (127)    36961 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_polygons_teapot.off
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_regions_bird.toml
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_regions_cheetah.toml
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_regions_cube.toml
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_regions_dragon.toml
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_regions_homer.toml
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/meshes_regions_teapot.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_data/setup_pooch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_integration_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_mask_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_mesh_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_parallel_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_plotly_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.620697 sleplet-1.4.8/src/sleplet/_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_scripts/plotting_on_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    11063 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_scripts/plotting_on_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_slepian_arbitrary_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_string_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 15:42:41.000000 sleplet-1.4.8/src/sleplet/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.628697 sleplet-1.4.8/src/sleplet/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/africa.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/axisymmetric_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/dirac_delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/earth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/elongated_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/flm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/fp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/harmonic_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/noise_earth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/ridgelets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian_africa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian_dirac_delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian_noise_africa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian_noise_south_america.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian_south_america.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian_wavelet_coefficients_africa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/slepian_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/south_america.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/spherical_harmonic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/squashed_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/functions/wmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/harmonic_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.628697 sleplet-1.4.8/src/sleplet/meshes/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/_mesh_slepian_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_basis_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_harmonic_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_noise_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_slepian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_noise_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/plot_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.628697 sleplet-1.4.8/src/sleplet/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/plotting/_create_plot_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/plotting/_create_plot_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.632697 sleplet-1.4.8/src/sleplet/slepian/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/slepian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/slepian/_slepian_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/slepian/region.py
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/slepian/slepian_arbitrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/slepian/slepian_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/slepian/slepian_limit_lat_lon.py
--rw-r--r--   0 runner    (1001) docker     (127)    14615 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/slepian/slepian_polar_cap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/slepian_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-22 15:42:36.000000 sleplet-1.4.8/src/sleplet/wavelet_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:42:41.632697 sleplet-1.4.8/src/sleplet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-05-22 15:42:41.000000 sleplet-1.4.8/src/sleplet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-22 15:42:41.000000 sleplet-1.4.8/src/sleplet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:42:41.000000 sleplet-1.4.8/src/sleplet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-22 15:42:41.000000 sleplet-1.4.8/src/sleplet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-22 15:42:41.000000 sleplet-1.4.8/src/sleplet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 15:42:41.000000 sleplet-1.4.8/src/sleplet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:26.272934 sleplet-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-22 15:53:20.000000 sleplet-1.4.9/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-05-22 15:53:20.000000 sleplet-1.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-05-22 15:53:20.000000 sleplet-1.4.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-22 15:53:20.000000 sleplet-1.4.9/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10066 2024-05-22 15:53:26.272934 sleplet-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-05-22 15:53:20.000000 sleplet-1.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-22 15:53:20.000000 sleplet-1.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:53:26.272934 sleplet-1.4.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:26.256934 sleplet-1.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:26.260933 sleplet-1.4.9/src/sleplet/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_array_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_bool_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_class_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_convolution_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:26.264934 sleplet-1.4.9/src/sleplet/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_data/create_earth_flm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_data/create_wmap_flm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39339 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_data/meshes_polygons_bird.off
+-rw-r--r--   0 runner    (1001) docker     (127)   111621 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_data/meshes_polygons_cheetah.off
+-rw-r--r--   0 runner    (1001) docker     (127)   321932 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_data/meshes_polygons_cube.off
+-rw-r--r--   0 runner    (1001) docker     (127)    65194 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_data/meshes_polygons_dragon.off
+-rw-r--r--   0 runner    (1001) docker     (127)   329591 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_data/meshes_polygons_homer.off
+-rw-r--r--   0 runner    (1001) docker     (127)    36961 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_data/meshes_polygons_teapot.off
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_data/meshes_regions_bird.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_data/meshes_regions_cheetah.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_data/meshes_regions_cube.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_data/meshes_regions_dragon.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_data/meshes_regions_homer.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_data/meshes_regions_teapot.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_data/setup_pooch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_integration_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_mask_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_mesh_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_parallel_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_plotly_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:26.264934 sleplet-1.4.9/src/sleplet/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_scripts/plotting_on_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11063 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_scripts/plotting_on_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_slepian_arbitrary_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_string_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 15:53:26.000000 sleplet-1.4.9/src/sleplet/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:26.268934 sleplet-1.4.9/src/sleplet/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/africa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/axisymmetric_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/dirac_delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/earth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/elongated_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/flm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/fp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/harmonic_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/noise_earth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/ridgelets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/slepian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/slepian_africa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/slepian_dirac_delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/slepian_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/slepian_noise_africa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/slepian_noise_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/slepian_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/slepian_wavelet_coefficients_africa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/slepian_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/south_america.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/spherical_harmonic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/squashed_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/functions/wmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/harmonic_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:26.272934 sleplet-1.4.9/src/sleplet/meshes/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/meshes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/meshes/_mesh_slepian_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/meshes/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/meshes/mesh_basis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/meshes/mesh_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/meshes/mesh_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/meshes/mesh_harmonic_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/meshes/mesh_noise_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/meshes/mesh_slepian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/meshes/mesh_slepian_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/meshes/mesh_slepian_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/meshes/mesh_slepian_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/meshes/mesh_slepian_noise_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/meshes/mesh_slepian_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/plot_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:26.272934 sleplet-1.4.9/src/sleplet/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/plotting/_create_plot_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/plotting/_create_plot_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:26.272934 sleplet-1.4.9/src/sleplet/slepian/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/slepian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/slepian/_slepian_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/slepian/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/slepian/slepian_arbitrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/slepian/slepian_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/slepian/slepian_limit_lat_lon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14615 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/slepian/slepian_polar_cap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/slepian_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-22 15:53:20.000000 sleplet-1.4.9/src/sleplet/wavelet_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:26.272934 sleplet-1.4.9/src/sleplet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10066 2024-05-22 15:53:26.000000 sleplet-1.4.9/src/sleplet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-22 15:53:26.000000 sleplet-1.4.9/src/sleplet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:53:26.000000 sleplet-1.4.9/src/sleplet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-22 15:53:26.000000 sleplet-1.4.9/src/sleplet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-22 15:53:26.000000 sleplet-1.4.9/src/sleplet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 15:53:26.000000 sleplet-1.4.9/src/sleplet.egg-info/top_level.txt
```

### Comparing `sleplet-1.4.8/CITATION.cff` & `sleplet-1.4.9/CITATION.cff`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/CODE_OF_CONDUCT.md` & `sleplet-1.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/CONTRIBUTING.md` & `sleplet-1.4.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/LICENCE.txt` & `sleplet-1.4.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/PKG-INFO` & `sleplet-1.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleplet
-Version: 1.4.8
+Version: 1.4.9
 Summary: Slepian Scale-Discretised Wavelets in Python
 Author-email: "Patrick J. Roddy" <patrickjamesroddy@gmail.com>
 License: BSD 3-Clause Licence
         
         Copyright (c) 2017-2024, Patrick Roddy
         All rights reserved.
         
@@ -74,15 +74,14 @@
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: tox; extra == "dev"
-Requires-Dist: tox-uv; extra == "dev"
 Requires-Dist: tuna; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: pdoc3; extra == "docs"
 Provides-Extra: readme
 Requires-Dist: pytest-codeblocks; extra == "readme"
 
@@ -96,15 +95,15 @@
 [![Python](https://img.shields.io/pypi/pyversions/sleplet)](https://www.python.org)
 [![repostatus](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![Test](https://github.com/astro-informatics/sleplet/actions/workflows/test.yaml/badge.svg)](https://github.com/astro-informatics/sleplet/actions/workflows/test.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/astro-informatics/sleplet/badge.svg?branch=main)](https://coveralls.io/github/astro-informatics/sleplet?branch=main)
 
 [![JOSS](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2/status.svg)](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2)
 [![PyOpenSci](https://tinyurl.com/y22nb8up)](https://github.com/pyOpenSci/software-submission/issues/148)
-[![Citation](https://img.shields.io/badge/cite-SLEPLET-yellow)](#citing)
+[![Citation](https://img.shields.io/badge/cite-SLEPLET-yellow)](https://github.com/astro-informatics/sleplet/blob/main/README.md#citing)
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Renovate](https://img.shields.io/badge/renovate-enabled-orange?logo=renovatebot)](https://renovatebot.com)
 
 `SLEPLET` is a Python package for the construction of Slepian wavelets in the
 spherical and manifold (via meshes) settings. The API of `SLEPLET` has been
 designed in an object-orientated manner and is easily extendible. Upon
```

### Comparing `sleplet-1.4.8/README.md` & `sleplet-1.4.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [![Python](https://img.shields.io/pypi/pyversions/sleplet)](https://www.python.org)
 [![repostatus](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![Test](https://github.com/astro-informatics/sleplet/actions/workflows/test.yaml/badge.svg)](https://github.com/astro-informatics/sleplet/actions/workflows/test.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/astro-informatics/sleplet/badge.svg?branch=main)](https://coveralls.io/github/astro-informatics/sleplet?branch=main)
 
 [![JOSS](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2/status.svg)](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2)
 [![PyOpenSci](https://tinyurl.com/y22nb8up)](https://github.com/pyOpenSci/software-submission/issues/148)
-[![Citation](https://img.shields.io/badge/cite-SLEPLET-yellow)](#citing)
+[![Citation](https://img.shields.io/badge/cite-SLEPLET-yellow)](https://github.com/astro-informatics/sleplet/blob/main/README.md#citing)
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Renovate](https://img.shields.io/badge/renovate-enabled-orange?logo=renovatebot)](https://renovatebot.com)
 
 `SLEPLET` is a Python package for the construction of Slepian wavelets in the
 spherical and manifold (via meshes) settings. The API of `SLEPLET` has been
 designed in an object-orientated manner and is easily extendible. Upon
```

### Comparing `sleplet-1.4.8/pyproject.toml` & `sleplet-1.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
 optional-dependencies = {dev = [
     "build",
     "mypy",
     "pre-commit",
     "pytest",
     "ruff",
     "tox",
-    "tox-uv",
     "tuna",
     "twine",
 ], docs = [
     "pdoc3",
 ], readme = [
     "pytest-codeblocks",
 ]}
```

### Comparing `sleplet-1.4.8/src/sleplet/__init__.py` & `sleplet-1.4.9/src/sleplet/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_bool_methods.py` & `sleplet-1.4.9/src/sleplet/_bool_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_class_lists.py` & `sleplet-1.4.9/src/sleplet/_class_lists.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_convolution_methods.py` & `sleplet-1.4.9/src/sleplet/_convolution_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_data/create_earth_flm.py` & `sleplet-1.4.9/src/sleplet/_data/create_earth_flm.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_data/create_wmap_flm.py` & `sleplet-1.4.9/src/sleplet/_data/create_wmap_flm.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_data/meshes_polygons_bird.off` & `sleplet-1.4.9/src/sleplet/_data/meshes_polygons_bird.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_data/meshes_polygons_cheetah.off` & `sleplet-1.4.9/src/sleplet/_data/meshes_polygons_cheetah.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_data/meshes_polygons_cube.off` & `sleplet-1.4.9/src/sleplet/_data/meshes_polygons_cube.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_data/meshes_polygons_dragon.off` & `sleplet-1.4.9/src/sleplet/_data/meshes_polygons_dragon.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_data/meshes_polygons_homer.off` & `sleplet-1.4.9/src/sleplet/_data/meshes_polygons_homer.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_data/meshes_polygons_teapot.off` & `sleplet-1.4.9/src/sleplet/_data/meshes_polygons_teapot.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_data/setup_pooch.py` & `sleplet-1.4.9/src/sleplet/_data/setup_pooch.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_integration_methods.py` & `sleplet-1.4.9/src/sleplet/_integration_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_mask_methods.py` & `sleplet-1.4.9/src/sleplet/_mask_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_mesh_methods.py` & `sleplet-1.4.9/src/sleplet/_mesh_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_parallel_methods.py` & `sleplet-1.4.9/src/sleplet/_parallel_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_plotly_methods.py` & `sleplet-1.4.9/src/sleplet/_plotly_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_scripts/plotting_on_mesh.py` & `sleplet-1.4.9/src/sleplet/_scripts/plotting_on_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_scripts/plotting_on_sphere.py` & `sleplet-1.4.9/src/sleplet/_scripts/plotting_on_sphere.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_slepian_arbitrary_methods.py` & `sleplet-1.4.9/src/sleplet/_slepian_arbitrary_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_smoothing.py` & `sleplet-1.4.9/src/sleplet/_smoothing.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/_string_methods.py` & `sleplet-1.4.9/src/sleplet/_string_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/__init__.py` & `sleplet-1.4.9/src/sleplet/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/africa.py` & `sleplet-1.4.9/src/sleplet/functions/africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py` & `sleplet-1.4.9/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py` & `sleplet-1.4.9/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py` & `sleplet-1.4.9/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/axisymmetric_wavelets.py` & `sleplet-1.4.9/src/sleplet/functions/axisymmetric_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/coefficients.py` & `sleplet-1.4.9/src/sleplet/functions/coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/dirac_delta.py` & `sleplet-1.4.9/src/sleplet/functions/dirac_delta.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/earth.py` & `sleplet-1.4.9/src/sleplet/functions/earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/elongated_gaussian.py` & `sleplet-1.4.9/src/sleplet/functions/elongated_gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/flm.py` & `sleplet-1.4.9/src/sleplet/functions/flm.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/fp.py` & `sleplet-1.4.9/src/sleplet/functions/fp.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/gaussian.py` & `sleplet-1.4.9/src/sleplet/functions/gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/harmonic_gaussian.py` & `sleplet-1.4.9/src/sleplet/functions/harmonic_gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/identity.py` & `sleplet-1.4.9/src/sleplet/functions/identity.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/noise_earth.py` & `sleplet-1.4.9/src/sleplet/functions/noise_earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/ridgelets.py` & `sleplet-1.4.9/src/sleplet/functions/ridgelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/slepian.py` & `sleplet-1.4.9/src/sleplet/functions/slepian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/slepian_africa.py` & `sleplet-1.4.9/src/sleplet/functions/slepian_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/slepian_dirac_delta.py` & `sleplet-1.4.9/src/sleplet/functions/slepian_dirac_delta.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/slepian_identity.py` & `sleplet-1.4.9/src/sleplet/functions/slepian_identity.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/slepian_noise_africa.py` & `sleplet-1.4.9/src/sleplet/functions/slepian_noise_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/slepian_noise_south_america.py` & `sleplet-1.4.9/src/sleplet/functions/slepian_noise_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/slepian_south_america.py` & `sleplet-1.4.9/src/sleplet/functions/slepian_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/slepian_wavelet_coefficients_africa.py` & `sleplet-1.4.9/src/sleplet/functions/slepian_wavelet_coefficients_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py` & `sleplet-1.4.9/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/slepian_wavelets.py` & `sleplet-1.4.9/src/sleplet/functions/slepian_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/south_america.py` & `sleplet-1.4.9/src/sleplet/functions/south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/spherical_harmonic.py` & `sleplet-1.4.9/src/sleplet/functions/spherical_harmonic.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/squashed_gaussian.py` & `sleplet-1.4.9/src/sleplet/functions/squashed_gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/functions/wmap.py` & `sleplet-1.4.9/src/sleplet/functions/wmap.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/harmonic_methods.py` & `sleplet-1.4.9/src/sleplet/harmonic_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/meshes/__init__.py` & `sleplet-1.4.9/src/sleplet/meshes/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/meshes/_mesh_slepian_decomposition.py` & `sleplet-1.4.9/src/sleplet/meshes/_mesh_slepian_decomposition.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/meshes/mesh.py` & `sleplet-1.4.9/src/sleplet/meshes/mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/meshes/mesh_basis_functions.py` & `sleplet-1.4.9/src/sleplet/meshes/mesh_basis_functions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/meshes/mesh_coefficients.py` & `sleplet-1.4.9/src/sleplet/meshes/mesh_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/meshes/mesh_field.py` & `sleplet-1.4.9/src/sleplet/meshes/mesh_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/meshes/mesh_harmonic_coefficients.py` & `sleplet-1.4.9/src/sleplet/meshes/mesh_harmonic_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/meshes/mesh_noise_field.py` & `sleplet-1.4.9/src/sleplet/meshes/mesh_noise_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/meshes/mesh_slepian.py` & `sleplet-1.4.9/src/sleplet/meshes/mesh_slepian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_coefficients.py` & `sleplet-1.4.9/src/sleplet/meshes/mesh_slepian_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_field.py` & `sleplet-1.4.9/src/sleplet/meshes/mesh_slepian_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_functions.py` & `sleplet-1.4.9/src/sleplet/meshes/mesh_slepian_functions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_noise_field.py` & `sleplet-1.4.9/src/sleplet/meshes/mesh_slepian_noise_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py` & `sleplet-1.4.9/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/meshes/mesh_slepian_wavelets.py` & `sleplet-1.4.9/src/sleplet/meshes/mesh_slepian_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/noise.py` & `sleplet-1.4.9/src/sleplet/noise.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/plot_methods.py` & `sleplet-1.4.9/src/sleplet/plot_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/plotting/_create_plot_mesh.py` & `sleplet-1.4.9/src/sleplet/plotting/_create_plot_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/plotting/_create_plot_sphere.py` & `sleplet-1.4.9/src/sleplet/plotting/_create_plot_sphere.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/slepian/_slepian_decomposition.py` & `sleplet-1.4.9/src/sleplet/slepian/_slepian_decomposition.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/slepian/region.py` & `sleplet-1.4.9/src/sleplet/slepian/region.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/slepian/slepian_arbitrary.py` & `sleplet-1.4.9/src/sleplet/slepian/slepian_arbitrary.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/slepian/slepian_functions.py` & `sleplet-1.4.9/src/sleplet/slepian/slepian_functions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/slepian/slepian_limit_lat_lon.py` & `sleplet-1.4.9/src/sleplet/slepian/slepian_limit_lat_lon.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/slepian/slepian_polar_cap.py` & `sleplet-1.4.9/src/sleplet/slepian/slepian_polar_cap.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/slepian_methods.py` & `sleplet-1.4.9/src/sleplet/slepian_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet/wavelet_methods.py` & `sleplet-1.4.9/src/sleplet/wavelet_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.8/src/sleplet.egg-info/PKG-INFO` & `sleplet-1.4.9/src/sleplet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleplet
-Version: 1.4.8
+Version: 1.4.9
 Summary: Slepian Scale-Discretised Wavelets in Python
 Author-email: "Patrick J. Roddy" <patrickjamesroddy@gmail.com>
 License: BSD 3-Clause Licence
         
         Copyright (c) 2017-2024, Patrick Roddy
         All rights reserved.
         
@@ -74,15 +74,14 @@
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: tox; extra == "dev"
-Requires-Dist: tox-uv; extra == "dev"
 Requires-Dist: tuna; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: pdoc3; extra == "docs"
 Provides-Extra: readme
 Requires-Dist: pytest-codeblocks; extra == "readme"
 
@@ -96,15 +95,15 @@
 [![Python](https://img.shields.io/pypi/pyversions/sleplet)](https://www.python.org)
 [![repostatus](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![Test](https://github.com/astro-informatics/sleplet/actions/workflows/test.yaml/badge.svg)](https://github.com/astro-informatics/sleplet/actions/workflows/test.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/astro-informatics/sleplet/badge.svg?branch=main)](https://coveralls.io/github/astro-informatics/sleplet?branch=main)
 
 [![JOSS](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2/status.svg)](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2)
 [![PyOpenSci](https://tinyurl.com/y22nb8up)](https://github.com/pyOpenSci/software-submission/issues/148)
-[![Citation](https://img.shields.io/badge/cite-SLEPLET-yellow)](#citing)
+[![Citation](https://img.shields.io/badge/cite-SLEPLET-yellow)](https://github.com/astro-informatics/sleplet/blob/main/README.md#citing)
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Renovate](https://img.shields.io/badge/renovate-enabled-orange?logo=renovatebot)](https://renovatebot.com)
 
 `SLEPLET` is a Python package for the construction of Slepian wavelets in the
 spherical and manifold (via meshes) settings. The API of `SLEPLET` has been
 designed in an object-orientated manner and is easily extendible. Upon
```

### Comparing `sleplet-1.4.8/src/sleplet.egg-info/SOURCES.txt` & `sleplet-1.4.9/src/sleplet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

