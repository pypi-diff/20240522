# Comparing `tmp/cotengra-0.6.1.tar.gz` & `tmp/cotengra-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cotengra-0.6.1.tar", last modified: Wed May 15 21:37:34 2024, max compression
+gzip compressed data, was "cotengra-0.6.2.tar", last modified: Wed May 22 00:54:32 2024, max compression
```

## Comparing `cotengra-0.6.1.tar` & `cotengra-0.6.2.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.467719 cotengra-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-15 21:37:22.000000 cotengra-0.6.1/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.427719 cotengra-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.431719 cotengra-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-15 21:37:22.000000 cotengra-0.6.1/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-15 21:37:22.000000 cotengra-0.6.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-15 21:37:22.000000 cotengra-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-15 21:37:22.000000 cotengra-0.6.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-15 21:37:22.000000 cotengra-0.6.1/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-15 21:37:22.000000 cotengra-0.6.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-15 21:37:22.000000 cotengra-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-15 21:37:34.467719 cotengra-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-15 21:37:22.000000 cotengra-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.427719 cotengra-0.6.1/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.435719 cotengra-0.6.1/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-15 21:37:22.000000 cotengra-0.6.1/ci/requirements/py-base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-15 21:37:22.000000 cotengra-0.6.1/ci/requirements/py-mac.yml
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-15 21:37:22.000000 cotengra-0.6.1/ci/requirements/py-no-oe.yml
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-15 21:37:22.000000 cotengra-0.6.1/ci/requirements/py-win.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.435719 cotengra-0.6.1/cotengra/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 21:37:34.000000 cotengra-0.6.1/cotengra/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    28858 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)   132859 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8286 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/core_multi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.439719 cotengra-0.6.1/cotengra/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15899 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/experimental/path_compressed_branchbound.py
--rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/experimental/path_compressed_mcts.py
--rw-r--r--   0 runner    (1001) docker     (127)    28097 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/hypergraph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.439719 cotengra-0.6.1/cotengra/hyperoptimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/hyperoptimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41260 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/hyperoptimizers/hyper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/hyperoptimizers/hyper_baytune.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/hyperoptimizers/hyper_choco.py
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/hyperoptimizers/hyper_nevergrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/hyperoptimizers/hyper_optuna.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/hyperoptimizers/hyper_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/hyperoptimizers/hyper_skopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    33562 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/oe.py
--rw-r--r--   0 runner    (1001) docker     (127)    15256 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.439719 cotengra-0.6.1/cotengra/pathfinders/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.443719 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/cut_kKaHyPar_sea20.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/cut_rKaHyPar_sea20.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/km1_kKaHyPar_sea20.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/km1_rKaHyPar_sea20.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.443719 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/old/
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/old/cut_kKaHyPar_sea20.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/old/cut_rKaHyPar_sea20.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/old/km1_kKaHyPar_sea20.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/old/km1_rKaHyPar_sea20.ini
--rw-r--r--   0 runner    (1001) docker     (127)    48385 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12996 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_compressed.py
--rw-r--r--   0 runner    (1001) docker     (127)    18038 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_compressed_greedy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_flowcutter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_greedy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_igraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_kahypar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_quickbb.py
--rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/path_simulated_annealing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/pathfinders/treedecomp.py
--rw-r--r--   0 runner    (1001) docker     (127)    51499 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    48584 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/schematic.py
--rw-r--r--   0 runner    (1001) docker     (127)    28660 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)    41222 2024-05-15 21:37:22.000000 cotengra-0.6.1/cotengra/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.463719 cotengra-0.6.1/cotengra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-15 21:37:34.000000 cotengra-0.6.1/cotengra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-15 21:37:34.000000 cotengra-0.6.1/cotengra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 21:37:34.000000 cotengra-0.6.1/cotengra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-15 21:37:34.000000 cotengra-0.6.1/cotengra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 21:37:34.000000 cotengra-0.6.1/cotengra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.447719 cotengra-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.447719 cotengra-0.6.1/docs/_pygments/
--rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/_pygments/_pygments_dark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/_pygments/_pygments_light.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.447719 cotengra-0.6.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/_static/logo-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    22713 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/_static/logo-full.png
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/_static/my-styles.css
--rw-r--r--   0 runner    (1001) docker     (127)    21837 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/advanced.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    77146 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/basics.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)   596952 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/contraction.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.451719 cotengra-0.6.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)  2748603 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/examples/ex_compressed_contraction.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   871844 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/examples/ex_large_output_lazy.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   318454 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/high-level-interface.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/index_examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)   324466 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/trees.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1311527 2024-05-15 21:37:22.000000 cotengra-0.6.1/docs/visualization.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.463719 cotengra-0.6.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)  1627407 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/Example - Reproducing 2005.06787.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1635278 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/Example - Reproducing 2103-03074.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1892297 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/Quantum Circuit Example Old.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1598303 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/Quantum Circuit Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    42045 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/circuit_n53_m10_s0_e0_pABCDCDAB.qsim
--rw-r--r--   0 runner    (1001) docker     (127)    50412 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/circuit_n53_m12_s0_e0_pABCDCDAB.qsim
--rw-r--r--   0 runner    (1001) docker     (127)    83874 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/circuit_n53_m20_s0_e0_pABCDCDAB.qsim
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/ex_jax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/ex_mpi_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-15 21:37:22.000000 cotengra-0.6.1/examples/ex_mpi_spmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-15 21:37:22.000000 cotengra-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 21:37:34.467719 cotengra-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-15 21:37:22.000000 cotengra-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.463719 cotengra-0.6.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)    28953 2024-05-15 21:37:22.000000 cotengra-0.6.1/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:34.463719 cotengra-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 21:37:22.000000 cotengra-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-15 21:37:22.000000 cotengra-0.6.1/tests/test_compressed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-05-15 21:37:22.000000 cotengra-0.6.1/tests/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-15 21:37:22.000000 cotengra-0.6.1/tests/test_hypergraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-15 21:37:22.000000 cotengra-0.6.1/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-05-15 21:37:22.000000 cotengra-0.6.1/tests/test_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-15 21:37:22.000000 cotengra-0.6.1/tests/test_paths_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-15 21:37:22.000000 cotengra-0.6.1/tests/test_slicer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-15 21:37:22.000000 cotengra-0.6.1/tests/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.842135 cotengra-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-22 00:54:20.000000 cotengra-0.6.2/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.802135 cotengra-0.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.806135 cotengra-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-22 00:54:20.000000 cotengra-0.6.2/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-22 00:54:20.000000 cotengra-0.6.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-22 00:54:20.000000 cotengra-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 00:54:20.000000 cotengra-0.6.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-22 00:54:20.000000 cotengra-0.6.2/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-22 00:54:20.000000 cotengra-0.6.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-22 00:54:20.000000 cotengra-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-22 00:54:32.842135 cotengra-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-22 00:54:20.000000 cotengra-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.802135 cotengra-0.6.2/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.806135 cotengra-0.6.2/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-22 00:54:20.000000 cotengra-0.6.2/ci/requirements/py-base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-22 00:54:20.000000 cotengra-0.6.2/ci/requirements/py-mac.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-22 00:54:20.000000 cotengra-0.6.2/ci/requirements/py-no-oe.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-22 00:54:20.000000 cotengra-0.6.2/ci/requirements/py-win.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.810135 cotengra-0.6.2/cotengra/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 00:54:32.000000 cotengra-0.6.2/cotengra/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29163 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)   133180 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8286 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/core_multi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.810135 cotengra-0.6.2/cotengra/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15899 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/experimental/path_compressed_branchbound.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/experimental/path_compressed_mcts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28097 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/hypergraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.810135 cotengra-0.6.2/cotengra/hyperoptimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/hyperoptimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41260 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/hyperoptimizers/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/hyperoptimizers/hyper_baytune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/hyperoptimizers/hyper_choco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/hyperoptimizers/hyper_nevergrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/hyperoptimizers/hyper_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/hyperoptimizers/hyper_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/hyperoptimizers/hyper_skopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33562 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/oe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15256 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.814135 cotengra-0.6.2/cotengra/pathfinders/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.814135 cotengra-0.6.2/cotengra/pathfinders/kahypar_profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/kahypar_profiles/cut_kKaHyPar_sea20.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/kahypar_profiles/cut_rKaHyPar_sea20.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/kahypar_profiles/km1_kKaHyPar_sea20.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/kahypar_profiles/km1_rKaHyPar_sea20.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.814135 cotengra-0.6.2/cotengra/pathfinders/kahypar_profiles/old/
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/kahypar_profiles/old/cut_kKaHyPar_sea20.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/kahypar_profiles/old/cut_rKaHyPar_sea20.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/kahypar_profiles/old/km1_kKaHyPar_sea20.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/kahypar_profiles/old/km1_rKaHyPar_sea20.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    48385 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/path_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12996 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/path_compressed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18038 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/path_compressed_greedy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/path_flowcutter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/path_greedy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/path_igraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/path_kahypar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/path_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/path_quickbb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/path_simulated_annealing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/pathfinders/treedecomp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51499 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48584 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/schematic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28660 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41222 2024-05-22 00:54:20.000000 cotengra-0.6.2/cotengra/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.838135 cotengra-0.6.2/cotengra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-22 00:54:32.000000 cotengra-0.6.2/cotengra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-22 00:54:32.000000 cotengra-0.6.2/cotengra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 00:54:32.000000 cotengra-0.6.2/cotengra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-22 00:54:32.000000 cotengra-0.6.2/cotengra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 00:54:32.000000 cotengra-0.6.2/cotengra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.818135 cotengra-0.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.822135 cotengra-0.6.2/docs/_pygments/
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/_pygments/_pygments_dark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/_pygments/_pygments_light.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.822135 cotengra-0.6.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/_static/logo-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    22713 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/_static/logo-full.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/_static/my-styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    21837 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/advanced.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    77146 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/basics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)   596952 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/contraction.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.826135 cotengra-0.6.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)  2748603 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/examples/ex_compressed_contraction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   871844 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/examples/ex_large_output_lazy.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   318454 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/high-level-interface.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/index_examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)   324466 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/trees.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1311527 2024-05-22 00:54:20.000000 cotengra-0.6.2/docs/visualization.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.834135 cotengra-0.6.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)  1627407 2024-05-22 00:54:20.000000 cotengra-0.6.2/examples/Example - Reproducing 2005.06787.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1635278 2024-05-22 00:54:20.000000 cotengra-0.6.2/examples/Example - Reproducing 2103-03074.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1892297 2024-05-22 00:54:20.000000 cotengra-0.6.2/examples/Quantum Circuit Example Old.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1598303 2024-05-22 00:54:20.000000 cotengra-0.6.2/examples/Quantum Circuit Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    42045 2024-05-22 00:54:20.000000 cotengra-0.6.2/examples/circuit_n53_m10_s0_e0_pABCDCDAB.qsim
+-rw-r--r--   0 runner    (1001) docker     (127)    50412 2024-05-22 00:54:20.000000 cotengra-0.6.2/examples/circuit_n53_m12_s0_e0_pABCDCDAB.qsim
+-rw-r--r--   0 runner    (1001) docker     (127)    83874 2024-05-22 00:54:20.000000 cotengra-0.6.2/examples/circuit_n53_m20_s0_e0_pABCDCDAB.qsim
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-22 00:54:20.000000 cotengra-0.6.2/examples/ex_jax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-22 00:54:20.000000 cotengra-0.6.2/examples/ex_mpi_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-22 00:54:20.000000 cotengra-0.6.2/examples/ex_mpi_spmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-22 00:54:20.000000 cotengra-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 00:54:32.842135 cotengra-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-22 00:54:20.000000 cotengra-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.834135 cotengra-0.6.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    28953 2024-05-22 00:54:20.000000 cotengra-0.6.2/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:32.838135 cotengra-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 00:54:20.000000 cotengra-0.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-22 00:54:20.000000 cotengra-0.6.2/tests/test_compressed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-05-22 00:54:20.000000 cotengra-0.6.2/tests/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-22 00:54:20.000000 cotengra-0.6.2/tests/test_hypergraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-22 00:54:20.000000 cotengra-0.6.2/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-05-22 00:54:20.000000 cotengra-0.6.2/tests/test_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-22 00:54:20.000000 cotengra-0.6.2/tests/test_paths_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-22 00:54:20.000000 cotengra-0.6.2/tests/test_slicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-22 00:54:20.000000 cotengra-0.6.2/tests/test_tree.py
```

### Comparing `cotengra-0.6.1/.github/workflows/pypi-release.yml` & `cotengra-0.6.2/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/.github/workflows/test.yml` & `cotengra-0.6.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/.gitignore` & `cotengra-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/LICENSE.md` & `cotengra-0.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/PKG-INFO` & `cotengra-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cotengra
-Version: 0.6.1
+Version: 0.6.2
 Summary: Hyper optimized contraction trees for large tensor networks and einsums.
 Home-page: https://github.com/jcmgray/cotengra
 Author: Johnnie Gray
 Author-email: johnniemcgray@gmail.com
 License: Apache
 Project-URL: Bug Reports, https://github.com/jcmgray/cotengra/issues
 Project-URL: Source, https://github.com/jcmgray/cotengra/
```

### Comparing `cotengra-0.6.1/README.md` & `cotengra-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/__init__.py` & `cotengra-0.6.2/cotengra/__init__.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/contract.py` & `cotengra-0.6.2/cotengra/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -719,16 +719,25 @@
                 implementation = "cotengra"
             else:
                 implementation = "autoray"
 
         if implementation == "cotengra":
             _einsum, _tensordot = einsum, tensordot
         elif implementation == "autoray":
-            _einsum = get_lib_fn(backend, "einsum")
-            _tensordot = get_lib_fn(backend, "tensordot")
+            try:
+                _einsum = get_lib_fn(backend, "einsum")
+            except ImportError:
+                # fallback to cotengra (matmul) implementation
+                _einsum = einsum
+
+            try:
+                _tensordot = get_lib_fn(backend, "tensordot")
+            except ImportError:
+                # fallback to cotengra (matmul) implementation
+                _tensordot = tensordot
         else:
             # manually supplied
             _einsum, _tensordot = implementation
 
         # temporary storage for intermediates
         N = len(arrays)
         temps = {
```

### Comparing `cotengra-0.6.1/cotengra/core.py` & `cotengra-0.6.2/cotengra/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,17 @@
                 self.appearances[ix] = self.appearances.get(ix, 0) + 1
         # adding output appearances ensures these are never contracted away,
         # N.B. if after this step every appearance count is exactly 2,
         # then there are no 'hyper' indices in the contraction
         for ix in self.output:
             self.appearances[ix] = self.appearances.get(ix, 0) + 1
 
-        #
+        # this stores potentialy preprocessing steps that are not part of the
+        # main contraction tree, but assumed to have been applied, for example
+        # tracing or summing over indices that appear only once
         self.preprocessing = {}
 
         # mapping of parents to children - the core binary tree object
         self.children = {}
 
         # information about all the nodes
         self.info = {}
@@ -734,14 +736,21 @@
 
     def has_preprocessing(self):
         # touch all inputs legs, since preprocessing is lazily computed
         for node in self.gen_leaves():
             self.get_legs(node)
         return bool(self.preprocessing)
 
+    def has_hyper_indices(self):
+        """Check if there are any 'hyper' indices in the contraction, i.e.
+        indices that don't appear exactly twice, when considering the inputs
+        and output.
+        """
+        return any(ix_count != 2 for ix_count in self.appearances.values())
+
     @cached_node_property("legs")
     def get_legs(self, node):
         """Get the effective 'outer' indices for the collection of tensors
         in ``node``.
         """
         node_extent = len(node)
 
@@ -791,23 +800,15 @@
     def get_can_dot(self, node):
         """Get whether this contraction can be performed as a dot product (i.e.
         with ``tensordot``), or else requires ``einsum``, as it has indices
         that don't appear exactly twice in either the inputs or the output.
         """
         l, r = self.children[node]
         sp, sl, sr = map(self.get_legs, (node, l, r))
-
-        srl_symmdiff = sl.copy()
-        for ix, ix_count in sr.items():
-            if ix in srl_symmdiff:
-                srl_symmdiff.pop(ix)
-            else:
-                srl_symmdiff[ix] = ix_count
-
-        return srl_symmdiff == sp
+        return set(sp) == set(sl).symmetric_difference(sr)
 
     @cached_node_property("inds")
     def get_inds(self, node):
         """Get the indices of this node - an ordered string version of
         ``get_legs`` that starts with ``tree.inputs`` and maintains the order
         they appear in each contraction 'ABC,abc->ABCabc', to match tensordot.
         """
```

### Comparing `cotengra-0.6.1/cotengra/core_multi.py` & `cotengra-0.6.2/cotengra/core_multi.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/experimental/path_compressed_branchbound.py` & `cotengra-0.6.2/cotengra/experimental/path_compressed_branchbound.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/experimental/path_compressed_mcts.py` & `cotengra-0.6.2/cotengra/experimental/path_compressed_mcts.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/hypergraph.py` & `cotengra-0.6.2/cotengra/hypergraph.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/hyperoptimizers/hyper.py` & `cotengra-0.6.2/cotengra/hyperoptimizers/hyper.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/hyperoptimizers/hyper_baytune.py` & `cotengra-0.6.2/cotengra/hyperoptimizers/hyper_baytune.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/hyperoptimizers/hyper_choco.py` & `cotengra-0.6.2/cotengra/hyperoptimizers/hyper_choco.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/hyperoptimizers/hyper_nevergrad.py` & `cotengra-0.6.2/cotengra/hyperoptimizers/hyper_nevergrad.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/hyperoptimizers/hyper_optuna.py` & `cotengra-0.6.2/cotengra/hyperoptimizers/hyper_optuna.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/hyperoptimizers/hyper_random.py` & `cotengra-0.6.2/cotengra/hyperoptimizers/hyper_random.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/hyperoptimizers/hyper_skopt.py` & `cotengra-0.6.2/cotengra/hyperoptimizers/hyper_skopt.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/interface.py` & `cotengra-0.6.2/cotengra/interface.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/oe.py` & `cotengra-0.6.2/cotengra/oe.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/parallel.py` & `cotengra-0.6.2/cotengra/parallel.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/cut_kKaHyPar_sea20.ini` & `cotengra-0.6.2/cotengra/pathfinders/kahypar_profiles/cut_kKaHyPar_sea20.ini`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/cut_rKaHyPar_sea20.ini` & `cotengra-0.6.2/cotengra/pathfinders/kahypar_profiles/cut_rKaHyPar_sea20.ini`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/km1_kKaHyPar_sea20.ini` & `cotengra-0.6.2/cotengra/pathfinders/kahypar_profiles/km1_kKaHyPar_sea20.ini`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/km1_rKaHyPar_sea20.ini` & `cotengra-0.6.2/cotengra/pathfinders/kahypar_profiles/km1_rKaHyPar_sea20.ini`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/old/cut_kKaHyPar_sea20.ini` & `cotengra-0.6.2/cotengra/pathfinders/kahypar_profiles/old/cut_kKaHyPar_sea20.ini`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/old/cut_rKaHyPar_sea20.ini` & `cotengra-0.6.2/cotengra/pathfinders/kahypar_profiles/old/cut_rKaHyPar_sea20.ini`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/old/km1_kKaHyPar_sea20.ini` & `cotengra-0.6.2/cotengra/pathfinders/kahypar_profiles/old/km1_kKaHyPar_sea20.ini`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/kahypar_profiles/old/km1_rKaHyPar_sea20.ini` & `cotengra-0.6.2/cotengra/pathfinders/kahypar_profiles/old/km1_rKaHyPar_sea20.ini`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/path_basic.py` & `cotengra-0.6.2/cotengra/pathfinders/path_basic.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/path_compressed.py` & `cotengra-0.6.2/cotengra/pathfinders/path_compressed.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/path_compressed_greedy.py` & `cotengra-0.6.2/cotengra/pathfinders/path_compressed_greedy.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/path_flowcutter.py` & `cotengra-0.6.2/cotengra/pathfinders/path_flowcutter.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/path_greedy.py` & `cotengra-0.6.2/cotengra/pathfinders/path_greedy.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/path_igraph.py` & `cotengra-0.6.2/cotengra/pathfinders/path_igraph.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/path_kahypar.py` & `cotengra-0.6.2/cotengra/pathfinders/path_kahypar.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/path_labels.py` & `cotengra-0.6.2/cotengra/pathfinders/path_labels.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/path_quickbb.py` & `cotengra-0.6.2/cotengra/pathfinders/path_quickbb.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/path_simulated_annealing.py` & `cotengra-0.6.2/cotengra/pathfinders/path_simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/pathfinders/treedecomp.py` & `cotengra-0.6.2/cotengra/pathfinders/treedecomp.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/plot.py` & `cotengra-0.6.2/cotengra/plot.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/presets.py` & `cotengra-0.6.2/cotengra/presets.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/schematic.py` & `cotengra-0.6.2/cotengra/schematic.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/scoring.py` & `cotengra-0.6.2/cotengra/scoring.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/slicer.py` & `cotengra-0.6.2/cotengra/slicer.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra/utils.py` & `cotengra-0.6.2/cotengra/utils.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/cotengra.egg-info/PKG-INFO` & `cotengra-0.6.2/cotengra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cotengra
-Version: 0.6.1
+Version: 0.6.2
 Summary: Hyper optimized contraction trees for large tensor networks and einsums.
 Home-page: https://github.com/jcmgray/cotengra
 Author: Johnnie Gray
 Author-email: johnniemcgray@gmail.com
 License: Apache
 Project-URL: Bug Reports, https://github.com/jcmgray/cotengra/issues
 Project-URL: Source, https://github.com/jcmgray/cotengra/
```

### Comparing `cotengra-0.6.1/cotengra.egg-info/SOURCES.txt` & `cotengra-0.6.2/cotengra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/docs/Makefile` & `cotengra-0.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/docs/_pygments/_pygments_dark.py` & `cotengra-0.6.2/docs/_pygments/_pygments_dark.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/docs/_pygments/_pygments_light.py` & `cotengra-0.6.2/docs/_pygments/_pygments_light.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/docs/_static/logo-favicon.ico` & `cotengra-0.6.2/docs/_static/logo-favicon.ico`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/docs/_static/logo-full.png` & `cotengra-0.6.2/docs/_static/logo-full.png`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/docs/_static/my-styles.css` & `cotengra-0.6.2/docs/_static/my-styles.css`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/docs/advanced.ipynb` & `cotengra-0.6.2/docs/advanced.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/docs/basics.ipynb` & `cotengra-0.6.2/docs/basics.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/docs/changelog.md` & `cotengra-0.6.2/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 # Changelog
 
-## v0.6.1 (unreleased)
+## v0.6.2 (2024-05-21)
+
+**Bug fixes**
+
+- Fix final, output contractions being mistakenly marked as not tensordot-able.
+- When `implementation="autoray"` don't require a backend to have both `einsum` and `tensordot`, instead fallback to `cotengra`'s own.
+
+
+## v0.6.1 (2024-05-15)
 
 **Breaking changes**
 
 - The number of workers initialized (for non-distributed pools) is now set to, in order of preference, 1. the environment variable `COTENGRA_NUM_WORKERS`, 2. the environment variable `OMP_NUM_THREADS`, or 3. `os.cpu_count()`.
 
 **Enhancements**
```

### Comparing `cotengra-0.6.1/docs/conf.py` & `cotengra-0.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/docs/contraction.ipynb` & `cotengra-0.6.2/docs/contraction.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/docs/examples/ex_compressed_contraction.ipynb` & `cotengra-0.6.2/docs/examples/ex_compressed_contraction.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/docs/examples/ex_large_output_lazy.ipynb` & `cotengra-0.6.2/docs/examples/ex_large_output_lazy.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/docs/high-level-interface.ipynb` & `cotengra-0.6.2/docs/high-level-interface.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/docs/index.md` & `cotengra-0.6.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/docs/installation.md` & `cotengra-0.6.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/docs/make.bat` & `cotengra-0.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/docs/trees.ipynb` & `cotengra-0.6.2/docs/trees.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/docs/visualization.ipynb` & `cotengra-0.6.2/docs/visualization.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/examples/Example - Reproducing 2005.06787.ipynb` & `cotengra-0.6.2/examples/Example - Reproducing 2005.06787.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/examples/Example - Reproducing 2103-03074.ipynb` & `cotengra-0.6.2/examples/Example - Reproducing 2103-03074.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/examples/Quantum Circuit Example Old.ipynb` & `cotengra-0.6.2/examples/Quantum Circuit Example Old.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/examples/Quantum Circuit Example.ipynb` & `cotengra-0.6.2/examples/Quantum Circuit Example.ipynb`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/examples/circuit_n53_m10_s0_e0_pABCDCDAB.qsim` & `cotengra-0.6.2/examples/circuit_n53_m10_s0_e0_pABCDCDAB.qsim`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/examples/circuit_n53_m12_s0_e0_pABCDCDAB.qsim` & `cotengra-0.6.2/examples/circuit_n53_m12_s0_e0_pABCDCDAB.qsim`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/examples/circuit_n53_m20_s0_e0_pABCDCDAB.qsim` & `cotengra-0.6.2/examples/circuit_n53_m20_s0_e0_pABCDCDAB.qsim`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/examples/ex_jax.py` & `cotengra-0.6.2/examples/ex_jax.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/examples/ex_mpi_executor.py` & `cotengra-0.6.2/examples/ex_mpi_executor.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/examples/ex_mpi_spmd.py` & `cotengra-0.6.2/examples/ex_mpi_spmd.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/pyproject.toml` & `cotengra-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/setup.py` & `cotengra-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/src/lib.rs` & `cotengra-0.6.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/tests/test_compressed.py` & `cotengra-0.6.2/tests/test_compressed.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/tests/test_compute.py` & `cotengra-0.6.2/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/tests/test_hypergraph.py` & `cotengra-0.6.2/tests/test_hypergraph.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/tests/test_interface.py` & `cotengra-0.6.2/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/tests/test_optimizers.py` & `cotengra-0.6.2/tests/test_optimizers.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/tests/test_paths_basic.py` & `cotengra-0.6.2/tests/test_paths_basic.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/tests/test_slicer.py` & `cotengra-0.6.2/tests/test_slicer.py`

 * *Files identical despite different names*

### Comparing `cotengra-0.6.1/tests/test_tree.py` & `cotengra-0.6.2/tests/test_tree.py`

 * *Files identical despite different names*

