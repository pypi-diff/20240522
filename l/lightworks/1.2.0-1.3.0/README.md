# Comparing `tmp/lightworks-1.2.0.tar.gz` & `tmp/lightworks-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightworks-1.2.0.tar", last modified: Wed Apr 10 10:00:07 2024, max compression
+gzip compressed data, was "lightworks-1.3.0.tar", last modified: Wed May 22 12:58:39 2024, max compression
```

## Comparing `lightworks-1.2.0.tar` & `lightworks-1.3.0.tar`

### file list

```diff
@@ -1,100 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.165912 lightworks-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 10:00:02.000000 lightworks-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-10 10:00:07.165912 lightworks-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-10 10:00:02.000000 lightworks-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.153911 lightworks-1.2.0/lightworks/
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/__version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.153911 lightworks-1.2.0/lightworks/emulator/
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.153911 lightworks-1.2.0/lightworks/emulator/annotated_state/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/annotated_state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/annotated_state/annotated_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.153911 lightworks-1.2.0/lightworks/emulator/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/backend/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/backend/permanent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/backend/slos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.157912 lightworks-1.2.0/lightworks/emulator/components/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/components/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    16118 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/components/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.157912 lightworks-1.2.0/lightworks/emulator/results/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/results/sampling_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    19154 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/results/simulation_result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.157912 lightworks-1.2.0/lightworks/emulator/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/simulation/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/simulation/probability_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    11103 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/simulation/quick_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16650 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/simulation/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/simulation/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.157912 lightworks-1.2.0/lightworks/emulator/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/emulator/utils/state_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.157912 lightworks-1.2.0/lightworks/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.157912 lightworks-1.2.0/lightworks/sdk/circuit/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21867 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/circuit/circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    20083 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/circuit/circuit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/circuit/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/circuit/unitary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.157912 lightworks-1.2.0/lightworks/sdk/optimisation/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/optimisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16573 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/optimisation/optimisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.157912 lightworks-1.2.0/lightworks/sdk/qubit/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/qubit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/qubit/single_qubit_gates.py
--rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/qubit/two_qubit_gates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.161912 lightworks-1.2.0/lightworks/sdk/state/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/state/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.161912 lightworks-1.2.0/lightworks/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/utils/circuit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/utils/matrix_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/utils/permutation_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/utils/state_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.161912 lightworks-1.2.0/lightworks/sdk/visualisation/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/visualisation/display.py
--rw-r--r--   0 runner    (1001) docker     (127)    12688 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/visualisation/display_components_mpl.py
--rw-r--r--   0 runner    (1001) docker     (127)    14157 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/visualisation/display_components_svg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/visualisation/draw_circuit_mpl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-10 10:00:03.000000 lightworks-1.2.0/lightworks/sdk/visualisation/draw_circuit_svg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.165912 lightworks-1.2.0/lightworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-10 10:00:07.000000 lightworks-1.2.0/lightworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-10 10:00:07.000000 lightworks-1.2.0/lightworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:00:07.000000 lightworks-1.2.0/lightworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 10:00:07.000000 lightworks-1.2.0/lightworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 10:00:07.000000 lightworks-1.2.0/lightworks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-10 10:00:03.000000 lightworks-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:00:07.165912 lightworks-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-10 10:00:03.000000 lightworks-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.153911 lightworks-1.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.165912 lightworks-1.2.0/tests/emulator/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/analyzer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/annotatedstate_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/cnot_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/detector_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8860 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/quicksampler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/result_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18571 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/simulator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/emulator/source_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:07.165912 lightworks-1.2.0/tests/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19554 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/sdk/circuit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/sdk/compiledcircuit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/sdk/display_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/sdk/parameter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/sdk/qubit_gate_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/sdk/state_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-10 10:00:03.000000 lightworks-1.2.0/tests/sdk/util_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.592154 lightworks-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 12:58:13.000000 lightworks-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-22 12:58:39.592154 lightworks-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-22 12:58:13.000000 lightworks-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.576154 lightworks-1.3.0/lightworks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/__version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.580154 lightworks-1.3.0/lightworks/emulator/
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.580154 lightworks-1.3.0/lightworks/emulator/annotated_state/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/annotated_state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/annotated_state/annotated_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.580154 lightworks-1.3.0/lightworks/emulator/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/backend/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/backend/permanent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/backend/slos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.580154 lightworks-1.3.0/lightworks/emulator/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/components/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/components/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.580154 lightworks-1.3.0/lightworks/emulator/results/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9372 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/results/sampling_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/results/simulation_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.580154 lightworks-1.3.0/lightworks/emulator/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11851 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/simulation/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/simulation/probability_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11311 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/simulation/quick_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18633 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/simulation/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/simulation/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.584154 lightworks-1.3.0/lightworks/emulator/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/utils/state_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.584154 lightworks-1.3.0/lightworks/qubit/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/qubit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.584154 lightworks-1.3.0/lightworks/qubit/gates/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/qubit/gates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/qubit/gates/single_qubit_gates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/qubit/gates/two_qubit_gates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.584154 lightworks-1.3.0/lightworks/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.584154 lightworks-1.3.0/lightworks/sdk/circuit/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29551 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/circuit/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/circuit/circuit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/circuit/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/circuit/unitary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.584154 lightworks-1.3.0/lightworks/sdk/optimisation/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/optimisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16573 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/optimisation/optimisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.584154 lightworks-1.3.0/lightworks/sdk/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/state/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.588154 lightworks-1.3.0/lightworks/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/utils/circuit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/utils/heralding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/utils/matrix_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/utils/permutation_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/utils/state_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.588154 lightworks-1.3.0/lightworks/sdk/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/visualisation/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15875 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/visualisation/display_components_mpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17005 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/visualisation/display_components_svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/visualisation/draw_circuit_mpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/visualisation/draw_circuit_svg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.592154 lightworks-1.3.0/lightworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-22 12:58:39.000000 lightworks-1.3.0/lightworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-22 12:58:39.000000 lightworks-1.3.0/lightworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:58:39.000000 lightworks-1.3.0/lightworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-22 12:58:39.000000 lightworks-1.3.0/lightworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 12:58:39.000000 lightworks-1.3.0/lightworks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-22 12:58:13.000000 lightworks-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:58:39.592154 lightworks-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-22 12:58:13.000000 lightworks-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.576154 lightworks-1.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.588154 lightworks-1.3.0/tests/emulator/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/analyzer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/annotatedstate_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/cnot_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/detector_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11795 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/quicksampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/result_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23566 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/simulator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/source_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.592154 lightworks-1.3.0/tests/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27061 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/sdk/circuit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/sdk/compiledcircuit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/sdk/display_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/sdk/parameter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/sdk/qubit_gate_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/sdk/state_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/sdk/util_test.py
```

### Comparing `lightworks-1.2.0/LICENSE` & `lightworks-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/PKG-INFO` & `lightworks-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightworks
-Version: 1.2.0
+Version: 1.3.0
 Summary: Open-source Python SDK for photonic quantum computation.
 Home-page: https://github.com/Aegiq/lightworks
 Author: Aegiq Ltd.
 License: Apache 2.0
 Project-URL: Source, https://github.com/Aegiq/lightworks
 Project-URL: Documentation, https://aegiq.github.io/lightworks/
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `lightworks-1.2.0/README.md` & `lightworks-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/__init__.py` & `lightworks-1.3.0/lightworks/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,21 +38,24 @@
         different objects for simulation of the system, which provide various
         capabilities and outputs.
 
 """
 
 from .__version import __version__
 
-from .sdk import Circuit, Unitary
-from .sdk import Parameter, ParameterDict
-from .sdk import Display
-from .sdk import State
-from .sdk import random_unitary, random_permutation
-from .sdk import db_loss_to_transmission, transmission_to_db_loss
-from .sdk import Optimisation
-from .sdk import qubit
+from . import qubit
+from . import emulator
+
+from .sdk.circuit import Circuit, Unitary
+from .sdk.circuit import Parameter, ParameterDict
+from .sdk.visualisation import Display
+from .sdk.state import State
+from .sdk.utils import random_unitary, random_permutation
+from .sdk.utils import db_loss_to_transmission, transmission_to_db_loss
+from .sdk.optimisation import Optimisation
+
 from .sdk.utils.exceptions import *
 
 __all__ = ["Circuit", "Unitary", "Display", "State", "random_unitary", 
            "random_permutation", "db_loss_to_transmission", 
            "transmission_to_db_loss", "Parameter", "ParameterDict", 
-           "Optimisation"]
+           "Optimisation", "emulator", "qubit"]
```

### Comparing `lightworks-1.2.0/lightworks/__version.py` & `lightworks-1.3.0/lightworks/__version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.2.0"
+__version__ = "1.3.0"
```

### Comparing `lightworks-1.2.0/lightworks/emulator/__init__.py` & `lightworks-1.3.0/lightworks/emulator/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         heralding criteria. This means it can be used to analyze how well a 
         circuit performs for a given task. It can also produce an error rate 
         and value for circuit performance (how often a valid output will be 
         produced).     
                     
 """
 
-from .components import *
-from .simulation import *
-from .backend import *
-from .utils import *
+from .components import Source, Detector
+from .simulation import Simulator, Sampler, Analyzer, QuickSampler
+from .backend import Backend
+
+from .utils.exceptions import *
 
 __all__ = ["Simulator", "Sampler", "Source", "Detector", 
            "Analyzer", "QuickSampler", "Backend"]
```

### Comparing `lightworks-1.2.0/lightworks/emulator/annotated_state/__init__.py` & `lightworks-1.3.0/lightworks/emulator/annotated_state/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/emulator/annotated_state/annotated_state.py` & `lightworks-1.3.0/lightworks/emulator/annotated_state/annotated_state.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/emulator/backend/__init__.py` & `lightworks-1.3.0/lightworks/emulator/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/emulator/backend/backend.py` & `lightworks-1.3.0/lightworks/emulator/backend/backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .permanent import Permanent
 from .slos import SLOS
 from ..utils import fock_basis, BackendError
-from ...sdk import State
+from ...sdk.state import State
 from ...sdk.circuit.circuit_compiler import CompiledCircuit
 
 from numpy import ndarray
 
 class Backend:
     """
     Provide central location for selecting and interacting with different 
@@ -142,16 +142,19 @@
             
         Raises:
         
             BackendError: Raised if this method is called with an incompatible
                 backend.
                 
         """
-        
-        if self.backend == "permanent":    
+        # Return empty distribution when 0 photons in input
+        if input_state.n_photons == 0:
+            pdist = {State([0]*circuit.n_modes) : 1}
+        # Otherwise vary distribution calculation method
+        elif self.backend == "permanent":    
             # Add extra states for loss modes here when included
             if circuit.loss_modes > 0:
                 input_state = input_state + State([0]*circuit.loss_modes) 
             pdist = {}
             # For a given input work out all possible outputs
             out_states = fock_basis(len(input_state), input_state.n_photons)
             for ostate in out_states:
```

### Comparing `lightworks-1.2.0/lightworks/emulator/backend/permanent.py` & `lightworks-1.3.0/lightworks/emulator/backend/permanent.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from ...sdk import State
+from ...sdk.state import State
 
 import numpy as np
 from thewalrus import perm
 from math import factorial, prod
 
 class Permanent:
     """
```

### Comparing `lightworks-1.2.0/lightworks/emulator/backend/slos.py` & `lightworks-1.3.0/lightworks/emulator/backend/slos.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from ...sdk import State
+from ...sdk.state import State
 
 import numpy as np
 from math import factorial
 
 class SLOS:
     """
     Contains calculate function for SLOS method.
```

### Comparing `lightworks-1.2.0/lightworks/emulator/components/__init__.py` & `lightworks-1.3.0/lightworks/emulator/components/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/emulator/components/detector.py` & `lightworks-1.3.0/lightworks/emulator/components/detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """
 Class to simulate detector response when sampling, including detector 
 efficiency, dark counts and non-photon number resolving detectors.
 """
 
-from ...sdk import State
+from ...sdk.state import State
 
 from random import random
 from numbers import Number
 
 class Detector:
     """
     Creates a detector which can be used to model the presence of imperfect
```

### Comparing `lightworks-1.2.0/lightworks/emulator/components/source.py` & `lightworks-1.3.0/lightworks/emulator/components/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 This class is used to model a non-ideal source of single photons, it can be 
 used to build input state variations, accounting for a non-ideal brightness,
 impurity in the single photon stream and indistinguishability between different
 photons.
 """
 
 from ..annotated_state import AnnotatedState
-from ...sdk import State
+from ...sdk.state import State
+
 from numbers import Number
 
 class Source:
     """
     Simulates an imperfect single photon source to model properties of photon 
     inputs in the Sampler.
```

### Comparing `lightworks-1.2.0/lightworks/emulator/results/__init__.py` & `lightworks-1.3.0/lightworks/emulator/results/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/emulator/results/sampling_result.py` & `lightworks-1.3.0/lightworks/emulator/results/sampling_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from ..utils import ResultCreationError
-from ...sdk import State
+from ...sdk.state import State
 
 import numpy as np
 import matplotlib.pyplot as plt
 import pandas as pd
 
 class SamplingResult:
     """
@@ -147,21 +147,15 @@
                 mapped_result[new_s] += val
             else:
                 mapped_result[new_s] = val
         return self._recombine_mapped_result(mapped_result)
         
     def _recombine_mapped_result(self, mapped_result: dict):
         """Creates a new Result object from mapped data."""
-        r = SamplingResult(mapped_result, self.input)
-        for k, v in self.__dict__.items():
-            if k not in ['input', 'outputs', 'dictionary', 
-                         '_SamplingResult__input', '_SamplingResult__outputs', 
-                         '_SamplingResult__dict']:
-                r.__dict__[k] = v
-        return r
+        return SamplingResult(mapped_result, self.input)
         
     def plot(self, show: bool = False, 
              state_labels: dict = {}) -> tuple | None:
         """
         Create a plot of the data contained in the result. This will either 
         take the form of a heatmap or bar chart, depending on the nature of the
         data contained in the Result object.
```

### Comparing `lightworks-1.2.0/lightworks/emulator/results/simulation_result.py` & `lightworks-1.3.0/lightworks/emulator/results/simulation_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from ..utils import ResultCreationError
-from ...sdk import State
+from ...sdk.state import State
 
 import numpy as np
 import matplotlib.pyplot as plt
 import pandas as pd
 
 class SimulationResult:
     """
@@ -237,17 +237,14 @@
         for i, in_state in enumerate(self.inputs):
             for j, out_state in enumerate(unique_outputs):
                 if out_state in mapped_result[in_state]:
                     array[i,j] = mapped_result[in_state][out_state]
         r =  SimulationResult(array, result_type = self.result_type,
                               inputs = self.inputs, 
                               outputs = list(unique_outputs))
-        for k, v in self.__dict__.items():
-            if k not in ['result_type', 'array', 'inputs', 'outputs', 'r']:
-                r.__dict__[k] = v
         return r
     
     def plot(self, conv_to_probability: bool = False, show: bool = False,
              state_labels: dict = {}) -> tuple | None:
         """
         Create a plot of the data contained in the result. This will either 
         take the form of a heatmap or bar chart, depending on the nature of the
```

### Comparing `lightworks-1.2.0/lightworks/emulator/simulation/__init__.py` & `lightworks-1.3.0/lightworks/emulator/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/emulator/simulation/analyzer.py` & `lightworks-1.3.0/lightworks/emulator/simulation/analyzer.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from ..backend import Backend
 from ..utils import fock_basis
 from ..utils import ModeMismatchError, PhotonNumberError
 from ..results import SimulationResult
-from ...sdk import State, Circuit
+from ...sdk.state import State
+from ...sdk.circuit import Circuit
+from ...sdk.utils import add_heralds_to_state
 
 import numpy as np
 from types import FunctionType
 
 
 class Analyzer:
     """
@@ -28,15 +30,15 @@
     cases where we want to look at the transformations between a specific 
     subset of states. It is useful for the simulation of probabilities in 
     cases where loss and circuit errors are likely to be a factor. As part of
     the process a performance and error rate metric are calculated.  
     
     Args:
     
-        circuit : The circuit to simulate.
+        circuit (Circuit) : The circuit to simulate.
         
     Attribute:
     
         performance : The total probabilities of mapping between the states 
             provided compared with all possible states.
                       
         error_rate : Given an expected mapping, the analyzer will determine the
@@ -44,16 +46,14 @@
         
     """
     def __init__ (self, circuit: Circuit) -> None:
         
         # Assign key parameters to attributes
         self.circuit = circuit
         # Create empty list/dict to store other quantities
-        self.in_heralds = {}
-        self.out_heralds = {}
         self.post_selects = []
         self.__backend = Backend("permanent")
         
         return
     
     @property
     def circuit(self) -> Circuit:
@@ -66,37 +66,18 @@
     @circuit.setter
     def circuit(self, value: Circuit) -> None:
         if not isinstance(value, Circuit):
             raise TypeError(
                 "Provided circuit should be a Circuit or Unitary object.")
         self.__circuit = value
     
-    def set_herald(self, in_mode: int, n_photons: int = 0, 
-                   out_mode: int | None = None) -> None:
-        """
-        Set heralded modes for the circuit
-        """
-        if out_mode is None:
-            out_mode = in_mode
-        if type(in_mode) != int or type(out_mode) != int:
-            raise TypeError("Mode numbers should be integers.")
-        if in_mode >= self.circuit.n_modes or out_mode >= self.circuit.n_modes:
-            raise ValueError("Mode outside of circuit range.")
-        if in_mode in self.in_heralds:
-            raise ValueError("Heralding already set for given input mode.")
-        if out_mode in self.out_heralds:
-            raise ValueError("Heralding already set for given output mode.")
-        self.in_heralds[in_mode] = n_photons
-        self.out_heralds[out_mode] = n_photons
-        
-        return
-    
     def set_post_selection(self, function: FunctionType) -> None:
         """
-        Add post selection functions, these should apply to non-heralded modes.
+        Add post selection functions, these should only act across the 
+        non-heralded modes of the circuit.
         """
         # NOTE: If multiple lambda functions are created and passed to this 
         # using a loop this may create issues related to how lambda functions
         # use out of scope variables. See the following for more info:
         # https://docs.python.org/3/faq/programming.html#why-do-lambdas-defined-in-a-loop-with-different-values-all-return-the-same-result
         if not isinstance(function, FunctionType):
             raise TypeError("Post-selection rule should be a function.")
@@ -122,16 +103,16 @@
         Returns:
         
             SimulationResult : A dictionary containing an array of probability 
                 values between the provided inputs/outputs. 
             
         """
         self.__circuit_built = self.circuit._build()
-        n_modes = self.__circuit_built.n_modes - len(self.in_heralds)
-        if self.in_heralds != self.out_heralds:
+        n_modes = self.circuit.input_modes
+        if self.circuit.heralds["input"] != self.circuit.heralds["output"]:
             raise RuntimeError(
                 "Mismatch in number of heralds on the input/output modes, it "
                 "is likely this results from a herald being added twice or "
                 "modified.")
         # Convert state to list of States if not provided for single state case
         if type(inputs) is State:
                 inputs = [inputs] 
@@ -168,57 +149,41 @@
         """
         probs = np.zeros((len(full_inputs), len(full_outputs)))
         for i, ins in enumerate(full_inputs):
             for j, outs in enumerate(full_outputs):
                 # No loss case
                 if not self.__circuit_built.loss_modes:
                     probs[i, j] += self.__backend.probability(
-                        self.__circuit_built.U_full, ins.s, outs.s)
+                        self.__circuit_built.U_full, ins.s, outs)
                 # Lossy case
                 else:
                     # Photon number preserved
-                    if ins.n_photons == outs.n_photons:
-                        outs = (outs + 
-                                State([0]*self.__circuit_built.loss_modes))
+                    if ins.n_photons == sum(outs):
+                        outs = outs + [0]*self.__circuit_built.loss_modes
                         probs[i, j] += self.__backend.probability(
-                            self.__circuit_built.U_full, ins.s, outs.s)
+                            self.__circuit_built.U_full, ins.s, outs)
                     # Otherwise
                     else:
                         # If n_out < n_in work out all loss mode combinations
                         # and find probability of each
-                        n_loss = ins.n_photons - outs.n_photons
+                        n_loss = ins.n_photons - sum(outs)
                         if n_loss < 0:
                             raise PhotonNumberError(
                                 "Output photon number larger than input "
                                 "number.")
                         # Find loss states and find probability of each
                         loss_states = fock_basis(
                             self.__circuit_built.loss_modes, n_loss)
                         for ls in loss_states:
-                            fs = outs + State(ls)
+                            fs = outs + ls
                             probs[i, j] += self.__backend.probability(
-                                self.__circuit_built.U_full, ins.s, fs.s)     
+                                self.__circuit_built.U_full, ins.s, fs)     
                             
         return probs
     
-    def _build_state(self, state: State, herald: FunctionType) -> State:
-        """
-        Add heralded modes to a provided state
-        """
-        count = 0
-        new_state = [0]*self.__circuit_built.n_modes
-        for i in range(self.__circuit_built.n_modes):
-            if i in herald:
-                new_state[i] = herald[i]
-            else:
-                new_state[i] = state[count]
-                count += 1
-        
-        return State(new_state)
-    
     def _calculate_error_rate(self, probabilities: np.ndarray, inputs: list, 
                               outputs: list, expected: dict) -> float:
         """
         Calculate the error rate for a set of expected mappings between inputs 
         and outputs, given the results calculated by the analyzer.
         """
         # Check all inputs in expectation mapping
@@ -245,30 +210,31 @@
         return np.mean(errors)
     
     def _process_inputs(self, inputs: list) -> list:
         """
         Takes the provided inputs, perform error checking on them and adds any 
         heralded photons that are required, returning full states..
         """
-        n_modes = self.__circuit_built.n_modes - len(self.in_heralds)
+        n_modes = self.circuit.input_modes
         # Ensure all photon numbers are the same   
         ns = [s.n_photons for s in inputs]
         if min(ns) != max(ns):
             raise PhotonNumberError(
                 "Mismatch in photon numbers between inputs")
         full_inputs = []
+        in_heralds = self.circuit.heralds["input"]
         # Check dimensions of input and add heralded photons
         for state in inputs:
             if len(state) != n_modes:
                 raise ModeMismatchError(
                     "Input states are of the wrong dimension. Remember to "
                     "subtract heralded modes.")
             # Also validate state values
             state._validate()
-            full_inputs += [self._build_state(state, self.in_heralds)]
+            full_inputs += [State(add_heralds_to_state(state, in_heralds))]
         # Add extra states for loss modes here when included
         if self.__circuit_built.loss_modes > 0:
             full_inputs = [s + State([0]*self.__circuit_built.loss_modes) 
                            for s in full_inputs]
         return full_inputs
     
     def _generate_outputs(self, n_modes: int, 
@@ -285,21 +251,23 @@
         else:
             outputs = []
             for n in range(0, n_photons+1):
                 outputs += fock_basis(n_modes, n)
         # Filter outputs according to post selection and add heralded photons
         filtered_outputs = []
         full_outputs = []
+        out_heralds = self.circuit.heralds["output"]
         for state in outputs:
-            fo  = self._build_state(state, self.out_heralds)
             # Check output meets all post selection rules
             for funcs in self.post_selects:
-                if not funcs(fo):
+                if not funcs(state):
                     break
             else:
+                fo  = add_heralds_to_state(
+                          state, out_heralds)
                 filtered_outputs += [State(state)]
                 full_outputs += [fo]
         # Check some valid outputs found
         if not full_outputs:
             raise ValueError(
                 "No valid outputs found, consider relaxing post-selection.")
```

### Comparing `lightworks-1.2.0/lightworks/emulator/simulation/probability_distribution.py` & `lightworks-1.3.0/lightworks/emulator/simulation/probability_distribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from ..backend import Backend
-from ...sdk import State
+from ...sdk.state import State
 from ...sdk.circuit.circuit_compiler import CompiledCircuit
 
 class ProbabilityDistributionCalc:
     
     @staticmethod
     def state_prob_calc(circuit: CompiledCircuit, inputs: dict,
                         backend: Backend) -> dict:
```

### Comparing `lightworks-1.2.0/lightworks/emulator/simulation/quick_sampler.py` & `lightworks-1.3.0/lightworks/emulator/simulation/quick_sampler.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from ..backend import Backend
 from ..utils import fock_basis, ModeMismatchError
 from ..results import SamplingResult
-from ...sdk import State, Circuit
+from ...sdk.state import State
+from ...sdk.circuit import Circuit
+from ...sdk.utils import add_heralds_to_state
 
 import numpy as np
 from random import random
 from types import FunctionType
 from collections import Counter
 from typing import Any
 
@@ -40,27 +42,28 @@
         
         input_state (State) : The input state to use with the circuit for 
             sampling.
         
         photon_counting (bool, optional) : Toggle whether or not photon number
             resolving detectors are used.
         
-        herald (function, optional) : A function which applies a provided set 
-            of heralding checks to a state.
+        post_select (function, optional) : A function which applies a set of
+            post-selection criteria to the output state. This will be checked
+            on th
 
     """
     
     def __init__(self, circuit: Circuit, input_state: State, 
                  photon_counting: bool = True,
-                 herald: FunctionType | None = None) -> None:
+                 post_select: FunctionType | None = None) -> None:
         
         # Assign parameters to attributes
         self.circuit = circuit
         self.input_state = input_state
-        self.herald = herald
+        self.post_select = post_select
         self.photon_counting = photon_counting
         self.__backend = Backend("permanent")
         
         return
     
     @property
     def circuit(self) -> Circuit:
@@ -82,32 +85,32 @@
         """The input state to be used for sampling."""
         return self.__input_state
     
     @input_state.setter
     def input_state(self, value: State) -> None:
         if type(value) != State:
             raise TypeError("A single input of type State should be provided.")
-        if len(value) != self.circuit.n_modes:
+        if len(value) != self.circuit.input_modes:
             raise ModeMismatchError("Incorrect input length.")
         # Also validate state values
         value._validate()
         self.__input_state = value
         
     @property
-    def herald(self) -> FunctionType:
-        """A function to be used to post-selection of outputs."""
-        return self.__herald
+    def post_select(self) -> FunctionType:
+        """A function to be used for post-selection of outputs."""
+        return self.__post_select
     
-    @herald.setter
-    def herald(self, value: FunctionType | None) -> None:
+    @post_select.setter
+    def post_select(self, value: FunctionType | None) -> None:
         if value is None:
             value = lambda s: True
         if type(value) != FunctionType:
-            raise TypeError("Provided herald value should be a function.")
-        self.__herald = value
+            raise TypeError("Provided post_select value should be a function.")
+        self.__post_select = value
         
     @property
     def photon_counting(self) -> bool:
         """Details whether photon number resolving detectors are in use."""
         return self.__photon_counting
         
     @photon_counting.setter
@@ -121,23 +124,23 @@
         """
         The output probability distribution for the currently set configuration
         of the QuickSampler. This is re-calculated as the QuickSampler 
         parameters are changed.
         """
         if self._check_parameter_updates():
             # Check circuit and input modes match
-            if self.circuit.n_modes != len(self.input_state):
+            if self.circuit.input_modes != len(self.input_state):
                 raise ValueError(
                     "Mismatch in number of modes between input and circuit.")
             # For given input work out all possible outputs
             out_states = fock_basis(len(self.input_state), 
                                     self.input_state.n_photons)
             if not self.photon_counting:
                 out_states = [s for s in out_states if max(s) == 1]
-            out_states = [s for s in out_states if self.herald(s)]
+            out_states = [s for s in out_states if self.post_select(s)]
             if not out_states:
                 raise ValueError(
                     "Heralding function removed all possible outputs.")
             # Find the probability distribution
             pdist = self._calculate_probabiltiies(out_states)
             # Then assign calculated distribution to attribute
             self.__probability_distribution = pdist
@@ -228,33 +231,38 @@
     
     def _gen_calculation_values(self) -> list:
         """
         Stores all current parameters used with the sampler in a list and 
         returns this.
         """
         # Store circuit unitary and input state
-        vals = [self.__circuit.U_full, self.input_state, self.herald, 
+        vals = [self.__circuit.U_full, self.input_state, self.post_select, 
                 self.photon_counting]
         return vals
     
     def _calculate_probabiltiies(self, outputs: list) -> dict:
         """
         Calculate the probabilities of all of the provided outputs and returns
         this as a normalised distribution.
         """
         # Build circuit to avoid unnecessary recalculation of quantities
         built_circuit = self.circuit._build()
+        # Include circuit heralds to input
+        in_state = add_heralds_to_state(self.input_state, 
+                                        self.circuit.heralds["input"])
         # Add extra states on input for loss modes here when included
-        in_state = self.input_state + State([0]*built_circuit.loss_modes)
+        in_state += [0]*built_circuit.loss_modes
         pdist = {}
+        out_heralds = self.circuit.heralds["output"]
         # Loop through possible outputs and calculate probability of each
         for ostate in outputs:
-            p = self.__backend.probability(
-                built_circuit.U_full, in_state.s, 
-                ostate + [0]*built_circuit.loss_modes)
+            full_ostate = add_heralds_to_state(ostate, out_heralds)
+            full_ostate += [0]*built_circuit.loss_modes
+            p = self.__backend.probability(built_circuit.U_full, in_state, 
+                                           full_ostate)
             # Add output to distribution
             if p > 0:
                 pdist[State(ostate)] = p
         # Normalise probability distribution
         p_total = sum(pdist.values())
         for s, p in pdist.items():
             pdist[s] = p/p_total
@@ -267,21 +275,14 @@
         normalised.
         """
         cdist, pcon = {}, 0
         for s, p in dist.items():
             pcon += p
             cdist[s] = pcon
         return cdist
-    
-    def _fermionic_checks(self, in_state):
-        """Perform additional checks when doing fermionic sampling."""
-        if max(in_state) > 1:
-            raise ValueError(
-                "Max number of photons per mode must be 1 when using "
-                "fermionic statistics.")
         
     def _check_random_seed(self, seed: Any) -> int | None:
         """Process a supplied random seed."""
         if not isinstance(seed, (int, type(None))):
             if int(seed) == seed:
                 seed = int(seed)
             else:
```

### Comparing `lightworks-1.2.0/lightworks/emulator/simulation/sampler.py` & `lightworks-1.3.0/lightworks/emulator/simulation/sampler.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 # limitations under the License.
 
 from .probability_distribution import ProbabilityDistributionCalc as PDC
 from ..backend import Backend
 from ..utils import ModeMismatchError
 from ..results import SamplingResult
 from ..components import Source, Detector
-from ...sdk import State, Circuit
+from ...sdk.state import State
+from ...sdk.circuit import Circuit
+from ...sdk.utils import add_heralds_to_state, remove_heralds_from_state
 
 import numpy as np
 from random import random
 from types import FunctionType
 from collections import Counter
 from typing import Any
 
@@ -87,15 +89,15 @@
         """The input state to be used for sampling."""
         return self.__input_state
     
     @input_state.setter
     def input_state(self, value: State) -> None:
         if type(value) != State:
             raise TypeError("A single input of type State should be provided.")
-        if len(value) != self.circuit.n_modes:
+        if len(value) != self.circuit.input_modes:
             raise ModeMismatchError(
                 "Incorrect input length for provided circuit.")
         # Also validate state values
         value._validate()
         self.__input_state = value
         
     @property
@@ -150,31 +152,38 @@
         """
         The output probability distribution for the currently set configuration
         of the Sampler. This is re-calculated as the Sampler parameters are 
         changed.
         """
         if self._check_parameter_updates():
             # Check circuit and input modes match
-            if self.circuit.n_modes != len(self.input_state):
+            if self.circuit.input_modes != len(self.input_state):
                 raise ValueError(
                     "Mismatch in number of modes between input and circuit.")
-            # Check inputs are valid depending on the statistics 
-            all_inputs = self.source._build_statistics(self.input_state)
+            # Add heralds to the included input
+            input_state = add_heralds_to_state(
+                self.input_state, self.circuit.heralds["input"])
+            input_state = State(input_state)
+            # Then build with source
+            all_inputs = self.source._build_statistics(input_state)
             if isinstance(next(iter(all_inputs)), State):
-                pdist = PDC.state_prob_calc(self.circuit._build(), all_inputs,
-                                            self.backend)
+                pdist = PDC.state_prob_calc(
+                    self.circuit._build(), all_inputs, self.backend)
             else:
-                pdist = PDC.annotated_state_prob_calc(self.circuit._build(), 
-                                                      all_inputs,
-                                                      self.backend)
+                pdist = PDC.annotated_state_prob_calc(
+                    self.circuit._build(), all_inputs, self.backend)
             # Special case to catch an empty distribution
             if not pdist:
                 pdist = {State([0]*self.circuit.n_modes) : 1}
             # Assign calculated distribution to attribute
             self.__probability_distribution = pdist
+            herald_modes = list(self.circuit.heralds["output"].keys())
+            self.__full_to_heralded = {
+                s: State(remove_heralds_from_state(s, herald_modes)) 
+                for s in pdist}
             self.__calculation_values = self._gen_calculation_values()
             # Also pre-calculate continuous distribution
             self.__continuous_distribution = self._convert_to_continuous(pdist)
         return self.__probability_distribution
     
     @property
     def continuous_distribution(self) -> dict:
@@ -200,125 +209,171 @@
         pval = random()
         for state, cd in self.continuous_distribution.items():
             if pval < cd:
                 break
         # Return this as the found state - only return modes of interest
         return self.detector._get_output(state)
     
-    def sample_N_inputs(self, N: int, herald: FunctionType = None, 
+    def sample_N_inputs(self, N: int, post_select: FunctionType = None, 
                         min_detection: int = 0, 
                         seed: int|None = None) -> SamplingResult:
         """
         Function to sample from the configured system by running N clock cycles
         of the system. In each of these clock cycles the input may differ from
         the target input, dependent on the source properties, and there may be
         a number of imperfections in place which means that photons are not
         measured or false detections occur. This means it is possible to for 
         less than N measured states to be returned.
         
         Args:
         
             N (int) : The number of samples to take from the circuit.
         
-            herald (function, optional) : A function which applies a provided
-                set of heralding checks to a state.
+            post_select (function, optional) : A function which applies a 
+                provided set of post-selection criteria to a state.
                                       
             min_detection (int, optional) : Post-select on a given minimum 
-                total number of photons, this should include any heralded 
+                total number of photons, this should not include any heralded 
                 photons.
                                           
             seed (int|None, optional) : Option to provide a random seed to 
                 reproducibly generate samples from the function. This is 
                 optional and can remain as None if this is not required.
         
         Returns:
         
             SamplingResult : A dictionary containing the different output 
                 states and the number of counts for each one.
                     
         """
         # Create always true herald if one isn't provided
-        if herald is None:
-            herald = lambda s: True
-        if type(min_detection) != int:
+        if post_select is None:
+            def post_select(s): return True
+        if (not isinstance(min_detection, int) or 
+            isinstance(min_detection, bool)):
             raise TypeError("Post-selection value should be an integer.")
-        if type(herald) != FunctionType:
-            raise TypeError("Provided herald value should be a function.")
+        if not isinstance(post_select, FunctionType):
+            raise TypeError("Provided post_select value should be a function.")
         pdist = self.probability_distribution
         vals = np.zeros(len(pdist), dtype=object)
         for i, k in enumerate(pdist.keys()):
             vals[i] = k
         # Generate N random samples and then process and count output states
         np.random.seed(self._check_random_seed(seed))
         samples = np.random.choice(vals, p = list(pdist.values()), size = N)
         filtered_samples = []
+        # Get heralds and pre-calculate items
+        heralds = self.circuit.heralds["output"]
+        if heralds:
+            if max(heralds.values()) > 1 and not self.detector.photon_counting:
+                raise ValueError(
+                    "Non photon number resolving detectors cannot be used when"
+                    "a heralded mode has more than 1 photon.")
+        herald_modes = list(heralds.keys())
+        herald_items = list(heralds.items())
+        # Process output states
         for state in samples:
-            # Process output state
             state = self.detector._get_output(state)
-            if herald(state) and state.n_photons >= min_detection:
-                filtered_samples.append(state)
+            # Checks herald requirements are met
+            for m, n in herald_items:
+                if state[m] != n:
+                    break
+            # If met then remove heralded modes and store
+            else:
+                if heralds:
+                    if state not in self.__full_to_heralded:
+                        self.__full_to_heralded[state] = State(
+                            remove_heralds_from_state(state, herald_modes))
+                    hs = self.__full_to_heralded[state]
+                else:
+                    hs = state
+                if (post_select(hs) and hs.n_photons >= min_detection):
+                    filtered_samples.append(hs)
         results = dict(Counter(filtered_samples))
         results = SamplingResult(results, self.input_state)
         return results
     
-    def sample_N_outputs(self, N: int, herald: FunctionType = None, 
+    def sample_N_outputs(self, N: int, post_select: FunctionType = None, 
                          min_detection: int = 0, 
                          seed: int|None = None) -> SamplingResult:
         """
         Function to generate N output samples from a system, according to a set
         of selection criteria. The function will raise an error if the 
         selection criteria is too strict and removes all outputs. Also note 
         this cannot be used to simulate detector dark counts.
         
         Args:
         
             N (int) : The number of samples that are to be returned.
             
-            herald (function, optional) : A function which applies a provided
-                set of heralding checks to a state.
+            post_select (function, optional) : A function which applies a 
+                provided set of post-selection criteria to a state.
                                       
             min_detection (int, optional) : Post-select on a given minimum 
-                total number of photons, this should include any heralded 
+                total number of photons, this should not include any heralded 
                 photons.
                                   
             seed (int|None, optional) : Option to provide a random seed to 
                 reproducibly generate samples from the function. This is 
                 optional and can remain as None if this is not required.
                                   
         Returns:
         
             SamplingResult : A dictionary containing the different output 
                 states and the number of counts for each one.
                                          
         """
-        # Create always true herald if one isn't provided
-        if herald is None:
-            herald = lambda s: True
-        if type(min_detection) != int:
+        # Create always true post_select if one isn't provided
+        if post_select is None:
+            def post_select(s): return True
+        if (not isinstance(min_detection, int) or 
+            isinstance(min_detection, bool)):
             raise TypeError("Post-selection value should be an integer.")
-        if type(herald) != FunctionType:
-            raise TypeError("Provided herald value should be a function.")
+        if not isinstance(post_select, FunctionType):
+            raise TypeError("Provided post_select value should be a function.")
         pdist = self.probability_distribution
         # Check no detector dark counts included
         if self.detector.p_dark != 0:
             raise ValueError("Not supported when using detector dark counts")
-        # Apply threshold affect + and post selection criteria
-        if not self.detector.photon_counting:
-            new_dist = {}
-            for s, p in pdist.items():
-                new_s = State([min(i,1) for i in s])
-                if new_s.n_photons >= min_detection and herald(new_s):
+        # Get heralds and pre-calculate items
+        heralds = self.circuit.heralds["output"]
+        if heralds:
+            if max(heralds.values()) > 1 and not self.detector.photon_counting:
+                raise ValueError(
+                    "Non photon number resolving detectors cannot be used when"
+                    "a heralded mode has more than 1 photon.")
+        herald_modes = list(heralds.keys())
+        herald_items = list(heralds.items())
+        # Convert distribution using provided data
+        new_dist = {}
+        for s, p in pdist.items():
+            # Apply threshold detection
+            if not self.detector.photon_counting:
+                s = State([min(i,1) for i in s])
+            # Check heralds
+            for m, n in herald_items:
+                if s[m] != n:
+                    break
+            else:
+                # Then remove herald modes
+                if heralds:
+                    if s not in self.__full_to_heralded:
+                        self.__full_to_heralded[s] = State(
+                            remove_heralds_from_state(s, herald_modes))
+                    new_s = self.__full_to_heralded[s]
+                else:
+                    new_s = s
+                # Check state meets min detection and post-selection criteria
+                # across remaining modes
+                if new_s.n_photons >= min_detection and post_select(new_s):
                     if new_s in new_dist:
                         new_dist[new_s] += p
                     else:
                         new_dist[new_s] = p
-            pdist = new_dist
-        else:
-            pdist = {s:p for s, p in pdist.items() 
-                     if s.n_photons >= min_detection and herald(s)}
+        pdist = new_dist
         # Check some states are found
         if not pdist:
             raise ValueError(
                 "No output states compatible with provided criteria.")
         # Re-normalise distribution probabilities
         probs = np.array(list(pdist.values()))
         probs = probs/sum(probs) 
@@ -369,35 +424,22 @@
                      "probability_threshold"]:
             vals.append(self.source.__getattribute__(prop))
         return vals
     
     def _convert_to_continuous(self, dist: dict) -> dict:
         """
         Convert a probability distribution to continuous for sampling, with 
-        normalisation also being applied."""
+        normalisation also being applied.
+        """
         cdist, pcon = {}, 0
         total = sum(dist.values())
         for s, p in dist.items():
             pcon += p
             cdist[s] = pcon/total
         return cdist
-    
-    def _fermionic_checks(self, in_state: State, source: Source) -> None:
-        """Perform additional checks when doing fermionic sampling."""
-        if max(in_state) > 1:
-            raise ValueError(
-                "Max number of photons per mode must be 1 when using " 
-                "fermionic statistics.")
-        if source.purity < 1:
-            raise ValueError(
-                "Fermionic sampling does not support non-ideal purity.")
-        if source.indistinguishability < 1:
-            raise ValueError(
-                "Fermionic sampling does not support indistinguishability "
-                "modification.")
         
     def _check_random_seed(self, seed: Any) -> int | None:
         """Process a supplied random seed."""
         if not isinstance(seed, (int, type(None))):
             if int(seed) == seed:
                 seed = int(seed)
             else:
```

### Comparing `lightworks-1.2.0/lightworks/emulator/simulation/simulator.py` & `lightworks-1.3.0/lightworks/emulator/simulation/simulator.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from ..backend import Backend
 from ..utils import fock_basis
 from ..utils import ModeMismatchError, PhotonNumberError
 from ..results import SimulationResult
-from ...sdk import State, Circuit
+from ...sdk.state import State
+from ...sdk.circuit import Circuit
+from ...sdk.utils import add_heralds_to_state
 
 import numpy as np
 
 
 class Simulator:
     """
     Simulates a circuit for a provided number of inputs and outputs, returning
@@ -83,84 +85,85 @@
         # Convert state to list of States if not provided for single state case
         if type(inputs) is State:
                 inputs = [inputs]
         # Then process inputs list
         inputs = self._process_inputs(inputs)
         # And then either generate or process outputs
         inputs, outputs = self._process_outputs(inputs, outputs)
-        # Add extra states for loss modes here when included
-        if circuit.loss_modes > 0:
-            inputs = [s + State([0]*circuit.loss_modes) for s in inputs]
-            outputs = [s + State([0]*circuit.loss_modes) for s in outputs]
+        in_heralds = self.circuit.heralds["input"]
+        out_heralds = self.circuit.heralds["output"]
         # Calculate permanent for the given inputs and outputs and return 
         # values
         amplitudes = np.zeros((len(inputs), len(outputs)), dtype = complex)
         for i, ins in enumerate(inputs):
+            in_state = add_heralds_to_state(ins, in_heralds)
+            in_state += [0]*circuit.loss_modes
             for j, outs in enumerate(outputs):
+                out_state = add_heralds_to_state(outs, out_heralds)
+                out_state += [0]*circuit.loss_modes
                 amplitudes[i, j] = self.__backend.probability_amplitude(
-                    circuit.U_full, ins.s, outs.s)
-        if circuit.loss_modes > 0:
-            inputs = [s[:circuit.n_modes] for s in inputs]
-            outputs = [s[:circuit.n_modes] for s in outputs]
+                    circuit.U_full, in_state, out_state)
         # Return results and corresponding states as dictionary
         results = {"amplitudes" : amplitudes, "inputs" : inputs, 
                    "outputs" : outputs}
         results = SimulationResult(amplitudes, "probability_amplitude", 
                                    inputs = inputs, outputs = outputs)
         return results
     
     def _process_inputs(self, inputs: list) -> list:
         """Performs all required processing/checking on the input states."""
+        input_modes = self.circuit.input_modes
         # Check each input
         for state in inputs:
             # Ensure correct type
             if not isinstance(state, State):
                 raise TypeError(
                     "inputs should be a State or list of State objects.")  
             # Dimension check
-            if len(state) != self.circuit.n_modes:
+            if len(state) != input_modes:
                 raise ModeMismatchError(
                     "One or more input states have an incorrect number of "
                     "modes, correct number of modes is "
-                    f"{self.circuit.n_modes}.")
+                    f"{input_modes}.")
             # Also validate state values
             state._validate()
         return inputs
     
     def _process_outputs(self, inputs: list, 
                          outputs: list | None) -> tuple[list, list]:
         """
         Processes the provided outputs or generates them if no inputs were 
         provided. Returns both the inputs and outputs.
         """
+        input_modes = self.circuit.input_modes
         # If outputs not specified then determine all combinations
         if outputs is None:
             ns = [s.n_photons for s in inputs]
             if min(ns) != max(ns):
                 raise PhotonNumberError(
                     "Mismatch in total photon number between inputs, this is "
                     "not currently supported by the Simulator.")
-            outputs = fock_basis(self.circuit.n_modes, max(ns))
+            outputs = fock_basis(input_modes, max(ns))
             outputs = [State(s) for s in outputs]
         # Otherwise check provided outputs
         else:
             if type(outputs) is State:
                 outputs = [outputs]
-            # Check type and for fermionic statistics
+            # Check type and dimension is correct
             for state in outputs:
                 # Ensure correct type
                 if not isinstance(state, State):
                     raise TypeError(
                         "outputs should be a State or list of State objects.")  
                 # Dimension check
-                if len(state) != self.circuit.n_modes:
+                if len(state) != input_modes:
                     raise ModeMismatchError(
                         "One or more input states have an incorrect number of "
                         "modes, correct number of modes is "
-                        f"{self.circuit.n_modes}.")
+                        f"{input_modes}.")
                 # Also validate state values
                 state._validate()
             # Ensure photon numbers are the same in all states - variation not 
             # currently supported
             ns = [s.n_photons for s in inputs + outputs]
             if min(ns) != max(ns):
                 raise PhotonNumberError(
```

### Comparing `lightworks-1.2.0/lightworks/emulator/utils/__init__.py` & `lightworks-1.3.0/lightworks/emulator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/emulator/utils/exceptions.py` & `lightworks-1.3.0/lightworks/emulator/utils/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Contains all custom exceptions created for the emulator section of Lightworks.
 """
 
-from ...sdk import LightworksError
+from ...sdk.utils import LightworksError
 
 class EmulatorError(LightworksError):
     """
     Generic error for emulator which sub classes the main LightworksError
     """
     pass
```

### Comparing `lightworks-1.2.0/lightworks/emulator/utils/state_utils.py` & `lightworks-1.3.0/lightworks/emulator/utils/state_utils.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/sdk/__init__.py` & `lightworks-1.3.0/lightworks/sdk/circuit/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,12 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .circuit import *
-from .visualisation import *
-from .state import *
-from .utils import *
-from .optimisation import *
+from .circuit import Circuit
+from .unitary import Unitary
+from .parameters import Parameter, ParameterDict
```

### Comparing `lightworks-1.2.0/lightworks/sdk/circuit/__init__.py` & `lightworks-1.3.0/lightworks/qubit/gates/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,10 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .circuit import Circuit
-from .unitary import Unitary
-from .parameters import Parameter, ParameterDict
+from .single_qubit_gates import H, X, Y, Z, S, T
+from .two_qubit_gates import CZ, CNOT, CZ_Heralded, CNOT_Heralded
```

### Comparing `lightworks-1.2.0/lightworks/sdk/circuit/circuit.py` & `lightworks-1.3.0/lightworks/sdk/circuit/circuit.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 from .circuit_compiler import CompiledCircuit, CompiledUnitary
 from .parameters import Parameter
 from ..utils import ModeRangeError, DisplayError
 from ..utils import CircuitCompilationError
 from ..utils import unpack_circuit_spec, compress_mode_swaps
 from ..utils import convert_non_adj_beamsplitters
+from ..utils import add_modes_to_circuit_spec, add_empty_mode_to_circuit_spec
 from ..visualisation import Display
 
 from typing import Any, Union
 from numbers import Number
 import matplotlib.pyplot as plt
 from IPython import display
 from copy import copy, deepcopy
@@ -50,102 +51,210 @@
         if not isinstance(n_modes, int):
             if int(n_modes) == n_modes:
                 n_modes = int(n_modes)
             else:
                 raise TypeError("Number of modes should be an integer.")
         self.__n_modes = n_modes
         self.__circuit_spec = []
+        self.__in_heralds = {}
+        self.__out_heralds = {}
+        self.__external_in_heralds = {}
+        self.__external_out_heralds = {}
         self.__show_parameter_values = False
+        self.__internal_modes = []
         
         return
     
     def __add__(self, value: "Circuit") -> "Circuit":
         """Defines custom addition behaviour for two circuits."""
-        if isinstance(value, Circuit):
-            if self.__n_modes != value.__n_modes:
-                raise ModeRangeError(
-                    "Two circuits to add must have the same number of modes.")
-            # Create new circuits and combine circuits specs to create new one
-            new_circ = Circuit(self.__n_modes)
-            new_circ.__circuit_spec = (self.__circuit_spec + 
-                                       value.__circuit_spec)
-            return new_circ
-        else:
+        if not isinstance(value, Circuit):
             raise TypeError(
                 "Addition only supported between two Circuit objects.")
-        
+        if self.n_modes != value.n_modes:
+            raise ModeRangeError(
+                "Two circuits to add must have the same number of modes.")
+        if self.heralds["input"] or value.heralds["input"]:
+            raise NotImplementedError(
+                "Support for heralds when combining circuits not yet "
+                "implemented.")
+        # Create new circuits and combine circuits specs to create new one
+        new_circ = Circuit(self.n_modes)
+        new_circ.__circuit_spec = (self.__circuit_spec + 
+                                    value.__circuit_spec)
+        return new_circ
+                    
     @property
     def U(self) -> np.ndarray:
         """
         The effective unitary that the circuit implements across modes. This 
         will include the effect of any loss within a circuit. It is calculated 
         using the parameter values at the time that the attribute is called.
         """
-        return self._build().U_full[:self.__n_modes, :self.__n_modes]
+        return self._build().U_full[:self.n_modes, :self.n_modes]
     
     @property
     def U_full(self) -> np.ndarray:
         """
         The full unitary for the created circuit, this will include the 
         additional modes used for the simulation of loss, if this has been 
         included in the circuit.
         """
         return self._build().U_full
     
     @property
     def n_modes(self) -> int:
-        """Returns number of modes in the circuit."""
+        """The number of modes in the circuit."""
         return self.__n_modes
     
     @n_modes.setter
     def n_modes(self, value: Any) -> None:
         """
         Prevents modification of n_modes attribute after circuit creation.
         """
         raise AttributeError("Number of circuit modes cannot be modified.")
     
     @property
+    def input_modes(self):
+        """
+        The number of input modes that should be specified, accounting for the 
+        heralds used in the circuit.
+        """
+        return self.n_modes - len(self.heralds["input"])
+    
+    @property
+    def heralds(self) -> dict:
+        """
+        A dictionary which details the set heralds on the inputs and outputs of
+        the circuit.
+        """
+        return {"input" : copy(self.__in_heralds), 
+                "output" : copy(self.__out_heralds)}
+        
+    @property
     def _display_spec(self) -> list:
-        """Returns display spec for the circuit."""
+        """The display spec for the circuit."""
         return self._get_display_spec()
+    
+    @property
+    def _internal_modes(self) -> list:
+        return self.__internal_modes
+    
+    @property
+    def _external_heralds(self) -> dict:
+        """
+        Stores details of heralds which are on the outside of a circuit (i.e.
+        were not added as part of a group).
+        """
+        return {"input" : copy(self.__external_in_heralds), 
+                "output" : copy(self.__external_out_heralds)}
         
     def add(self, circuit: Union["Circuit", "Unitary"], mode: int = 0,         # type: ignore - ignores Pylance warning raised by undefined unitary component
-            group: bool = False, name: str = "Circuit") -> None:
+            group: bool = False, name: str | None = None) -> None:
         """
         Can be used to add either another Circuit or a Unitary component to the
         existing circuit. This can either have the same size or be smaller than
         the circuit which is being added to.
         
         Args:
         
             circuit (Circuit | Unitary) : The circuit/component that is to be 
                 added.
                                                        
             mode (int, optional) : The first mode on which the circuit should 
                 be placed. If not specified it defaults to zero.
         """
-        if isinstance(circuit, Circuit):
-            self._mode_in_range(mode)
-            if mode + circuit.__n_modes > self.__n_modes:
-                raise ModeRangeError("Circuit to add is outside of mode range")
-            if group:
-                spec = unpack_circuit_spec(circuit.__circuit_spec)
+        if not isinstance(circuit, Circuit):
+            raise TypeError(
+                "Add method only supported for Circuit or Unitary objects.")
+        # Remap mode
+        mode = self._map_mode(mode)
+        self._mode_in_range(mode)
+        # Make copy of circuit to avoid modification
+        circuit_copy = circuit.copy()
+        # Use unpack groups and check if heralds are used
+        circuit_copy.unpack_groups()
+        spec = circuit_copy.__circuit_spec
+        # Force grouping if heralding included
+        if circuit_copy.heralds["input"]:
+            group = True
+        # When name not provided set this
+        if name is None:
+            spec = circuit.__circuit_spec
+            # Special case where name is retrieved from previous group
+            if len(spec) == 1 and spec[0][0] == "group":
+                name = spec[0][1][1]
+            # Otherwise default to circuit
             else:
-                spec = circuit.__circuit_spec
-            add_cs = self._add_mode_to_circuit_spec(spec, mode)
-            if not group:
-                self.__circuit_spec = self.__circuit_spec + add_cs
+                name = "Circuit"
+        # When grouping use unpacked circuit
+        if group:
+            circuit = circuit_copy
+        spec = circuit.__circuit_spec
+        # Check circuit size is valid
+        n_heralds = len(circuit.heralds["input"])
+        if mode + circuit.n_modes - n_heralds > self.n_modes:
+            raise ModeRangeError("Circuit to add is outside of mode range")
+        
+        # Include any existing internal modes into the circuit to be added
+        for i in sorted(self.__internal_modes):
+            # Need to account for shifts when adding new heralds
+            target_mode = i - mode
+            for m in circuit.heralds["input"]:
+                if target_mode > m:
+                    target_mode += 1
+            if 0 <= target_mode < circuit.n_modes:
+                spec = circuit._add_empty_mode(spec, target_mode)
+        # Then add new modes for heralds from circuit and also add swaps to
+        # enforce that the input and output herald are on the same mode
+        provisional_swaps = {}
+        for i, m in enumerate(sorted(circuit.heralds["input"])):
+            self.__circuit_spec = self._add_empty_mode(self.__circuit_spec, 
+                                                       mode + m)
+            self.__internal_modes.append(mode+m)
+            # Current limitation is that heralding should be on the same mode
+            # when adding, so use a mode swap to compensate for this.
+            herald_loc = list(circuit.heralds["input"].keys()).index(m)
+            out_herald = list(circuit.heralds["output"].keys())[herald_loc]
+            provisional_swaps[out_herald] = m
+        # Convert provisional swaps into full list and add to circuit
+        current_mode = 0
+        swaps = {}
+        # Loop over all modes in circuit to find swaps
+        for i in range(circuit.n_modes):
+            # If used as a key then take value from provisional swaps
+            if i in provisional_swaps.keys():
+                swaps[i] = provisional_swaps[i]
+            # Otherwise then map mode to lowest mode possible
             else:
-                self.__circuit_spec.append(["group", (add_cs, name, mode, 
-                                                      mode + 
-                                                      circuit.__n_modes - 1)])
+                while current_mode in provisional_swaps.values():
+                    current_mode += 1
+                if i != current_mode:
+                    swaps[i] = current_mode
+                current_mode += 1
+        # Skip for cases where swaps do not alter mode structure    
+        if list(swaps.keys()) != list(swaps.values()):
+            spec.append(["mode_swaps", (swaps, None)])
+        # Update heralds to enforce input and output are on the same mode
+        new_heralds = {"input" : circuit.heralds["input"],
+                       "output" : circuit.heralds["input"]}
+        # Also add all included heralds to the heralds dict
+        for m in new_heralds["input"]:
+            self.__in_heralds[m+mode] = new_heralds["input"][m]
+            self.__out_heralds[m+mode] = new_heralds["input"][m]
+        # And shift all components in circuit by required amount
+        add_cs = add_modes_to_circuit_spec(spec, mode)
+        
+        # Then add circuit spec, adjusting how this is included
+        if not group:
+            self.__circuit_spec = self.__circuit_spec + add_cs
         else:
-            raise TypeError(
-                "Add method only supported for Circuit or Unitary objects.")
-        
+            self.__circuit_spec.append(["group", (add_cs, name, mode, 
+                                                  mode + circuit.n_modes - 1,
+                                                  new_heralds)
+                                        ])
         return
     
     def add_bs(self, mode_1: int, mode_2: int = None, 
                reflectivity: float = 0.5, loss: float = 0,
                convention: str = "Rx") -> None:
         """
         Add a beam splitter of specified reflectivity between two modes to the 
@@ -165,16 +274,19 @@
             loss (float, optional) : The loss of the beam splitter, this should
                 be positive and given in dB.
                                      
             convention (str, optional) : The convention to use for the beam 
                 splitter, should be either "Rx" (the default value) or "H".
                 
         """
+        if mode_2 is None: 
+            mode_2 = mode_1 + 1
+        mode_1 = self._map_mode(mode_1)
         self._mode_in_range(mode_1)
-        if mode_2 is None: mode_2 = mode_1 + 1
+        mode_2 = self._map_mode(mode_2)
         if mode_1 == mode_2:
             raise ModeRangeError(
                 "Beam splitter must act across two different modes.")
         self._mode_in_range(mode_2)
         self._check_loss(loss)
         # Check correct convention is given
         all_convs = ["Rx", "H"]
@@ -200,14 +312,15 @@
             
             phi (float) : The angular phase shift to apply.
             
             loss (float, optional) : The loss of the phase shifter, this should
                 be positive and given in dB.
                                                    
         """
+        mode = self._map_mode(mode)
         self._mode_in_range(mode)
         self._check_loss(loss)
         self.__circuit_spec.append(["ps", (mode, phi)])
         if isinstance(loss, Parameter) or loss > 0:
             self.add_loss(mode, loss)
         
     def add_loss(self, mode: int, loss: float = 0) -> None:
@@ -218,14 +331,15 @@
         
             mode (int) : The mode on which the loss channel acts.
                         
             loss (float, optional) : The loss applied to the selected mode, 
                 this should be positive and given in dB.
                                                
         """
+        mode = self._map_mode(mode)
         self._mode_in_range(mode)
         self._check_loss(loss)
         self.__circuit_spec.append(["loss", (mode, loss)])
         
     def add_barrier(self, modes: list | None = None) -> None:
         """
         Adds a barrier to separate different parts of a circuit. This is 
@@ -234,15 +348,17 @@
         Args:
         
             modes (list | None) : The modes over which the barrier should be
                 applied to.
                 
         """
         if modes == None:
-            modes = [i for i in range(self.__n_modes)]
+            modes = [i for i in 
+                     range(self.n_modes-len(self.__internal_modes))]
+        modes = [self._map_mode(i) for i in modes]
         for m in modes:
             self._mode_in_range(m)
         self.__circuit_spec.append(["barrier", tuple([modes])])
         
     def add_mode_swaps(self, swaps: dict) -> None:
         """
         Performs swaps between a given set of modes. The keys of the dictionary
@@ -253,25 +369,66 @@
         
         Args:
         
             swaps (dict) : A dictionary detailing the original modes and the 
                 locations that they are to be swapped to. 
                            
         """
+        # Remap swap dict
+        swaps = {self._map_mode(mi) : self._map_mode(mo) 
+                 for mi, mo in swaps.items()}
         # Perform some error checking steps
         in_modes = sorted(list(swaps.keys()))
         out_modes = sorted(list(swaps.values()))
         if in_modes != out_modes:
             raise ValueError(
                 "Mode swaps not complete, dictionary keys and values should "
                 "contain the same modes.")
         for m in in_modes:
             self._mode_in_range(m)
         self.__circuit_spec.append(["mode_swaps", (swaps, None)])
         
+    def add_herald(self, n_photons: int, input_mode: int, 
+                   output_mode: int = None) -> None:
+        """
+        Add a herald across a selected input/output of the circuit. If only one
+        mode is specified then this will be used for both the input and output.
+        
+        Args:
+        
+            n_photons (int) : The number of photons to use for the heralding.
+            
+            input_mode (int) : The input mode to use for the herald.
+            
+            output_mode (int | None, optional) : The output mode for the 
+                herald, if this is not specified it will be set to the value of
+                the input mode.
+        
+        """
+        if not isinstance(n_photons, int) or isinstance(n_photons, bool):
+            raise TypeError(
+                "Number of photons for herald should be an integer.")
+        n_photons = int(n_photons)
+        if output_mode is None:
+            output_mode = input_mode
+        input_mode = self._map_mode(input_mode)
+        output_mode = self._map_mode(output_mode)
+        self._mode_in_range(input_mode)
+        self._mode_in_range(output_mode)
+        # Check if herald already used on input or output
+        if input_mode in self.__in_heralds:
+            raise ValueError("Heralding already set for chosen input mode.")
+        if output_mode in self.__out_heralds:
+            raise ValueError("Heralding already set for chosen output mode.")
+        # If not then update dictionaries
+        self.__in_heralds[input_mode] = n_photons
+        self.__out_heralds[output_mode] = n_photons
+        self.__external_in_heralds[input_mode] = n_photons
+        self.__external_out_heralds[output_mode] = n_photons
+        
     def display(self, show_parameter_values: bool = False, 
                 display_loss: bool = False, 
                 mode_labels: list | None = None,
                 display_type: str = "svg") -> None:
         """
         Displays the current circuit with parameters set using either their 
         current values or labels.
@@ -338,20 +495,27 @@
         """
         new_circ = Circuit(self.n_modes)
         if not freeze_parameters:
             new_circ.__circuit_spec = copy(self.__circuit_spec)
         else:
             copied_spec = deepcopy(self.__circuit_spec)
             new_circ.__circuit_spec = self._freeze_params(copied_spec)
+        new_circ.__in_heralds = copy(self.__in_heralds)
+        new_circ.__out_heralds = copy(self.__out_heralds)
+        new_circ.__external_in_heralds = copy(self.__external_in_heralds)
+        new_circ.__external_out_heralds = copy(self.__external_out_heralds)
         return new_circ
     
     def unpack_groups(self) -> None:
         """
         Unpacks any component groups which may have been added to the circuit.
         """
+        self.__internal_modes = []
+        self.__external_in_heralds = self.__in_heralds
+        self.__external_out_heralds = self.__out_heralds
         self.__circuit_spec = unpack_circuit_spec(self.__circuit_spec)
         return
         
     def compress_mode_swaps(self) -> None:
         """
         Takes a provided circuit spec and will try to compress any more swaps
         such that the circuit length is reduced. Note that any components in a 
@@ -385,35 +549,38 @@
         
         return circuit
     
     def _build_process(self) -> CompiledCircuit:
         """
         Contains full process for convert a circuit into a compiled one.
         """
-        circuit = CompiledCircuit(self.__n_modes)
+        circuit = CompiledCircuit(self.n_modes)
         
         for cs, params in unpack_circuit_spec(self.__circuit_spec):
             got_params = [p.get() if isinstance(p, Parameter) else p 
                           for p in params]
             if cs == "bs":
                 circuit.add_bs(*got_params)
             elif cs == "ps":
                 circuit.add_ps(*got_params)
             elif cs == "loss":
                 circuit.add_loss(*got_params)
             elif cs == "barrier":
-                circuit.add_barrier(got_params[0])
+                pass
             elif cs == "mode_swaps":
                 circuit.add_mode_swaps(got_params[0])
             elif cs == "unitary":
                 unitary = CompiledUnitary(params[1], params[2])
                 circuit.add(unitary, params[0])
             else:
                 raise CircuitCompilationError(
                     "Component in circuit spec not recognised.")
+        heralds = self.heralds
+        for i, o in zip(heralds["input"], heralds["output"]):
+            circuit.add_herald(heralds["input"][i], i, o)
         
         return circuit
     
     def _mode_in_range(self, mode: int) -> bool:
         """
         Check a mode exists within the created circuit and also confirm it is 
         an integer.
@@ -424,58 +591,62 @@
         elif isinstance(mode, bool): 
             raise TypeError("Mode number should be an integer.")
         elif not isinstance(mode, int):
             if int(mode) == mode:
                 mode = int(mode)
             else:
                 raise TypeError("Mode number should be an integer.")
-        if 0 <= mode < self.__n_modes:
+        if 0 <= mode < self.n_modes:
             return True
         else:
             raise ModeRangeError(
                 "Selected mode(s) is not within the range of the created "
                 "circuit.")
+            
+    def _map_mode(self, mode: int) -> int:
+        """
+        Maps a provided mode to the corresponding internal mode
+        """
+        for i in sorted(self.__internal_modes):
+            if mode >= i:
+                mode += 1
+        return mode
         
     def _check_loss(self, loss: float) -> bool:
         """
         Check that loss is positive and toggle _loss_included if not already 
         done.
         """
         if isinstance(loss, Parameter):
             loss = loss.get()
         if not isinstance(loss, Number) or isinstance(loss, bool):
             raise TypeError("Loss value should be numerical or a Parameter.")
         if loss < 0:
             raise ValueError("Provided loss values should be greater than 0.")
         else:
             return True
-        
-    def _add_mode_to_circuit_spec(self, circuit_spec: list, mode: int) -> list:
+    
+    def _add_empty_mode(self, circuit_spec: list, mode: int) -> list:
         """
-        Takes an existing circuit spec and adds a given number of modes to each
-        of the elements.
+        Adds an empty mode at the selected location to a provided circuit spec.
         """
-        new_circuit_spec = []
-        for c, params in circuit_spec:
-            params = list(params)
-            if c in ["bs"]:
-                params[0] = params[0] + mode
-                params[1] = params[1] + mode
-            elif c == "barrier":
-                params = [p+mode for p in params[0]]
-                params = tuple([params])
-            elif c == "mode_swaps":
-                params[0] = {k+mode:v+mode for k,v in params[0].items()}
-            elif c == "group":
-                params[0] = self._add_mode_to_circuit_spec(params[0], mode)
-                params[2] += mode
-                params[3] += mode
-            else:
-                params[0] = params[0] + mode
-            new_circuit_spec.append([c, tuple(params)])
+        self.__n_modes += 1
+        new_circuit_spec = add_empty_mode_to_circuit_spec(circuit_spec, mode)
+        # Also modify heralds as required
+        to_modify = ["__in_heralds", "__out_heralds", 
+                     "__external_in_heralds", "__external_out_heralds"]
+        for tm in to_modify:
+            new_heralds = {}
+            for m, n in getattr(self, "_Circuit" + tm).items():
+                m += 1 if m >= mode else 0
+                new_heralds[m] = n
+            setattr(self, "_Circuit" + tm, new_heralds)
+        # Add internal mode storage
+        self.__internal_modes = [m + 1 if m >= mode else m 
+                                 for m in self.__internal_modes]
         return new_circuit_spec
         
     def _get_display_spec(self) -> list:
         """
         Creates a parameterized version of the circuit build spec using the 
         included components.
         """
@@ -505,15 +676,15 @@
                 display_spec.append(("mode_swaps", cparams[0], None))
             elif cs == "unitary":
                 nm = params[1].shape[0]
                 display_spec.append(("unitary", [cparams[0], cparams[0]+nm-1], 
                                      params[2]))
             elif cs == "group":
                 display_spec.append(("group", [params[2], params[3]], 
-                                   (params[1])))
+                                   (params[1], params[4])))
             else:
                 raise DisplayError("Component in circuit spec not recognised.")
             
         return display_spec
     
     def _freeze_params(self, spec: list|tuple) -> list|tuple:
         """
```

### Comparing `lightworks-1.2.0/lightworks/sdk/circuit/circuit_compiler.py` & `lightworks-1.3.0/lightworks/sdk/circuit/circuit_compiler.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from ..utils import permutation_mat_from_swaps_dict
 from ..visualisation import Display
 
 from typing import Any
 import numpy as np
 import matplotlib.pyplot as plt
 from IPython import display
+from copy import copy
 
 
 class CompiledCircuit:
     """
     Used for building an arbitrary photonic circuit from a set of fundamental 
     components, creating the unitary matrices which represent each component
     and combining them together. This class is not intended to be directly 
@@ -56,30 +57,31 @@
     def __init__(self, n_modes: int) -> None:
         
         if not isinstance(n_modes, int):
             if int(n_modes) == n_modes:
                 n_modes = int(n_modes)
             else:
                 raise TypeError("Number of modes should be an integer.")
-        self.n_modes = n_modes
+        self._n_modes = n_modes
         self._loss_included = False
         self.U = np.identity(n_modes, dtype = complex)
         self.U_full = np.identity(n_modes, dtype = complex)
         self._loss_modes = 0
-        self._display_spec = []
+        self._in_heralds = {}
+        self._out_heralds = {}
         
         return
     
     def __add__(self, value: "CompiledCircuit") -> "CompiledCircuit":
         """Method for addition of two circuits."""
         if isinstance(value, CompiledCircuit):
             if self.n_modes != value.n_modes:
                 raise ModeRangeError(
                     "Mismatch in number of circuit modes, used add method to "
-                    "add a circuits of a different size.")
+                    "add circuits of a different size.")
             nm = self.n_modes
             newU = value.U @ self.U 
             loss = self._loss_included or value._loss_included
             if loss:
                 l1 = self._loss_modes
                 l2 = value._loss_modes
                 newU_full = np.identity(nm + l1 + l2, dtype=complex)
@@ -96,38 +98,38 @@
                 l1, l2 = 0, 0
             # Create a new circuit and manually assign attributes
             newCirc = CompiledCircuit(nm)
             newCirc._loss_included = loss
             newCirc.U = newU
             newCirc.U_full = newU_full
             newCirc._loss_modes = l1 + l2
-            newCirc._display_spec = self._display_spec + value._display_spec
             return newCirc
         else:
             raise TypeError("Addition only supported between two circuits.")
         
-    def __setattr__(self, __name: str, __value: Any) -> None:
-        # Prevent n_modes attribute being changed after creation
-        if __name == "n_modes":
-            if not hasattr(self, "n_modes"):
-                self.__dict__[__name] = __value
-            else:
-                raise AttributeError(
-                    "Number of modes should not be modified after Circuit "
-                    "creation.")
-        else:
-            super().__setattr__(__name, __value)
-            
+    @property
+    def n_modes(self) -> int:
+        return self._n_modes
+
+    @n_modes.setter
+    def n_modes(self, value: Any) -> None:
+        raise AttributeError(
+            "Number of modes should not be modified after Circuit creation.")
+        
     @property
     def loss_modes(self):
         """Returns number of loss modes used in the circuit."""
         return self._loss_modes
+    
+    @property
+    def heralds(self) -> dict:
+        return {"input" : copy(self._in_heralds), 
+                "output" : copy(self._out_heralds)}
         
-    def add(self, circuit: "CompiledCircuit", mode: int, group: bool = False, 
-            name: str = "Circuit") -> None:
+    def add(self, circuit: "CompiledCircuit", mode: int) -> None:
         """
         Add a circuit which is of a different size (but smaller than) the 
         original circuit.
         
         Args:
         
             circuit (Circuit) : The smaller circuit which is to be added onto
@@ -166,41 +168,25 @@
             new_U_full = np.identity(self.n_modes+lm, dtype=complex)
             new_U_full[mode:mode+nm, mode:mode+nm] = Uc_full[:nm, :nm]
             new_U_full[self.n_modes:, self.n_modes:] = Uc_full[nm:, nm:]
             new_U_full[mode:mode+nm, self.n_modes:] = Uc_full[:nm, nm:]
             new_U_full[self.n_modes:, mode:mode+nm] = Uc_full[nm:, :nm]
         else:
             new_U_full = new_U.copy()
-        # Modify build spec of circuit to add so it is the same size
-        if not group:
-            new_display_spec = []
-            for spec in circuit._display_spec:
-                c, cmodes, params = spec
-                if isinstance(cmodes, int):
-                    cmodes = cmodes + mode
-                elif isinstance(cmodes, list):
-                    cmodes = [mode + m for m in cmodes]
-                elif isinstance(cmodes, dict):
-                    cmodes = {mode+im:mode+om for im, om in cmodes.items()}
-                new_display_spec += [(c, cmodes, params)]
-        # Otherwise set build spec to be grouped object
-        else:
-            new_display_spec = [("group", [mode, mode+nm-1], (name))]
         # Assign modified attributes to circuit to add
         to_add = CompiledCircuit(self.n_modes)
         to_add.U = new_U
         to_add.U_full = new_U_full
-        to_add._display_spec = new_display_spec
         to_add._loss_included = circuit._loss_included
         to_add._loss_modes = circuit._loss_modes
         # Use built in addition function to combine the circuit
         new_circuit = self + to_add
         # Copy created attributes from new circuit
         for k in self.__dict__.keys():
-            self.__dict__[k] = new_circuit.__dict__[k]
+            setattr(self, k, getattr(new_circuit, k))
             
         return
     
     def add_bs(self, mode_1: int, mode_2: int | None = None, 
                reflectivity: float = 0.5, convention: str = "Rx") -> None:
         """
         Function to add a beam splitter of specified reflectivity between two 
@@ -255,17 +241,14 @@
                 arr[mode_1, mode_1] = np.cos(theta)
                 arr[mode_1, mode_2] = np.sin(theta)
                 arr[mode_2, mode_1] = np.sin(theta)
                 arr[mode_2, mode_2] = -np.cos(theta)
         # Update unitaries
         self.U = U_bs @ self.U
         self.U_full = U_bs_full @ self.U_full
-        # Update build spec attribute
-        self._display_spec = self._display_spec + [("BS", [mode_1, mode_2], 
-                                                   (reflectivity))]
         return
     
     def add_ps(self, mode: int, phi: float) -> None:
         """
         Applies a phase shift to a given mode in the circuit.
         
         Args:
@@ -280,16 +263,14 @@
         U_ps = np.identity(self.n_modes, dtype=complex)
         U_ps[mode, mode] = np.exp(1j*phi)
         U_ps_full = np.identity(self.n_modes+self.loss_modes, dtype=complex)
         U_ps_full[mode, mode] = np.exp(1j*phi)
         self.U = U_ps @ self.U
         # Calculate U_full with loss
         self.U_full = U_ps_full @ self.U_full
-        # Update build spec attribute
-        self._display_spec = self._display_spec + [("PS", mode, (phi))]
         return
     
     def add_loss(self, mode: int, loss: float = 0) -> None:
         """
         Adds a loss channel to the specified mode of the circuit.
         
         Args:
@@ -316,37 +297,14 @@
             if loss > 0:
                 U_lc = self._loss_mat(mode_total, mode, mode_total-1, loss)
             else:
                 U_lc = np.identity(mode_total, dtype = complex)
         else:
             U_full = self.U_full
         self.U_full = U_lc @ U_full
-        # Update build spec attributes
-        if loss > 0:
-            self._display_spec = self._display_spec + [("LC", mode, (loss))]
-        return
-    
-    def add_barrier(self, modes: list | None = None) -> None:
-        """
-        Adds a barrier to separate different parts a the circuit. This is 
-        applied to the specified modes.
-        
-        Args:
-        
-            modes (list | None) : The modes over which the barrier should be
-                applied to.
-                
-        """
-        if modes == None:
-            modes = [i for i in range(self.n_modes)]
-        if type(modes) != list:
-            raise TypeError("Modes to apply barrier to should be a list.")
-        for m in modes:
-            self._mode_in_range(m)
-        self._display_spec = self._display_spec + [("barrier", modes, None)]
         return
     
     def add_mode_swaps(self, swaps: dict) -> None:
         """
         Performs swaps between a given set of modes. The keys of the dictionary
         should correspond to the initial modes and the values to the modes they
         are swapped to. It is also required that all mode swaps are complete,
@@ -374,50 +332,50 @@
         U = permutation_mat_from_swaps_dict(swaps, self.n_modes)
         # Expand to include loss modes
         U_full = np.identity(self.n_modes + self._loss_modes, dtype=complex)
         U_full[:self.n_modes, :self.n_modes] = U[:, :]
         # Combine with existing matrices
         self.U = U @ self.U
         self.U_full = U_full @ self.U_full
-        self._display_spec = self._display_spec + [("mode_swaps", swaps, 
-                                                    None)]
 
         return
     
-    def display(self, display_loss: bool = False, 
-                mode_labels: list | None = None, 
-                display_type: str = "svg") -> None:
+    def add_herald(self, n_photons: int, input_mode: int, 
+                   output_mode: int = None) -> None:
         """
-        Displays the current circuit.
+        Add a herald across a selected input/output of the circuit. If only one
+        mode is specified then this will be used for both the input and output.
         
         Args:
         
-            display_loss (bool, optional) : Choose whether to display loss
-                components in the figure, defaults to False.
-                                            
-            mode_labels (list|None, optional) : Optionally provided a list of 
-                mode labels which will be used to name the mode something other
-                than numerical values. Can be set to None to use default 
-                values.
-                                                
-            display_type (str, optional) : Selects whether the drawsvg or 
-                matplotlib module should be used for displaying the circuit. 
-                Should either be 'svg' or 'mpl', defaults to 'svg'.
-                
-        """
-        
-        return_ = Display(self, display_loss = display_loss, 
-                          mode_labels = mode_labels,
-                          display_type = display_type)
-        if display_type == "mpl":
-            plt.show()
-        elif display_type == "svg":
-            display.display(return_)
+            n_photons (int) : The number of photons to use for the heralding.
+            
+            input_mode (int) : The input mode to use for the herald.
+            
+            output_mode (int | None, optional) : The output mode for the 
+                herald, if this is not specified it will be set to the value of
+                the input mode.
         
-        return
+        """
+        if not isinstance(n_photons, int) or isinstance(n_photons, bool):
+            raise TypeError(
+                "Number of photons for herald should be an integer.")
+        n_photons = int(n_photons)
+        if output_mode is None:
+            output_mode = input_mode
+        self._mode_in_range(input_mode)
+        self._mode_in_range(output_mode)
+        # Check if herald already used on input or output
+        if input_mode in self._in_heralds:
+            raise ValueError("Heralding already set for chosen input mode.")
+        if output_mode in self._out_heralds:
+            raise ValueError("Heralding already set for chosen output mode.")
+        # If not then update dictionaries
+        self._in_heralds[input_mode] = n_photons
+        self._out_heralds[output_mode] = n_photons
     
     def _grow_unitary(self, U: np.ndarray, n: int) -> np.ndarray:
         """Function to grow a unitary by a given n modes"""
         ns = U.shape[0]
         Ug = np.identity(ns + n, dtype = complex)
         Ug[:ns, :ns] = U
         return Ug
@@ -481,14 +439,12 @@
         if not isinstance(label, str):
             raise TypeError("Label for unitary should be a string.")
         
         # Also check label
         # Assign attributes of unitary
         self.U = unitary
         self.U_full = unitary
-        self.n_modes = unitary.shape[0]
+        self._n_modes = unitary.shape[0]
         self._loss_included = False
         self._loss_modes = 0
-        # Will need to add unitary to build spec
-        self._display_spec = [("unitary", [0, self.n_modes-1], label)]
         
         return
```

### Comparing `lightworks-1.2.0/lightworks/sdk/circuit/parameters.py` & `lightworks-1.3.0/lightworks/sdk/circuit/parameters.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/sdk/circuit/unitary.py` & `lightworks-1.3.0/lightworks/sdk/circuit/unitary.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Dedicated unitary component for implement unitary matrices on a circuit.
+Dedicated unitary component for implementing unitary matrices on a circuit.
 """
 
 from .circuit import Circuit
 from ..utils import check_unitary
 
 import numpy as np
```

### Comparing `lightworks-1.2.0/lightworks/sdk/optimisation/__init__.py` & `lightworks-1.3.0/lightworks/sdk/optimisation/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/sdk/optimisation/optimisation.py` & `lightworks-1.3.0/lightworks/sdk/optimisation/optimisation.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/sdk/qubit/__init__.py` & `lightworks-1.3.0/lightworks/qubit/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,9 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .single_qubit_gates import H, X, Y, Z, S, T
-from .two_qubit_gates import CZ, CNOT, CZ_Heralded, CNOT_Heralded
+from .gates import H, X, Y, Z, S, T, CZ, CNOT, CZ_Heralded, CNOT_Heralded
+
+__all__ = ["H", "X", "Y", "Z", "S", "T", "CZ", "CNOT", "CZ_Heralded", 
+           "CNOT_Heralded"]
```

### Comparing `lightworks-1.2.0/lightworks/sdk/qubit/single_qubit_gates.py` & `lightworks-1.3.0/lightworks/qubit/gates/single_qubit_gates.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """
 Contains a variety of qubit components, designed for implementing required 
 qubit processing functionality in lightworks.
 """
 
-from ..circuit import Unitary
+from ...sdk.circuit import Unitary
 
 import numpy as np
 
 class H(Unitary):
     """
     Implements a Hadamard across a pair of modes corresponding to a dual-rail 
     encoded qubit.
```

### Comparing `lightworks-1.2.0/lightworks/sdk/qubit/two_qubit_gates.py` & `lightworks-1.3.0/lightworks/qubit/gates/two_qubit_gates.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,37 +14,41 @@
 
 """
 Contains a variety of two qubit components, designed for implementing required 
 qubit processing functionality in lightworks.
 """
 
 from .single_qubit_gates import H
-from ..circuit import Unitary, Circuit
-from ..utils import permutation_mat_from_swaps_dict
+from ...sdk.circuit import Unitary, Circuit
+from ...sdk.utils import permutation_mat_from_swaps_dict
 
 import numpy as np
 
-class CZ(Unitary):
+class CZ(Circuit):
     """
     Post-selected CZ gate that acts across two dual-rail encoded qubits. This 
     gate occupies a total of 6 modes, where modes 0 & 5 are used for 0 photon
     heralds, modes 1 & 2 correspond to the 0 & 1 states of the control qubit 
     and modes 3 & 4 correspond to the 0 & 1 states of the target qubit. This
     gate requires additional post-selection in which only one photon should be 
     measured across each of the pairs of modes which encode a qubit.    
     """
     def __init__(self) -> None:
             
-        u_bs = np.array([[-1,2**0.5],[2**0.5,1]])/3**0.5
-        unitary = np.identity(6, dtype = complex)
+        U_bs = np.array([[-1,2**0.5],[2**0.5,1]])/3**0.5
+        U = np.identity(6, dtype = complex)
         for i in range(0,6,2):
-            unitary[i:i+2,i:i+2] = u_bs[:,:]
-        unitary[3,:] = -unitary[3,:]
+            U[i:i+2,i:i+2] = U_bs[:,:]
+        U[3,:] = -U[3,:]
+        unitary = Unitary(U, label = "CZ")
+        unitary.add_herald(0, 0, 0)
+        unitary.add_herald(0, 5, 5)
         
-        super().__init__(unitary, "CZ")
+        super().__init__(4)
+        self.add(unitary, 0, group = True, name = "CZ")
         
     def show_layout(self):
         """
         Shows the mode layout of the selected gate, detailing the location of
         the qubits and modes used for post-selection/heralding as well as 
         photon numbers on these modes.
         """
@@ -66,21 +70,21 @@
     heralds, modes 1 & 2 correspond to the 0 & 1 states of the control qubit 
     and modes 3 & 4 correspond to the 0 & 1 states of the target qubit. This
     gate requires additional post-selection in which only one photon should be 
     measured across each of the pairs of modes which encode a qubit.
     """
     def __init__(self) -> None:
         
-        super().__init__(6)
+        super().__init__(4)
         
         # Create CNOT from combination of H and CZ
-        circ = Circuit(6)
-        circ.add(H(), 3)
+        circ = Circuit(4)
+        circ.add(H(), 2)
         circ.add(CZ(), 0)
-        circ.add(H(), 3)
+        circ.add(H(), 2)
         
         self.add(circ, 0, group = True, name = "CNOT")
         
     def show_layout(self):
         """
         Shows the mode layout of the selected gate, detailing the location of
         the qubits and modes used for post-selection/heralding as well as 
@@ -93,53 +97,60 @@
         c1 --|  CNOT  |--   _|
         t0 --|        |--    | 1 photon
         t1 --|        |--   _|
          0 --|________|-- 0 
         """
         print(rep)
         
-class CZ_Heralded(Unitary):
+class CZ_Heralded(Circuit):
     """
     Heralded version of the CZ gate which acts across two dual-rail encoded 
     qubits, using two NS gates with ancillary photons to herald the success of 
     the transformation. This gate occupies 8 modes, where modes 0 & 7 are used 
     as 0 photon heralds, modes 1 & 6 are used as 1 photon heralds, mode 2 & 3
     correspond to the 0 & 1 states of the control qubit and modes 4 & 5 
     correspond to the 0 & 1 states of the target qubit. The heralded gate does
     not require any post-selection on the output qubits, other than that they
     are not lost (i.e a total of 4 photons should be measured at the output
     of the system), allowing it to be cascaded with other two qubit gates.
     """
     def __init__(self) -> None:
         
-        unitary = np.identity(8, dtype = complex)
+        U = np.identity(8, dtype = complex)
         
         U_ns = np.array([[1-2**0.5, 2**-0.25, (3/(2**0.5) - 2)**0.5],
                          [2**-0.25, 0.5, 0.5 - 2**-0.5],
                          [(3/(2**0.5) - 2)**0.5, 0.5 - 2**-0.5, 2**0.5 - 0.5]])
-        unitary[1:4, 1:4] = np.flip(U_ns, axis=(0,1))[:,:]
-        unitary[4:7, 4:7] = U_ns[:,:]
+        U[1:4, 1:4] = np.flip(U_ns, axis=(0,1))[:,:]
+        U[4:7, 4:7] = U_ns[:,:]
         # Apply pi phase shifts on mode 3
-        unitary[:,3] = -unitary[:,3]
+        U[:,3] = -U[:,3]
         
         # Define beam splitter action
         U_bs = np.identity(8, dtype=complex)
         U_bs[3,3] = 1/2**0.5
         U_bs[4,4] = 1/2**0.5
         U_bs[3,4] = 1j/2**0.5
         U_bs[4,3] = 1j/2**0.5
         
         # Define mode reconfiguration so qubits are on central 4 modes
         swaps = {2:0, 0:1, 1:2, 5:7, 7:6, 6:5}
         U_perm1 = permutation_mat_from_swaps_dict(swaps, 8)
         U_perm2 = np.conj(U_perm1.T)
         
-        unitary = U_perm2 @ U_bs @ unitary @ U_bs @ U_perm1
+        U = U_perm2 @ U_bs @ U @ U_bs @ U_perm1
         
-        super().__init__(unitary, "CZ (Heralded)")
+        unitary = Unitary(U)
+        unitary.add_herald(0, 0, 0)
+        unitary.add_herald(1, 1, 1)
+        unitary.add_herald(1, 6, 6)
+        unitary.add_herald(0, 7, 7)
+        
+        super().__init__(4)
+        self.add(unitary, 0, group = True, name = "CZ")
         
     def show_layout(self):
         """
         Shows the mode layout of the selected gate, detailing the location of
         the qubits and modes used for post-selection/heralding as well as 
         photon numbers on these modes.
         """
@@ -166,21 +177,21 @@
     correspond to the 0 & 1 states of the target qubit. The heralded gate does
     not require any post-selection on the output qubits, other than that they
     are not lost (i.e a total of 4 photons should be measured at the output
     of the system), allowing it to be cascaded with other two qubit gates.
     """
     def __init__(self) -> None:
         
-        super().__init__(8)
+        super().__init__(4)
         
         # Create CNOT from combination of H and CZ
-        circ = Circuit(8)
-        circ.add(H(), 4)
+        circ = Circuit(4)
+        circ.add(H(), 2)
         circ.add(CZ_Heralded(), 0)
-        circ.add(H(), 4)
+        circ.add(H(), 2)
         
         self.add(circ, 0, group = True, name = "CNOT (Heralded)")
         
     def show_layout(self):
         """
         Shows the mode layout of the selected gate, detailing the location of
         the qubits and modes used for post-selection/heralding as well as
```

### Comparing `lightworks-1.2.0/lightworks/sdk/state/__init__.py` & `lightworks-1.3.0/lightworks/sdk/state/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/sdk/state/state.py` & `lightworks-1.3.0/lightworks/sdk/state/state.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/sdk/utils/__init__.py` & `lightworks-1.3.0/lightworks/sdk/utils/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .matrix_utils import check_unitary, random_unitary, random_permutation
+from .matrix_utils import (check_unitary, random_unitary, random_permutation,
+                           add_mode_to_unitary)
 from .state_utils import fock_basis, state_to_string
 from .exceptions import *
 from .conversion import db_loss_to_transmission, transmission_to_db_loss
 from .permutation_conversion import permutation_mat_from_swaps_dict
 from .circuit_utils import unpack_circuit_spec
 from .circuit_utils import convert_non_adj_beamsplitters
-from .circuit_utils import compress_mode_swaps
+from .circuit_utils import compress_mode_swaps, add_empty_mode_to_circuit_spec
+from .circuit_utils import add_modes_to_circuit_spec
+from .heralding_utils import add_heralds_to_state, remove_heralds_from_state
```

### Comparing `lightworks-1.2.0/lightworks/sdk/utils/conversion.py` & `lightworks-1.3.0/lightworks/sdk/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/sdk/utils/exceptions.py` & `lightworks-1.3.0/lightworks/sdk/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/sdk/utils/matrix_utils.py` & `lightworks-1.3.0/lightworks/sdk/utils/matrix_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -123,8 +123,35 @@
                 np.imag(product[i,j]) > precision):
                 unitary = False
             # Off diagonals
             elif i != j and (np.real(product[i,j] > precision) or 
                 np.imag(product[i,j]) > precision):
                 unitary = False
     # Return whether matrix is unitary or not
-    return unitary
+    return unitary
+
+def add_mode_to_unitary(unitary: np.ndarray, add_mode: int) -> np.ndarray:
+    """
+    Adds a new mode (through inclusion of an extra row/column) to the provided 
+    unitary at the selected location.
+    
+    Args:
+    
+        unitary (np.ndarray) : The unitary to add a mode to.
+        
+        add_mode (int) : The location at which a new mode should be added to 
+            the circuit.
+            
+    Returns:
+    
+        np.ndarray : The converted unitary matr
+    
+    """
+    dim = unitary.shape[0] + 1
+    new_U = np.identity(dim, dtype = complex)
+    # Diagonals
+    new_U[:add_mode, :add_mode] = unitary[:add_mode, :add_mode]
+    new_U[add_mode+1:, add_mode+1:] = unitary[add_mode:, add_mode:]
+    # Off-diagonals
+    new_U[:add_mode, add_mode+1:] = unitary[:add_mode, add_mode:]
+    new_U[add_mode+1:, :add_mode] = unitary[add_mode:, :add_mode]
+    return new_U
```

### Comparing `lightworks-1.2.0/lightworks/sdk/utils/permutation_conversion.py` & `lightworks-1.3.0/lightworks/sdk/utils/permutation_conversion.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/sdk/utils/state_utils.py` & `lightworks-1.3.0/lightworks/sdk/utils/state_utils.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/sdk/visualisation/__init__.py` & `lightworks-1.3.0/lightworks/sdk/visualisation/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/sdk/visualisation/display.py` & `lightworks-1.3.0/lightworks/sdk/visualisation/display.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/lightworks/sdk/visualisation/display_components_mpl.py` & `lightworks-1.3.0/lightworks/sdk/visualisation/display_components_mpl.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,18 +29,18 @@
     
     def _add_ps(self, mode: int, phi: float) -> None:
         """Add a phase shifter to the axis."""
         # Set size of phase shifter box and length of connector
         size = 0.5
         con_length = 0.5
         # Get x and y locs of target modes
-        xloc = self.locations[mode]
-        yloc = mode
+        xloc = self.x_locations[mode]
+        yloc = self.y_locations[mode]
         # Add input waveguides
-        self._add_wg(xloc, mode, con_length)
+        self._add_wg(xloc, yloc, con_length)
         xloc += con_length
         # Add phase shifter square
         rect = patches.Rectangle((xloc, yloc-size/2), size, size, 
                                  facecolor = "#e8532b", edgecolor = "black")
         self.ax.add_patch(rect)
         # Include text to label applied phase shift
         self.ax.text(xloc + size/2, yloc, "PS", horizontalalignment = "center", 
@@ -70,37 +70,39 @@
             phi_text = "$\\phi =$ " + phi
         self.ax.text(xloc + size/2, yloc + size/2 + 0.15, 
                      phi_text, color= "black", size = 5,
                      horizontalalignment = "center", 
                      verticalalignment = "center")
         xloc += size
         # Add output waveguides
-        self._add_wg(xloc, mode, con_length)
+        self._add_wg(xloc, yloc, con_length)
         # Update mode locations list
-        self.locations[mode] = xloc + con_length
+        self.x_locations[mode] = xloc + con_length
         
         return
     
     def _add_bs(self, mode1: int, mode2: int, ref: float) -> None:
         """Add a beam splitter across to provided modes to the axis."""
         size_x = 0.5 # x beam splitter size
         con_length = 0.5 # input/output waveguide length
         offset = 0.5 # Offset of beam splitter shape from mode centres
-        size_y = offset + abs(mode2 - mode1) # Find y size
+        size_y = offset + abs(self.y_locations[mode2] - 
+                              self.y_locations[mode1]) # Find y size
         # Get x and y locations
-        yloc = min(mode1, mode2)
-        xloc = max(self.locations[mode1:mode2+1])
+        yloc = self.y_locations[min(mode1, mode2)]
+        xloc = max(self.x_locations[mode1:mode2+1])
         # Add initial connectors for any modes which haven't reach xloc yet:
-        for i, loc in enumerate(self.locations[mode1:mode2+1]):
-            if loc < xloc:
-                self._add_wg(loc, yloc + i, xloc - loc)
+        for i, loc in enumerate(self.x_locations[mode1:mode2+1]):
+            if loc < xloc and i+mode1 not in self.herald_modes:
+                self._add_wg(loc, self.y_locations[i+mode1], xloc - loc)
         # Add input waveguides for all included modes
         modes = range(min(mode1, mode2), max(mode1, mode2) + 1, 1)
         for i in modes:
-            self._add_wg(xloc, i, con_length)
+            if i not in self.herald_modes:
+                self._add_wg(xloc, self.y_locations[i], con_length)
         xloc += con_length
         # Add beam splitter rectangle shape
         rect = patches.Rectangle((xloc, yloc-offset/2), size_x, size_y, 
                                  facecolor = "#3e368d", alpha = 1, 
                                  edgecolor = "black")
         self.ax.add_patch(rect)
         # Label beam splitter as BS and display reflectivity
@@ -111,37 +113,36 @@
             ref = round(ref, 4)
         self.ax.text(xloc + size_x/2, yloc + size_y - offset/2 + 0.15, 
                      f"$r =$ {ref}", color= "black", size = 5,
                      horizontalalignment = "center", 
                      verticalalignment = "center")
         # For any modes in between the beam splitter modes add a waveguide 
         # across the beam splitter
-        if mode2 - mode1 > 1:
-            for i in range(mode1+1, mode2):
-                self._add_wg(xloc, i, size_x)
+        for i in range(mode1+1, mode2):
+            if i not in self.herald_modes:
+                self._add_wg(xloc, self.y_locations[i], size_x)
         xloc += size_x
-        # Add output waveguides
-        for i in modes:
-            self._add_wg(xloc, i, con_length)
-        # Update mode locations
+        # Add output waveguides and update mode locations
         for i in modes:
-            self.locations[i] = xloc + con_length
+            if i not in self.herald_modes:
+                self._add_wg(xloc, self.y_locations[i], con_length)
+            self.x_locations[i] = xloc + con_length
             
         return
     
     def _add_loss(self, mode: int, loss: float) -> None:
         """Add a loss channel to the specified mode"""
         # Set size of loss element and input/output waveguide length
         size = 0.5
         con_length = 0.5
         # Get x and y locations
-        xloc = self.locations[mode]
-        yloc = mode
+        xloc = self.x_locations[mode]
+        yloc = self.y_locations[mode]
         # Add an input waveguide
-        self._add_wg(xloc, mode, con_length)
+        self._add_wg(xloc, yloc, con_length)
         xloc += con_length
         # Add loss elements
         rect = patches.Rectangle((xloc, yloc-size/2), size, size, 
                                  facecolor = "grey", edgecolor = "black")
         self.ax.add_patch(rect)
         # Label element and add text will loss amount in dB
         self.ax.text(xloc + size/2, yloc, "L", horizontalalignment = "center", 
@@ -152,55 +153,57 @@
             loss_text = "$loss =$ " + loss
         self.ax.text(xloc + size/2, yloc + size/2 + 0.15, 
                      loss_text, color = "black", 
                      size = 5, horizontalalignment = "center", 
                      verticalalignment = "center")
         xloc += size
         # Add output waveguide
-        self._add_wg(xloc, mode, con_length)
+        self._add_wg(xloc, yloc, con_length)
         # Update mode position
-        self.locations[mode] = xloc + con_length
+        self.x_locations[mode] = xloc + con_length
         
         return
     
     def _add_barrier(self, modes: list) -> None:
         """
         Add a barrier which will separate different parts of the circuit. This
         is applied to the provided modes.
         """
         max_loc = 0
         for m in modes:
-            max_loc = max(max_loc, self.locations[m])
+            max_loc = max(max_loc, self.x_locations[m])
         for m in modes:
-            loc = self.locations[m]
+            loc = self.x_locations[m]
             if loc < max_loc:
-                self._add_wg(loc, m, max_loc - loc)
-            self.locations[m] = max_loc
+                self._add_wg(loc, self.y_locations[m], max_loc - loc)
+            self.x_locations[m] = max_loc
         
         return
     
     def _add_mode_swaps(self, swaps: dict) -> None:
         """Add mode swaps between provided modes to the axis."""
         size_x = 1 # x beam splitter size
         con_length = 0.25 # input/output waveguide length
         min_mode = min(swaps)
         max_mode = max(swaps)
         # Get x and y locations
-        xloc = max(self.locations[min_mode:max_mode+1])
+        xloc = max(self.x_locations[min_mode:max_mode+1])
         ylocs = []
         for i, j in swaps.items():
-            ylocs.append((i, j))
+            if i not in self.herald_modes:
+                ylocs.append((self.y_locations[i], self.y_locations[j]))
         # Add initial connectors for any modes which haven't reach xloc yet:
-        for i, loc in enumerate(self.locations[min_mode:max_mode+1]):
-            if loc < xloc:
-                self._add_wg(loc, min_mode + i, xloc - loc)
+        for i, loc in enumerate(self.x_locations[min_mode:max_mode+1]):
+            if loc < xloc and i + min_mode not in self.herald_modes:
+                self._add_wg(loc, self.y_locations[min_mode + i], xloc - loc)
         # Add input waveguides for all included modes
         modes = range(min_mode, max_mode + 1, 1)
         for i in modes:
-            self._add_wg(xloc, i, con_length)
+            if i not in self.herald_modes:
+                self._add_wg(xloc, self.y_locations[i], con_length)
         xloc += con_length
         for y0, y1 in ylocs:
             w = self.wg_width/2
             if y0 < y1:
                 dx1 = w*np.arctan(abs(y1-y0)/size_x)
                 dx2 = 0
             else:
@@ -209,93 +212,136 @@
             points = [(xloc+dx1, y0-w), (xloc, y0-w), (xloc, y0+w), 
                       (xloc+dx2, y0+w), (xloc+size_x-dx1, y1+w), 
                       (xloc+size_x, y1+w), (xloc+size_x, y1-w),
                       (xloc+size_x-dx2, y1-w)]
             poly = patches.Polygon(points, facecolor = "black")
             self.ax.add_patch(poly)
         xloc += size_x
-        # Add output waveguides
+        # Add output waveguides update mode locations
         for i in modes:
-            self._add_wg(xloc, i, con_length)
-        # Update mode locations
-        for i in modes:
-            self.locations[i] = xloc + con_length
+            if i not in self.herald_modes:
+                self._add_wg(xloc, self.y_locations[i], con_length)
+            self.x_locations[i] = xloc + con_length
             
         return
     
     def _add_unitary(self, mode1: int, mode2: int, label: str) -> None:
         """Add a unitary representation to the axis."""
         size_x = 1 # Unitary x size
         con_length = 0.5 # Input/output waveguide lengths
         offset = 0.5 # Offset of unitary square from modes
-        size_y = offset + abs(mode2 - mode1) # Find total unitary size
+        size_y = offset + abs(self.y_locations[mode2] - 
+                              self.y_locations[mode1]) # Find total unitary size
         # Get x and y positions
-        yloc = min(mode1, mode2)
-        xloc = max(self.locations[mode1:mode2+1])
+        yloc = self.y_locations[min(mode1, mode2)]
+        xloc = max(self.x_locations[mode1:mode2+1])
         # Add initial connectors for any modes which haven't reach xloc yet:
-        for i, loc in enumerate(self.locations[mode1:mode2+1]):
-            if loc < xloc:
-                self._add_wg(loc, yloc + i, xloc - loc)
+        for i, loc in enumerate(self.x_locations[mode1:mode2+1]):
+            if loc < xloc and i + mode1 not in self.herald_modes:
+                self._add_wg(loc, self.y_locations[i+mode1], xloc - loc)
         # Add input waveguides
         modes = range(min(mode1, mode2), max(mode1, mode2)+1, 1)
         for i in modes:
-            self._add_wg(xloc, i, con_length)
+            if i not in self.herald_modes:
+                self._add_wg(xloc, self.y_locations[i], con_length)
         xloc += con_length
         # Add unitary shape and label
         rect = patches.Rectangle((xloc, yloc-offset/2), size_x, size_y, 
                                  facecolor = "#1a0f36", 
                                  edgecolor = "black")
         self.ax.add_patch(rect)
         s = 10 if len(label) == 1 else 8
         r = 90 if len(label) > 2 else 0
-        self.ax.text(xloc + size_x/2, yloc + abs(mode2 - mode1)/2, 
+        self.ax.text(xloc + size_x/2, yloc + (size_y-offset)/2, 
                      label, horizontalalignment = "center", size = s,
                      verticalalignment = "center", color = "white",
                      rotation = r)
         xloc += size_x
-        # Add output waveguides
-        for i in modes:
-            self._add_wg(xloc, i, con_length)
-        # Update mode positions
+        # Add output waveguides and update mode positions
         for i in modes:
-            self.locations[i] = xloc + con_length
+            if i not in self.herald_modes:
+                self._add_wg(xloc, self.y_locations[i], con_length)
+            self.x_locations[i] = xloc + con_length
             
         return
     
-    def _add_grouped_circuit(self, mode1: int, mode2: int, name: str) -> None:
+    def _add_grouped_circuit(self, mode1: int, mode2: int, name: str,
+                             heralds: dict) -> None:
         """Add a grouped circuit drawing to the axis."""
         size_x = 1 # x size
         con_length = 0.5 # Input/output waveguide lengths
+        extra_length = 0.5 if heralds["input"] or heralds["output"] else 0
         offset = 0.5 # Offset of square from modes
-        size_y = offset + abs(mode2 - mode1) # Find total unitary size
+        size_y = offset + abs(self.y_locations[mode2] - 
+                              self.y_locations[mode1]) # Find total unitary size
         # Get x and y positions
-        yloc = min(mode1, mode2)
-        xloc = max(self.locations[mode1:mode2+1])
+        yloc = self.y_locations[min(mode1, mode2)]
+        xloc = max(self.x_locations[mode1:mode2+1])
         # Add initial connectors for any modes which haven't reach xloc yet:
-        for i, loc in enumerate(self.locations[mode1:mode2+1]):
-            if loc < xloc:
-                self._add_wg(loc, yloc + i, xloc - loc)
+        for i, loc in enumerate(self.x_locations[mode1:mode2+1]):
+            if loc < xloc and i+mode1 not in self.herald_modes:
+                self._add_wg(loc, self.y_locations[i+mode1], xloc - loc)
         # Add input waveguides
         modes = range(min(mode1, mode2), max(mode1, mode2)+1, 1)
         for i in modes:
-            self._add_wg(xloc, i, con_length)
-        xloc += con_length
+            if i not in self.herald_modes:
+                self._add_wg(xloc, self.y_locations[i], 
+                             con_length + extra_length)
+            elif i - mode1 in heralds["input"]:
+                self._add_wg(xloc + extra_length, self.y_locations[i], 
+                             con_length)
+        xloc += con_length + extra_length
         # Add circuit shape and label
         rect = patches.Rectangle((xloc, yloc-offset/2), size_x, size_y, 
                                  facecolor = "#1a0f36", 
                                  edgecolor = "black")
         self.ax.add_patch(rect)
         s = 10 if len(name) == 1 else 8
         r = 90 if len(name) > 2 else 0
-        self.ax.text(xloc + size_x/2, yloc + abs(mode2 - mode1)/2, 
+        self.ax.text(xloc + size_x/2, yloc + (size_y-offset)/2, 
                      name, horizontalalignment = "center", size = s,
                      verticalalignment = "center", color = "white", 
                      rotation = r)
         xloc += size_x
-        # Add output waveguides
-        for i in modes:
-            self._add_wg(xloc, i, con_length)
-        # Update mode positions
+        # Add output waveguides and update mode positions
         for i in modes:
-            self.locations[i] = xloc + con_length
+            if i not in self.herald_modes:
+                self._add_wg(xloc, self.y_locations[i], 
+                             con_length + extra_length)
+            elif i - mode1 in heralds["output"]:
+                self._add_wg(xloc, self.y_locations[i], con_length)
+            self.x_locations[i] = xloc + con_length + extra_length
             
-        return
+        # Modify provided heralds by mode offset and then add at locations
+        shifted_heralds = {
+            "input" : {m+mode1:n for m, n in heralds["input"].items()},
+            "output" : {m+mode1:n for m, n in heralds["output"].items()}
+            }
+        self._add_heralds(shifted_heralds, xloc-size_x-con_length, 
+                          xloc+con_length)
+            
+        return
+    
+    def _add_heralds(self, heralds: dict, start_loc: float, 
+                     end_loc: float) -> None:
+        """Adds display of all heralds to circuit."""
+        size = 0.2
+        # Input heralds
+        for mode, num in heralds["input"].items():
+            xloc = start_loc
+            yloc = self.y_locations[mode]
+            circle = patches.Circle((xloc, yloc), size, facecolor = "#3e368d", 
+                                    edgecolor = "black")
+            self.ax.add_patch(circle)
+            self.ax.text(xloc, yloc+0.01, str(num), color = "white", size = 8, 
+                         horizontalalignment = "center", 
+                         verticalalignment = "center")
+        # Output heralds
+        for mode, num in heralds["output"].items():
+            xloc = end_loc
+            yloc = self.y_locations[mode]
+            circle = patches.Circle((xloc, yloc), size, facecolor = "#3e368d", 
+                                    edgecolor = "black")
+            self.ax.add_patch(circle)
+            self.ax.text(xloc, yloc+0.01, str(num), color = "white", size = 8, 
+                         horizontalalignment = "center", 
+                         verticalalignment = "center")
```

### Comparing `lightworks-1.2.0/lightworks/sdk/visualisation/display_components_svg.py` & `lightworks-1.3.0/lightworks/sdk/visualisation/display_components_svg.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         return
     
     def _add_ps(self, mode: int, phi: float) -> None:
         """Add a phase shifter to the drawing."""
         size = 50
         con_length = 50
         # Get current x and y locations for the mode
-        xloc = self.locations[mode]
-        yloc = (mode+1)*self.dy
+        xloc = self.x_locations[mode]
+        yloc = self.y_locations[mode]
         # Input waveguide
         self._add_wg(xloc, yloc, con_length)
         xloc += con_length
         # Add phase shifter section
         self.draw_spec += [("ps", (xloc, yloc, size))]
         self.draw_spec += [("text", ("PS", xloc+size/2, yloc+2, 0, 25, "white",
                                      "centred"))]
@@ -63,103 +63,111 @@
         else:
             phi_text = phi
         self.draw_spec += [("text", (f"φ = {phi_text}", xloc+size/2, 
                                      yloc+size, 0, 18, "black", "centred"))]
         xloc += size
         # Output waveguide
         self._add_wg(xloc, yloc, con_length)
-        self.locations[mode] = xloc + con_length
+        self.x_locations[mode] = xloc + con_length
         
         return
         
     def _add_bs(self, mode1: int, mode2: int, ref: float) -> None:
         """Add a beam splitter across to provided modes to the drawing."""
         size_x = 50 # x beam splitter size
         con_length = 50 # input/output waveguide length
         offset = 50 # Offset of beam splitter shape from mode centres
-        size_y = offset + abs(mode2 - mode1)*self.dy
+        if mode1 > mode2:
+            mode1, mode2 = mode2, mode1
+        size_y = offset + self.y_locations[mode2] - self.y_locations[mode1]
         # Get x and y locations
-        yloc = (min(mode1, mode2)+1)*self.dy
-        xloc = max(self.locations[mode1:mode2+1])
+        yloc = self.y_locations[mode1]
+        xloc = max(self.x_locations[mode1:mode2+1])
         # Add initial connectors for any modes which haven't reach xloc yet:
-        for i, loc in enumerate(self.locations[mode1:mode2+1]):
-            if loc < xloc:
-                self._add_wg(loc, yloc + i*self.dy, xloc - loc)
+        for i, loc in enumerate(self.x_locations[mode1:mode2+1]):
+            if loc < xloc and i+mode1 not in self.herald_modes:
+                self._add_wg(loc, self.y_locations[mode1+i], xloc - loc)
         # Add input waveguides for all included modes
-        modes = range(min(mode1, mode2), max(mode1, mode2) + 1, 1)
-        for i in modes:
-            self._add_wg(xloc, (i+1)*self.dy, con_length)
+        for i in range(mode1, mode2 + 1):
+            if i not in self.herald_modes:
+                self._add_wg(xloc, self.y_locations[i], con_length)
         xloc += con_length
         # Add beam splitter section
-        dy = - 50 if abs(mode2-mode1)%2 == 0 else 0
         self.draw_spec += [("bs", (xloc, yloc, size_x, size_y, offset/2))]
+        # TODO: Need to tweak how the beam splitter location is decided
+        mode_between = 0
+        for i in range(mode1 + 1, mode2 + 1, 1):
+            if i not in self.herald_modes:
+                mode_between += 1
+        dy = - 50 if mode_between%2 == 0 else 0
         self.draw_spec += [("text", ("BS", xloc+size_x/2, 
                                      (yloc + (size_y-offset)/2 + dy), 0,
                                      25, "white", "centred"))]
         if not isinstance(ref, str):
             ref = round(ref,4)
         self.draw_spec += [("text", (f"r = {ref}", xloc+size_x/2, 
                                      yloc + size_y, 0, 18, "black", 
                                      "centred"))]
         # For any modes in between the beam splitter modes add a waveguide 
         # across the beam splitter
-        if mode2 - mode1 > 1:
-            for i in range(mode1+1, mode2):
-                self._add_wg(xloc, (i+1)*self.dy, size_x)
+        for i in range(mode1+1, mode2):
+            if i not in self.herald_modes:
+                self._add_wg(xloc, self.y_locations[i], size_x)
         xloc += size_x
-        # Add output waveguides
-        for i in modes:
-            self._add_wg(xloc, (i+1)*self.dy, con_length)
-        # Update mode locations
-        for i in modes:
-            self.locations[i] = xloc + con_length
+        # Add output waveguides and update mode locations
+        for i in range(mode1, mode2 + 1):
+            if i not in self.herald_modes:
+                self._add_wg(xloc, self.y_locations[i], con_length)
+            self.x_locations[i] = xloc + con_length
         
         return
     
     def _add_unitary(self, mode1: int, mode2: int, label: str) -> None:
         """Add a unitary matrix representation to the drawing."""
         size_x = 100 # Unitary x size
         con_length = 50 # Input/output waveguide lengths
         offset = 50 # Offset of unitary square from modes
-        size_y = offset + abs(mode2 - mode1)*self.dy # Find total size
+        size_y = offset + self.y_locations[mode2] - self.y_locations[mode1]
         # Get x and y positions
-        yloc = (min(mode1, mode2)+1)*self.dy
-        xloc = max(self.locations[mode1:mode2+1])
+        yloc = self.y_locations[mode1]
+        xloc = max(self.x_locations[mode1:mode2+1])
         # Add initial connectors for any modes which haven't reach xloc yet:
-        for i, loc in enumerate(self.locations[mode1:mode2+1]):
-            if loc < xloc:
-                self._add_wg(loc, yloc + i*self.dy, xloc - loc)
+        for i, loc in enumerate(self.x_locations[mode1:mode2+1]):
+            if loc < xloc and i + mode1 not in self.herald_modes:
+                self._add_wg(loc, self.y_locations[mode1 + i], xloc - loc)
         # Add input waveguides
         modes = range(min(mode1, mode2), max(mode1, mode2)+1, 1)
         for i in modes:
-            self._add_wg(xloc, (i+1)*self.dy, con_length)
+            if i not in self.herald_modes:
+                self._add_wg(xloc, self.y_locations[i], con_length)
         xloc += con_length
         # Add unitary shape and U label
         self.draw_spec += [("unitary", (xloc, yloc, size_x, size_y, offset/2))]
         s = 25 if self.N > 2 else 20
         s = 35 if len(label) == 1 else s
         r = 270 if len(label) > 2 else 0
         self.draw_spec += [("text", (label, xloc+size_x/2, 
                                      yloc + (size_y-offset)/2, r, s, 
                                      "white", "centred"))]
         xloc += size_x
         # Add output waveguides and update mode positions
         for i in modes:
-            self._add_wg(xloc, (i+1)*self.dy, con_length)
-            self.locations[i] = xloc + con_length
+            if i not in self.herald_modes:
+                self._add_wg(xloc, self.y_locations[i], con_length)
+            self.x_locations[i] = xloc + con_length
             
         return
     
     def _add_loss(self, mode: int, loss: float) -> None:
         """Add a loss channel to the specified mode."""
         size = 50
         con_length = 50
         # Get current x and y locations for the mode
-        xloc = self.locations[mode]
-        yloc = (mode+1)*self.dy
+        xloc = self.x_locations[mode]
+        yloc = self.y_locations[mode]
         # Input waveguide
         self._add_wg(xloc, yloc, con_length)
         xloc += con_length
         # Add phase shifter section
         self.draw_spec += [("lc", (xloc, yloc, size))]
         self.draw_spec += [("text", ("L", xloc+size/2, yloc+2, 0, 25, "white",
                                      "centred"))]
@@ -168,102 +176,138 @@
             loss = str(round(loss, 4)) + " dB"
         self.draw_spec += [("text", (f"loss = {loss}", 
                                      xloc+size/2, yloc+size, 0, 18, "black",
                                      "centred"))]
         xloc += size
         # Output waveguide
         self._add_wg(xloc, yloc, con_length)
-        self.locations[mode] = xloc + con_length
+        self.x_locations[mode] = xloc + con_length
         
         return
     
     def _add_barrier(self, modes: list) -> None:
         """
         Add a barrier which will separate different parts of the circuit. This
         is applied to the provided modes.
         """
-        max_loc = max([self.locations[m] for m in modes])
+        max_loc = max([self.x_locations[m] for m in modes])
         for m in modes:
-            loc = self.locations[m]
+            loc = self.x_locations[m]
             if loc < max_loc:
-                self._add_wg(loc, (m+1)*self.dy, max_loc - loc)
-            self.locations[m] = max_loc
+                self._add_wg(loc, self.y_locations[m], max_loc - loc)
+            self.x_locations[m] = max_loc
         
         return
     
     def _add_mode_swaps(self, swaps: dict) -> None:
         """Add mode swaps between provided modes to the drawing."""
         con_length = 25 # input/output waveguide length
         min_mode = min(swaps)
         max_mode = max(swaps)
         size_x = 50+20*(max_mode-min_mode) # x length of swap element
         # Add in missing mode for swap
         for m in range(min_mode, max_mode+1):
             if m not in swaps:
                 swaps[m] = m
         # Get x and y locations
-        xloc = max(self.locations[min_mode:max_mode+1])
+        xloc = max(self.x_locations[min_mode:max_mode+1])
         ylocs = []
         for i, j in swaps.items():
-            ylocs.append(((i+1)*self.dy, (j+1)*self.dy))
+            if i not in self.herald_modes:
+                ylocs.append((self.y_locations[i], self.y_locations[j]))
         # Add initial connectors for any modes which haven't reach xloc yet:
-        for i, loc in enumerate(self.locations[min_mode:max_mode+1]):
-            if loc < xloc:
-                self._add_wg(loc, (min_mode+i+1)*self.dy, xloc - loc)
+        for i, loc in enumerate(self.x_locations[min_mode:max_mode+1]):
+            if loc < xloc and i + min_mode not in self.herald_modes:
+                self._add_wg(loc, self.y_locations[min_mode+i], xloc - loc)
         # Add input waveguides for all included modes
         modes = range(min_mode, max_mode+1, 1)
         for i in modes:
-            self._add_wg(xloc, (i+1)*self.dy, con_length)
+            if i not in self.herald_modes:
+                self._add_wg(xloc, self.y_locations[i], con_length)
         xloc += con_length
         # Add beam splitter section
         self.draw_spec += [("mode_swaps", (xloc, ylocs, size_x))]
         xloc += size_x
-        # Add output waveguides
+        # Add output waveguides update mode locations
         for i in modes:
-            self._add_wg(xloc, (i+1)*self.dy, con_length)
-        # Update mode locations
-        for i in modes:
-            self.locations[i] = xloc + con_length
+            if i not in self.herald_modes:
+                self._add_wg(xloc, self.y_locations[i], con_length)
+            self.x_locations[i] = xloc + con_length
         
         return
     
-    def _add_grouped_circuit(self, mode1: int, mode2: int, name: str) -> None:
+    def _add_grouped_circuit(self, mode1: int, mode2: int, name: str,
+                             heralds: dict) -> None:
         """Add a grouped_circuit representation to the drawing."""
         size_x = 100 # Drawing x size
         con_length = 50 # Input/output waveguide lengths
+        extra_length = 50 if heralds["input"] or heralds["output"] else 0
         offset = 50 # Offset of square from modes
-        size_y = offset + abs(mode2 - mode1)*self.dy # Find total size
+        size_y = offset + self.y_locations[mode2] - self.y_locations[mode1]
         # Get x and y positions
-        yloc = (min(mode1, mode2)+1)*self.dy
-        xloc = max(self.locations[mode1:mode2+1])
+        yloc = self.y_locations[mode1]
+        xloc = max(self.x_locations[mode1:mode2+1])
         # Add initial connectors for any modes which haven't reach xloc yet:
-        for i, loc in enumerate(self.locations[mode1:mode2+1]):
-            if loc < xloc:
-                self._add_wg(loc, yloc + i*self.dy, xloc - loc)
+        for i, loc in enumerate(self.x_locations[mode1:mode2+1]):
+            if loc < xloc and i+mode1 not in self.herald_modes:
+                self._add_wg(loc, self.y_locations[mode1 + i], xloc - loc)
         # Add input waveguides
         modes = range(min(mode1, mode2), max(mode1, mode2)+1, 1)
         for i in modes:
-            self._add_wg(xloc, (i+1)*self.dy, con_length)
-        xloc += con_length
+            if i not in self.herald_modes:
+                self._add_wg(xloc, self.y_locations[i], con_length + extra_length)
+            elif i - mode1 in heralds["input"]:
+                self._add_wg(xloc + extra_length, self.y_locations[i], con_length)
+        xloc += con_length + extra_length
         # Add unitary shape and U label
         self.draw_spec += [("group", (xloc, yloc, size_x, size_y, offset/2))]
         s = 25 if self.N > 2 else 20
         s = 35 if len(name) == 1 else s
         r = 270 if len(name) > 2 else 0
         self.draw_spec += [("text", (name, xloc+size_x/2, 
                                      yloc + (size_y-offset)/2, r, s, 
                                      "white", "centred"))]
         xloc += size_x
         # Add output waveguides and update mode positions
         for i in modes:
-            self._add_wg(xloc, (i+1)*self.dy, con_length)
-            self.locations[i] = xloc + con_length
+            if i not in self.herald_modes:
+                self._add_wg(xloc, self.y_locations[i], con_length + extra_length)
+            elif i - mode1 in heralds["output"]:
+                self._add_wg(xloc, self.y_locations[i], con_length)
+            self.x_locations[i] = xloc + con_length + extra_length
+            
+        # Modify provided heralds by mode offset and then add at locations
+        shifted_heralds = {
+            "input" : {m+mode1:n for m, n in heralds["input"].items()},
+            "output" : {m+mode1:n for m, n in heralds["output"].items()}
+            }
+        self._add_heralds(shifted_heralds, xloc-size_x-con_length, 
+                          xloc+con_length)
             
         return
     
+    def _add_heralds(self, heralds: dict, start_loc: float, 
+                     end_loc: float) -> None:
+        """Adds display of all heralds to circuit."""
+        size = 25
+        # Input heralds
+        for mode, num in heralds["input"].items():
+            xloc = start_loc
+            yloc = self.y_locations[mode]
+            self.draw_spec += [("herald", (xloc, yloc, size))]
+            self.draw_spec += [("text", (str(num), xloc, yloc+2.5, 0, 30, 
+                                         "white", "centred"))]
+        # Output heralds
+        for mode, num in heralds["output"].items():
+            xloc = end_loc
+            yloc = self.y_locations[mode]
+            self.draw_spec += [("herald", (xloc, yloc, size))]
+            self.draw_spec += [("text", (str(num), xloc, yloc+2.5, 0, 30, 
+                                         "white", "centred"))]
+    
 class DisplayComponentsSVG:
     
     def _draw_wg(self, x: float, y: float, length: float) -> None:
         
         r = draw.Rectangle(x, y-self.wg_width/2, length, self.wg_width, 
                            fill = "black")
         self.d.append(r)
@@ -315,15 +359,15 @@
             raise DisplayError("Alignment value not recognised.")
         t = draw.Text(text, size, x, y, fill = colour, text_anchor = ta,
                       dominant_baseline = db, 
                       transform = f"rotate({rotation}, {x}, {y})")
         self.d.append(t)
         return
     
-    def _draw_mode_swaps(self, x, ys, size_x):
+    def _draw_mode_swaps(self, x: float, ys: list, size_x: float):
         
         for y0, y1 in ys:
             w = self.wg_width/2
             m = np.arctan(abs(y1-y0)/size_x)
             if y0 < y1:
                 dx1 = w*m
                 dx2 = 0
@@ -341,8 +385,14 @@
     
     def _draw_grouped_circuit(self, x: float, y: float, size_x: float, 
                               size_y: float, offset_y: float) -> None:
         
         r = draw.Rectangle(x, y-offset_y, size_x, size_y, fill = "#1a0f36", 
                            stroke = "black", rx = 5, ry = 5)
         self.d.append(r)
+        return
+    
+    def _draw_herald(self, x: float, y: float, size: float):
+        
+        c = draw.Circle(x, y, size, fill = "#3e368d", stroke = "black")
+        self.d.append(c)
         return
```

### Comparing `lightworks-1.2.0/lightworks/sdk/visualisation/draw_circuit_mpl.py` & `lightworks-1.3.0/lightworks/sdk/visualisation/draw_circuit_mpl.py`

 * *Files 22% similar despite different names*

```diff
@@ -41,14 +41,16 @@
     
     def __init__(self, circuit: "Circuit", display_loss: bool = False,         # type:ignore - Hide warning raised by "Circuit"
                  mode_labels: list[str] | None = None) -> None:
         
         self.circuit = circuit
         self.display_loss = display_loss
         self.mode_labels = mode_labels
+        self.N = self.circuit.n_modes
+        self.herald_modes = self.circuit._internal_modes
         
     def draw(self) -> tuple[plt.figure, plt.axes]:
         
         # Set a waveguide width and get mode number
         self.wg_width = 0.05
         N = self.circuit.n_modes
         # Adjust size of figure according to circuit with min size 4 and max 40
@@ -56,21 +58,39 @@
         s = max(s, 4)
         # Create fig and set aspect to equal
         self.fig, self.ax = plt.subplots(figsize = (s, s), dpi = 200)
         self.ax.set_aspect('equal')
         # Manually adjust figure height
         h = max(N, 4)
         self.fig.set_figheight(h)
-        self.ax.set_ylim(N, -1)
+        dy = 1
+        dy_smaller = 0.6
+        self.y_locations = []
+        # Set mode y locations
+        yloc = 0
+        for i in range(self.N):
+            self.y_locations.append(yloc)
+            if i+1 in self.herald_modes:
+                yloc += dy_smaller
+            elif i in self.herald_modes:
+                yloc += dy_smaller
+            else:
+                yloc += dy
         # Set a starting length and add a waveguide for each mode
         init_length = 0.5
         if False:
             self._add_wg(0, i-self.wg_width/2, init_length)
         # Create a list to store the positions of each mode
-        self.locations = [init_length]*N
+        self.x_locations = [init_length]*N
+        # Add extra waveguides when using heralds
+        if self.circuit._external_heralds["input"]:
+            for i in range(self.N):
+                if i not in self.herald_modes:
+                    self._add_wg(self.x_locations[i], self.y_locations[i], 0.5)
+                    self.x_locations[i] += 0.5
         # Loop over build spec and add each component
         for spec in self.circuit._display_spec:
             c, modes = spec[0:2]
             params = spec[2]
             if c == "PS":
                 self._add_ps(modes, params)
             elif c == "BS":
@@ -80,40 +100,65 @@
                     m1, m2 = m2, m1
                 self._add_bs(m1, m2, ref)
             elif c == "LC" and self.display_loss:
                 self._add_loss(modes, params)
             elif c == "barrier":
                 self._add_barrier(modes)
             elif c == "mode_swaps":
+                if not modes:
+                    continue
                 self._add_mode_swaps(modes)
             elif c == "unitary":
                 m1, m2 = modes
                 if m1 > m2:
                     m1, m2 = m2, m1
                 self._add_unitary(m1, m2, params)
             elif c == "group":
                 m1, m2 = modes
                 if m1 > m2:
                     m1, m2 = m2, m1
-                self._add_grouped_circuit(m1, m2, params)
+                name, heralds = params
+                self._add_grouped_circuit(m1, m2, name, heralds)
         # Add any final lengths as required
-        final_loc = max(self.locations)
-        for i, loc in enumerate(self.locations):    
-            if loc < final_loc:
+        final_loc = max(self.x_locations)
+        # Extend final waveguide if herald included
+        if (self.circuit._external_heralds["output"]):
+            final_loc += 0.5
+        for i, loc in enumerate(self.x_locations):    
+            if loc < final_loc and i not in self.herald_modes:
                 length = final_loc - loc
-                rect = patches.Rectangle((loc, i-self.wg_width/2), length, 
-                                         self.wg_width, facecolor = "black")
-                self.ax.add_patch(rect)
+                self._add_wg(loc, self.y_locations[i], length)
+                self.x_locations[i] += length
+                
+        # Add heralding display
+        self._add_heralds(self.circuit._external_heralds, init_length,
+                          final_loc)
+                
         # Set axes limits using locations and mode numbers
-        self.ax.set_xlim(0, max(self.locations) + 0.5)
-        self.ax.set_yticks(range(0, N))
+        self.ax.set_xlim(0, max(self.x_locations) + 0.5)
+        self.ax.set_ylim(max(self.y_locations) + 1, -1)
+        self.ax.set_yticks(self.y_locations)
         if self.mode_labels is not None:
-            if len(self.mode_labels) != N:
+            exp_len = N - len(self.herald_modes)
+            if len(self.mode_labels) != exp_len:
                 raise DisplayError(
                     "Length of provided mode labels list should be equal to "
-                    "the number of modes.")
-            self.ax.set_yticklabels(self.mode_labels)
+                    f"the number of useable modes ({exp_len}).")
+            mode_labels = self.mode_labels
+        else:
+            mode_labels = range(N - len(self.herald_modes))
+        mode_labels = [str(m) for m in mode_labels]
+        # Include heralded modes in mode labels
+        full_mode_labels = []
+        count = 0
+        for i in range(N):
+            if i not in self.herald_modes:
+                full_mode_labels.append(mode_labels[count])
+                count += 1
+            else:
+                full_mode_labels.append("-")
+        self.ax.set_yticklabels(full_mode_labels)
         self.ax.set_xticks([])
 
         return self.fig, self.ax
```

### Comparing `lightworks-1.2.0/lightworks/sdk/visualisation/draw_circuit_svg.py` & `lightworks-1.3.0/lightworks/sdk/visualisation/draw_circuit_svg.py`

 * *Files 20% similar despite different names*

```diff
@@ -38,102 +38,147 @@
     """
     
     def __init__(self, circuit: "Circuit", display_loss: bool = False,         # type:ignore - Hide warning raised by "Circuit"
                  mode_labels: list[str] = None) -> None:
         
         self.circuit = circuit
         self.display_loss = display_loss
-        self.mode_labels = mode_labels
+        self.herald_modes = self.circuit._internal_modes
         # Set a waveguide width and get mode number
         self.wg_width = 8
         self.N = self.circuit.n_modes
         self.draw_spec = []
         self.dy = 125
-        init_length = 100        
+        self.dy_smaller = 75
+        self.y_locations = []
+        # Set mode y locations
+        yloc = self.dy
+        for i in range(self.N):
+            self.y_locations.append(yloc)
+            if i+1 in self.herald_modes:
+                yloc += self.dy_smaller
+            elif i in self.herald_modes:
+                yloc += self.dy_smaller
+            else:
+                yloc += self.dy
+        init_length = 100
         # Add the mode labels
-        if mode_labels is None:
-            mode_labels = range(self.N)
+        if mode_labels is not None:
+            exp_len = self.N - len(self.herald_modes)
+            if len(mode_labels) != exp_len:
+                raise DisplayError(
+                    "Length of provided mode labels list should be equal to "
+                    f"the number of useable modes ({exp_len}).")
+        else:
+            mode_labels = range(self.N - len(self.herald_modes))
         # Convert all labels to strings
         mode_labels = [str(m) for m in mode_labels]
+        full_mode_labels = []
+        count = 0
+        for i in range(self.N):
+            if i not in self.herald_modes:
+                full_mode_labels.append(mode_labels[count])
+                count += 1
+            else:
+                full_mode_labels.append("-")
+        mode_labels = full_mode_labels
         # Adjust canvas size for long labels
         max_len = max([len(m) for m in mode_labels])
         if max_len > 4: init_length += (max_len-4)*17.5
         for m, label in enumerate(mode_labels):
-            self.draw_spec += [("text", (label, init_length-20, 
-                                         (m+1)*self.dy + 2, 0, 25, "black", 
-                                         "right"))]
+            self.draw_spec += [("text", 
+                                (label, init_length-20, 
+                                 self.y_locations[m] + 2, 0, 25, "black", 
+                                 "right"))
+                               ]
         self._init_length = init_length
         # Create list of locations for each mode
-        self.locations = [init_length+50]*self.N
+        self.x_locations = [init_length+50]*self.N
+        # Add extra waveguides when using heralds
+        if self.circuit._external_heralds["input"]:
+            for m in range(self.N):
+                if m not in self.herald_modes:
+                    self._add_wg(self.x_locations[m], self.y_locations[m], 50)
+                    self.x_locations[m] += 50
         # Loop over each element in the build spec and add
         for spec in self.circuit._display_spec:
             c, modes = spec[0:2]
             params = spec[2]
             if c == "PS":
                 self._add_ps(modes, params)
-            elif c == "BS":
+            elif c == "BS": # TODO
                 m1, m2 = modes
                 ref = params
                 if m1 > m2:
                     m1, m2 = m2, m1
                 self._add_bs(m1, m2, ref)
             elif c == "LC" and self.display_loss:
                 self._add_loss(modes, params)
-            elif c == "barrier":
+            elif c == "barrier": 
                 self._add_barrier(modes)
-            elif c == "mode_swaps":
+            elif c == "mode_swaps": # TODO
+                if not modes:
+                    continue
                 self._add_mode_swaps(modes)
-            elif c == "unitary":
+            elif c == "unitary": # TODO
                 m1, m2 = modes
                 if m1 > m2:
                     m1, m2 = m2, m1
                 self._add_unitary(m1, m2, params)
-            elif c == "group":
+            elif c == "group": # TODO
                 m1, m2 = modes
                 if m1 > m2:
                     m1, m2 = m2, m1
-                self._add_grouped_circuit(m1, m2, params)
+                name, heralds = params
+                self._add_grouped_circuit(m1, m2, name, heralds)
         
-        maxloc = max(self.locations)
-        for i, loc in enumerate(self.locations):
-            if loc < maxloc:
-                self._add_wg(loc, (i+1)*self.dy, maxloc-loc)
-                self.locations[i] = maxloc
+        maxloc = max(self.x_locations)
+        # Extend final waveguide if herald included
+        if self.circuit._external_heralds["output"]:
+            maxloc += 50
+        for i, loc in enumerate(self.x_locations):
+            if loc < maxloc and i not in self.herald_modes:
+                self._add_wg(loc, self.y_locations[i], maxloc-loc)
+                self.x_locations[i] = maxloc
+        
+        # Add heralding display
+        self._add_heralds(self.circuit._external_heralds, self._init_length+50,
+                          maxloc)
                 
         for i in range(self.N):
-            self.locations[i] += 50
+            self.x_locations[i] += 50
         
         return
         
     def draw(self) -> draw.Drawing:
         """
         Draws the circuit as defined in the initial class class:
         
         Returns:
         
             draw.Drawing : The created drawing with all circuit components.
         
         """
         extra_lower = 0
         # Create a new drawing of the correct size
-        self.d = draw.Drawing(max(self.locations) + 100, 
-                              (self.N+1)*self.dy + extra_lower)
+        self.d = draw.Drawing(max(self.x_locations) + 100, 
+                              max(self.y_locations) + self.dy + extra_lower)
         
-        # Add frame around circuit
         border = 100
-        dx = max(self.locations) - self._init_length
-        dy = (self.N-1)*self.dy + border*2 + extra_lower
+        # Add frame around circuit
+        dx = max(self.x_locations) - self._init_length
+        dy = max(self.y_locations) - self.dy + 2*border + extra_lower
         self.d.append(draw.Rectangle(self._init_length, self.dy-border, dx, dy,
                                      fill = 'none', stroke = "black"))
         # Add ticks to left side of frame
         length, width = 8, 1
         for i in range(self.N):
             self.d.append(draw.Rectangle(self._init_length-length, 
-                                         (i+1)*self.dy-width/2, length, width,
-                                         fill = "black"))
+                                         self.y_locations[i]-width/2, length, 
+                                         width, fill = "black"))
         
         # Loop over each element in the drawing spec and add
         for c, data in self.draw_spec:
             if c == "wg":
                 self._draw_wg(*data)
             elif c == "ps":
                 self._draw_ps(*data)
@@ -145,19 +190,21 @@
                 self._draw_loss(*data)
             elif c == "mode_swaps":
                 self._draw_mode_swaps(*data)
             elif c == "unitary":
                 self._draw_unitary(*data)
             elif c == "group":
                 self._draw_grouped_circuit(*data)
+            elif c == "herald":
+                self._draw_herald(*data)
             else:
                 raise DisplayError("Element in draw spec not recognised.")
                 
         # Adjust size of figure to meet target scale
-        target_scale = min(50+self.N*65, 900)
+        target_scale = min(50+(self.N-len(self.herald_modes))*65, 900)
         #target_scale = max(target_scale, 200)
         self.d.set_pixel_scale(1)
         w,h = self.d.calc_render_size()
         self.d.set_pixel_scale(target_scale/h)
 
         return self.d
```

### Comparing `lightworks-1.2.0/lightworks.egg-info/PKG-INFO` & `lightworks-1.3.0/lightworks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightworks
-Version: 1.2.0
+Version: 1.3.0
 Summary: Open-source Python SDK for photonic quantum computation.
 Home-page: https://github.com/Aegiq/lightworks
 Author: Aegiq Ltd.
 License: Apache 2.0
 Project-URL: Source, https://github.com/Aegiq/lightworks
 Project-URL: Documentation, https://aegiq.github.io/lightworks/
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `lightworks-1.2.0/lightworks.egg-info/SOURCES.txt` & `lightworks-1.3.0/lightworks.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -27,31 +27,33 @@
 lightworks/emulator/simulation/probability_distribution.py
 lightworks/emulator/simulation/quick_sampler.py
 lightworks/emulator/simulation/sampler.py
 lightworks/emulator/simulation/simulator.py
 lightworks/emulator/utils/__init__.py
 lightworks/emulator/utils/exceptions.py
 lightworks/emulator/utils/state_utils.py
+lightworks/qubit/__init__.py
+lightworks/qubit/gates/__init__.py
+lightworks/qubit/gates/single_qubit_gates.py
+lightworks/qubit/gates/two_qubit_gates.py
 lightworks/sdk/__init__.py
 lightworks/sdk/circuit/__init__.py
 lightworks/sdk/circuit/circuit.py
 lightworks/sdk/circuit/circuit_compiler.py
 lightworks/sdk/circuit/parameters.py
 lightworks/sdk/circuit/unitary.py
 lightworks/sdk/optimisation/__init__.py
 lightworks/sdk/optimisation/optimisation.py
-lightworks/sdk/qubit/__init__.py
-lightworks/sdk/qubit/single_qubit_gates.py
-lightworks/sdk/qubit/two_qubit_gates.py
 lightworks/sdk/state/__init__.py
 lightworks/sdk/state/state.py
 lightworks/sdk/utils/__init__.py
 lightworks/sdk/utils/circuit_utils.py
 lightworks/sdk/utils/conversion.py
 lightworks/sdk/utils/exceptions.py
+lightworks/sdk/utils/heralding_utils.py
 lightworks/sdk/utils/matrix_utils.py
 lightworks/sdk/utils/permutation_conversion.py
 lightworks/sdk/utils/state_utils.py
 lightworks/sdk/visualisation/__init__.py
 lightworks/sdk/visualisation/display.py
 lightworks/sdk/visualisation/display_components_mpl.py
 lightworks/sdk/visualisation/display_components_svg.py
```

### Comparing `lightworks-1.2.0/setup.py` & `lightworks-1.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 from setuptools import setup, find_packages
 
 version = {}
 with open("lightworks/__version.py") as f:
-      exec(f.read(), version)
+    exec(f.read(), version)
 
-setup(name = "lightworks",
-      author = "Aegiq Ltd.",
-      version = version["__version__"],
-      description = "Open-source Python SDK for photonic quantum computation.",
-      long_description = open("README.md", encoding="utf-8").read(),
-      long_description_content_type = "text/markdown",
-      url = "https://github.com/Aegiq/lightworks",
-      project_urls={
-        "Source": "https://github.com/Aegiq/lightworks",
-        "Documentation": "https://aegiq.github.io/lightworks/",
+setup(
+    name = "lightworks",
+    author = "Aegiq Ltd.",
+    version = version["__version__"],
+    description = "Open-source Python SDK for photonic quantum computation.",
+    long_description = open("README.md", encoding="utf-8").read(),
+    long_description_content_type = "text/markdown",
+    url = "https://github.com/Aegiq/lightworks",
+    project_urls = {
+        "Source" : "https://github.com/Aegiq/lightworks",
+        "Documentation" : "https://aegiq.github.io/lightworks/",
     },
-      license = "Apache 2.0",
-      packages = find_packages(where=".", exclude = ["tests"]),
-      python_requires = ">=3.10",
-      install_requires = ["thewalrus==0.20.0", 
-                          "matplotlib>=3.7.1",
-                          "pandas>=2.0.1", 
-                          "numpy>=1.24.3", 
-                          "bayesian-optimization>=1.4.3", 
-                          "drawsvg>=2.3.0", 
-                          "zoopt>=0.4.2", 
-                          "pyarrow", 
-                          "ipython"
-                          ],
-      classifiers = ["License :: OSI Approved :: Apache Software License",
-                     "Natural Language :: English",
-                     "Programming Language :: Python",
-                     "Programming Language :: Python :: 3.10",
-                     "Programming Language :: Python :: 3.11",
-                     "Programming Language :: Python :: 3.12",
-                     "Operating System :: OS Independent"
-                     ]
-      )
+    license = "Apache 2.0",
+    packages = find_packages(where=".", exclude = ["tests"]),
+    python_requires = ">=3.10",
+    install_requires = [
+        "thewalrus==0.20.0", 
+        "matplotlib>=3.7.1",
+        "pandas>=2.0.1", 
+        "numpy>=1.24.3", 
+        "bayesian-optimization>=1.4.3", 
+        "drawsvg>=2.3.0", 
+        "zoopt>=0.4.2", 
+        "pyarrow", 
+        "ipython"
+    ],
+    classifiers = [
+        "License :: OSI Approved :: Apache Software License",
+        "Natural Language :: English",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Operating System :: OS Independent"
+    ]
+)
```

### Comparing `lightworks-1.2.0/tests/emulator/__init__.py` & `lightworks-1.3.0/lightworks/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/tests/emulator/analyzer_test.py` & `lightworks-1.3.0/tests/emulator/analyzer_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,17 +74,18 @@
         analyzer = Analyzer(self.circuit)
         results = analyzer.analyze(State([2,0,0,0]))
         p = results[State([0,1,0,1])]
         assert pytest.approx(p, 1e-8) == 0.0022854516590
         
     def test_analyzer_complex(self):
         """Check analyzer result when using post-selection and heralding."""
+        # Add heralding mode
+        self.circuit.add_herald(0, 3)
         analyzer = Analyzer(self.circuit)
         # Just heralding
-        analyzer.set_herald(3, 0)
         results = analyzer.analyze(State([1,0,1]))
         p = results[State([0,1,1])]
         assert pytest.approx(p, 1e-8) == 0.091713377373246
         # Heralding + post-selection
         analyzer.set_post_selection(lambda s: s[0] == 1)
         results = analyzer.analyze(State([1,0,1]))
         p = results[State([1,1,0])]
@@ -93,17 +94,43 @@
         assert pytest.approx(results.performance, 1e-8) == 0.03181835438235
         
     def test_analyzer_complex_lossy(self):
         """
         Check analyzer result when using post-selection and heralding with a 
         lossy circuit.
         """
+        # Add heralding mode
+        self.lossy_circuit.add_herald(0, 3)
         analyzer = Analyzer(self.lossy_circuit)
         # Just heralding
-        analyzer.set_herald(3, 0)
+        results = analyzer.analyze(State([1,0,1]))
+        p = results[State([0,1,0])]
+        assert pytest.approx(p, 1e-8) == 0.062204471804458
+        # Heralding + post-selection
+        analyzer.set_post_selection(lambda s: s[0] == 0)
+        results = analyzer.analyze(State([1,0,1]))
+        p = results[State([0,0,1])]
+        assert pytest.approx(p, 1e-8) == 0.0202286624257920
+        p = results[State([0,0,0])]
+        assert pytest.approx(p, 1e-8) == 0.6051457174354371
+        # Check performance metric
+        assert pytest.approx(results.performance, 1e-8) == 0.6893563871958014
+        
+    def test_analyzer_complex_lossy_added_circuit(self):
+        """
+        Check analyzer result when using post-selection and heralding with a 
+        lossy circuit which has been added to another circuit.
+        """
+        # Add heralding mode
+        self.lossy_circuit.add_herald(0, 3)
+        new_circ = Circuit(self.lossy_circuit.n_modes - 
+                           len(self.lossy_circuit.heralds["input"]))
+        new_circ.add(self.lossy_circuit)
+        analyzer = Analyzer(new_circ)
+        # Just heralding
         results = analyzer.analyze(State([1,0,1]))
         p = results[State([0,1,0])]
         assert pytest.approx(p, 1e-8) == 0.062204471804458
         # Heralding + post-selection
         analyzer.set_post_selection(lambda s: s[0] == 0)
         results = analyzer.analyze(State([1,0,1]))
         p = results[State([0,0,1])]
```

### Comparing `lightworks-1.2.0/tests/emulator/annotatedstate_test.py` & `lightworks-1.3.0/tests/emulator/annotatedstate_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/tests/emulator/backend_test.py` & `lightworks-1.3.0/tests/emulator/backend_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/tests/emulator/cnot_test.py` & `lightworks-1.3.0/tests/emulator/cnot_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,25 +9,30 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from lightworks import State, Circuit
-from lightworks.emulator import Sampler, Source, Detector
+from lightworks.emulator import Sampler, Source, Detector, Backend
+from lightworks.qubit import CNOT
+
+import pytest
 
 from numpy import arccos, pi
 
+@pytest.mark.parametrize("backend", [Backend("permanent"), Backend("slos")])
 class TestCNOT:
     """
     Samples from a non-heralded CNOT circuit with loss, imperfect source and 
-    detector to check that the correct results is produced.  
+    detector to check that the correct results is produced. It tests this with 
+    both permanent and slos backends.
     """
     
-    def test_cnot_sample_n_inputs(self):
+    def test_cnot_sample_n_inputs(self, backend):
         """
         Checks the correct output is produced from the CNOT gate when sampling 
         N inputs from the system. Note, very occasionally this test may fail 
         due to the probabilistic nature of the sampler. It is only a concern if
         this happens consistently.
         """
         # Create CNOT circuit
@@ -47,27 +52,27 @@
         # Define imperfect source and detector
         source = Source(purity = 0.99, brightness = 0.4, 
                         indistinguishability = 0.94)
         detector = Detector(efficiency = 0.9, p_dark = 1e-5, 
                             photon_counting = False)
         # Then define sampler with the input state |10>
         sampler = Sampler(cnot_circuit, State([0,0,1,1,0,0]), source = source, 
-                          detector = detector)
+                          detector = detector, backend = backend)
         # Can then define the heralding required to get the correct output and
         # generate a set of samples
         herald = lambda s: (s[0] == 0 and s[5] == 0 and s[1] + s[2] == 1 and 
                             s[3] + s[4] == 1)
-        results = sampler.sample_N_inputs(20000, herald = herald)
+        results = sampler.sample_N_inputs(20000, post_select = herald)
         # We expect the state |11> (|0,0,1,0,1,0> in mode language) with 
         # reasonable fidelity, so we will assert this is measured for > 80% of
         # the total samples which met the herald condition
         eff = results[State([0,0,1,0,1,0])] / sum(results.values())
         assert eff > 0.8
         
-    def test_cnot_sample_n_outputs(self):
+    def test_cnot_sample_n_outputs(self, backend):
         """
         Checks the correct output is produced from the CNOT gate when sampling 
         N outputs from the system. Note, very occasionally this test may fail 
         due to the probabilistic nature of the sampler. It is only a concern if
         this happens consistently.
         """
         # Create CNOT circuit
@@ -86,18 +91,71 @@
                 cnot_circuit.add_barrier()
         # Define imperfect source and detector
         source = Source(purity = 0.99, brightness = 0.4, 
                         indistinguishability = 0.94)
         detector = Detector(efficiency = 0.9, photon_counting = False)
         # Then define sampler with the input state |10>
         sampler = Sampler(cnot_circuit, State([0,0,1,1,0,0]), source = source, 
-                          detector = detector)
+                          detector = detector, backend = backend)
         # Can then define the heralding required to get the correct output and
         # generate a set of samples
         herald = lambda s: (s[0] == 0 and s[5] == 0 and s[1] + s[2] == 1 and 
                             s[3] + s[4] == 1)
-        results = sampler.sample_N_outputs(20000, herald = herald)
+        results = sampler.sample_N_outputs(20000, post_select = herald)
         # We expect the state |11> (|0,0,1,0,1,0> in mode language) with 
         # reasonable fidelity, so we will assert this is measured for > 80% of
         # the total samples which met the herald condition
         eff = results[State([0,0,1,0,1,0])] / 20000
         assert eff > 0.8
+        
+    def test_cnot_sample_n_inputs_built_in(self, backend):
+        """
+        Checks the correct output is produced from the built-in CNOT gate when 
+        sampling N inputs from the system. Note, very occasionally this test 
+        may fail due to the probabilistic nature of the sampler. It is only a 
+        concern if this happens consistently.
+        """
+        # Create CNOT circuit
+        cnot_circuit = CNOT()
+        # Define imperfect source and detector
+        source = Source(purity = 0.99, brightness = 0.4, 
+                        indistinguishability = 0.94)
+        detector = Detector(efficiency = 0.9, p_dark = 1e-5, 
+                            photon_counting = False)
+        # Then define sampler with the input state |10>
+        sampler = Sampler(cnot_circuit, State([0,1,1,0]), source = source, 
+                          detector = detector, backend = backend)
+        # Can then define the post-selection required to get the correct output and
+        # generate a set of samples
+        post_select = lambda s: (s[0] + s[1] == 1 and s[2] + s[3] == 1)
+        results = sampler.sample_N_inputs(20000, post_select = post_select)
+        # We expect the state |11> (|0,1,0,1> in mode language) with 
+        # reasonable fidelity, so we will assert this is measured for > 80% of
+        # the total samples which met the herald condition
+        eff = results[State([0,1,0,1])] / sum(results.values())
+        assert eff > 0.8
+        
+    def test_cnot_sample_n_outputs_built_in(self, backend):
+        """
+        Checks the correct output is produced from the built-in CNOT gate when 
+        sampling N outputs from the system. Note, very occasionally this test 
+        may fail due to the probabilistic nature of the sampler. It is only a 
+        concern if this happens consistently.
+        """
+        # Create CNOT circuit
+        cnot_circuit = CNOT()
+        # Define imperfect source and detector
+        source = Source(purity = 0.99, brightness = 0.4, 
+                        indistinguishability = 0.94)
+        detector = Detector(efficiency = 0.9, photon_counting = False)
+        # Then define sampler with the input state |10>
+        sampler = Sampler(cnot_circuit, State([0,1,1,0]), source = source, 
+                          detector = detector, backend = backend)
+        # Can then define the post-selection required to get the correct output and
+        # generate a set of samples
+        post_select = lambda s: (s[0] + s[1] == 1 and s[2] + s[3] == 1)
+        results = sampler.sample_N_outputs(20000, post_select = post_select)
+        # We expect the state |11> (|0,1,0,1> in mode language) with 
+        # reasonable fidelity, so we will assert this is measured for > 80% of
+        # the total samples which met the herald condition
+        eff = results[State([0,1,0,1])] / 20000
+        assert eff > 0.8
```

### Comparing `lightworks-1.2.0/tests/emulator/detector_test.py` & `lightworks-1.3.0/tests/emulator/detector_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/tests/emulator/quicksampler_test.py` & `lightworks-1.3.0/tests/emulator/quicksampler_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -75,27 +75,27 @@
         """
         Checks that the probability distribution calculated by the sampler is 
         correct.
         """
         unitary = Unitary(random_unitary(4, seed = 43))
         sampler = QuickSampler(unitary, State([1,0,1,0]), 
                                photon_counting = False, 
-                               herald = lambda s: s[0] == 0)
+                               post_select = lambda s: s[0] == 0)
         p = sampler.probability_distribution[State([0,1,1,0])]
         assert p == pytest.approx(0.3156177858, 1e-8)
         
     def test_sampling_2photons_in_mode(self):
         """
         Checks that the probability distribution calculated by the sampler is 
         correct when using 2 photons in a single mode.
         """
         unitary = Unitary(random_unitary(4, seed = 43))
         sampler = QuickSampler(unitary, State([0,2,0,0]), 
                                photon_counting = False, 
-                               herald = lambda s: s[0] == 0)
+                               post_select = lambda s: s[0] == 0)
         p = sampler.probability_distribution[State([0,1,1,0])]
         assert p == pytest.approx(0.071330233065, 1e-8)
             
     def test_lossy_sampling(self):
         """
         Checks that the probability distribution calculated by the sampler with
         a lossy circuit is correct.
@@ -106,15 +106,15 @@
         circuit.add_ps(1, 0.7, loss = 0.5)
         circuit.add_ps(3, 0.6, loss = 0.5)
         circuit.add_bs(1, loss = 1.3)
         circuit.add_bs(2, loss = 2)
         circuit.add_ps(1, 0.5, loss = 0.5)
         sampler = QuickSampler(circuit, State([1,0,1,0]), 
                                photon_counting = False, 
-                               herald = lambda s: s[0] == 0)
+                               post_select = lambda s: s[0] == 0)
         p = sampler.probability_distribution[State([0,1,1,0])]
         assert p == pytest.approx(0.386272843449, 1e-8)
         
     def test_circuit_update_with_sampler(self):
         """
         Checks that when a circuit is modified then the sampler recalculates 
         the probability distribution.
@@ -164,24 +164,24 @@
         sampler = QuickSampler(circuit, State([1,0,1,0]), 
                                photon_counting = True)
         p1 = sampler.probability_distribution
         sampler.photon_counting = False
         p2 = sampler.probability_distribution
         assert p1 != p2
         
-    def test_herald_update_with_sampler(self):
+    def test_post_select_update_with_sampler(self):
         """
-        Confirms that changing the herald function changes the produced 
+        Confirms that changing the post_select function changes the produced 
         results.
         """
         circuit = Unitary(random_unitary(4))
         sampler = QuickSampler(circuit, State([1,0,1,0]), 
-                               herald = lambda s: s[0] == 1)
+                               post_select = lambda s: s[0] == 1)
         p1 = sampler.probability_distribution
-        sampler.herald = lambda s: s[1] == 1
+        sampler.post_select = lambda s: s[1] == 1
         p2 = sampler.probability_distribution
         assert p1 != p2
     
     def test_circuit_assignment(self):
         """
         Confirms that a Circuit cannot be replaced with a non-Circuit through
         the circuit attribute.
@@ -201,26 +201,93 @@
         # Incorrect type
         with pytest.raises(TypeError):
             sampler.input_state = [1,2,3,4]
         # Incorrect number of modes
         with pytest.raises(ModeMismatchError):
             sampler.input_state = State([1,2,3])
             
-    def test_herald_assignment(self):
+    def test_post_select_assignment(self):
         """
-        Confirms that the herald attribute cannot be replaced with a 
+        Confirms that the post_select attribute cannot be replaced with a 
         non-function value.
         """
         circuit = Unitary(random_unitary(4))
         sampler = QuickSampler(circuit, State([1,0,1,0]))
         with pytest.raises(TypeError):
-            sampler.herald = True
+            sampler.post_select = True
             
     def test_photon_counting_assignment(self):
         """
         Confirms that the photon_counting attribute cannot be replaced with a 
         non-boolean value.
         """
         circuit = Unitary(random_unitary(4))
         sampler = QuickSampler(circuit, State([1,0,1,0]))
         with pytest.raises(TypeError):
-            sampler.photon_counting = 1
+            sampler.photon_counting = 1
+            
+    def test_herald_equivalent(self):
+        """
+        Checks that results are equivalent if a herald is used vs 
+        post-selection on a non-heralded circuit.
+        """
+        # First calculate distribution without heralding
+        circuit = Unitary(random_unitary(6))
+        sampler = QuickSampler(circuit, State([1,1,0,0,0,1]),
+                               post_select = lambda s: s[3] == 1 and s[2] == 0)
+        p1 = sampler.probability_distribution
+        # Then find with heralding
+        circuit.add_herald(1, 0, 3)
+        circuit.add_herald(0, 2)
+        sampler = QuickSampler(circuit, State([1,0,0,1]))
+        p2 = sampler.probability_distribution
+        for s in p2:
+            full_state = s[0:2] + State([0,1]) + s[2:]
+            assert pytest.approx(p2[s]) == p1[full_state]
+            
+    def test_herald_equivalent_lossy(self):
+        """
+        Checks that results are equivalent if a herald is used vs 
+        post-selection on a non-heralded circuit when lossy modes are 
+        introduced.
+        """
+        # First calculate distribution without heralding
+        circuit = Unitary(random_unitary(6))
+        for i in range(6):
+            circuit.add_loss(i, i+1)
+        sampler = QuickSampler(circuit, State([1,1,0,0,0,1]),
+                               post_select = lambda s: s[3] == 1 and s[2] == 0)
+        p1 = sampler.probability_distribution
+        # Then find with heralding
+        circuit.add_herald(1, 0, 3)
+        circuit.add_herald(0, 2)
+        sampler = QuickSampler(circuit, State([1,0,0,1]))
+        p2 = sampler.probability_distribution
+        for s in p2:
+            full_state = s[0:2] + State([0,1]) + s[2:]
+            assert pytest.approx(p2[s]) == p1[full_state]
+        
+    def test_herald_equivalent_grouped(self):
+        """
+        Checks that results are equivalent if a herald is used vs 
+        post-selection on a non-heralded circuit when the heralds are featured
+        as part of a grouped sub-circuit.
+        """
+        # First calculate distribution without heralding
+        circuit = Unitary(random_unitary(6))
+        for i in range(6):
+            circuit.add_loss(i, i+1)
+        sampler = QuickSampler(circuit, State([1,1,0,0,0,1]),
+                               post_select = lambda s: s[3] == 1 and s[2] == 0)
+        p1 = sampler.probability_distribution
+        # Then find with heralding
+        circuit.add_herald(1, 0, 3)
+        circuit.add_herald(0, 2)
+        # Create empty circuit and add original circuit to this
+        new_circuit = Circuit(4)
+        new_circuit.add(circuit, 0)
+        circuit = new_circuit
+        sampler = QuickSampler(circuit, State([1,0,0,1]))
+        p2 = sampler.probability_distribution
+        for s in p2:
+            full_state = s[0:2] + State([0,1]) + s[2:]
+            assert pytest.approx(p2[s]) == p1[full_state]
```

### Comparing `lightworks-1.2.0/tests/emulator/result_test.py` & `lightworks-1.3.0/tests/emulator/result_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,9 +149,9 @@
     def test_extra_attribute_assignment(self):
         """
         Check that miscellaneous additional kwargs can be provided in the 
         initial function call and that these are assigned to attributes.
         """
         r = SimulationResult(self.test_array, "probability_amplitude", 
                              inputs = self.test_inputs, 
-                             outputs = self.test_outputs, test_attr = 2.5)
-        assert r.test_attr == 2.5
+                             outputs = self.test_outputs, performance = 2.5)
+        assert r.performance == 2.5
```

### Comparing `lightworks-1.2.0/tests/emulator/sampler_test.py` & `lightworks-1.3.0/tests/emulator/sampler_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -453,8 +453,116 @@
                           backend = backend)
         results = sampler.sample_N_inputs(1000)
         sub_2_photon_states = False
         for s, c in results.items():
             if s.n_photons < 2:
                 sub_2_photon_states = True
                 break
-        assert sub_2_photon_states
+        assert sub_2_photon_states
+        
+    @pytest.mark.flaky(reruns = 2)
+    def test_herald_equivalent(self, backend):
+        """
+        Checks that results are equivalent if a herald is used vs 
+        post-selection on a non-heralded circuit.
+        """
+        circuit = Unitary(random_unitary(6))
+        # Sampler without built-in heralds
+        sampler = Sampler(circuit, State([1,1,0,1,0,0]), backend = backend)
+        results = sampler.sample_N_outputs(
+            50000, post_select = lambda s: s[1] == 1 and s[3] == 0)
+        # Then add and re-sample
+        circuit.add_herald(1, 0, 1)
+        circuit.add_herald(0, 2, 3)
+        sampler = Sampler(circuit, State([1,1,0,0]), backend = backend)
+        results2 = sampler.sample_N_outputs(50000)
+        # Check all results with outputs greater than 2000
+        for s, c in results2.items():
+            if c > 2000:
+                full_s = s[0:1] + State([1]) + s[1:2] + State([0]) + s[2:]
+                # Check results are within 10%
+                assert pytest.approx(results[full_s], 0.1) == results2[s]
+    
+    @pytest.mark.flaky(reruns = 2)            
+    def test_herald_equivalent_imperfect_source(self, backend):
+        """
+        Checks that results are equivalent if a herald is used vs 
+        post-selection on a non-heralded circuit, while also including an
+        imperfect photon source.
+        """
+        circuit = Unitary(random_unitary(6))
+        # Define source to use
+        source = Source(purity = 0.9, brightness = 0.9, 
+                        indistinguishability = 0.9)
+        # Sampler without built-in heralds
+        sampler = Sampler(circuit, State([1,1,0,1,0,0]), backend = backend,
+                          source = source)
+        results = sampler.sample_N_outputs(
+            50000, post_select = lambda s: s[1] == 1 and s[3] == 0)
+        # Then add and re-sample
+        circuit.add_herald(1, 0, 1)
+        circuit.add_herald(0, 2, 3)
+        sampler = Sampler(circuit, State([1,1,0,0]), backend = backend, 
+                          source = source)
+        results2 = sampler.sample_N_outputs(50000)
+        # Check all results with outputs greater than 2000
+        for s, c in results2.items():
+            if c > 2000:
+                full_s = s[0:1] + State([1]) + s[1:2] + State([0]) + s[2:]
+                # Check results are within 10%
+                assert pytest.approx(results[full_s], 0.1) == results2[s]
+    
+    @pytest.mark.flaky(reruns = 2)            
+    def test_herald_equivalent_lossy(self, backend):
+        """
+        Checks that results are equivalent if a herald is used vs 
+        post-selection on a non-heralded lossy circuit.
+        """
+        circuit = Unitary(random_unitary(6))
+        for i in range(6):
+            circuit.add_loss(i, i+1)
+        # Sampler without built-in heralds
+        sampler = Sampler(circuit, State([1,1,0,1,0,0]), backend = backend)
+        results = sampler.sample_N_outputs(
+            50000, post_select = lambda s: s[1] == 1 and s[3] == 0)
+        # Then add and re-sample
+        circuit.add_herald(1, 0, 1)
+        circuit.add_herald(0, 2, 3)
+        sampler = Sampler(circuit, State([1,1,0,0]), backend = backend)
+        results2 = sampler.sample_N_outputs(50000)
+        # Check all results with outputs greater than 2000
+        for s, c in results2.items():
+            if c > 2000:
+                full_s = s[0:1] + State([1]) + s[1:2] + State([0]) + s[2:]
+                # Check results are within 10%
+                assert pytest.approx(results[full_s], 0.1) == results2[s]
+    
+    @pytest.mark.flaky(reruns = 2)            
+    def test_herald_equivalent_lossy_imperfect_source(self, backend):
+        """
+        Checks that results are equivalent if a herald is used vs 
+        post-selection on a non-heralded lossy circuit, while also including an
+        imperfect photon source.
+        """
+        circuit = Unitary(random_unitary(6))
+        for i in range(6):
+            circuit.add_loss(i, i+1)
+        # Define source to use
+        source = Source(purity = 0.9, brightness = 0.9, 
+                        indistinguishability = 0.9)
+        # Sampler without built-in heralds
+        sampler = Sampler(circuit, State([1,1,0,1,0,0]), backend = backend, 
+                          source = source)
+        results = sampler.sample_N_outputs(
+            50000, post_select = lambda s: s[1] == 1 and s[3] == 0)
+        # Then add and re-sample
+        circuit.add_herald(1, 0, 1)
+        circuit.add_herald(0, 2, 3)
+        sampler = Sampler(circuit, State([1,1,0,0]), backend = backend, 
+                          source = source)
+        results2 = sampler.sample_N_outputs(50000)
+        # Check all results with outputs greater than 2000
+        for s, c in results2.items():
+            if c > 2000:
+                full_s = s[0:1] + State([1]) + s[1:2] + State([0]) + s[2:]
+                # Check results are within 10%
+                assert pytest.approx(results[full_s], 0.1) == results2[s]
```

### Comparing `lightworks-1.2.0/tests/emulator/source_test.py` & `lightworks-1.3.0/tests/emulator/source_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/tests/sdk/__init__.py` & `lightworks-1.3.0/tests/emulator/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/tests/sdk/compiledcircuit_test.py` & `lightworks-1.3.0/tests/sdk/compiledcircuit_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -156,55 +156,14 @@
             c2.add_loss(m, 0.1)
         c1.add(c2, 1)
         # Check unitary equivalence
         U1 = round(circ_comp.U_full, 8)
         U2 = round(c1.U_full, 8)
         assert (U1 == U2).all()
                 
-    def test_smaller_circuit_addition_grouped(self):
-        """
-        Confirms equivalence between building a single circuit and added a 
-        larger circuit to a smaller one with the add method, while using the 
-        group method.
-        """
-        # Comparison circuit
-        circ_comp = CompiledCircuit(6)
-        # First part
-        for i, m in enumerate([0,2,4,1,3,2]):
-            circ_comp.add_bs(m)
-            circ_comp.add_ps(m, i)
-        # Second part
-        for i in range(4):
-            for i, m in enumerate([3,1,3,2,1]):
-                circ_comp.add_ps(m+1, i)
-                circ_comp.add_bs(m)
-                circ_comp.add_ps(m, i)
-                circ_comp.add_loss(m, loss = 0.1)
-            circ_comp.add_mode_swaps({1:2, 2:3, 3:1})
-        # Addition circuit
-        c1 = CompiledCircuit(6)
-        for i, m in enumerate([0,2,4,1,3,2]):
-            c1.add_bs(m)
-            c1.add_ps(m, i)
-        c2 = CompiledCircuit(4)
-        for i, m in enumerate([2,0,2,1,0]):
-            c2.add_ps(m+1, i)
-            c2.add_bs(m)
-            c2.add_ps(m, i)
-            c2.add_loss(m, loss = 0.1)
-        c2.add_mode_swaps({0:1, 1:2, 2:0})
-        # Test combinations of True and False for group option
-        c2.add(c2, 0, group = True)
-        c2.add(c2, 0, group = False)
-        c1.add(c2, 1, group = True)
-        # Check unitary equivalence
-        U1 = round(circ_comp.U_full, 8)
-        U2 = round(c1.U_full, 8)
-        assert (U1 == U2).all()
-                
     def test_mode_modification(self):
         """
         Checks that the number of modes attribute cannot be modified as this is
         not intended for the circuit and could cause issues.
         """
         circuit = CompiledCircuit(4)
         with pytest.raises(AttributeError):
```

### Comparing `lightworks-1.2.0/tests/sdk/display_test.py` & `lightworks-1.3.0/tests/sdk/display_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,21 @@
         for i, m in enumerate([0,2,1,2,0,1]):
             self.circuit.add_bs(m)
             self.circuit.add_ps(m, phi = Parameter(i, label = f"p{i}"))
             self.circuit.add_bs(m, loss = 2)
             self.circuit.add_ps(m+1, phi = 3*i)
             self.circuit.add_loss(m, loss = 1)
         self.circuit.add_mode_swaps({0:2,2:1,1:0})
+        self.circuit.add_herald(1, 0, 0)
         self.circuit.add(Unitary(random_unitary(3, seed=1)), 1)
         self.circuit.add(Unitary(random_unitary(3, seed=1)), 0, group = True)
         circuit2 = Circuit(2)
         circuit2.add_bs(0)
         circuit2.add_ps(1, 2)
+        circuit2.add_herald(2,1,1)
         self.circuit.add(circuit2, 1)
         circuit2.add(circuit2, group=True)
         self.circuit.add(circuit2, 1, group = True)
     
     def test_circuit_display_method(self):
         """Checks that the display method works without any errors arising."""
         try:
@@ -78,15 +80,15 @@
         Checks that a circuit passed to the display function is able to be
         processed without any exceptions arising.
         """
         try:
             Display(self.circuit, display_loss = True)
         except:
             pytest.fail("Exception occurred during display operation.")
-            
+    
     def test_circuit_display_function_mpl(self):
         """
         Checks that a circuit passed to the display function is able to be
         processed without any exceptions arising for the matplotlib method.
         """
         # NOTE: There is a non intermittent issue that occurs during testing
         # with the subplots method in mpl. This can be fixed by altering the
```

### Comparing `lightworks-1.2.0/tests/sdk/parameter_test.py` & `lightworks-1.3.0/tests/sdk/parameter_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.2.0/tests/sdk/qubit_gate_test.py` & `lightworks-1.3.0/tests/sdk/qubit_gate_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from lightworks import State
 from lightworks.emulator import Simulator
-from lightworks.sdk.qubit import (H, X, Y, Z, S, T, CZ, CNOT, CZ_Heralded, 
-                                  CNOT_Heralded)
+from lightworks.qubit import (H, X, Y, Z, S, T, CZ, CNOT, CZ_Heralded, 
+                              CNOT_Heralded)
 
 import pytest
 import numpy as np
 
 class TestSingleQubitGates:
     
     def test_hadamard(self):
@@ -98,15 +98,15 @@
     
     def test_CZ(self):
         """
         Checks that the output of the post-selected CZ gate is correct and that
         the success probability is 1/9.
         """
         # Define all input combinations
-        states = [[0,1,0,1,0,0], [0,1,0,0,1,0], [0,0,1,1,0,0], [0,0,1,0,1,0]]
+        states = [[1,0,1,0], [1,0,0,1], [0,1,1,0], [0,1,0,1]]
         states = [State(s) for s in states]
         # Calculate probability amplitudes
         sim = Simulator(CZ())
         results = sim.simulate(states, states)
         # Check all results are identical except for |1,1> which has a -1
         amp = results[states[0], states[0]]
         assert pytest.approx(amp, 1e-6) == results[states[1], states[1]]
@@ -117,15 +117,15 @@
     
     def test_CNOT(self):
         """
         Checks that the output of the post-selected CNOT gate is correct and 
         that the success probability is 1/9.
         """
         # Define all input combinations
-        states = [[0,1,0,1,0,0], [0,1,0,0,1,0], [0,0,1,1,0,0], [0,0,1,0,1,0]]
+        states = [[1,0,1,0], [1,0,0,1], [0,1,1,0], [0,1,0,1]]
         states = [State(s) for s in states]
         # Calculate probability amplitudes
         sim = Simulator(CNOT())
         results = sim.simulate(states, states)
         # Check that swap occurs when control qubit is 1 but not otherwise
         amp = results[states[0], states[0]]
         assert pytest.approx(amp, 1e-6) == results[states[1], states[1]]
@@ -136,16 +136,15 @@
     
     def test_CZ_heralded(self):
         """
         Checks that the output of the heralded CZ gate is correct and that the 
         success probability is 1/16.
         """
         # Define all input combinations
-        states = [[0,1,1,0,1,0,1,0], [0,1,1,0,0,1,1,0],
-                  [0,1,0,1,1,0,1,0], [0,1,0,1,0,1,1,0]]
+        states = [[1,0,1,0], [1,0,0,1], [0,1,1,0], [0,1,0,1]]
         states = [State(s) for s in states]
         # Calculate probability amplitudes
         sim = Simulator(CZ_Heralded())
         results = sim.simulate(states, states)
         # Check all results are identical except for |1,1> which has a -1
         amp = results[states[0], states[0]]
         assert pytest.approx(amp, 1e-6) == results[states[1], states[1]]
@@ -156,16 +155,15 @@
     
     def test_CNOT_heralded(self):
         """
         Checks that the output of the heralded CNOT gate is correct and that 
         the success probability is 1/16.
         """
         # Define all input combinations
-        states = [[0,1,1,0,1,0,1,0], [0,1,1,0,0,1,1,0],
-                  [0,1,0,1,1,0,1,0], [0,1,0,1,0,1,1,0]]
+        states = [[1,0,1,0], [1,0,0,1], [0,1,1,0], [0,1,0,1]]
         states = [State(s) for s in states]
         # Calculate probability amplitudes
         sim = Simulator(CNOT_Heralded())
         results = sim.simulate(states, states)
         # Check that swap occurs when control qubit is 1 but not otherwise
         amp = results[states[0], states[0]]
         assert pytest.approx(amp, 1e-6) == results[states[1], states[1]]
```

### Comparing `lightworks-1.2.0/tests/sdk/state_test.py` & `lightworks-1.3.0/tests/sdk/state_test.py`

 * *Files identical despite different names*

