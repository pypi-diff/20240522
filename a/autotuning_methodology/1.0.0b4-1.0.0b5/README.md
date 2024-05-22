# Comparing `tmp/autotuning_methodology-1.0.0b4.tar.gz` & `tmp/autotuning_methodology-1.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotuning_methodology-1.0.0b4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "autotuning_methodology-1.0.0b5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `autotuning_methodology-1.0.0b4.tar` & `autotuning_methodology-1.0.0b5.tar`

### file list

```diff
@@ -1,85 +1,86 @@
--rw-r--r--   0        0        0      112 2024-05-17 07:20:07.464581 autotuning_methodology-1.0.0b4/.coveragerc
--rw-r--r--   0        0        0     1424 2024-05-17 07:20:07.464581 autotuning_methodology-1.0.0b4/.github/workflows/build-test-python-package.yml
--rw-r--r--   0        0        0      658 2024-05-17 07:20:07.464581 autotuning_methodology-1.0.0b4/.github/workflows/publish-documentation.yml
--rw-r--r--   0        0        0     1227 2024-05-17 07:20:07.464581 autotuning_methodology-1.0.0b4/.github/workflows/publish-package.yml
--rwxr-xr-x   0        0        0     3571 2024-05-17 07:20:07.468581 autotuning_methodology-1.0.0b4/.gitignore
--rw-r--r--   0        0        0      144 2024-05-17 07:20:07.468581 autotuning_methodology-1.0.0b4/.vscode/extensions.json
--rw-r--r--   0        0        0      605 2024-05-17 07:20:07.468581 autotuning_methodology-1.0.0b4/.vscode/settings.json
--rw-r--r--   0        0        0     4096 2024-05-17 07:20:07.468581 autotuning_methodology-1.0.0b4/CITATION.cff
--rw-r--r--   0        0        0     1077 2024-05-17 07:20:07.468581 autotuning_methodology-1.0.0b4/LICENSE
--rw-r--r--   0        0        0     7852 2024-05-17 07:20:07.468581 autotuning_methodology-1.0.0b4/README.md
--rw-r--r--   0        0        0     2597 2024-05-17 07:20:07.468581 autotuning_methodology-1.0.0b4/UML/.$Sequence Diagram.drawio.bkp
--rw-r--r--   0        0        0   302745 2024-05-17 07:20:07.468581 autotuning_methodology-1.0.0b4/UML/.$flowchart.drawio.bkp
--rw-r--r--   0        0        0     2585 2024-05-17 07:20:07.468581 autotuning_methodology-1.0.0b4/UML/Sequence Diagram.drawio
--rw-r--r--   0        0        0    26889 2024-05-17 07:20:07.468581 autotuning_methodology-1.0.0b4/UML/classes.pdf
--rw-r--r--   0        0        0   303637 2024-05-17 07:20:07.472581 autotuning_methodology-1.0.0b4/UML/flowchart/.$flowchart.drawio.bkp
--rw-r--r--   0        0        0   303637 2024-05-17 07:20:07.472581 autotuning_methodology-1.0.0b4/UML/flowchart/flowchart.drawio
--rw-r--r--   0        0        0   315705 2024-05-17 07:20:07.472581 autotuning_methodology-1.0.0b4/UML/flowchart/flowchart_output_generation.png
--rw-r--r--   0        0        0   267296 2024-05-17 07:20:07.472581 autotuning_methodology-1.0.0b4/UML/flowchart/flowchart_performance_curve_generation.png
--rw-r--r--   0        0        0   131133 2024-05-17 07:20:07.476581 autotuning_methodology-1.0.0b4/UML/flowchart/mini_plots/flowchart_plot_aggregated.png
--rw-r--r--   0        0        0    95756 2024-05-17 07:20:07.476581 autotuning_methodology-1.0.0b4/UML/flowchart/mini_plots/flowchart_plot_individual.png
--rw-r--r--   0        0        0     1074 2024-05-17 07:20:07.476581 autotuning_methodology-1.0.0b4/UML/flowchart/mini_plots/flowchart_plots.py
--rw-r--r--   0        0        0    15114 2024-05-17 07:20:07.476581 autotuning_methodology-1.0.0b4/UML/packages.pdf
--rw-r--r--   0        0        0     5736 2024-05-17 07:20:07.476581 autotuning_methodology-1.0.0b4/cached_data_used/cachefiles/ktt_values_to_kerneltuner.py
--rw-r--r--   0        0        0      634 2024-05-17 07:20:07.476581 autotuning_methodology-1.0.0b4/docs/Makefile
--rw-r--r--   0        0        0     1722 2024-05-17 07:20:07.476581 autotuning_methodology-1.0.0b4/docs/autotuning_methodology.rst
--rw-r--r--   0        0        0     2541 2024-05-17 07:20:07.476581 autotuning_methodology-1.0.0b4/docs/conf.py
--rw-r--r--   0        0        0     2225 2024-05-17 07:20:07.476581 autotuning_methodology-1.0.0b4/docs/contributing.rst
--rw-r--r--   0        0        0     2409 2024-05-17 07:20:07.476581 autotuning_methodology-1.0.0b4/docs/getting_started.rst
--rw-r--r--   0        0        0     1144 2024-05-17 07:20:07.476581 autotuning_methodology-1.0.0b4/docs/index.rst
--rw-r--r--   0        0        0      800 2024-05-17 07:20:07.476581 autotuning_methodology-1.0.0b4/docs/make.bat
--rw-r--r--   0        0        0   609663 2024-05-17 07:20:07.480581 autotuning_methodology-1.0.0b4/docs/source/example_aggregated.png
--rw-r--r--   0        0        0   315705 2024-05-17 07:20:07.480581 autotuning_methodology-1.0.0b4/docs/source/flowchart_output_generation.png
--rw-r--r--   0        0        0   267296 2024-05-17 07:20:07.480581 autotuning_methodology-1.0.0b4/docs/source/flowchart_performance_curve_generation.png
--rw-r--r--   0        0        0     5034 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/docs/source/logo_autotuning_methodology.svg
--rw-r--r--   0        0        0    36351 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/docs/source/logo_kernel_dashboard.svg
--rw-r--r--   0        0        0    42513 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/docs/source/logo_kernel_launcher.svg
--rw-r--r--   0        0        0    39816 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/docs/source/logo_kernel_tuner.svg
--rwxr-xr-x   0        0        0      983 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/experiment_files/bootstrap_hyperparams.json
--rw-r--r--   0        0        0     1625 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/experiment_files/example_visualizations.json
--rw-r--r--   0        0        0     1971 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/experiment_files/methodology_paper_evaluation.json
--rw-r--r--   0        0        0     1647 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/experiment_files/milo_hotspot.json
--rw-r--r--   0        0        0     1403 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/experiment_files/presentation_comparison.json
--rw-r--r--   0        0        0     2364 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/experiment_files/simple_example.json
--rw-r--r--   0        0        0     1745 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/experiment_files/test_random_calculated.json
--rw-r--r--   0        0        0     1409 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/experiment_files/test_scatter.json
--rwxr-xr-x   0        0        0     2275 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/experiment_files/test_searchspace_algorithms.json
--rw-r--r--   0        0        0      132 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/extra/.vscode/settings.json
--rwxr-xr-x   0        0        0    18897 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/extra/bootstrap_hyperparams_visualizer.py
--rwxr-xr-x   0        0        0    19811 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/extra/experiments_strategies.py
--rwxr-xr-x   0        0        0   119690 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/extra/experiments_strategies_hyperparamtuning.py
--rwxr-xr-x   0        0        0     7475 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/extra/generate_cachefile.py
--rw-r--r--   0        0        0    20608 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/extra/max_draw_k_from_n.py
--rw-r--r--   0        0        0     3259 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/extra/speedtest_index_performance.py
--rw-r--r--   0        0        0     1174 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/extra/speedtest_python_reversed_nan_sort.py
--rwxr-xr-x   0        0        0     2545 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/extra/try_BOtorch.py
--rwxr-xr-x   0        0        0     8426 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/extra/try_GPytorch.py
--rw-r--r--   0        0        0    20822 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/extra/try_isotonic_regression.py
--rwxr-xr-x   0        0        0      435 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/mypy.ini
--rw-r--r--   0        0        0     1089 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/noxfile.py
--rwxr-xr-x   0        0        0       17 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/profilings/.gitignore
--rw-r--r--   0        0        0     2816 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/pyproject.toml
--rw-r--r--   0        0        0       95 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/src/autotuning_methodology/__init__.py
--rw-r--r--   0        0        0    17647 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/src/autotuning_methodology/baseline.py
--rwxr-xr-x   0        0        0     8418 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/src/autotuning_methodology/caching.py
--rw-r--r--   0        0        0    51986 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/src/autotuning_methodology/curves.py
--rwxr-xr-x   0        0        0     9764 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/src/autotuning_methodology/experiments.py
--rwxr-xr-x   0        0        0    24377 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/src/autotuning_methodology/runner.py
--rwxr-xr-x   0        0        0     4138 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/src/autotuning_methodology/schema.json
--rw-r--r--   0        0        0    25701 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/src/autotuning_methodology/searchspace_statistics.py
--rw-r--r--   0        0        0     1787 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/src/autotuning_methodology/validators.py
--rwxr-xr-x   0        0        0    48490 2024-05-17 07:20:07.484581 autotuning_methodology-1.0.0b4/src/autotuning_methodology/visualize_experiments.py
--rw-r--r--   0        0        0  3269061 2024-05-17 07:20:07.496581 autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~0.json
--rw-r--r--   0        0        0  3255846 2024-05-17 07:20:07.500581 autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~1.json
--rw-r--r--   0        0        0  3483805 2024-05-17 07:20:07.512581 autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/mockfiles/mock_gpu.json
--rw-r--r--   0        0        0     2967 2024-05-17 07:20:07.512581 autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/mockfiles/mocktest_kernel_convolution.py
--rw-r--r--   0        0        0     1489 2024-05-17 07:20:07.512581 autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/mockfiles/test.json
--rw-r--r--   0        0        0     1476 2024-05-17 07:20:07.512581 autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/mockfiles/test_bad_kernel_path.json
--rw-r--r--   0        0        0     1465 2024-05-17 07:20:07.512581 autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/mockfiles/test_cached.json
--rw-r--r--   0        0        0     1453 2024-05-17 07:20:07.512581 autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/mockfiles/test_import_runs.json
--rw-r--r--   0        0        0     8913 2024-05-17 07:20:07.512581 autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/test_run_experiment.py
--rw-r--r--   0        0        0     2934 2024-05-17 07:20:07.512581 autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/test_visualization.py
--rw-r--r--   0        0        0     1978 2024-05-17 07:20:07.512581 autotuning_methodology-1.0.0b4/tests/autotuning_methodology/release/test_toml_file.py
--rw-r--r--   0        0        0       34 2024-05-17 07:20:07.512581 autotuning_methodology-1.0.0b4/tests/autotuning_methodology/unit/test_caching.py
--rw-r--r--   0        0        0     3464 2024-05-17 07:20:07.512581 autotuning_methodology-1.0.0b4/tests/autotuning_methodology/unit/test_curves.py
--rw-r--r--   0        0        0     9820 1970-01-01 00:00:00.000000 autotuning_methodology-1.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0      112 2024-05-22 14:49:23.947539 autotuning_methodology-1.0.0b5/.coveragerc
+-rw-r--r--   0        0        0     1424 2024-05-22 14:49:23.947539 autotuning_methodology-1.0.0b5/.github/workflows/build-test-python-package.yml
+-rw-r--r--   0        0        0      658 2024-05-22 14:49:23.947539 autotuning_methodology-1.0.0b5/.github/workflows/publish-documentation.yml
+-rw-r--r--   0        0        0     1227 2024-05-22 14:49:23.947539 autotuning_methodology-1.0.0b5/.github/workflows/publish-package.yml
+-rwxr-xr-x   0        0        0     3571 2024-05-22 14:49:23.947539 autotuning_methodology-1.0.0b5/.gitignore
+-rw-r--r--   0        0        0      144 2024-05-22 14:49:23.947539 autotuning_methodology-1.0.0b5/.vscode/extensions.json
+-rw-r--r--   0        0        0      605 2024-05-22 14:49:23.947539 autotuning_methodology-1.0.0b5/.vscode/settings.json
+-rw-r--r--   0        0        0     4096 2024-05-22 14:49:23.947539 autotuning_methodology-1.0.0b5/CITATION.cff
+-rw-r--r--   0        0        0     1077 2024-05-22 14:49:23.947539 autotuning_methodology-1.0.0b5/LICENSE
+-rw-r--r--   0        0        0     7917 2024-05-22 14:49:23.947539 autotuning_methodology-1.0.0b5/README.md
+-rw-r--r--   0        0        0     2597 2024-05-22 14:49:23.947539 autotuning_methodology-1.0.0b5/UML/.$Sequence Diagram.drawio.bkp
+-rw-r--r--   0        0        0   302745 2024-05-22 14:49:23.951539 autotuning_methodology-1.0.0b5/UML/.$flowchart.drawio.bkp
+-rw-r--r--   0        0        0     2585 2024-05-22 14:49:23.951539 autotuning_methodology-1.0.0b5/UML/Sequence Diagram.drawio
+-rw-r--r--   0        0        0    26889 2024-05-22 14:49:23.951539 autotuning_methodology-1.0.0b5/UML/classes.pdf
+-rw-r--r--   0        0        0   303637 2024-05-22 14:49:23.951539 autotuning_methodology-1.0.0b5/UML/flowchart/.$flowchart.drawio.bkp
+-rw-r--r--   0        0        0   303637 2024-05-22 14:49:23.951539 autotuning_methodology-1.0.0b5/UML/flowchart/flowchart.drawio
+-rw-r--r--   0        0        0   315705 2024-05-22 14:49:23.955539 autotuning_methodology-1.0.0b5/UML/flowchart/flowchart_output_generation.png
+-rw-r--r--   0        0        0   267296 2024-05-22 14:49:23.955539 autotuning_methodology-1.0.0b5/UML/flowchart/flowchart_performance_curve_generation.png
+-rw-r--r--   0        0        0   131133 2024-05-22 14:49:23.955539 autotuning_methodology-1.0.0b5/UML/flowchart/mini_plots/flowchart_plot_aggregated.png
+-rw-r--r--   0        0        0    95756 2024-05-22 14:49:23.955539 autotuning_methodology-1.0.0b5/UML/flowchart/mini_plots/flowchart_plot_individual.png
+-rw-r--r--   0        0        0     1074 2024-05-22 14:49:23.955539 autotuning_methodology-1.0.0b5/UML/flowchart/mini_plots/flowchart_plots.py
+-rw-r--r--   0        0        0    15114 2024-05-22 14:49:23.955539 autotuning_methodology-1.0.0b5/UML/packages.pdf
+-rw-r--r--   0        0        0     5736 2024-05-22 14:49:23.955539 autotuning_methodology-1.0.0b5/cached_data_used/cachefiles/ktt_values_to_kerneltuner.py
+-rw-r--r--   0        0        0      634 2024-05-22 14:49:23.959539 autotuning_methodology-1.0.0b5/docs/Makefile
+-rw-r--r--   0        0        0     1722 2024-05-22 14:49:23.959539 autotuning_methodology-1.0.0b5/docs/autotuning_methodology.rst
+-rw-r--r--   0        0        0     2541 2024-05-22 14:49:23.959539 autotuning_methodology-1.0.0b5/docs/conf.py
+-rw-r--r--   0        0        0     2225 2024-05-22 14:49:23.959539 autotuning_methodology-1.0.0b5/docs/contributing.rst
+-rw-r--r--   0        0        0     2409 2024-05-22 14:49:23.959539 autotuning_methodology-1.0.0b5/docs/getting_started.rst
+-rw-r--r--   0        0        0     1144 2024-05-22 14:49:23.959539 autotuning_methodology-1.0.0b5/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-05-22 14:49:23.959539 autotuning_methodology-1.0.0b5/docs/make.bat
+-rw-r--r--   0        0        0     1235 2024-05-22 14:49:23.959539 autotuning_methodology-1.0.0b5/docs/rsd_description.md
+-rw-r--r--   0        0        0   609663 2024-05-22 14:49:23.959539 autotuning_methodology-1.0.0b5/docs/source/example_aggregated.png
+-rw-r--r--   0        0        0   315705 2024-05-22 14:49:23.963539 autotuning_methodology-1.0.0b5/docs/source/flowchart_output_generation.png
+-rw-r--r--   0        0        0   267296 2024-05-22 14:49:23.963539 autotuning_methodology-1.0.0b5/docs/source/flowchart_performance_curve_generation.png
+-rw-r--r--   0        0        0     5034 2024-05-22 14:49:23.963539 autotuning_methodology-1.0.0b5/docs/source/logo_autotuning_methodology.svg
+-rw-r--r--   0        0        0    36351 2024-05-22 14:49:23.963539 autotuning_methodology-1.0.0b5/docs/source/logo_kernel_dashboard.svg
+-rw-r--r--   0        0        0    42513 2024-05-22 14:49:23.963539 autotuning_methodology-1.0.0b5/docs/source/logo_kernel_launcher.svg
+-rw-r--r--   0        0        0    39816 2024-05-22 14:49:23.963539 autotuning_methodology-1.0.0b5/docs/source/logo_kernel_tuner.svg
+-rwxr-xr-x   0        0        0      983 2024-05-22 14:49:23.963539 autotuning_methodology-1.0.0b5/experiment_files/bootstrap_hyperparams.json
+-rw-r--r--   0        0        0     1653 2024-05-22 14:49:23.963539 autotuning_methodology-1.0.0b5/experiment_files/example_visualizations.json
+-rw-r--r--   0        0        0     1971 2024-05-22 14:49:23.963539 autotuning_methodology-1.0.0b5/experiment_files/methodology_paper_evaluation.json
+-rw-r--r--   0        0        0     1647 2024-05-22 14:49:23.963539 autotuning_methodology-1.0.0b5/experiment_files/milo_hotspot.json
+-rw-r--r--   0        0        0     1403 2024-05-22 14:49:23.963539 autotuning_methodology-1.0.0b5/experiment_files/presentation_comparison.json
+-rw-r--r--   0        0        0     2364 2024-05-22 14:49:23.963539 autotuning_methodology-1.0.0b5/experiment_files/simple_example.json
+-rw-r--r--   0        0        0     1745 2024-05-22 14:49:23.963539 autotuning_methodology-1.0.0b5/experiment_files/test_random_calculated.json
+-rw-r--r--   0        0        0     1409 2024-05-22 14:49:23.963539 autotuning_methodology-1.0.0b5/experiment_files/test_scatter.json
+-rwxr-xr-x   0        0        0     2275 2024-05-22 14:49:23.963539 autotuning_methodology-1.0.0b5/experiment_files/test_searchspace_algorithms.json
+-rw-r--r--   0        0        0      132 2024-05-22 14:49:23.963539 autotuning_methodology-1.0.0b5/extra/.vscode/settings.json
+-rwxr-xr-x   0        0        0    18897 2024-05-22 14:49:23.963539 autotuning_methodology-1.0.0b5/extra/bootstrap_hyperparams_visualizer.py
+-rwxr-xr-x   0        0        0    19811 2024-05-22 14:49:23.963539 autotuning_methodology-1.0.0b5/extra/experiments_strategies.py
+-rwxr-xr-x   0        0        0   119690 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/extra/experiments_strategies_hyperparamtuning.py
+-rwxr-xr-x   0        0        0     7475 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/extra/generate_cachefile.py
+-rw-r--r--   0        0        0    20608 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/extra/max_draw_k_from_n.py
+-rw-r--r--   0        0        0     3259 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/extra/speedtest_index_performance.py
+-rw-r--r--   0        0        0     1174 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/extra/speedtest_python_reversed_nan_sort.py
+-rwxr-xr-x   0        0        0     2545 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/extra/try_BOtorch.py
+-rwxr-xr-x   0        0        0     8426 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/extra/try_GPytorch.py
+-rw-r--r--   0        0        0    20822 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/extra/try_isotonic_regression.py
+-rwxr-xr-x   0        0        0      435 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/mypy.ini
+-rw-r--r--   0        0        0     1089 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/noxfile.py
+-rwxr-xr-x   0        0        0       17 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/profilings/.gitignore
+-rw-r--r--   0        0        0     2816 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/pyproject.toml
+-rw-r--r--   0        0        0       95 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/src/autotuning_methodology/__init__.py
+-rw-r--r--   0        0        0    17647 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/src/autotuning_methodology/baseline.py
+-rwxr-xr-x   0        0        0     8418 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/src/autotuning_methodology/caching.py
+-rw-r--r--   0        0        0    51986 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/src/autotuning_methodology/curves.py
+-rwxr-xr-x   0        0        0     9832 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/src/autotuning_methodology/experiments.py
+-rwxr-xr-x   0        0        0    24377 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/src/autotuning_methodology/runner.py
+-rwxr-xr-x   0        0        0     4138 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/src/autotuning_methodology/schema.json
+-rw-r--r--   0        0        0    25701 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/src/autotuning_methodology/searchspace_statistics.py
+-rw-r--r--   0        0        0     1787 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/src/autotuning_methodology/validators.py
+-rwxr-xr-x   0        0        0    48490 2024-05-22 14:49:23.967539 autotuning_methodology-1.0.0b5/src/autotuning_methodology/visualize_experiments.py
+-rw-r--r--   0        0        0  3269061 2024-05-22 14:49:23.979539 autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~0.json
+-rw-r--r--   0        0        0  3255846 2024-05-22 14:49:23.983539 autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~1.json
+-rw-r--r--   0        0        0  3483805 2024-05-22 14:49:23.999539 autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/mockfiles/mock_gpu.json
+-rw-r--r--   0        0        0     2967 2024-05-22 14:49:23.999539 autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/mockfiles/mocktest_kernel_convolution.py
+-rw-r--r--   0        0        0     1489 2024-05-22 14:49:23.999539 autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/mockfiles/test.json
+-rw-r--r--   0        0        0     1476 2024-05-22 14:49:23.999539 autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/mockfiles/test_bad_kernel_path.json
+-rw-r--r--   0        0        0     1465 2024-05-22 14:49:23.999539 autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/mockfiles/test_cached.json
+-rw-r--r--   0        0        0     1453 2024-05-22 14:49:23.999539 autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/mockfiles/test_import_runs.json
+-rw-r--r--   0        0        0     8913 2024-05-22 14:49:23.999539 autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/test_run_experiment.py
+-rw-r--r--   0        0        0     2934 2024-05-22 14:49:23.999539 autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/test_visualization.py
+-rw-r--r--   0        0        0     1978 2024-05-22 14:49:23.999539 autotuning_methodology-1.0.0b5/tests/autotuning_methodology/release/test_toml_file.py
+-rw-r--r--   0        0        0       34 2024-05-22 14:49:23.999539 autotuning_methodology-1.0.0b5/tests/autotuning_methodology/unit/test_caching.py
+-rw-r--r--   0        0        0     3464 2024-05-22 14:49:23.999539 autotuning_methodology-1.0.0b5/tests/autotuning_methodology/unit/test_curves.py
+-rw-r--r--   0        0        0     9885 1970-01-01 00:00:00.000000 autotuning_methodology-1.0.0b5/PKG-INFO
```

### Comparing `autotuning_methodology-1.0.0b4/.github/workflows/build-test-python-package.yml` & `autotuning_methodology-1.0.0b5/.github/workflows/build-test-python-package.yml`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/.github/workflows/publish-documentation.yml` & `autotuning_methodology-1.0.0b5/.github/workflows/publish-documentation.yml`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/.github/workflows/publish-package.yml` & `autotuning_methodology-1.0.0b5/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/.gitignore` & `autotuning_methodology-1.0.0b5/.gitignore`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/.vscode/settings.json` & `autotuning_methodology-1.0.0b5/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/CITATION.cff` & `autotuning_methodology-1.0.0b5/CITATION.cff`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/LICENSE` & `autotuning_methodology-1.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/README.md` & `autotuning_methodology-1.0.0b5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 ![PyPI - License](https://img.shields.io/pypi/l/autotuning_methodology)
 [![Build Status](https://github.com/autotuningassociation/autotuning_methodology/actions/workflows/build-test-python-package.yml/badge.svg)](https://github.com/autotuningassociation/autotuning_methodology/actions/workflows/build-test-python-package.yml)
 [![Docs](https://img.shields.io/github/actions/workflow/status/autotuningassociation/autotuning_methodology/publish-documentation.yml?label=docs)](https://autotuningassociation.github.io/autotuning_methodology/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/autotuning_methodology)](https://pypi.org/project/autotuning_methodology/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/autotuning_methodology)](https://pypi.org/project/autotuning_methodology/)
 ![PyPI - Status](https://img.shields.io/pypi/status/autotuning_methodology)
+![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.11207515.svg)
 
  
 This repository contains the software package accompanying the paper "A Methodology for Comparing Auto-Tuning Optimization Algorithms". 
 It makes the guidelines in the methodology easy to apply: simply specify the  `.json` file, run `autotuning_visualize [path_to_json]` and wait for the results!
 
 ### Limitations & Future Work
 Currently, the stable releases of this software package are compatible with [Kernel Tuner](https://github.com/KernelTuner/kernel_tuner) and [KTT](https://github.com/HiPerCoRe/KTT), as in the paper. We plan to soon extend this to support more frameworks.
```

### Comparing `autotuning_methodology-1.0.0b4/UML/.$Sequence Diagram.drawio.bkp` & `autotuning_methodology-1.0.0b5/UML/.$Sequence Diagram.drawio.bkp`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/UML/.$flowchart.drawio.bkp` & `autotuning_methodology-1.0.0b5/UML/.$flowchart.drawio.bkp`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/UML/Sequence Diagram.drawio` & `autotuning_methodology-1.0.0b5/UML/Sequence Diagram.drawio`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/UML/classes.pdf` & `autotuning_methodology-1.0.0b5/UML/classes.pdf`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/UML/flowchart/.$flowchart.drawio.bkp` & `autotuning_methodology-1.0.0b5/UML/flowchart/.$flowchart.drawio.bkp`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/UML/flowchart/flowchart.drawio` & `autotuning_methodology-1.0.0b5/UML/flowchart/flowchart.drawio`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/UML/flowchart/flowchart_output_generation.png` & `autotuning_methodology-1.0.0b5/UML/flowchart/flowchart_output_generation.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/UML/flowchart/flowchart_performance_curve_generation.png` & `autotuning_methodology-1.0.0b5/UML/flowchart/flowchart_performance_curve_generation.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/UML/flowchart/mini_plots/flowchart_plot_aggregated.png` & `autotuning_methodology-1.0.0b5/UML/flowchart/mini_plots/flowchart_plot_aggregated.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/UML/flowchart/mini_plots/flowchart_plot_individual.png` & `autotuning_methodology-1.0.0b5/UML/flowchart/mini_plots/flowchart_plot_individual.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/UML/flowchart/mini_plots/flowchart_plots.py` & `autotuning_methodology-1.0.0b5/UML/flowchart/mini_plots/flowchart_plots.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/UML/packages.pdf` & `autotuning_methodology-1.0.0b5/UML/packages.pdf`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/cached_data_used/cachefiles/ktt_values_to_kerneltuner.py` & `autotuning_methodology-1.0.0b5/cached_data_used/cachefiles/ktt_values_to_kerneltuner.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/docs/Makefile` & `autotuning_methodology-1.0.0b5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/docs/autotuning_methodology.rst` & `autotuning_methodology-1.0.0b5/docs/autotuning_methodology.rst`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/docs/conf.py` & `autotuning_methodology-1.0.0b5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/docs/contributing.rst` & `autotuning_methodology-1.0.0b5/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/docs/getting_started.rst` & `autotuning_methodology-1.0.0b5/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/docs/index.rst` & `autotuning_methodology-1.0.0b5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/docs/make.bat` & `autotuning_methodology-1.0.0b5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/docs/source/example_aggregated.png` & `autotuning_methodology-1.0.0b5/docs/source/example_aggregated.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/docs/source/flowchart_output_generation.png` & `autotuning_methodology-1.0.0b5/docs/source/flowchart_output_generation.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/docs/source/flowchart_performance_curve_generation.png` & `autotuning_methodology-1.0.0b5/docs/source/flowchart_performance_curve_generation.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/docs/source/logo_autotuning_methodology.svg` & `autotuning_methodology-1.0.0b5/docs/source/logo_autotuning_methodology.svg`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/docs/source/logo_kernel_dashboard.svg` & `autotuning_methodology-1.0.0b5/docs/source/logo_kernel_dashboard.svg`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/docs/source/logo_kernel_launcher.svg` & `autotuning_methodology-1.0.0b5/docs/source/logo_kernel_launcher.svg`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/docs/source/logo_kernel_tuner.svg` & `autotuning_methodology-1.0.0b5/docs/source/logo_kernel_tuner.svg`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/experiment_files/bootstrap_hyperparams.json` & `autotuning_methodology-1.0.0b5/experiment_files/bootstrap_hyperparams.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/experiment_files/example_visualizations.json` & `autotuning_methodology-1.0.0b5/experiment_files/example_visualizations.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666666%*

 * *Differences: {"'cutoff_type'": "'time'", "'strategy_defaults'": "{'cutoff_margin': 1.1}"}*

```diff
@@ -2,15 +2,15 @@
     "GPUs": [
         "RTX_3090",
         "RTX_2080_Ti"
     ],
     "bruteforced_caches_path": "../cached_data_used/cachefiles",
     "cutoff_percentile": 0.95,
     "cutoff_percentile_start": 0.5,
-    "cutoff_type": "fevals",
+    "cutoff_type": "time",
     "folder_id": "example_visualization",
     "kernels": [
         "gemm"
     ],
     "kernels_path": "../cached_data_used/kernels",
     "minimization": true,
     "name": "Example visualization",
@@ -48,14 +48,15 @@
         {
             "display_name": "Simulated Annealing",
             "name": "simulated_annealing",
             "strategy": "simulated_annealing"
         }
     ],
     "strategy_defaults": {
+        "cutoff_margin": 1.1,
         "minimum_number_of_evaluations": 20,
         "record_data": [
             "time",
             "GFLOP/s"
         ],
         "repeats": 100,
         "stochastic": true
```

### Comparing `autotuning_methodology-1.0.0b4/experiment_files/methodology_paper_evaluation.json` & `autotuning_methodology-1.0.0b5/experiment_files/methodology_paper_evaluation.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/experiment_files/milo_hotspot.json` & `autotuning_methodology-1.0.0b5/experiment_files/milo_hotspot.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/experiment_files/presentation_comparison.json` & `autotuning_methodology-1.0.0b5/experiment_files/presentation_comparison.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/experiment_files/simple_example.json` & `autotuning_methodology-1.0.0b5/experiment_files/simple_example.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/experiment_files/test_random_calculated.json` & `autotuning_methodology-1.0.0b5/experiment_files/test_random_calculated.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/experiment_files/test_scatter.json` & `autotuning_methodology-1.0.0b5/experiment_files/test_scatter.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/experiment_files/test_searchspace_algorithms.json` & `autotuning_methodology-1.0.0b5/experiment_files/test_searchspace_algorithms.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/extra/bootstrap_hyperparams_visualizer.py` & `autotuning_methodology-1.0.0b5/extra/bootstrap_hyperparams_visualizer.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/extra/experiments_strategies.py` & `autotuning_methodology-1.0.0b5/extra/experiments_strategies.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/extra/experiments_strategies_hyperparamtuning.py` & `autotuning_methodology-1.0.0b5/extra/experiments_strategies_hyperparamtuning.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/extra/generate_cachefile.py` & `autotuning_methodology-1.0.0b5/extra/generate_cachefile.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/extra/max_draw_k_from_n.py` & `autotuning_methodology-1.0.0b5/extra/max_draw_k_from_n.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/extra/speedtest_index_performance.py` & `autotuning_methodology-1.0.0b5/extra/speedtest_index_performance.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/extra/speedtest_python_reversed_nan_sort.py` & `autotuning_methodology-1.0.0b5/extra/speedtest_python_reversed_nan_sort.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/extra/try_BOtorch.py` & `autotuning_methodology-1.0.0b5/extra/try_BOtorch.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/extra/try_GPytorch.py` & `autotuning_methodology-1.0.0b5/extra/try_GPytorch.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/extra/try_isotonic_regression.py` & `autotuning_methodology-1.0.0b5/extra/try_isotonic_regression.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/noxfile.py` & `autotuning_methodology-1.0.0b5/noxfile.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/pyproject.toml` & `autotuning_methodology-1.0.0b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.8.0,<4"]
 
 [project] # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#declaring-project-metadata
 name = "autotuning_methodology"
-version = "1.0.0b4"
+version = "1.0.0b5"
 authors = [{ name = "Floris-Jan Willemsen", email = "fjwillemsen97@gmail.com" }]
 description = "Software package easing implementation of the guidelines of the 2024 paper 'A Methodology for Comparing Auto-Tuning Optimization Algorithms'."
 keywords = ["autotuning", "auto-tuning", "methodology", "scientific"]
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `autotuning_methodology-1.0.0b4/src/autotuning_methodology/baseline.py` & `autotuning_methodology-1.0.0b5/src/autotuning_methodology/baseline.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/src/autotuning_methodology/caching.py` & `autotuning_methodology-1.0.0b5/src/autotuning_methodology/caching.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/src/autotuning_methodology/curves.py` & `autotuning_methodology-1.0.0b5/src/autotuning_methodology/curves.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/src/autotuning_methodology/experiments.py` & `autotuning_methodology-1.0.0b5/src/autotuning_methodology/experiments.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     experiment_folder_id: str = experiment["folder_id"]
     minimization: bool = experiment.get("minimization", True)
     cutoff_percentile: float = experiment.get("cutoff_percentile", 1)
     cutoff_type: str = experiment.get("cutoff_type", "fevals")
     assert cutoff_type == "fevals" or cutoff_type == "time", f"cutoff_type must be 'fevals' or 'time', is {cutoff_type}"
     curve_segment_factor: float = experiment.get("curve_segment_factor", 0.05)
     assert isinstance(curve_segment_factor, float), f"curve_segment_factor is not float, {type(curve_segment_factor)}"
-    strategies = get_strategies(experiment)
+    strategies: list[dict] = get_strategies(experiment)
 
     # add the kernel directory to the path to import the module, relative to the experiment file
     kernels_path = experiment_folderpath / Path(experiment["kernels_path"])
     if not kernels_path.exists():
         raise FileNotFoundError(f"No such path {kernels_path.resolve()}, CWD: {getcwd()}")
     sys.path.append(str(kernels_path))
     kernel_names = experiment["kernels"]
@@ -175,28 +175,30 @@
 
             print(f" | - optimizing kernel '{kernel_name}'")
             results_descriptions[gpu_name][kernel_name] = dict()
             for strategy in strategies:
                 strategy_name: str = strategy["name"]
                 strategy_display_name: str = strategy["display_name"]
                 stochastic = strategy["stochastic"]
+                cutoff_margin = strategy.get(
+                    "cutoff_margin", 1.1
+                )  # +10% margin, to make sure cutoff_point is reached by compensating for potential non-valid evaluations  # noqa: E501
                 print(f" | - | using strategy '{strategy['display_name']}'")
 
                 # setup the results description
                 if "options" not in strategy:
                     strategy["options"] = dict()
-                cutoff_margin = 1.1  # +10% margin, to make sure cutoff_point is reached by compensating for potential non-valid evaluations  # noqa: E501
 
-                # TODO make sure this works correctly
-                # if cutoff_type == 'time':
-                #     strategy['options']['time_limit'] = cutoff_point_time * cutoff_margin
-                # else:
-                strategy["options"]["max_fevals"] = min(
-                    int(ceil(cutoff_point_fevals * cutoff_margin)), searchspace_stats.size
-                )
+                # set when to stop
+                if cutoff_type == "time":
+                    strategy["options"]["time_limit"] = cutoff_point_time * cutoff_margin
+                else:
+                    strategy["options"]["max_fevals"] = min(
+                        int(ceil(cutoff_point_fevals * cutoff_margin)), searchspace_stats.size
+                    )
                 results_description = ResultsDescription(
                     experiment_folder_id,
                     kernel_name,
                     gpu_name,
                     strategy_name,
                     strategy_display_name,
                     stochastic,
```

### Comparing `autotuning_methodology-1.0.0b4/src/autotuning_methodology/runner.py` & `autotuning_methodology-1.0.0b5/src/autotuning_methodology/runner.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/src/autotuning_methodology/schema.json` & `autotuning_methodology-1.0.0b5/src/autotuning_methodology/schema.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/src/autotuning_methodology/searchspace_statistics.py` & `autotuning_methodology-1.0.0b5/src/autotuning_methodology/searchspace_statistics.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/src/autotuning_methodology/validators.py` & `autotuning_methodology-1.0.0b5/src/autotuning_methodology/validators.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/src/autotuning_methodology/visualize_experiments.py` & `autotuning_methodology-1.0.0b5/src/autotuning_methodology/visualize_experiments.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~0.json` & `autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~0.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~1.json` & `autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~1.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/mockfiles/mock_gpu.json` & `autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/mockfiles/mock_gpu.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/mockfiles/mocktest_kernel_convolution.py` & `autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/mockfiles/mocktest_kernel_convolution.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/mockfiles/test.json` & `autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/mockfiles/test.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/mockfiles/test_bad_kernel_path.json` & `autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/mockfiles/test_bad_kernel_path.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/mockfiles/test_cached.json` & `autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/mockfiles/test_cached.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/mockfiles/test_import_runs.json` & `autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/mockfiles/test_import_runs.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/test_run_experiment.py` & `autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/test_run_experiment.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/tests/autotuning_methodology/integration/test_visualization.py` & `autotuning_methodology-1.0.0b5/tests/autotuning_methodology/integration/test_visualization.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/tests/autotuning_methodology/release/test_toml_file.py` & `autotuning_methodology-1.0.0b5/tests/autotuning_methodology/release/test_toml_file.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/tests/autotuning_methodology/unit/test_curves.py` & `autotuning_methodology-1.0.0b5/tests/autotuning_methodology/unit/test_curves.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b4/PKG-INFO` & `autotuning_methodology-1.0.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotuning_methodology
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: Software package easing implementation of the guidelines of the 2024 paper 'A Methodology for Comparing Auto-Tuning Optimization Algorithms'.
 Keywords: autotuning,auto-tuning,methodology,scientific
 Author-email: Floris-Jan Willemsen <fjwillemsen97@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -49,14 +49,15 @@
 
 ![PyPI - License](https://img.shields.io/pypi/l/autotuning_methodology)
 [![Build Status](https://github.com/autotuningassociation/autotuning_methodology/actions/workflows/build-test-python-package.yml/badge.svg)](https://github.com/autotuningassociation/autotuning_methodology/actions/workflows/build-test-python-package.yml)
 [![Docs](https://img.shields.io/github/actions/workflow/status/autotuningassociation/autotuning_methodology/publish-documentation.yml?label=docs)](https://autotuningassociation.github.io/autotuning_methodology/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/autotuning_methodology)](https://pypi.org/project/autotuning_methodology/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/autotuning_methodology)](https://pypi.org/project/autotuning_methodology/)
 ![PyPI - Status](https://img.shields.io/pypi/status/autotuning_methodology)
+![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.11207515.svg)
 
  
 This repository contains the software package accompanying the paper "A Methodology for Comparing Auto-Tuning Optimization Algorithms". 
 It makes the guidelines in the methodology easy to apply: simply specify the  `.json` file, run `autotuning_visualize [path_to_json]` and wait for the results!
 
 ### Limitations & Future Work
 Currently, the stable releases of this software package are compatible with [Kernel Tuner](https://github.com/KernelTuner/kernel_tuner) and [KTT](https://github.com/HiPerCoRe/KTT), as in the paper. We plan to soon extend this to support more frameworks.
```

