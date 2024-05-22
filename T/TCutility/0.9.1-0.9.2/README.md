# Comparing `tmp/TCutility-0.9.1.tar.gz` & `tmp/TCutility-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TCutility-0.9.1.tar", last modified: Tue Feb  6 14:22:42 2024, max compression
+gzip compressed data, was "TCutility-0.9.2.tar", last modified: Tue Feb  6 15:09:48 2024, max compression
```

## Comparing `TCutility-0.9.1.tar` & `TCutility-0.9.2.tar`

### file list

```diff
@@ -1,87 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:22:42.909199 TCutility-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-06 14:22:30.000000 TCutility-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-06 14:22:30.000000 TCutility-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-02-06 14:22:42.909199 TCutility-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-02-06 14:22:30.000000 TCutility-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-06 14:22:30.000000 TCutility-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 14:22:42.909199 TCutility-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-06 14:22:30.000000 TCutility-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:22:42.893199 TCutility-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:22:42.909199 TCutility-0.9.1/src/TCutility.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-02-06 14:22:42.000000 TCutility-0.9.1/src/TCutility.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-02-06 14:22:42.000000 TCutility-0.9.1/src/TCutility.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 14:22:42.000000 TCutility-0.9.1/src/TCutility.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-06 14:22:42.000000 TCutility-0.9.1/src/TCutility.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-06 14:22:42.000000 TCutility-0.9.1/src/TCutility.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:22:42.901199 TCutility-0.9.1/src/tcutility/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:22:42.901199 TCutility-0.9.1/src/tcutility/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:22:42.901199 TCutility-0.9.1/src/tcutility/analysis/vdd/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/analysis/vdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/analysis/vdd/charge.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/analysis/vdd/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:22:42.901199 TCutility-0.9.1/src/tcutility/analysis/vibration/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/analysis/vibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/analysis/vibration/ts_vibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:22:42.901199 TCutility-0.9.1/src/tcutility/data/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:22:42.901199 TCutility-0.9.1/src/tcutility/data/_atom_data_info/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/data/_atom_data_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/data/_convert_to_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/data/atom.py
--rw-r--r--   0 runner    (1001) docker     (127)    90450 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/data/available_functionals.json
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/data/available_functionals.txt
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/data/basis_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/data/cosmo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/data/functionals.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/data/molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/formula.py
--rw-r--r--   0 runner    (1001) docker     (127)    15649 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:22:42.905199 TCutility-0.9.1/src/tcutility/job/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15531 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/job/adf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8768 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/job/ams.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/job/crest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/job/dftb.py
--rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/job/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/job/nmr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/job/orca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:22:42.905199 TCutility-0.9.1/src/tcutility/job/postscripts/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/job/postscripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/job/postscripts/clean_workdir.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/job/postscripts/split_crest_xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/job/postscripts/write_converged_geoms.py
--rw-r--r--   0 runner    (1001) docker     (127)    15806 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:22:42.905199 TCutility-0.9.1/src/tcutility/results/
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14756 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/results/adf.py
--rw-r--r--   0 runner    (1001) docker     (127)    24288 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/results/ams.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/results/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/results/dftb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/results/input_blocks
--rw-r--r--   0 runner    (1001) docker     (127)    20914 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/results/orca.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/results/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/spell_check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:22:42.905199 TCutility-0.9.1/src/tcutility/typing/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-06 14:22:30.000000 TCutility-0.9.1/src/tcutility/typing/arrays.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:22:42.909199 TCutility-0.9.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-02-06 14:22:31.000000 TCutility-0.9.1/test/test_adf_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-02-06 14:22:31.000000 TCutility-0.9.1/test/test_atom_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-02-06 14:22:31.000000 TCutility-0.9.1/test/test_ensure_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-06 14:22:31.000000 TCutility-0.9.1/test/test_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-02-06 14:22:31.000000 TCutility-0.9.1/test/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-06 14:22:31.000000 TCutility-0.9.1/test/test_input_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-02-06 14:22:31.000000 TCutility-0.9.1/test/test_molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-06 14:22:31.000000 TCutility-0.9.1/test/test_result_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-02-06 14:22:31.000000 TCutility-0.9.1/test/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-02-06 14:22:31.000000 TCutility-0.9.1/test/test_results_orca.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-02-06 14:22:31.000000 TCutility-0.9.1/test/test_spell_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     8492 2024-02-06 14:22:31.000000 TCutility-0.9.1/test/test_vdd_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-02-06 14:22:31.000000 TCutility-0.9.1/test/test_vibrational_ts_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:09:48.815091 TCutility-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-06 15:09:31.000000 TCutility-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-06 15:09:31.000000 TCutility-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-02-06 15:09:48.815091 TCutility-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-02-06 15:09:31.000000 TCutility-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-06 15:09:31.000000 TCutility-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 15:09:48.815091 TCutility-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-06 15:09:31.000000 TCutility-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:09:48.803091 TCutility-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:09:48.815091 TCutility-0.9.2/src/TCutility.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-02-06 15:09:48.000000 TCutility-0.9.2/src/TCutility.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-02-06 15:09:48.000000 TCutility-0.9.2/src/TCutility.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 15:09:48.000000 TCutility-0.9.2/src/TCutility.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-06 15:09:48.000000 TCutility-0.9.2/src/TCutility.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-06 15:09:48.000000 TCutility-0.9.2/src/TCutility.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:09:48.807091 TCutility-0.9.2/src/tcutility/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:09:48.807091 TCutility-0.9.2/src/tcutility/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:09:48.807091 TCutility-0.9.2/src/tcutility/analysis/vdd/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/analysis/vdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/analysis/vdd/charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/analysis/vdd/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:09:48.807091 TCutility-0.9.2/src/tcutility/analysis/vibration/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/analysis/vibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/analysis/vibration/ts_vibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:09:48.807091 TCutility-0.9.2/src/tcutility/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:09:48.807091 TCutility-0.9.2/src/tcutility/data/_atom_data_info/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/data/_atom_data_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/data/_atom_data_info/color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/data/_atom_data_info/name.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/data/_atom_data_info/radius.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/data/_atom_data_info/symbol.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/data/_convert_to_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/data/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90450 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/data/available_functionals.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/data/available_functionals.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/data/basis_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/data/cosmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/data/functionals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/data/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15649 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:09:48.811091 TCutility-0.9.2/src/tcutility/job/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15531 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/job/adf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8768 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/job/ams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/job/crest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/job/dftb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/job/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/job/nmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/job/orca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:09:48.811091 TCutility-0.9.2/src/tcutility/job/postscripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/job/postscripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/job/postscripts/clean_workdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/job/postscripts/split_crest_xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/job/postscripts/write_converged_geoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15806 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:09:48.811091 TCutility-0.9.2/src/tcutility/results/
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14756 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/results/adf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24288 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/results/ams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/results/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/results/dftb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/results/input_blocks
+-rw-r--r--   0 runner    (1001) docker     (127)    20914 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/results/orca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/results/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/spell_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:09:48.811091 TCutility-0.9.2/src/tcutility/typing/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-06 15:09:31.000000 TCutility-0.9.2/src/tcutility/typing/arrays.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:09:48.815091 TCutility-0.9.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-02-06 15:09:32.000000 TCutility-0.9.2/test/test_adf_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-02-06 15:09:32.000000 TCutility-0.9.2/test/test_atom_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-02-06 15:09:32.000000 TCutility-0.9.2/test/test_ensure_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-06 15:09:32.000000 TCutility-0.9.2/test/test_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-02-06 15:09:32.000000 TCutility-0.9.2/test/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-06 15:09:32.000000 TCutility-0.9.2/test/test_input_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-02-06 15:09:32.000000 TCutility-0.9.2/test/test_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-06 15:09:32.000000 TCutility-0.9.2/test/test_result_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-02-06 15:09:32.000000 TCutility-0.9.2/test/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-02-06 15:09:32.000000 TCutility-0.9.2/test/test_results_orca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-02-06 15:09:32.000000 TCutility-0.9.2/test/test_spell_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8492 2024-02-06 15:09:32.000000 TCutility-0.9.2/test/test_vdd_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-02-06 15:09:32.000000 TCutility-0.9.2/test/test_vibrational_ts_analysis.py
```

### Comparing `TCutility-0.9.1/LICENSE` & `TCutility-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/PKG-INFO` & `TCutility-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TCutility
-Version: 0.9.1
+Version: 0.9.2
 Summary: Utility package for working with AMS/ADF within the Theoretical Chemistry group at the Vrije Universiteit Amsterdam (TheoCheM). Makes use of plams - a package developed by SCM
 Author: TheoCheM group
 Maintainer: TheoCheM group
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `TCutility-0.9.1/README.md` & `TCutility-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/pyproject.toml` & `TCutility-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/TCutility.egg-info/PKG-INFO` & `TCutility-0.9.2/src/TCutility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TCutility
-Version: 0.9.1
+Version: 0.9.2
 Summary: Utility package for working with AMS/ADF within the Theoretical Chemistry group at the Vrije Universiteit Amsterdam (TheoCheM). Makes use of plams - a package developed by SCM
 Author: TheoCheM group
 Maintainer: TheoCheM group
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `TCutility-0.9.1/src/TCutility.egg-info/SOURCES.txt` & `TCutility-0.9.2/src/TCutility.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 src/tcutility/data/available_functionals.json
 src/tcutility/data/available_functionals.txt
 src/tcutility/data/basis_sets.py
 src/tcutility/data/cosmo.py
 src/tcutility/data/functionals.py
 src/tcutility/data/molecules.py
 src/tcutility/data/_atom_data_info/__init__.py
+src/tcutility/data/_atom_data_info/color.txt
+src/tcutility/data/_atom_data_info/name.txt
+src/tcutility/data/_atom_data_info/radius.txt
+src/tcutility/data/_atom_data_info/symbol.txt
 src/tcutility/job/__init__.py
 src/tcutility/job/adf.py
 src/tcutility/job/ams.py
 src/tcutility/job/crest.py
 src/tcutility/job/dftb.py
 src/tcutility/job/generic.py
 src/tcutility/job/nmr.py
```

### Comparing `TCutility-0.9.1/src/tcutility/__init__.py` & `TCutility-0.9.2/src/tcutility/__init__.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/analysis/vdd/manager.py` & `TCutility-0.9.2/src/tcutility/analysis/vdd/manager.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/analysis/vibration/ts_vibration.py` & `TCutility-0.9.2/src/tcutility/analysis/vibration/ts_vibration.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/cache.py` & `TCutility-0.9.2/src/tcutility/cache.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/data/atom.py` & `TCutility-0.9.2/src/tcutility/data/atom.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/data/available_functionals.json` & `TCutility-0.9.2/src/tcutility/data/available_functionals.json`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/data/available_functionals.txt` & `TCutility-0.9.2/src/tcutility/data/available_functionals.txt`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/data/cosmo.py` & `TCutility-0.9.2/src/tcutility/data/cosmo.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/data/functionals.py` & `TCutility-0.9.2/src/tcutility/data/functionals.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/data/molecules.py` & `TCutility-0.9.2/src/tcutility/data/molecules.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/formula.py` & `TCutility-0.9.2/src/tcutility/formula.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/geometry.py` & `TCutility-0.9.2/src/tcutility/geometry.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/job/adf.py` & `TCutility-0.9.2/src/tcutility/job/adf.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/job/ams.py` & `TCutility-0.9.2/src/tcutility/job/ams.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/job/crest.py` & `TCutility-0.9.2/src/tcutility/job/crest.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/job/dftb.py` & `TCutility-0.9.2/src/tcutility/job/dftb.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/job/generic.py` & `TCutility-0.9.2/src/tcutility/job/generic.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/job/nmr.py` & `TCutility-0.9.2/src/tcutility/job/nmr.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/job/orca.py` & `TCutility-0.9.2/src/tcutility/job/orca.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/job/postscripts/split_crest_xyz.py` & `TCutility-0.9.2/src/tcutility/job/postscripts/split_crest_xyz.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/job/postscripts/write_converged_geoms.py` & `TCutility-0.9.2/src/tcutility/job/postscripts/write_converged_geoms.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/log.py` & `TCutility-0.9.2/src/tcutility/log.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/molecule.py` & `TCutility-0.9.2/src/tcutility/molecule.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/report.py` & `TCutility-0.9.2/src/tcutility/report.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/results/__init__.py` & `TCutility-0.9.2/src/tcutility/results/__init__.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/results/adf.py` & `TCutility-0.9.2/src/tcutility/results/adf.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/results/ams.py` & `TCutility-0.9.2/src/tcutility/results/ams.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/results/cache.py` & `TCutility-0.9.2/src/tcutility/results/cache.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/results/dftb.py` & `TCutility-0.9.2/src/tcutility/results/dftb.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/results/input_blocks` & `TCutility-0.9.2/src/tcutility/results/input_blocks`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/results/orca.py` & `TCutility-0.9.2/src/tcutility/results/orca.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/results/result.py` & `TCutility-0.9.2/src/tcutility/results/result.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/slurm.py` & `TCutility-0.9.2/src/tcutility/slurm.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/src/tcutility/spell_check.py` & `TCutility-0.9.2/src/tcutility/spell_check.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/test/test_adf_properties.py` & `TCutility-0.9.2/test/test_adf_properties.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/test/test_atom_data.py` & `TCutility-0.9.2/test/test_atom_data.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/test/test_ensure_2d.py` & `TCutility-0.9.2/test/test_ensure_2d.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/test/test_formula.py` & `TCutility-0.9.2/test/test_formula.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/test/test_geometry.py` & `TCutility-0.9.2/test/test_geometry.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/test/test_molecules.py` & `TCutility-0.9.2/test/test_molecules.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/test/test_result_class.py` & `TCutility-0.9.2/test/test_result_class.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/test/test_results.py` & `TCutility-0.9.2/test/test_results.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/test/test_results_orca.py` & `TCutility-0.9.2/test/test_results_orca.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/test/test_spell_check.py` & `TCutility-0.9.2/test/test_spell_check.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/test/test_vdd_analysis.py` & `TCutility-0.9.2/test/test_vdd_analysis.py`

 * *Files identical despite different names*

### Comparing `TCutility-0.9.1/test/test_vibrational_ts_analysis.py` & `TCutility-0.9.2/test/test_vibrational_ts_analysis.py`

 * *Files identical despite different names*

