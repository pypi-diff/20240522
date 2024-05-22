# Comparing `tmp/pyGDM2-1.1.5.1.tar.gz` & `tmp/pygdm2-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGDM2-1.1.5.1.tar", last modified: Tue Mar  5 08:59:39 2024, max compression
+gzip compressed data, was "pygdm2-1.1.6.tar", last modified: Fri May 17 14:54:23 2024, max compression
```

## Comparing `pyGDM2-1.1.5.1.tar` & `pygdm2-1.1.6.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2024-03-05 08:59:39.077544 pyGDM2-1.1.5.1/
--rw-rw-r--   0 hans      (1000) hans      (1000)    35183 2018-02-12 08:58:24.000000 pyGDM2-1.1.5.1/LICENSE.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)       83 2018-02-12 08:58:24.000000 pyGDM2-1.1.5.1/MANIFEST.in
--rw-rw-r--   0 hans      (1000) hans      (1000)     5935 2024-03-05 08:59:39.077544 pyGDM2-1.1.5.1/PKG-INFO
--rw-rw-r--   0 hans      (1000) hans      (1000)     4912 2022-07-07 10:33:16.000000 pyGDM2-1.1.5.1/README.rst
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2024-03-05 08:59:38.833543 pyGDM2-1.1.5.1/examples/
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2024-03-05 08:59:38.869543 pyGDM2-1.1.5.1/examples/01_Mie/
--rw-rw-r--   0 hans      (1000) hans      (1000)     5585 2020-02-25 17:30:31.000000 pyGDM2-1.1.5.1/examples/01_Mie/example_mie_01_n2.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3174 2020-11-30 11:24:51.000000 pyGDM2-1.1.5.1/examples/01_Mie/example_mie_02_Au.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3755 2020-02-25 17:30:31.000000 pyGDM2-1.1.5.1/examples/01_Mie/example_mie_03_Si.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    16059 2018-02-12 08:58:24.000000 pyGDM2-1.1.5.1/examples/01_Mie/scat_mie_Au_D50nm.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)    15042 2018-02-12 08:58:24.000000 pyGDM2-1.1.5.1/examples/01_Mie/scat_mie_Si_D150nm.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)    16039 2018-02-12 08:58:24.000000 pyGDM2-1.1.5.1/examples/01_Mie/scat_mie_n2_D300nm.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)     1396 2021-05-10 19:30:14.000000 pyGDM2-1.1.5.1/examples/01_simple_simulation.py
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2024-03-05 08:59:38.889543 pyGDM2-1.1.5.1/examples/02_other_examples/
--rw-rw-r--   0 hans      (1000) hans      (1000)     3260 2020-02-25 17:30:31.000000 pyGDM2-1.1.5.1/examples/02_other_examples/example_other_01_SiSphere_FW_BW.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     4090 2020-11-30 11:24:51.000000 pyGDM2-1.1.5.1/examples/02_other_examples/example_other_02_splitring_dipole_farfield.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3201 2020-02-25 17:30:31.000000 pyGDM2-1.1.5.1/examples/02_other_examples/example_other_03_Lshape_polarconversion.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3275 2020-11-30 11:24:51.000000 pyGDM2-1.1.5.1/examples/02_other_examples/example_other_04_heat.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3197 2019-06-07 07:06:07.000000 pyGDM2-1.1.5.1/examples/02_other_examples/example_other_05_decayrate.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     5128 2020-02-25 17:30:31.000000 pyGDM2-1.1.5.1/examples/02_other_examples/example_other_06_rasterscan_thermoplasmonics.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     4043 2020-02-25 17:30:31.000000 pyGDM2-1.1.5.1/examples/02_other_examples/example_other_07_rasterscan_LDOS.py
--rwxrwxr-x   0 hans      (1000) hans      (1000)      106 2018-07-09 08:53:23.000000 pyGDM2-1.1.5.1/examples/02_other_examples/example_other_08_run_via_mpi.sh
--rw-rw-r--   0 hans      (1000) hans      (1000)     2023 2019-06-07 07:06:07.000000 pyGDM2-1.1.5.1/examples/02_other_examples/example_other_08_spectra_via_MPI.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     2974 2020-02-25 17:30:31.000000 pyGDM2-1.1.5.1/examples/02_other_examples/example_other_09_multipole_decomposition.py
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2024-03-05 08:59:38.889543 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/
--rw-rw-r--   0 hans      (1000) hans      (1000)     5033 2019-06-07 07:06:07.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/example_eo_01_scattering.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     2556 2019-06-07 07:06:07.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/example_eo_01b_scattering_analyze.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3086 2019-06-07 07:06:07.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/example_eo_02_nearfield.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     2332 2019-06-07 07:06:07.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/example_eo_02b_nearfield_analyze.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     6331 2020-02-25 17:30:31.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/example_eo_03_multi_objective.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3745 2020-02-25 17:30:31.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/example_eo_03b_multi_objective_analyze.py
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2024-03-05 08:59:38.977544 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2024-03-05 08:59:38.981544 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/eo_out/
--rw-rw-r--   0 hans      (1000) hans      (1000)       52 2018-02-12 08:58:24.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/eo_out/readme.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)     3282 2018-02-12 08:58:24.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_01_eo.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     1793 2018-02-12 08:58:24.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_02_eo_load_final.py
--rw-rw-r--   0 hans      (1000) hans      (1000)      598 2018-02-12 08:58:24.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_03_eo_continue_optimization.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     4582 2018-02-12 08:58:24.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_04_ownproblem.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     2845 2018-02-12 08:58:24.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_04b_ownproblem_analyze.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     5845 2018-02-12 08:58:24.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_05_ownmodel.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3030 2018-02-12 08:58:24.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_05b_ownmodel_analyze.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3160 2018-02-12 08:58:24.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_06_maximize_nearfield.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     2140 2018-02-12 08:58:24.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_06b_maximize_nearfield_analyze.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     5199 2018-02-12 08:58:24.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_07_multi_objective_problem.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3273 2018-02-12 08:58:24.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_07b_MO_analyze.py
--rw-rw-r--   0 hans      (1000) hans      (1000)      146 2019-06-07 07:06:07.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/readme.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)      280 2018-02-12 08:58:24.000000 pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/readme.txt
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2024-03-05 08:59:38.989544 pyGDM2-1.1.5.1/examples/04_tutorials/
--rw-rw-r--   0 hans      (1000) hans      (1000)     4753 2019-11-21 14:42:24.000000 pyGDM2-1.1.5.1/examples/04_tutorials/surface_plasmon.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    40882 2022-07-07 10:33:16.000000 pyGDM2-1.1.5.1/examples/04_tutorials/surface_plasmon_gold.png
--rw-rw-r--   0 hans      (1000) hans      (1000)    31794 2022-07-07 10:33:16.000000 pyGDM2-1.1.5.1/examples/04_tutorials/surface_plasmon_silicon.png
--rw-rw-r--   0 hans      (1000) hans      (1000)     2100 2020-11-30 11:24:51.000000 pyGDM2-1.1.5.1/examples/04_tutorials/using_callbacks.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     2278 2020-11-30 11:24:51.000000 pyGDM2-1.1.5.1/examples/04_tutorials/visualize_incident_field.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    40664 2020-03-25 20:50:47.000000 pyGDM2-1.1.5.1/examples/examples.tar.gz
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2024-03-05 08:59:39.005544 pyGDM2-1.1.5.1/pyGDM2/
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2024-03-05 08:59:39.017544 pyGDM2-1.1.5.1/pyGDM2/EO/
--rw-rw-r--   0 hans      (1000) hans      (1000)     1099 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/EO/__init__.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    13621 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/EO/core.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    29885 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/EO/models.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    16581 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/EO/problems.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    21324 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/EO/tools.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     1853 2024-03-05 08:59:12.000000 pyGDM2-1.1.5.1/pyGDM2/__init__.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    49243 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/core.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     9311 2024-03-05 08:59:12.000000 pyGDM2-1.1.5.1/pyGDM2/electron.py
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2024-03-05 08:59:39.017544 pyGDM2-1.1.5.1/pyGDM2/fields/
--rw-rw-r--   0 hans      (1000) hans      (1000)     2017 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/fields/__init__.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    47658 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/fields/deprecated.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     5613 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/fields/efield_class.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     4976 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/fields/electron.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    54374 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/fields/focused_beams.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    37755 2024-03-05 08:59:12.000000 pyGDM2-1.1.5.1/pyGDM2/fields/regular.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    60501 2024-03-05 08:59:12.000000 pyGDM2-1.1.5.1/pyGDM2/linear.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    57348 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/materials.py
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2024-03-05 08:59:39.017544 pyGDM2-1.1.5.1/pyGDM2/multipole/
--rw-rw-r--   0 hans      (1000) hans      (1000)     2017 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/multipole/__init__.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     9260 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/multipole/main.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    29861 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/multipole/polarizabilities.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    57246 2024-03-05 08:59:12.000000 pyGDM2-1.1.5.1/pyGDM2/multipole/processing.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     8025 2024-01-25 14:20:26.000000 pyGDM2-1.1.5.1/pyGDM2/multipole/propagators.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     4691 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/nonlinear.py
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2024-03-05 08:59:39.069544 pyGDM2-1.1.5.1/pyGDM2/propagators/
--rw-rw-r--   0 hans      (1000) hans      (1000)     1892 2023-06-30 08:52:10.000000 pyGDM2-1.1.5.1/pyGDM2/propagators/__init__.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    35658 2023-06-30 08:52:10.000000 pyGDM2-1.1.5.1/pyGDM2/propagators/propagators.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    36147 2023-06-30 08:52:10.000000 pyGDM2-1.1.5.1/pyGDM2/propagators/propagators_2D.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    53212 2023-06-30 08:52:10.000000 pyGDM2-1.1.5.1/pyGDM2/propagators/propagators_periodic.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    24901 2023-06-30 08:52:10.000000 pyGDM2-1.1.5.1/pyGDM2/propagators/propagators_periodic_slow.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    84230 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/structures.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    91116 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/tools.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    44118 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/visu.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    27130 2024-01-25 14:30:54.000000 pyGDM2-1.1.5.1/pyGDM2/visu3d.py
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2024-03-05 08:59:39.009544 pyGDM2-1.1.5.1/pyGDM2.egg-info/
--rw-rw-r--   0 hans      (1000) hans      (1000)     5935 2024-03-05 08:59:38.000000 pyGDM2-1.1.5.1/pyGDM2.egg-info/PKG-INFO
--rw-rw-r--   0 hans      (1000) hans      (1000)     3718 2024-03-05 08:59:38.000000 pyGDM2-1.1.5.1/pyGDM2.egg-info/SOURCES.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)        1 2024-03-05 08:59:38.000000 pyGDM2-1.1.5.1/pyGDM2.egg-info/dependency_links.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)       12 2024-03-05 08:59:38.000000 pyGDM2-1.1.5.1/pyGDM2.egg-info/requires.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)        7 2024-03-05 08:59:38.000000 pyGDM2-1.1.5.1/pyGDM2.egg-info/top_level.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)       80 2024-03-05 08:59:39.077544 pyGDM2-1.1.5.1/setup.cfg
--rw-rw-r--   0 hans      (1000) hans      (1000)     6069 2023-06-30 08:52:10.000000 pyGDM2-1.1.5.1/setup.py
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2024-03-05 08:59:39.077544 pyGDM2-1.1.5.1/tests/
--rw-rw-r--   0 hans      (1000) hans      (1000)    14956 2020-11-30 11:24:51.000000 pyGDM2-1.1.5.1/tests/basic_tests.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     1337 2020-12-04 22:18:43.000000 pyGDM2-1.1.5.1/tests/tests_propagators.py
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2024-05-17 14:54:23.396673 pygdm2-1.1.6/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    35183 2018-02-12 08:58:24.000000 pygdm2-1.1.6/LICENSE.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)       83 2018-02-12 08:58:24.000000 pygdm2-1.1.6/MANIFEST.in
+-rw-r--r--   0 pwiecha   (1000) pwiecha   (1000)     5970 2024-05-17 14:54:23.396673 pygdm2-1.1.6/PKG-INFO
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     4912 2022-07-07 10:33:16.000000 pygdm2-1.1.6/README.rst
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2024-05-17 14:54:23.381672 pygdm2-1.1.6/examples/
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2024-05-17 14:54:23.382672 pygdm2-1.1.6/examples/01_Mie/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     5585 2020-02-25 17:30:31.000000 pygdm2-1.1.6/examples/01_Mie/example_mie_01_n2.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3174 2020-11-30 11:24:51.000000 pygdm2-1.1.6/examples/01_Mie/example_mie_02_Au.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3755 2020-02-25 17:30:31.000000 pygdm2-1.1.6/examples/01_Mie/example_mie_03_Si.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    16059 2018-02-12 08:58:24.000000 pygdm2-1.1.6/examples/01_Mie/scat_mie_Au_D50nm.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    15042 2018-02-12 08:58:24.000000 pygdm2-1.1.6/examples/01_Mie/scat_mie_Si_D150nm.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    16039 2018-02-12 08:58:24.000000 pygdm2-1.1.6/examples/01_Mie/scat_mie_n2_D300nm.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     1396 2021-05-10 19:30:14.000000 pygdm2-1.1.6/examples/01_simple_simulation.py
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2024-05-17 14:54:23.384672 pygdm2-1.1.6/examples/02_other_examples/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3260 2020-02-25 17:30:31.000000 pygdm2-1.1.6/examples/02_other_examples/example_other_01_SiSphere_FW_BW.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     4090 2020-11-30 11:24:51.000000 pygdm2-1.1.6/examples/02_other_examples/example_other_02_splitring_dipole_farfield.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3201 2020-02-25 17:30:31.000000 pygdm2-1.1.6/examples/02_other_examples/example_other_03_Lshape_polarconversion.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3275 2020-11-30 11:24:51.000000 pygdm2-1.1.6/examples/02_other_examples/example_other_04_heat.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3197 2019-06-07 07:06:07.000000 pygdm2-1.1.6/examples/02_other_examples/example_other_05_decayrate.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     5128 2020-02-25 17:30:31.000000 pygdm2-1.1.6/examples/02_other_examples/example_other_06_rasterscan_thermoplasmonics.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     4043 2020-02-25 17:30:31.000000 pygdm2-1.1.6/examples/02_other_examples/example_other_07_rasterscan_LDOS.py
+-rwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)      106 2018-07-09 08:53:23.000000 pygdm2-1.1.6/examples/02_other_examples/example_other_08_run_via_mpi.sh
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2023 2019-06-07 07:06:07.000000 pygdm2-1.1.6/examples/02_other_examples/example_other_08_spectra_via_MPI.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2974 2020-02-25 17:30:31.000000 pygdm2-1.1.6/examples/02_other_examples/example_other_09_multipole_decomposition.py
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2024-05-17 14:54:23.386673 pygdm2-1.1.6/examples/03_evolutionary_optimization/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     5033 2019-06-07 07:06:07.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/example_eo_01_scattering.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2556 2019-06-07 07:06:07.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/example_eo_01b_scattering_analyze.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3086 2019-06-07 07:06:07.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/example_eo_02_nearfield.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2332 2019-06-07 07:06:07.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/example_eo_02b_nearfield_analyze.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     6331 2020-02-25 17:30:31.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/example_eo_03_multi_objective.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3745 2020-02-25 17:30:31.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/example_eo_03b_multi_objective_analyze.py
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2024-05-17 14:54:23.389673 pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2024-05-17 14:54:23.389673 pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/eo_out/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)       52 2018-02-12 08:58:24.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/eo_out/readme.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3282 2018-02-12 08:58:24.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_01_eo.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     1793 2018-02-12 08:58:24.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_02_eo_load_final.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)      598 2018-02-12 08:58:24.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_03_eo_continue_optimization.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     4582 2018-02-12 08:58:24.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_04_ownproblem.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2845 2018-02-12 08:58:24.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_04b_ownproblem_analyze.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     5845 2018-02-12 08:58:24.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_05_ownmodel.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3030 2018-02-12 08:58:24.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_05b_ownmodel_analyze.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3160 2018-02-12 08:58:24.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_06_maximize_nearfield.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2140 2018-02-12 08:58:24.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_06b_maximize_nearfield_analyze.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     5199 2018-02-12 08:58:24.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_07_multi_objective_problem.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3273 2018-02-12 08:58:24.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_07b_MO_analyze.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)      146 2019-06-07 07:06:07.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/readme.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)      280 2018-02-12 08:58:24.000000 pygdm2-1.1.6/examples/03_evolutionary_optimization/readme.txt
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2024-05-17 14:54:23.390673 pygdm2-1.1.6/examples/04_tutorials/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     4753 2019-11-21 14:42:24.000000 pygdm2-1.1.6/examples/04_tutorials/surface_plasmon.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    40882 2022-07-07 10:33:16.000000 pygdm2-1.1.6/examples/04_tutorials/surface_plasmon_gold.png
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    31794 2022-07-07 10:33:16.000000 pygdm2-1.1.6/examples/04_tutorials/surface_plasmon_silicon.png
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2100 2020-11-30 11:24:51.000000 pygdm2-1.1.6/examples/04_tutorials/using_callbacks.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2278 2020-11-30 11:24:51.000000 pygdm2-1.1.6/examples/04_tutorials/visualize_incident_field.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    40664 2020-03-25 20:50:47.000000 pygdm2-1.1.6/examples/examples.tar.gz
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2024-05-17 14:54:23.392673 pygdm2-1.1.6/pyGDM2/
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2024-05-17 14:54:23.393673 pygdm2-1.1.6/pyGDM2/EO/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     1099 2024-01-25 14:30:54.000000 pygdm2-1.1.6/pyGDM2/EO/__init__.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    13621 2024-01-25 14:30:54.000000 pygdm2-1.1.6/pyGDM2/EO/core.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    29885 2024-01-25 14:30:54.000000 pygdm2-1.1.6/pyGDM2/EO/models.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    16581 2024-01-25 14:30:54.000000 pygdm2-1.1.6/pyGDM2/EO/problems.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    21324 2024-01-25 14:30:54.000000 pygdm2-1.1.6/pyGDM2/EO/tools.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     1873 2024-05-17 14:53:50.000000 pygdm2-1.1.6/pyGDM2/__init__.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    49243 2024-01-25 14:30:54.000000 pygdm2-1.1.6/pyGDM2/core.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     9311 2024-03-05 08:59:12.000000 pygdm2-1.1.6/pyGDM2/electron.py
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2024-05-17 14:54:23.394673 pygdm2-1.1.6/pyGDM2/fields/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2017 2024-01-25 14:30:54.000000 pygdm2-1.1.6/pyGDM2/fields/__init__.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    47658 2024-01-25 14:30:54.000000 pygdm2-1.1.6/pyGDM2/fields/deprecated.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     5613 2024-01-25 14:30:54.000000 pygdm2-1.1.6/pyGDM2/fields/efield_class.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     4976 2024-01-25 14:30:54.000000 pygdm2-1.1.6/pyGDM2/fields/electron.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    54374 2024-01-25 14:30:54.000000 pygdm2-1.1.6/pyGDM2/fields/focused_beams.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    37755 2024-03-05 08:59:12.000000 pygdm2-1.1.6/pyGDM2/fields/regular.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    60501 2024-03-05 08:59:12.000000 pygdm2-1.1.6/pyGDM2/linear.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    57348 2024-01-25 14:30:54.000000 pygdm2-1.1.6/pyGDM2/materials.py
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2024-05-17 14:54:23.395673 pygdm2-1.1.6/pyGDM2/multipole/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2017 2024-01-25 14:30:54.000000 pygdm2-1.1.6/pyGDM2/multipole/__init__.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     9260 2024-01-25 14:30:54.000000 pygdm2-1.1.6/pyGDM2/multipole/main.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    29867 2024-03-25 16:35:19.000000 pygdm2-1.1.6/pyGDM2/multipole/polarizabilities.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    57246 2024-03-05 08:59:12.000000 pygdm2-1.1.6/pyGDM2/multipole/processing.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     8025 2024-01-25 14:20:26.000000 pygdm2-1.1.6/pyGDM2/multipole/propagators.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     4691 2024-01-25 14:30:54.000000 pygdm2-1.1.6/pyGDM2/nonlinear.py
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2024-05-17 14:54:23.395673 pygdm2-1.1.6/pyGDM2/propagators/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     1892 2023-06-30 08:52:10.000000 pygdm2-1.1.6/pyGDM2/propagators/__init__.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    35658 2023-06-30 08:52:10.000000 pygdm2-1.1.6/pyGDM2/propagators/propagators.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    36147 2023-06-30 08:52:10.000000 pygdm2-1.1.6/pyGDM2/propagators/propagators_2D.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    53212 2023-06-30 08:52:10.000000 pygdm2-1.1.6/pyGDM2/propagators/propagators_periodic.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    24901 2023-06-30 08:52:10.000000 pygdm2-1.1.6/pyGDM2/propagators/propagators_periodic_slow.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    84230 2024-01-25 14:30:54.000000 pygdm2-1.1.6/pyGDM2/structures.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    91910 2024-04-30 11:08:08.000000 pygdm2-1.1.6/pyGDM2/tools.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    47505 2024-04-30 10:44:16.000000 pygdm2-1.1.6/pyGDM2/visu.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    27130 2024-01-25 14:30:54.000000 pygdm2-1.1.6/pyGDM2/visu3d.py
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2024-05-17 14:54:23.396673 pygdm2-1.1.6/pyGDM2.egg-info/
+-rw-r--r--   0 pwiecha   (1000) pwiecha   (1000)     5970 2024-05-17 14:54:23.000000 pygdm2-1.1.6/pyGDM2.egg-info/PKG-INFO
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3718 2024-05-17 14:54:23.000000 pygdm2-1.1.6/pyGDM2.egg-info/SOURCES.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)        1 2024-05-17 14:54:23.000000 pygdm2-1.1.6/pyGDM2.egg-info/dependency_links.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)       12 2024-05-17 14:54:23.000000 pygdm2-1.1.6/pyGDM2.egg-info/requires.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)        7 2024-05-17 14:54:23.000000 pygdm2-1.1.6/pyGDM2.egg-info/top_level.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)       80 2024-05-17 14:54:23.397673 pygdm2-1.1.6/setup.cfg
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     4824 2024-05-17 14:52:42.000000 pygdm2-1.1.6/setup.py
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2024-05-17 14:54:23.396673 pygdm2-1.1.6/tests/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    14956 2020-11-30 11:24:51.000000 pygdm2-1.1.6/tests/basic_tests.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     1337 2020-12-04 22:18:43.000000 pygdm2-1.1.6/tests/tests_propagators.py
```

### Comparing `pyGDM2-1.1.5.1/LICENSE.txt` & `pygdm2-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/PKG-INFO` & `pygdm2-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: pyGDM2
-Version: 1.1.5.1
+Version: 1.1.6
 Summary: A python full-field electrodynamical solver, based on the Green dyadic method (volume integral technique in frequency domain).
 Home-page: https://gitlab.com/wiechapeter/pyGDM2
+Download-URL: 
 Author: Peter R. Wiecha
 Author-email: pwiecha@laas.fr
 License: GPLv3+
 Keywords: coupled dipoles method,green dyadic method,electrodynamical simulations,nano optics,frequency-domain
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7
 License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: numba
 
 ***********************************
 Requirements / Installation
 ***********************************
 
 pyGDM is an open source python toolkit for electro-dynamical simulations, implementing the `Green dyadic method (GDM) <https://doi.org/10.1088/0034-4885/68/8/R05>`_, a volume discretization technique. 
 pyGDM is based on simulation codes and theoretical models developed over the past 20 years by `Christian Girard <http://www.cemes.fr/Theory-of-Complex-Nano-optical?lang=en>`_ at CEMES (see e.g. `Ch. Girard 2005 Rep. Prog. Phys. 68 1883 <https://doi.org/10.1088/0034-4885/68/8/R05>`_), with contributions from G. Colas des Francs, A. Arbouet, R. Marty, C. Majorel, A. Patoux, Y. Brûlé and P.R. Wiecha.
@@ -148,9 +150,7 @@
    - P\. R. Wiecha
 
 
 
    
 
 
-
-
```

### Comparing `pyGDM2-1.1.5.1/README.rst` & `pygdm2-1.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/01_Mie/example_mie_01_n2.py` & `pygdm2-1.1.6/examples/01_Mie/example_mie_01_n2.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/01_Mie/example_mie_02_Au.py` & `pygdm2-1.1.6/examples/01_Mie/example_mie_02_Au.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/01_Mie/example_mie_03_Si.py` & `pygdm2-1.1.6/examples/01_Mie/example_mie_03_Si.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/01_Mie/scat_mie_Au_D50nm.txt` & `pygdm2-1.1.6/examples/01_Mie/scat_mie_Au_D50nm.txt`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/01_Mie/scat_mie_Si_D150nm.txt` & `pygdm2-1.1.6/examples/01_Mie/scat_mie_Si_D150nm.txt`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/01_Mie/scat_mie_n2_D300nm.txt` & `pygdm2-1.1.6/examples/01_Mie/scat_mie_n2_D300nm.txt`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/01_simple_simulation.py` & `pygdm2-1.1.6/examples/01_simple_simulation.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/02_other_examples/example_other_01_SiSphere_FW_BW.py` & `pygdm2-1.1.6/examples/02_other_examples/example_other_01_SiSphere_FW_BW.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/02_other_examples/example_other_02_splitring_dipole_farfield.py` & `pygdm2-1.1.6/examples/02_other_examples/example_other_02_splitring_dipole_farfield.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/02_other_examples/example_other_03_Lshape_polarconversion.py` & `pygdm2-1.1.6/examples/02_other_examples/example_other_03_Lshape_polarconversion.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/02_other_examples/example_other_04_heat.py` & `pygdm2-1.1.6/examples/02_other_examples/example_other_04_heat.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/02_other_examples/example_other_05_decayrate.py` & `pygdm2-1.1.6/examples/02_other_examples/example_other_05_decayrate.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/02_other_examples/example_other_06_rasterscan_thermoplasmonics.py` & `pygdm2-1.1.6/examples/02_other_examples/example_other_06_rasterscan_thermoplasmonics.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/02_other_examples/example_other_07_rasterscan_LDOS.py` & `pygdm2-1.1.6/examples/02_other_examples/example_other_07_rasterscan_LDOS.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/02_other_examples/example_other_08_spectra_via_MPI.py` & `pygdm2-1.1.6/examples/02_other_examples/example_other_08_spectra_via_MPI.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/02_other_examples/example_other_09_multipole_decomposition.py` & `pygdm2-1.1.6/examples/02_other_examples/example_other_09_multipole_decomposition.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/example_eo_01_scattering.py` & `pygdm2-1.1.6/examples/03_evolutionary_optimization/example_eo_01_scattering.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/example_eo_01b_scattering_analyze.py` & `pygdm2-1.1.6/examples/03_evolutionary_optimization/example_eo_01b_scattering_analyze.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/example_eo_02_nearfield.py` & `pygdm2-1.1.6/examples/03_evolutionary_optimization/example_eo_02_nearfield.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/example_eo_02b_nearfield_analyze.py` & `pygdm2-1.1.6/examples/03_evolutionary_optimization/example_eo_02b_nearfield_analyze.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/example_eo_03_multi_objective.py` & `pygdm2-1.1.6/examples/03_evolutionary_optimization/example_eo_03_multi_objective.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/example_eo_03b_multi_objective_analyze.py` & `pygdm2-1.1.6/examples/03_evolutionary_optimization/example_eo_03b_multi_objective_analyze.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_01_eo.py` & `pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_01_eo.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_02_eo_load_final.py` & `pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_02_eo_load_final.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_03_eo_continue_optimization.py` & `pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_03_eo_continue_optimization.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_04_ownproblem.py` & `pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_04_ownproblem.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_04b_ownproblem_analyze.py` & `pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_04b_ownproblem_analyze.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_05_ownmodel.py` & `pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_05_ownmodel.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_05b_ownmodel_analyze.py` & `pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_05b_ownmodel_analyze.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_06_maximize_nearfield.py` & `pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_06_maximize_nearfield.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_06b_maximize_nearfield_analyze.py` & `pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_06b_maximize_nearfield_analyze.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_07_multi_objective_problem.py` & `pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_07_multi_objective_problem.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/03_evolutionary_optimization/pagmo1_API/example_eo_07b_MO_analyze.py` & `pygdm2-1.1.6/examples/03_evolutionary_optimization/pagmo1_API/example_eo_07b_MO_analyze.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/04_tutorials/surface_plasmon.py` & `pygdm2-1.1.6/examples/04_tutorials/surface_plasmon.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/04_tutorials/surface_plasmon_gold.png` & `pygdm2-1.1.6/examples/04_tutorials/surface_plasmon_gold.png`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/04_tutorials/surface_plasmon_silicon.png` & `pygdm2-1.1.6/examples/04_tutorials/surface_plasmon_silicon.png`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/04_tutorials/using_callbacks.py` & `pygdm2-1.1.6/examples/04_tutorials/using_callbacks.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/04_tutorials/visualize_incident_field.py` & `pygdm2-1.1.6/examples/04_tutorials/visualize_incident_field.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/examples/examples.tar.gz` & `pygdm2-1.1.6/examples/examples.tar.gz`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/EO/__init__.py` & `pygdm2-1.1.6/pyGDM2/EO/__init__.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/EO/core.py` & `pygdm2-1.1.6/pyGDM2/EO/core.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/EO/models.py` & `pygdm2-1.1.6/pyGDM2/EO/models.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/EO/problems.py` & `pygdm2-1.1.6/pyGDM2/EO/problems.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/EO/tools.py` & `pygdm2-1.1.6/pyGDM2/EO/tools.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/__init__.py` & `pygdm2-1.1.6/pyGDM2/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,19 +23,20 @@
         - P.R. Wiecha (maintainer)
         - Ch. Girard
         - A. Arbouet
         - C. Majorel
         - A. Patoux
         - G. Colas des Francs
         - Y. Brûlé
+        - S. Garrigou
     
 """
 __name__ = 'pyGDM2'
-__version__ = '1.1.5.1'
-__date__ = "03/05/2024"   # MM/DD/YYY
+__version__ = '1.1.6'
+__date__ = "05/17/2024"   # MM/DD/YYY
 __author__ = 'Peter R. Wiecha'
 
 __all__ = ["core", "materials", "structures", "fields", 
            "propagators", "propagators_2D", "propagators_periodic",
            "linear", "nonlinear", 
            "tools", "visu", 
            "EO"]
```

### Comparing `pyGDM2-1.1.5.1/pyGDM2/core.py` & `pygdm2-1.1.6/pyGDM2/core.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/electron.py` & `pygdm2-1.1.6/pyGDM2/electron.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/fields/__init__.py` & `pygdm2-1.1.6/pyGDM2/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/fields/deprecated.py` & `pygdm2-1.1.6/pyGDM2/fields/deprecated.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/fields/efield_class.py` & `pygdm2-1.1.6/pyGDM2/fields/efield_class.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/fields/electron.py` & `pygdm2-1.1.6/pyGDM2/fields/electron.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/fields/focused_beams.py` & `pygdm2-1.1.6/pyGDM2/fields/focused_beams.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/fields/regular.py` & `pygdm2-1.1.6/pyGDM2/fields/regular.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/linear.py` & `pygdm2-1.1.6/pyGDM2/linear.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/materials.py` & `pygdm2-1.1.6/pyGDM2/materials.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/multipole/__init__.py` & `pygdm2-1.1.6/pyGDM2/multipole/__init__.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/multipole/main.py` & `pygdm2-1.1.6/pyGDM2/multipole/main.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/multipole/polarizabilities.py` & `pygdm2-1.1.6/pyGDM2/multipole/polarizabilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -667,15 +667,15 @@
     qm = np.array([np.sum(np.matmul(K_QM_E[...,i,:,:], E0[:,:,None]), axis=(0,2)) for i in range(3)])
     
     return qm
 
 
 def extract_effective_polarizability(sim, method='lu',
                                      which_moments=['p1','m'], long_wavelength_approx=True,
-                                     illumination_mode='dipole', npoints=25, r_sphere=1000,
+                                     illumination_mode='dipole', npoints=10, r_sphere=5000,
                                      store_simulation_object=False):
     """Extract effective electric and magnetic dipole polarizability for structure
     
     solve inverse problem of adjusting polarizability for different illuminations
     via pseudoinverse
     
     *doc to be completed*
@@ -689,15 +689,15 @@
     """
     from pyGDM2 import fields
     from pyGDM2 import tools
     from scipy import linalg
     
     def sample_spherical(npoints, ndim=3):
         """random pos. on sphere (R=1). from: https://stackoverflow.com/questions/33976911"""
-        vec = np.random.randn(ndim, npoints)
+        vec = np.random.randn(ndim, npoints) - 0.5
         vec /= np.linalg.norm(vec, axis=0)
         return vec
 
     ## dipoles of random position and random orientation
     wavelengths = sim.efield.wavelengths
     
     r0 = np.average(sim.struct.geometry, axis=0)
```

### Comparing `pyGDM2-1.1.5.1/pyGDM2/multipole/processing.py` & `pygdm2-1.1.6/pyGDM2/multipole/processing.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/multipole/propagators.py` & `pygdm2-1.1.6/pyGDM2/multipole/propagators.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/nonlinear.py` & `pygdm2-1.1.6/pyGDM2/nonlinear.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/propagators/__init__.py` & `pygdm2-1.1.6/pyGDM2/propagators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/propagators/propagators.py` & `pygdm2-1.1.6/pyGDM2/propagators/propagators.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/propagators/propagators_2D.py` & `pygdm2-1.1.6/pyGDM2/propagators/propagators_2D.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/propagators/propagators_periodic.py` & `pygdm2-1.1.6/pyGDM2/propagators/propagators_periodic.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/propagators/propagators_periodic_slow.py` & `pygdm2-1.1.6/pyGDM2/propagators/propagators_periodic_slow.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/structures.py` & `pygdm2-1.1.6/pyGDM2/structures.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2/tools.py` & `pygdm2-1.1.6/pyGDM2/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -922,14 +922,34 @@
     
     else:
         raise Exception("Got no valid structure data.")
     
     return step
 
 
+def get_enclosing_sphere_radius(struct):
+    from pyGDM2 import structures
+    
+    ## coordinate list
+    if type(struct) in [list, np.ndarray]:
+        from scipy.spatial import distance
+        geometry = get_geometry(struct, return_type='tuples')
+    
+    r0 = np.mean(geometry, axis=0)
+    step = get_step_from_geometry(geometry)
+
+    geo_center_abs = np.abs(geometry - r0)
+    geo_origin_abs = geo_center_abs - np.min(geo_center_abs, dim=0)[None,0]
+    dist_to_origin = np.linalg.norm(geo_origin_abs, dim=1)
+    dist_to_edge = np.max(dist_to_origin) + step
+
+    return dist_to_edge
+
+        
+
 def get_mesh_from_geometry(geo, N_try=20, warn=True, verbose=0):
     """Try to identify the mesh type from the dipole positions
     
     If meshpoint determination fails, falling back to `cube`
     
     
     Parameters
@@ -2221,16 +2241,16 @@
                                                 ivalues]), NX, NY)
     return NF_MAP, extent
 
 
 
 
 
-def adapt_map_to_structure_mesh(mapping, structure, projection=None,
-                                min_dist=1.1,
+def adapt_map_to_structure_mesh(mapping, structure, projection="xy",
+                                min_dist=0.61,
                                 occupy_all_geo_positions=False, verbose=False):
     """changes the positions of mapping coordinates close to structure meshpoints
     
     All coordinates closer than a minimum (e.g. the stepsize) to a meshpoint 
     of the nanostructure are replaced by the position of the closest meshpoint.
     Optionally all meshpoint positions can be added to the mapping.
     
@@ -2239,19 +2259,20 @@
     mapping : list of 3-tuples
         list containing the mapping coordinates. 
     
     structure : list of coordinate 3-tuples or :class:`.core.simulation`
         instance of object containing the mapping information. Accepts list 
         of coordinate tuples or instance of :class:`.core.simulation`
     
-    projection : str, default: None
+    projection : str, default: "xy"
         consider some geometric projection. possible values: ['XY', 'XZ', 'YZ', None]
         if None: use closest meshpoint no matter which direction in space. If 
         one of the strings, only consider meshpoints in the same plane as the mapping
         coordinates.
+        Defaults to "XY", since the electron beam direction is by default along Z.
         
     min_dist : float, default: 1.5
         minimum distance to meshpoints in units of stepsize
     
     occupy_all_geo_positions : bool, default: False
         if true and a planar mapping or a specific projection is chosen, 
         all positions in the geometry-mesh plane closest to the scan-height will 
@@ -2277,15 +2298,15 @@
         raise Exception("It seems scipy is not installed. Scipy is required " +
                         "by `nearfield` for detecting internal field positions. " +
                         "Please install scipy >=v0.17, or set `val_inside_struct`=None.")
     import time
 
     ## --- check the mapping data
     if len(np.shape(mapping)) == 1:
-        if len(mapping) == 3:
+        if len(mapping) == 3:  # single position
             mapping = np.array([[mapping[0], mapping[1], mapping[2]]])
         else: 
             raise ValueError("If 'mapping' is tuple, must consist of *exactly* 3 elements!")
     elif len(np.shape(mapping)) == 2:
         if np.shape(mapping)[1] != 3:
             raise ValueError("'mapping' must consist of 3-tuples!")
     else:
@@ -2298,19 +2319,19 @@
             projection = 'yz'
         elif  len(np.unique(r_probe.T[1]))==1:
             projection = 'xz'
         elif  len(np.unique(r_probe.T[2]))==1:
             projection = 'xy'
     
     if projection.lower() == 'xz':
-        projection = 1
+        projection = 1; dim_idx = [0, 2]
     elif projection.lower() == 'xy':
-        projection = 2
+        projection = 2; dim_idx = [0, 1]
     elif projection.lower() == 'yz':
-        projection = 0
+        projection = 0; dim_idx = [1, 2]
     elif projection != 99:
         raise ValueError("'projection' must be one of [None, 'XZ', 'XY', 'YZ'].")
     
     ## --- get stepsize and structure coordinates
     step = get_step_from_geometry(structure)
     geo = get_geometry(structure).copy().T
     
@@ -2331,18 +2352,18 @@
     else:
         scan_levels = np.unique(r_probe.T[projection])
         for lvl in scan_levels:
             lvl_indices = r_probe.T[projection]==lvl
             for i, R in enumerate(r_probe[lvl_indices]):
                 new_r_probe.append(R)
                 ## check if meshpoint is too close
-                dist_list = norm(geo - R, axis=1)
+                dist_list = norm(geo[:,dim_idx] - R[dim_idx], axis=1)
                 idcs_min_dist = np.argsort(dist_list)
                 if abs(dist_list[idcs_min_dist[0]]) <= min_dist*step:
-                    new_r_probe[-1] = geo[idcs_min_dist[0]].copy()
+                    new_r_probe[-1][dim_idx] = geo[idcs_min_dist[0], dim_idx].copy()
                     new_r_probe[-1][projection] = lvl
         if occupy_all_geo_positions:
             ## for every 'height' level in mapping, add full geometry plane closest to that level
             unique_geo_planes = np.unique(geo.T[projection])
             for lvl in scan_levels:
                 closest_geo_plane_lvl = unique_geo_planes[np.argmin(np.abs(unique_geo_planes-lvl))]
                 _geo_lvl = geo.copy()[geo.T[projection]==closest_geo_plane_lvl]
```

### Comparing `pyGDM2-1.1.5.1/pyGDM2/visu.py` & `pygdm2-1.1.6/pyGDM2/visu.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,15 +77,25 @@
             print("2dstep= {:.1f}, distsum={:.2f} --> mesh: '{}'".format(step2d, distsum, meshtype))
     except KeyError:
         warnings.warn("Mesh not detected, falling back to 'cubic'.")
         meshtype = 'cube'
     
     return meshtype
         
+        
+def _get_axis_existing_or_new():
+    import matplotlib.pyplot as plt
 
+    if len(plt.get_fignums()) == 0:
+        show = True
+        ax = plt.subplot()
+    else:
+        show = False
+        ax = plt.gca()
+    return ax, show
 
 
 
 
 ########################################################################
 ##                      VISUALIZATION FUNCTIONS
 ########################################################################
@@ -248,220 +258,302 @@
         plt.show()
     
     return im
 
 
 
 
-def structure_contour(struct, projection='auto', color='k', 
-                      N_points=4, borders=3, lw=1, s=5, style='lines', 
-                      input_mesh='auto', tit='', ax=None,
-                      add_first_point=True, show=True, **kwargs):
-    """Contour around structure
+def enlarge_struct_geometry(geometry, enlargement, axis1=0, axis2=1, version='colinear'):
+    """ Create fake dipoles shifted by enlargement 
     
-    further kwargs are passed to matplotlib's  `scatter` or `plot`
+    Shift in the +/- axis1 direction and +/- axis2 direction. 
+    Version 'colinear' is a colinear shift (along axis), 
+    Version 'diagonal' is diagonal shift. Subroutine for structure_contour_smooth
+    """
+    add_geo1 = np.copy(geometry)
+    add_geo2 = np.copy(geometry)
+    add_geo3 = np.copy(geometry)
+    add_geo4 = np.copy(geometry)
+    if version == 'colinear' :
+        add_geo1[:,axis1] += enlargement
+        add_geo2[:,axis1] -= enlargement
+        add_geo3[:,axis2] += enlargement
+        add_geo4[:,axis2] -= enlargement
+    if version == 'diagonal' :
+        add_geo1[:,axis1] += enlargement
+        add_geo2[:,axis1] += enlargement
+        add_geo3[:,axis1] -= enlargement
+        add_geo4[:,axis1] -= enlargement
+        add_geo1[:,axis2] += enlargement
+        add_geo2[:,axis2] -= enlargement
+        add_geo3[:,axis2] += enlargement
+        add_geo4[:,axis2] -= enlargement
+
+    enlarged_geo = np.concatenate((geometry,add_geo1,add_geo2,add_geo3,add_geo4),axis=0)
+    return enlarged_geo
+
+def alpha_shape(points, alpha, only_outer=True):
+    """
+    Compute the alpha shape (concave hull) of a set of points.
+    :param points: np.array of shape (n,2) points.
+    :param alpha: alpha value.
+    :param only_outer: boolean value to specify if we keep only the outer border
+    or also inner edges.
+    :return: set of (i,j) pairs representing edges of the alpha-shape. (i,j) are
+    the indices in the points array.
+    from : https://karobben.github.io/2022/03/07/Python/point_outline/
+    """
+    from scipy.spatial import Delaunay
+    assert points.shape[0] > 3, "Need at least four points"
+    def add_edge(edges, i, j):
+        """
+        Add an edge between the i-th and j-th points,
+        if not in the list already
+        """
+        if (i, j) in edges or (j, i) in edges:
+            # already added
+            assert (j, i) in edges, "Can't go twice over same directed edge right?"
+            if only_outer:
+                # if both neighboring triangles are in shape, it's not a boundary edge
+                edges.remove((j, i))
+            return
+        edges.add((i, j))
+    tri = Delaunay(points)
+    edges = set()
+    # Loop over triangles:
+    # ia, ib, ic = indices of corner points of the triangle
+    for ia, ib, ic in tri.simplices:
+        pa = points[ia]
+        pb = points[ib]
+        pc = points[ic]
+        # Computing radius of triangle circumcircle
+        # www.mathalino.com/reviewer/derivation-of-formulas/derivation-of-formula-for-radius-of-circumcircle
+        a = np.sqrt((pa[0] - pb[0]) ** 2 + (pa[1] - pb[1]) ** 2)
+        b = np.sqrt((pb[0] - pc[0]) ** 2 + (pb[1] - pc[1]) ** 2)
+        c = np.sqrt((pc[0] - pa[0]) ** 2 + (pc[1] - pa[1]) ** 2)
+        s = (a + b + c) / 2.0
+        area = np.sqrt(s * (s - a) * (s - b) * (s - c))
+        circum_r = a * b * c / (4.0 * area)
+        if circum_r < alpha:
+            add_edge(edges, ia, ib)
+            add_edge(edges, ib, ic)
+            add_edge(edges, ic, ia)
+    return edges
+
+
+def structure_contour_old(struct, r_contour=1, projection='auto', color='k',
+                             borders=3, lw=1, tit='', ax=None, show=True, 
+                             split=False, split_axis='x', split_value=0, 
+                             phys_accurate=False, phys_enlarge_vers='colinear',
+                             **kwargs):
+    """Contour around structure via alpha shape
+    
+    Contour is smoothed by drawing outer line of 2D projection.
+    All further kwargs are passed to matplotlib's `ax.plot`.
+    
+    Contributed by Simon Garrigou.
     
     Parameters
     ----------
-    struct : list or :class:`.core.simulation`
-          either list of 3d coordinate tuples or simulation description object
-          
+    struct : list or :class:`.core.simulation` 
+        either list of 3d coordinate tuples or simulation description object
+    
     projection : str, default: 'auto'
         which 2D projection to plot: "auto", "XY", "YZ", "XZ"
-          
+    
+    r_contour : float, default=1
+        radius for contour computation : higher = smoother but can go over gaps sometimes
+
     color : str or matplotlib color, default: "b"
-          matplotlib-compatible color for scatter
-      
-    N_points : int, default: 4
-          number of additional points to calculate at each meshpoint-side 
-          (basically meant for style "dots", default: 4)
-      
+        matplotlib-compatible color for scatter
+
     borders : float, default: 3
-          additional space limits around plot in units of stepsize
-      
-    lw : float, default: 1
-          linewidth as used by `pyplot.plot` (style='lines' only)
-         
-    s : float, default: 5
-          symbol scaling for scatterplot as used by `pyplot.scatter` 
-          (style='dots' only)
-         
-    stlye : str, default: 'lines'
-          Style of plot. One of ["dots", "lines"]
-          
-    input_mesh : str, default: 'auto'
-          mesh type, default: "auto" (try to infer meshtype from geometry).
-          one of ["auto", "cube", "hex", "hex2", "hex_onelayer1", "hex_onelayer2"]
+        additional space limits around plot in units of stepsize
     
+    lw : float, default: 1
+        linewidth as used by `pyplot.plot` (style='lines' only)
+        
     tit : str, default: ""
         title for plot (optional)
     
     ax : matplotlib `axes`, default: None (=create new)
-           axes object (matplotlib) to plot into
+        axes object (matplotlib) to plot into
     
-    add_first_point : bool, default: True
-          If True, adds first point twice in order to close the contour. 
-          Might cause some strange lines if a single edge meshpoint is first in 
-          the geometry.
-      
     show : bool, default: True
-          directly show plot
-          
-    Returns
-    -------
-    matplotlib's `scatter` or `line` return value : 
-        contour plot object
-    
+        directly show plot
+
+    split : bool, default : False 
+        choice to split the structure in two sub-structures along an axis, 
+        contour for each structure is plotted then
+        
+    split_axis : str, default: 'x'
+        axis for the structure split (among 'x', 'y', 'z')
+        
+    split_value : float, default : 0
+        Position on the axis of the splitting plane
+
+    phys_accurate : bool, default : False
+        Enlarge structure to take in account the physical meaning of 
+        the discretization cell, Working only for cubic for now.
+        
+    phys_enlarge_vers : str, default : 'colinear'
+        'colinear' or 'diagonal' for the artificial enlargement 
+        procedure, will play at the corners    
     """
+    geo = tools.get_geometry(struct)
+    step = tools.get_step_from_geometry(struct)
+
+    if phys_accurate:
+        geo
+
     if ax is None:
         ax = plt.gca()
-    
-    if N_points<2:
-        raise ValueError("'N_points' must be >= 2!")
-    
-    geo = tools.get_geometry(struct)
+
     if projection.lower() == 'auto':
         projection = _automatic_projection_select(*geo)
+
     struct2D = tools.get_geometry_2d_projection(struct, projection=projection)
-    struct2D = np.round(struct2D, 5)
-    
-    ## get meshtype
-    if input_mesh.lower() == 'auto':
-        input_mesh = _automatic_mesh_detect_2D(struct2D)
-    
-    
-    if input_mesh.lower() == 'cube':
-        NN_bulk, mb = 4, 1.1
-        NN_sf = 4
-    elif input_mesh.lower() in ['hex', 'hex1']:
-        NN_bulk, mb = 3, np.sqrt(2)
-        NN_sf = 3
-    elif input_mesh.lower() == 'hex2':
-        NN_bulk, mb = 4, np.sqrt(1.3)
-        NN_sf = 4
-    elif input_mesh.lower() == 'hex3':
-        NN_bulk, mb = 4, 1.7
-        NN_sf = 4
-    elif input_mesh.lower() in ['hex_onelayer1']:
-        NN_bulk, mb = 3, np.sqrt(1)
-        NN_sf = 6
-    elif input_mesh.lower() in ['hex_onelayer2', 'hex_onelayer']:
-        NN_bulk, mb = 6, 2
-        NN_sf = 2
-    SF, SF_vec = tools.get_surface_meshpoints(struct2D, NN_bulk=NN_bulk, max_bound=mb,
-                                              NN_surface=NN_sf, max_bound_sf=5.0)
-    
-    step = tools.get_step_from_geometry(struct)
-    d = step/2.
-    if input_mesh.lower() in ['hex', 'hex1', 'hex2', 'hex3']:
-        d /= 2.#np.sqrt(2)
-    if input_mesh.lower() in ['hex_onelayer1', 'hex_onelayer2']:
-        d /= 2.
-    
-    if projection.lower() == 'xy':
-        coord_idx = [0,1]
-    elif projection.lower() == 'yz':
-        coord_idx = [1,2]
-    elif projection.lower() == 'xz':
-        coord_idx = [0,2]
-    
-    ## --- calculate the contour-pixel positions
-    SF_plot = []
-    for i, vec in enumerate(SF_vec):
-        x, y = SF[i][coord_idx]
-#==============================================================================
-#         CUBE MESH
-#==============================================================================
-        if input_mesh.lower() == 'cube':
-            if round(vec[coord_idx[0]]) != 0:
-                for i in range(N_points):
-                    SF_plot.append([x + np.sign(vec[coord_idx[0]])*d, 
-                                    y-d + d*i/((N_points-1)/2.)])
-            
-            if round(vec[coord_idx[1]]) != 0:
-                    for i in range(N_points):
-                        SF_plot.append([x-d + d*i/((N_points-1)/2.), 
-                                        y + np.sign(vec[coord_idx[1]])*d])
-#==============================================================================
-#         HEXAGONAL MESH
-#==============================================================================
-        if input_mesh.lower() in ['hex', 'hex1', 'hex2', 'hex3', 'hex_onelayer1', 'hex_onelayer2']:
-            SF_plot.append([x + d*vec[coord_idx[0]], 
-                            y + d*vec[coord_idx[1]]])
-    if len(SF_plot)==0:
-        raise ValueError("Empty surface data! Please check mesh-type (parameter `input_mesh`) and input structure data.")
-    X, Y = tools.unique_rows(np.array(SF_plot)).T
-    
-    ## --- plot as scatter
-    if style.lower() == 'dots':
-        cont = ax.scatter(X, Y, color=color, s=s, **kwargs)
-    
-    ## --- plot as lines
-    elif style.lower() == 'lines':
-        from scipy.spatial import cKDTree as KDTree
-        geometry_line = np.transpose([X, Y])
-        
-        ## sort coordinates such, that each point follows a closest neighbor
-        i_pos = 0
-        ordered_list = [ [geometry_line[i_pos]] ]
-        for i in range(len(geometry_line)-1):
-            pos = geometry_line[i_pos]
-            
-            ## query for nearest neighbor (exclude "self-position")
-            kdtree = KDTree(geometry_line)
-            closest = kdtree.query(pos, k=2)
-            idx_closest = closest[1][1]
-            
-            ## stop if no next neighbour found
-            if idx_closest >= len(geometry_line):
-                break
-            
-            ## if separate structure detected: start new list for contour-line
-            min_dist_fact = 0.9
-            if input_mesh.lower() in ['hex', 'hex1', 'hex2', 'hex3', 'hex_onelayer1', 'hex_onelayer2']:
-                min_dist_fact = 1.42
-            if closest[0][1] > step*1.4*min_dist_fact:
-                ordered_list[-1].append(ordered_list[-1][0])
-                ordered_list.append([])
-            
-            ordered_list[-1].append(geometry_line[idx_closest])
-            geometry_line = np.delete(geometry_line, i_pos, 0)
-            
-            if i_pos < idx_closest:
-                idx_closest -= 1
-            i_pos = idx_closest
-        
-        ordered_list[-1].append(geometry_line[0])  # add last remaining point
-        if add_first_point:
-            ordered_list[-1].append(ordered_list[-1][0])  # add first point to close the loop
-        
-        ## --- plot all contours
-        for sub_struct in ordered_list:
-            Xs, Ys = np.transpose(sub_struct)
-            cont = ax.plot(Xs,Ys, color=color, lw=lw, **kwargs)
-            
-    else:
-        raise ValueError("`style` must be one of ['dots', 'lines']")
-       
+    struct2D = np.round(struct2D, 5)[:,0:2]
+
+    if split : # split the structure along plane orthogonal to split_axis at split_value position
+        struct1 = copy.deepcopy(struct)
+        struct2 = copy.deepcopy(struct)
+        
+        if split_axis=='x' : 
+            ind = 0
+        elif split_axis=='y' : 
+            ind = 1
+        elif split_axis=='z' : 
+            ind = 2
+        else : print("Warning, wrong splitting axis value, must be among 'x','y','z'")
+        separation_list_geo1 = []
+        separation_list_geo2 = []
+        for ipos,pos in enumerate(geo.T) : 
+            if pos[ind]<split_value :
+                separation_list_geo2.append(ipos)
+            else : 
+                separation_list_geo1.append(ipos)
+    
+        struct1.geometry = np.delete(geo.T, separation_list_geo1,0)
+        struct2.geometry = np.delete(geo.T, separation_list_geo2,0)
+
+        if projection.lower() == 'auto':
+            projection = _automatic_projection_select(*geo)
+
+        if phys_accurate : 
+            if projection.lower() == 'xy':
+                ind1, ind2 = 0,1
+            elif projection.lower() == 'yz':
+                ind1, ind2 = 1,2
+            elif projection.lower() == 'xz':
+                ind1, ind2 = 0,2
+
+            struct1.geometry = enlarge_struct_geometry(struct1.geometry, step/2, ind1,ind2,version=phys_enlarge_vers)
+            struct2.geometry = enlarge_struct_geometry(struct2.geometry, step/2, ind1,ind2,version=phys_enlarge_vers)
+
+        struct2D1 = tools.get_geometry_2d_projection(struct1, projection=projection) #needs struct object to work, hence the copy procedure + replacement of each geometry
+        struct2D2 = tools.get_geometry_2d_projection(struct2, projection=projection)
+        struct2D1 = np.round(struct2D1, 5)[:,0:2]
+        struct2D2 = np.round(struct2D2, 5)[:,0:2]
+
+        edges1 = alpha_shape(struct2D1, alpha=r_contour, only_outer=True)
+        edges2 = alpha_shape(struct2D2, alpha=r_contour, only_outer=True)
+
+        # --- plot the contours
+        plt.gca().set_aspect('equal')
+        for i, j in edges1:
+            ax.plot(struct2D1[[i, j], 0], struct2D1[[i, j], 1],color=color,lw=lw)
+        for i, j in edges2:
+            ax.plot(struct2D2[[i, j], 0], struct2D2[[i, j], 1],color=color,lw=lw)
+
+    else : 
+        if phys_accurate : 
+            struct1 = copy.deepcopy(struct)
+            if projection.lower() == 'xy':
+                ind1, ind2 = 0,1
+            elif projection.lower() == 'yz':
+                ind1, ind2 = 1,2
+            elif projection.lower() == 'xz':
+                ind1, ind2 = 0,2
+            struct1.geometry = enlarge_struct_geometry(struct1.geometry, step/2, ind1,ind2,version=phys_enlarge_vers)
+            struct2D = tools.get_geometry_2d_projection(struct1, projection=projection)
+            struct2D = np.round(struct2D, 5)[:,0:2]
+
+        edges = alpha_shape(struct2D, alpha=r_contour, only_outer=True)
+        ## --- plot the contours
+        plt.gca().set_aspect('equal')
+        for i, j in edges:
+            cont = ax.plot(struct2D[[i, j], 0], struct2D[[i, j], 1], color=color, lw=lw, **kwargs)
+
     if tit:
         ax.set_title(tit)
-        
+
+    X = struct2D[:,0]
+    Y = struct2D[:,1]
     if show: 
         ax.set_aspect("equal")
         ax.set_xlabel("{} (nm)".format(projection[0]))
         ax.set_ylabel("{} (nm)".format(projection[1]))
         ax.set_xlim(X.min()-borders*step, X.max()+borders*step)
         ax.set_ylim(Y.min()-borders*step, Y.max()+borders*step)
-    
         plt.show()
     
     return cont
     
 
 
+def structure_contour(struct, r_contour=1, projection='auto', color='k',
+                            alpha_value=0.05, borders=3, lw=1, alpha=1.0,tit='',
+                            set_ax_aspect=True, 
+                            **kwargs):
+
+    import alphashape
+    
+    geo = tools.get_geometry(struct)
+    step = tools.get_step_from_geometry(struct)
+
+    # prep
+    ax, show = _get_axis_existing_or_new()
+    if "show" in kwargs:
+        show = kwargs.pop("show")
+    if set_ax_aspect:
+        ax.set_aspect("equal")
+
+    # get geometry projection
+    if projection.lower() == "auto":
+        projection = _automatic_projection_select(*geo)
+    
+    pos_proj = tools.get_geometry_2d_projection(struct, projection=projection)
+    pos_proj = np.round(pos_proj, 5)[:,:2]
+    
+
+    # expand geometry by a half-step (outer points)
+    pos_px = pos_proj + np.array([[step / 2, step / 2]])
+    pos_mx = pos_proj + np.array([[-step / 2, step / 2]])
+    pos_py = pos_proj + np.array([[step / 2, -step / 2]])
+    pos_my = pos_proj + np.array([[-step / 2, -step / 2]])
+    pos2d_exp = np.concatenate([pos_px, pos_mx, pos_py, pos_my])
+
+    # concave hull (alpha shape)
+    alpha_shape = alphashape.alphashape(pos2d_exp, alpha_value)
+    xx, yy = alpha_shape.exterior.coords.xy
+    xx, yy = xx.tolist(), yy.tolist()
+
+    # plot
+    ax.plot(xx, yy, color=color, alpha=alpha, **kwargs)
+    ax.autoscale(tight=False)
+    ax.set_xlabel("{} (nm)".format(projection[0]))
+    ax.set_ylabel("{} (nm)".format(projection[1]))
+    if tit:
+        plt.title(tit)
+    if show:
+        plt.show()
+    else:
+        return ax
+
 ##----------------------------------------------------------------------
 ##                     INTERNAL FIELD - FUNDAMENTAL
 ##----------------------------------------------------------------------
 def vectorfield(NF, struct=None, projection='auto', complex_part='real', 
                 tit='',
                 slice_level=None,
                 scale=10.0, vecwidth=1.0, cmap=cm.Blues, cmin=0.3,
```

### Comparing `pyGDM2-1.1.5.1/pyGDM2/visu3d.py` & `pygdm2-1.1.6/pyGDM2/visu3d.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/pyGDM2.egg-info/PKG-INFO` & `pygdm2-1.1.6/pyGDM2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: pyGDM2
-Version: 1.1.5.1
+Version: 1.1.6
 Summary: A python full-field electrodynamical solver, based on the Green dyadic method (volume integral technique in frequency domain).
 Home-page: https://gitlab.com/wiechapeter/pyGDM2
+Download-URL: 
 Author: Peter R. Wiecha
 Author-email: pwiecha@laas.fr
 License: GPLv3+
 Keywords: coupled dipoles method,green dyadic method,electrodynamical simulations,nano optics,frequency-domain
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7
 License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: numba
 
 ***********************************
 Requirements / Installation
 ***********************************
 
 pyGDM is an open source python toolkit for electro-dynamical simulations, implementing the `Green dyadic method (GDM) <https://doi.org/10.1088/0034-4885/68/8/R05>`_, a volume discretization technique. 
 pyGDM is based on simulation codes and theoretical models developed over the past 20 years by `Christian Girard <http://www.cemes.fr/Theory-of-Complex-Nano-optical?lang=en>`_ at CEMES (see e.g. `Ch. Girard 2005 Rep. Prog. Phys. 68 1883 <https://doi.org/10.1088/0034-4885/68/8/R05>`_), with contributions from G. Colas des Francs, A. Arbouet, R. Marty, C. Majorel, A. Patoux, Y. Brûlé and P.R. Wiecha.
@@ -148,9 +150,7 @@
    - P\. R. Wiecha
 
 
 
    
 
 
-
-
```

### Comparing `pyGDM2-1.1.5.1/pyGDM2.egg-info/SOURCES.txt` & `pygdm2-1.1.6/pyGDM2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/tests/basic_tests.py` & `pygdm2-1.1.6/tests/basic_tests.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.5.1/tests/tests_propagators.py` & `pygdm2-1.1.6/tests/tests_propagators.py`

 * *Files identical despite different names*

