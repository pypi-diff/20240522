# Comparing `tmp/timeseriesflattener-2.2.4.tar.gz` & `tmp/timeseriesflattener-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseriesflattener-2.2.4.tar", last modified: Fri May 17 12:54:26 2024, max compression
+gzip compressed data, was "timeseriesflattener-2.2.5.tar", last modified: Wed May 22 07:30:38 2024, max compression
```

## Comparing `timeseriesflattener-2.2.4.tar` & `timeseriesflattener-2.2.5.tar`

### file list

```diff
@@ -1,214 +1,213 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.301473 timeseriesflattener-2.2.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.237473 timeseriesflattener-2.2.4/.devcontainer/
--rw-r--r--   0 root         (0) root         (0)     1639 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.devcontainer/devcontainer.json
--rw-r--r--   0 root         (0) root         (0)      148 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.devcontainer/post-start.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.237473 timeseriesflattener-2.2.4/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.225473 timeseriesflattener-2.2.4/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.237473 timeseriesflattener-2.2.4/.github/actions/test/
--rw-r--r--   0 root         (0) root         (0)      901 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/actions/test/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.237473 timeseriesflattener-2.2.4/.github/actions/test_tutorials/
--rw-r--r--   0 root         (0) root         (0)      885 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/actions/test_tutorials/action.yml
--rw-r--r--   0 root         (0) root         (0)      529 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)     1689 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/recommended_repo_setup.md
--rw-r--r--   0 root         (0) root         (0)      465 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/setup_ci.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.237473 timeseriesflattener-2.2.4/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      636 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/workflows/benchmark.yml
--rw-r--r--   0 root         (0) root         (0)      720 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)      849 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      898 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      727 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/workflows/generate_paper_pdf.yml
--rw-r--r--   0 root         (0) root         (0)     1939 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/workflows/main_test_and_release.yml
--rw-r--r--   0 root         (0) root         (0)     1025 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     1132 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)      788 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.github/workflows/static_type_checks.yml
--rw-r--r--   0 root         (0) root         (0)     2885 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.gitignore
--rw-r--r--   0 root         (0) root         (0)      697 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.python-version
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.241473 timeseriesflattener-2.2.4/.vscode/
--rw-r--r--   0 root         (0) root         (0)      346 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.vscode/extensions.json
--rw-r--r--   0 root         (0) root         (0)      249 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.vscode/settings.json
--rw-r--r--   0 root         (0) root         (0)     1373 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.vscode/tasks.json
--rw-r--r--   0 root         (0) root         (0)     1286 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)    74868 2024-05-17 12:54:21.000000 timeseriesflattener-2.2.4/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5238 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4474 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1031 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1087 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      262 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/Makefile
--rw-r--r--   0 root         (0) root         (0)    11525 2024-05-17 12:54:26.301473 timeseriesflattener-2.2.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7649 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/README.md
--rw-r--r--   0 root         (0) root         (0)     1763 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.241473 timeseriesflattener-2.2.4/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.241473 timeseriesflattener-2.2.4/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    15406 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    49714 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)    49714 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   424821 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/_static/terminology_figure.png
--rw-r--r--   0 root         (0) root         (0)      291 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/aggregators.rst
--rw-r--r--   0 root         (0) root         (0)     4115 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2097 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     1013 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/feature_specifications.rst
--rw-r--r--   0 root         (0) root         (0)      295 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/flattener.rst
--rw-r--r--   0 root         (0) root         (0)     5165 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      299 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/installation.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.245473 timeseriesflattener-2.2.4/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)   128585 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/tutorials/01_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    50850 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/tutorials/02_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)    29677 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/tutorials/03_text.ipynb
--rw-r--r--   0 root         (0) root         (0)     5314 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/tutorials/04_from_legacy.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.245473 timeseriesflattener-2.2.4/docs/tutorials/img/
--rw-r--r--   0 root         (0) root         (0)    78953 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/tutorials/img/term_a.png
--rw-r--r--   0 root         (0) root         (0)   109486 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/tutorials/img/term_b.png
--rw-r--r--   0 root         (0) root         (0)   107613 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/tutorials/img/term_c.png
--rw-r--r--   0 root         (0) root         (0)   250306 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/tutorials/img/term_d.png
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/docs/tutorials.rst
--rw-r--r--   0 root         (0) root         (0)     1833 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/example.py
--rw-r--r--   0 root         (0) root         (0)    49714 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/icon.png
--rw-r--r--   0 root         (0) root         (0)      426 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/lefthook.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.245473 timeseriesflattener-2.2.4/paper/
--rw-r--r--   0 root         (0) root         (0)    14392 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9344 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)     4633 2024-05-17 12:54:21.000000 timeseriesflattener-2.2.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2520 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/requirements-dev.lock
--rw-r--r--   0 root         (0) root         (0)     1474 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/requirements.lock
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 12:54:26.301473 timeseriesflattener-2.2.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.245473 timeseriesflattener-2.2.4/src/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/conftest.py
--rw-r--r--   0 root         (0) root         (0)     5207 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/test_benchmark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.249472 timeseriesflattener-2.2.4/src/timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)      776 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1467 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/_frame_validator.py
--rw-r--r--   0 root         (0) root         (0)     3924 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/_intermediary_frames.py
--rw-r--r--   0 root         (0) root         (0)     3922 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/aggregators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.253473 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      227 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/default_column_names.py
--rw-r--r--   0 root         (0) root         (0)     3708 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/from_legacy.py
--rw-r--r--   0 root         (0) root         (0)     2978 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/meta.py
--rw-r--r--   0 root         (0) root         (0)     2498 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/outcome.py
--rw-r--r--   0 root         (0) root         (0)     1899 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/prediction_times.py
--rw-r--r--   0 root         (0) root         (0)     1389 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/predictor.py
--rw-r--r--   0 root         (0) root         (0)     1434 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/static.py
--rw-r--r--   0 root         (0) root         (0)     1349 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/test_from_legacy.py
--rw-r--r--   0 root         (0) root         (0)     1917 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/test_specs.py
--rw-r--r--   0 root         (0) root         (0)     2144 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/timedelta.py
--rw-r--r--   0 root         (0) root         (0)     1241 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/timestamp_frame.py
--rw-r--r--   0 root         (0) root         (0)     7279 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/flattener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.253473 timeseriesflattener-2.2.4/src/timeseriesflattener/frame_utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/frame_utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      505 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/frame_utilities/_horisontally_concat.py
--rw-r--r--   0 root         (0) root         (0)      644 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py
--rw-r--r--   0 root         (0) root         (0)     1049 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/process_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.253473 timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1043 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/static.py
--rw-r--r--   0 root         (0) root         (0)    10309 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/temporal.py
--rw-r--r--   0 root         (0) root         (0)     1864 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/test_static.py
--rw-r--r--   0 root         (0) root         (0)    10592 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/test_temporal.py
--rw-r--r--   0 root         (0) root         (0)     1542 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/timedelta.py
--rw-r--r--   0 root         (0) root         (0)     5207 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/test_aggregators.py
--rw-r--r--   0 root         (0) root         (0)    12858 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/test_flattener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.253473 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/
--rw-r--r--   0 root         (0) root         (0)     1519 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/load_synth_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.257473 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5619 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
--rw-r--r--   0 root         (0) root         (0)     2746 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
--rw-r--r--   0 root         (0) root         (0)     1958 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
--rw-r--r--   0 root         (0) root         (0)      983 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.229472 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.229472 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.257473 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1494 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.273473 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      754 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)      830 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      807 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      731 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   200734 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv
--rw-r--r--   0 root         (0) root         (0)   248865 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
--rw-r--r--   0 root         (0) root         (0)     5511 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/testing/utils_for_testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.273473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/
--rw-r--r--   0 root         (0) root         (0)      264 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2855 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     1070 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/df_transforms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.273473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_cache/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2016 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py
--rw-r--r--   0 root         (0) root         (0)     6160 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.273473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_specs/
--rw-r--r--   0 root         (0) root         (0)     5535 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_specs/group_specs.py
--rw-r--r--   0 root         (0) root         (0)     7823 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_specs/single_specs.py
--rw-r--r--   0 root         (0) root         (0)    35315 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2150 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/flattened_ds_validator.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/logger.py
--rw-r--r--   0 root         (0) root         (0)     7524 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/misc_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.277473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/
--rw-r--r--   0 root         (0) root         (0)     2981 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/load_synth_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.277473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5527 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py
--rw-r--r--   0 root         (0) root         (0)     2697 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py
--rw-r--r--   0 root         (0) root         (0)     1962 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py
--rw-r--r--   0 root         (0) root         (0)      923 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.229472 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.229472 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.277473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1461 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.277473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/models/
--rw-r--r--   0 root         (0) root         (0)     1877 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py
--rw-r--r--   0 root         (0) root         (0)    25543 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl
--rw-r--r--   0 root         (0) root         (0)     1015 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.293473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      709 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)      795 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      772 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      696 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   200734 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv
--rw-r--r--   0 root         (0) root         (0)   248865 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv
--rw-r--r--   0 root         (0) root         (0)     5446 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/utils_for_testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.293473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.293473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_feature_cache/
--rw-r--r--   0 root         (0) root         (0)     3308 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.293473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13595 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     1295 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py
--rw-r--r--   0 root         (0) root         (0)     3399 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.297473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23392 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
--rw-r--r--   0 root         (0) root         (0)     2663 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
--rw-r--r--   0 root         (0) root         (0)     2308 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
--rw-r--r--   0 root         (0) root         (0)     2321 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
--rw-r--r--   0 root         (0) root         (0)     5796 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2420 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.297473 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/utils/
--rw-r--r--   0 root         (0) root         (0)      984 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/src/timeseriesflattener/v1/utils/pydantic_basemodel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:54:26.297473 timeseriesflattener-2.2.4/src/timeseriesflattener.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11525 2024-05-17 12:54:26.000000 timeseriesflattener-2.2.4/src/timeseriesflattener.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8537 2024-05-17 12:54:26.000000 timeseriesflattener-2.2.4/src/timeseriesflattener.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 12:54:26.000000 timeseriesflattener-2.2.4/src/timeseriesflattener.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      650 2024-05-17 12:54:26.000000 timeseriesflattener-2.2.4/src/timeseriesflattener.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-05-17 12:54:26.000000 timeseriesflattener-2.2.4/src/timeseriesflattener.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     8330 2024-05-17 12:54:20.000000 timeseriesflattener-2.2.4/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.516650 timeseriesflattener-2.2.5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.448650 timeseriesflattener-2.2.5/.devcontainer/
+-rw-r--r--   0 root         (0) root         (0)     1639 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.devcontainer/devcontainer.json
+-rw-r--r--   0 root         (0) root         (0)      148 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.devcontainer/post-start.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.452650 timeseriesflattener-2.2.5/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.440650 timeseriesflattener-2.2.5/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.452650 timeseriesflattener-2.2.5/.github/actions/test/
+-rw-r--r--   0 root         (0) root         (0)      901 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/actions/test/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.452650 timeseriesflattener-2.2.5/.github/actions/test_tutorials/
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/actions/test_tutorials/action.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/dependabot.yml
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/pull_request_template.md
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/recommended_repo_setup.md
+-rw-r--r--   0 root         (0) root         (0)      465 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/setup_ci.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.452650 timeseriesflattener-2.2.5/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      636 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/workflows/benchmark.yml
+-rw-r--r--   0 root         (0) root         (0)      720 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)      849 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      898 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      727 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/workflows/generate_paper_pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     1939 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/workflows/main_test_and_release.yml
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)      788 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      697 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.python-version
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.452650 timeseriesflattener-2.2.5/.vscode/
+-rw-r--r--   0 root         (0) root         (0)      346 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.vscode/extensions.json
+-rw-r--r--   0 root         (0) root         (0)      249 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.vscode/settings.json
+-rw-r--r--   0 root         (0) root         (0)     1373 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.vscode/tasks.json
+-rw-r--r--   0 root         (0) root         (0)     1286 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)    75066 2024-05-22 07:30:32.000000 timeseriesflattener-2.2.5/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5238 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4474 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      262 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/Makefile
+-rw-r--r--   0 root         (0) root         (0)    11525 2024-05-22 07:30:38.516650 timeseriesflattener-2.2.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7649 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/README.md
+-rw-r--r--   0 root         (0) root         (0)     1763 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.456650 timeseriesflattener-2.2.5/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.456650 timeseriesflattener-2.2.5/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)    15406 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    49714 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)    49714 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   424821 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/_static/terminology_figure.png
+-rw-r--r--   0 root         (0) root         (0)      291 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/aggregators.rst
+-rw-r--r--   0 root         (0) root         (0)     4115 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     1013 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/feature_specifications.rst
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/flattener.rst
+-rw-r--r--   0 root         (0) root         (0)     5165 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      299 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/installation.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.456650 timeseriesflattener-2.2.5/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)   128585 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/tutorials/01_basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    50850 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/tutorials/02_advanced.ipynb
+-rw-r--r--   0 root         (0) root         (0)    29677 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/tutorials/03_text.ipynb
+-rw-r--r--   0 root         (0) root         (0)     5314 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/tutorials/04_from_legacy.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.460650 timeseriesflattener-2.2.5/docs/tutorials/img/
+-rw-r--r--   0 root         (0) root         (0)    78953 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/tutorials/img/term_a.png
+-rw-r--r--   0 root         (0) root         (0)   109486 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/tutorials/img/term_b.png
+-rw-r--r--   0 root         (0) root         (0)   107613 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/tutorials/img/term_c.png
+-rw-r--r--   0 root         (0) root         (0)   250306 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/tutorials/img/term_d.png
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/tutorials.rst
+-rw-r--r--   0 root         (0) root         (0)     1833 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/example.py
+-rw-r--r--   0 root         (0) root         (0)    49714 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/icon.png
+-rw-r--r--   0 root         (0) root         (0)      426 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/lefthook.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.460650 timeseriesflattener-2.2.5/paper/
+-rw-r--r--   0 root         (0) root         (0)    14392 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9344 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)     4633 2024-05-22 07:30:32.000000 timeseriesflattener-2.2.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/requirements-dev.lock
+-rw-r--r--   0 root         (0) root         (0)     1474 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/requirements.lock
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 07:30:38.516650 timeseriesflattener-2.2.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.460650 timeseriesflattener-2.2.5/src/
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     5193 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/test_benchmark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.464650 timeseriesflattener-2.2.5/src/timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)      776 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/_frame_validator.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/_intermediary_frames.py
+-rw-r--r--   0 root         (0) root         (0)     3922 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/aggregators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.464650 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3708 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/from_legacy.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/meta.py
+-rw-r--r--   0 root         (0) root         (0)     2658 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/outcome.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)     1504 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/predictor.py
+-rw-r--r--   0 root         (0) root         (0)     1367 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/static.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/test_from_legacy.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/test_specs.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/timedelta.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/timestamp_frame.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/flattener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.468650 timeseriesflattener-2.2.5/src/timeseriesflattener/frame_utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/frame_utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      505 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/frame_utilities/_horisontally_concat.py
+-rw-r--r--   0 root         (0) root         (0)      614 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/process_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.468650 timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/static.py
+-rw-r--r--   0 root         (0) root         (0)    10312 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/temporal.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/test_static.py
+-rw-r--r--   0 root         (0) root         (0)    10592 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/test_temporal.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/timedelta.py
+-rw-r--r--   0 root         (0) root         (0)     5207 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/test_aggregators.py
+-rw-r--r--   0 root         (0) root         (0)    12858 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/test_flattener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.468650 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/
+-rw-r--r--   0 root         (0) root         (0)     1519 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/load_synth_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.468650 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5619 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
+-rw-r--r--   0 root         (0) root         (0)      983 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.444650 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.444650 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.468650 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1494 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.484650 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      754 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)      830 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      807 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      731 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   200734 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv
+-rw-r--r--   0 root         (0) root         (0)   248865 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 root         (0) root         (0)     5511 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.488650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/
+-rw-r--r--   0 root         (0) root         (0)      264 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2855 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/df_transforms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.488650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2016 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6160 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.488650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_specs/
+-rw-r--r--   0 root         (0) root         (0)     5548 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_specs/group_specs.py
+-rw-r--r--   0 root         (0) root         (0)     7846 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_specs/single_specs.py
+-rw-r--r--   0 root         (0) root         (0)    35315 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/flattened_ds_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/logger.py
+-rw-r--r--   0 root         (0) root         (0)     7546 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/misc_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.488650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/
+-rw-r--r--   0 root         (0) root         (0)     2981 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/load_synth_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.492650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5527 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py
+-rw-r--r--   0 root         (0) root         (0)     2697 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py
+-rw-r--r--   0 root         (0) root         (0)     1962 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py
+-rw-r--r--   0 root         (0) root         (0)      923 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.444650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.444650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.492650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1461 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.492650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/models/
+-rw-r--r--   0 root         (0) root         (0)     1877 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py
+-rw-r--r--   0 root         (0) root         (0)    25543 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl
+-rw-r--r--   0 root         (0) root         (0)     1015 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.508650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      709 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)      795 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      772 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      696 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   200734 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv
+-rw-r--r--   0 root         (0) root         (0)   248865 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 root         (0) root         (0)     5464 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.508650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.508650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_feature_cache/
+-rw-r--r--   0 root         (0) root         (0)     3308 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.508650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13595 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.512650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23392 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
+-rw-r--r--   0 root         (0) root         (0)     2663 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
+-rw-r--r--   0 root         (0) root         (0)     2321 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     5796 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.512650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/utils/
+-rw-r--r--   0 root         (0) root         (0)      984 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/utils/pydantic_basemodel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.512650 timeseriesflattener-2.2.5/src/timeseriesflattener.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11525 2024-05-22 07:30:38.000000 timeseriesflattener-2.2.5/src/timeseriesflattener.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8475 2024-05-22 07:30:38.000000 timeseriesflattener-2.2.5/src/timeseriesflattener.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 07:30:38.000000 timeseriesflattener-2.2.5/src/timeseriesflattener.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      650 2024-05-22 07:30:38.000000 timeseriesflattener-2.2.5/src/timeseriesflattener.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-05-22 07:30:38.000000 timeseriesflattener-2.2.5/src/timeseriesflattener.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     8330 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/tasks.py
```

### Comparing `timeseriesflattener-2.2.4/.devcontainer/devcontainer.json` & `timeseriesflattener-2.2.5/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/.github/actions/test/action.yml` & `timeseriesflattener-2.2.5/.github/actions/test/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/.github/actions/test_tutorials/action.yml` & `timeseriesflattener-2.2.5/.github/actions/test_tutorials/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/.github/dependabot.yml` & `timeseriesflattener-2.2.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/.github/recommended_repo_setup.md` & `timeseriesflattener-2.2.5/.github/recommended_repo_setup.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/.github/workflows/benchmark.yml` & `timeseriesflattener-2.2.5/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/.github/workflows/check_for_rej.yml` & `timeseriesflattener-2.2.5/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/.github/workflows/dependabot_automerge.yml` & `timeseriesflattener-2.2.5/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/.github/workflows/documentation.yml` & `timeseriesflattener-2.2.5/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/.github/workflows/generate_paper_pdf.yml` & `timeseriesflattener-2.2.5/.github/workflows/generate_paper_pdf.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/.github/workflows/main_test_and_release.yml` & `timeseriesflattener-2.2.5/.github/workflows/main_test_and_release.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/.github/workflows/pre-commit.yml` & `timeseriesflattener-2.2.5/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/.github/workflows/stalebot.yml` & `timeseriesflattener-2.2.5/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/.github/workflows/static_type_checks.yml` & `timeseriesflattener-2.2.5/.github/workflows/static_type_checks.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/.gitignore` & `timeseriesflattener-2.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/.pre-commit-config.yaml` & `timeseriesflattener-2.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/.vscode/tasks.json` & `timeseriesflattener-2.2.5/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/.zenodo.json` & `timeseriesflattener-2.2.5/.zenodo.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/CHANGELOG.md` & `timeseriesflattener-2.2.5/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.2.5 (2024-05-22)
+
+### Fix
+
+* Use Union in pydantic basemodels ([`a80a9c2`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/a80a9c24c6eb7e0ceadba021eb4474325b560a38))
+
 ## v2.2.4 (2024-05-17)
 
 ### Fix
 
 * Don't mix types in HasValuesAggregator fallback ([`dfdf5dd`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/dfdf5dd1417639e76ec1639f7c689464c1012f05))
 
 ### Documentation
```

### Comparing `timeseriesflattener-2.2.4/CODE_OF_CONDUCT.md` & `timeseriesflattener-2.2.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/CONTRIBUTING.md` & `timeseriesflattener-2.2.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/Dockerfile` & `timeseriesflattener-2.2.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/LICENSE` & `timeseriesflattener-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/PKG-INFO` & `timeseriesflattener-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 2.2.4
+Version: 2.2.5
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.2.4 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.2.5 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-2.2.4/README.md` & `timeseriesflattener-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/citation.cff` & `timeseriesflattener-2.2.5/citation.cff`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/docs/Makefile` & `timeseriesflattener-2.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/docs/_static/favicon.ico` & `timeseriesflattener-2.2.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/docs/_static/icon.png` & `timeseriesflattener-2.2.5/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/docs/_static/icon_dark.png` & `timeseriesflattener-2.2.5/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/docs/_static/terminology_figure.png` & `timeseriesflattener-2.2.5/docs/_static/terminology_figure.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/docs/conf.py` & `timeseriesflattener-2.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/docs/faq.rst` & `timeseriesflattener-2.2.5/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/docs/feature_specifications.rst` & `timeseriesflattener-2.2.5/docs/feature_specifications.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/docs/index.rst` & `timeseriesflattener-2.2.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/docs/tutorials/01_basic.ipynb` & `timeseriesflattener-2.2.5/docs/tutorials/01_basic.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/docs/tutorials/02_advanced.ipynb` & `timeseriesflattener-2.2.5/docs/tutorials/02_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/docs/tutorials/03_text.ipynb` & `timeseriesflattener-2.2.5/docs/tutorials/03_text.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/docs/tutorials/04_from_legacy.ipynb` & `timeseriesflattener-2.2.5/docs/tutorials/04_from_legacy.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/docs/tutorials/img/term_a.png` & `timeseriesflattener-2.2.5/docs/tutorials/img/term_a.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/docs/tutorials/img/term_b.png` & `timeseriesflattener-2.2.5/docs/tutorials/img/term_b.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/docs/tutorials/img/term_c.png` & `timeseriesflattener-2.2.5/docs/tutorials/img/term_c.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/docs/tutorials/img/term_d.png` & `timeseriesflattener-2.2.5/docs/tutorials/img/term_d.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/example.py` & `timeseriesflattener-2.2.5/example.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/icon.png` & `timeseriesflattener-2.2.5/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/paper/paper.bib` & `timeseriesflattener-2.2.5/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/paper/paper.md` & `timeseriesflattener-2.2.5/paper/paper.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/pyproject.toml` & `timeseriesflattener-2.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timeseriesflattener"
-version = "2.2.4"
+version = "2.2.5"
 authors = [
   { name = "Lasse Hansen", email = "lasseh0310@gmail.com" },
   { name = "Jakob Grøhn Damgaard", email = "bokajgd@gmail.com" },
   { name = "Kenneth Enevoldsen" },
   { name = "Martin Bernstorff", email = "martinbernstorff@gmail.com" },
 ]
 description = "A package for converting time series data from e.g. electronic health records into wide format data."
```

### Comparing `timeseriesflattener-2.2.4/requirements-dev.lock` & `timeseriesflattener-2.2.5/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/requirements.lock` & `timeseriesflattener-2.2.5/requirements.lock`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/conftest.py` & `timeseriesflattener-2.2.5/src/conftest.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/test_benchmark.py` & `timeseriesflattener-2.2.5/src/test_benchmark.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import joblib
 import numpy as np
 import polars as pl
 import pytest
 from iterpy.iter import Iter
 from timeseriesflattener.aggregators import Aggregator, MaxAggregator, MeanAggregator
-from timeseriesflattener.feature_specs.meta import LookDistance, ValueFrame
+from timeseriesflattener.feature_specs.meta import ValueFrame
 from timeseriesflattener.feature_specs.prediction_times import PredictionTimeFrame
 from timeseriesflattener.feature_specs.predictor import PredictorSpec
 from timeseriesflattener.flattener import Flattener
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
@@ -46,15 +46,15 @@
 
 @cache.cache()
 def _generate_benchmark_dataset(
     n_pred_times: int,
     n_features: int,
     n_observations_per_pred_time: int,
     aggregations: Sequence[Literal["max", "mean"]],
-    lookbehinds: Sequence[LookDistance | tuple[LookDistance, LookDistance]],
+    lookbehinds: Sequence[dt.timedelta | tuple[dt.timedelta, dt.timedelta]],
 ) -> BenchmarkDataset:
     pred_time_df = PredictionTimeFrame(
         init_df=pl.LazyFrame(
             {
                 "entity_id": list(range(n_pred_times)),
                 "pred_timestamp": [
                     dt.datetime.now() + dt.timedelta(days=random.randint(i, i + 10))
```

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/__init__.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/__init__.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/_frame_validator.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/_frame_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/_intermediary_frames.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/_intermediary_frames.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,37 +2,31 @@
 
 from dataclasses import InitVar, dataclass
 from typing import TYPE_CHECKING
 
 import polars as pl
 
 from ._frame_validator import _validate_col_name_columns_exist
-from .feature_specs.default_column_names import (
-    default_prediction_time_uuid_col_name,
-    default_timestamp_col_name,
-)
 from .frame_utilities.anyframe_to_lazyframe import _anyframe_to_lazyframe
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
-    from .feature_specs.meta import ValueType
-
 if TYPE_CHECKING:
     import datetime as dt
 
 
 @dataclass(frozen=True)
 class TimeMaskedFrame:
     """A frame that has had all values outside its lookbehind and lookahead distances masked."""
 
     init_df: pl.LazyFrame
     value_col_names: Sequence[str]
-    timestamp_col_name: str = default_timestamp_col_name
-    prediction_time_uuid_col_name: str = default_prediction_time_uuid_col_name
+    timestamp_col_name: str = "timestamp"
+    prediction_time_uuid_col_name: str = "prediction_time_uuid"
     validate_cols_exist: bool = True
 
     def __post_init__(self):
         if self.validate_cols_exist:
             _validate_col_name_columns_exist(obj=self)
 
     @property
@@ -43,20 +37,20 @@
         return self.init_df.collect()
 
 
 @dataclass
 class AggregatedValueFrame:
     df: pl.LazyFrame
     value_col_name: str
-    prediction_time_uuid_col_name: str = default_prediction_time_uuid_col_name
+    prediction_time_uuid_col_name: str = "prediction_time_uuid"
 
     def __post_init__(self):
         _validate_col_name_columns_exist(obj=self)
 
-    def fill_nulls(self, fallback: ValueType) -> AggregatedValueFrame:
+    def fill_nulls(self, fallback: int | float | str | None) -> AggregatedValueFrame:
         filled = self.df.with_columns(
             pl.col(self.value_col_name)
             .fill_null(fallback)
             .alias(f"{self.value_col_name}_fallback_{fallback}")
         ).drop([self.value_col_name])
 
         return AggregatedValueFrame(
@@ -72,15 +66,15 @@
 
 
 @dataclass
 class TimeDeltaFrame:
     df: pl.LazyFrame
     value_col_names: Sequence[str]
     value_timestamp_col_name: str
-    prediction_time_uuid_col_name: str = default_prediction_time_uuid_col_name
+    prediction_time_uuid_col_name: str = "prediction_time_uuid"
     timedelta_col_name: str = "time_from_prediction_to_value"
 
     def __post_init__(self):
         _validate_col_name_columns_exist(obj=self)
 
     def get_timedeltas(self) -> Sequence[dt.datetime]:
         return self.collect().get_column(self.timedelta_col_name).to_list()
```

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/aggregators.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/aggregators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/from_legacy.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/from_legacy.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/meta.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/meta.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,38 @@
 from __future__ import annotations
 
 import datetime as dt
-from collections.abc import Sequence
 from dataclasses import InitVar, dataclass
-from typing import TYPE_CHECKING, Literal, Union
+from typing import Literal
 
 import pandas as pd
 import polars as pl
 
-from timeseriesflattener.feature_specs.default_column_names import default_entity_id_col_name
-
 from .._frame_validator import _validate_col_name_columns_exist
 from ..frame_utilities.anyframe_to_lazyframe import _anyframe_to_lazyframe
 
-if TYPE_CHECKING:
-    from typing_extensions import TypeAlias
-
-
-ValueType = Union[int, float, str, None]
-InitDF_T = Union[pl.LazyFrame, pl.DataFrame, pd.DataFrame]
-
-
-LookDistance = dt.timedelta
-
-
-LookDistances: TypeAlias = Sequence[Union[LookDistance, tuple[LookDistance, LookDistance]]]
-
 
 @dataclass
 class ValueFrame:
     """A frame that contains the values of a time series.
 
     Must contain columns:
         entity_id_col_name: The name of the column containing the entity ids. Must be a string, and the column's values must be strings which are unique.
         value_timestamp_col_name: The name of the column containing the timestamps. Must be a string, and the column's values must be datetimes.
         Additional columns containing the values of the time series. The name of the columns will be used for feature naming.
     """
 
-    init_df: InitVar[InitDF_T]
-    entity_id_col_name: str = default_entity_id_col_name
+    init_df: InitVar[pl.LazyFrame | pl.DataFrame | pd.DataFrame]
+    entity_id_col_name: str = "entity_id"
     value_timestamp_col_name: str = "timestamp"
     coerce_to_lazy: InitVar[bool] = True
 
-    def __post_init__(self, init_df: InitDF_T, coerce_to_lazy: bool):
+    def __post_init__(
+        self, init_df: pl.LazyFrame | pl.DataFrame | pd.DataFrame, coerce_to_lazy: bool
+    ):
         if coerce_to_lazy:
             self.df = _anyframe_to_lazyframe(init_df)
         else:
             self.df: pl.LazyFrame = init_df
 
         _validate_col_name_columns_exist(obj=self)
         self.value_col_names = [
@@ -59,30 +45,30 @@
         if isinstance(self.df, pl.DataFrame):
             return self.df
         return self.df.collect()
 
 
 @dataclass(frozen=True)
 class LookPeriod:
-    first: LookDistance
-    last: LookDistance
+    first: dt.timedelta
+    last: dt.timedelta
 
     def __post_init__(self):
         if self.first >= self.last:
             raise ValueError(
                 f"Invalid LookPeriod. The first value ({self.first}) must be smaller than the large value ({self.last})."
             )
 
 
 def _lookdistance_to_normalised_lookperiod(
-    lookdistance: LookDistance | tuple[LookDistance, LookDistance],
+    lookdistance: dt.timedelta | tuple[dt.timedelta, dt.timedelta],
     direction: Literal["ahead", "behind"],
 ) -> LookPeriod:
     is_ahead = direction == "ahead"
-    if isinstance(lookdistance, LookDistance):
+    if isinstance(lookdistance, dt.timedelta):
         return LookPeriod(
             first=dt.timedelta(days=0) if is_ahead else -lookdistance,
             last=lookdistance if is_ahead else dt.timedelta(0),
         )
     return LookPeriod(
         first=lookdistance[0] if is_ahead else -lookdistance[1],
         last=lookdistance[1] if is_ahead else -lookdistance[0],
```

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/outcome.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/outcome.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from __future__ import annotations
 
+import datetime as dt
 from dataclasses import InitVar, dataclass
 from typing import TYPE_CHECKING
 
 import polars as pl
 
 from .._frame_validator import _validate_col_name_columns_exist
-from .meta import LookDistances, ValueFrame, ValueType, _lookdistance_to_normalised_lookperiod
+from .meta import ValueFrame, _lookdistance_to_normalised_lookperiod
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from ..aggregators import Aggregator
     from .timestamp_frame import TimestampValueFrame
 
 
 @dataclass
 class OutcomeSpec:
     """Specification for an outcome. If your outcome is binary/boolean, you can use BooleanOutcomeSpec instead."""
 
     value_frame: ValueFrame
-    lookahead_distances: InitVar[LookDistances]
+    lookahead_distances: InitVar[Sequence[dt.timedelta | tuple[dt.timedelta, dt.timedelta]]]
     aggregators: Sequence[Aggregator]
-    fallback: ValueType
+    fallback: int | float | str | None
     column_prefix: str = "outc"
 
-    def __post_init__(self, lookahead_distances: LookDistances):
+    def __post_init__(
+        self, lookahead_distances: Sequence[dt.timedelta | tuple[dt.timedelta, dt.timedelta]]
+    ):
         self.normalised_lookperiod = [
             _lookdistance_to_normalised_lookperiod(lookdistance=lookdistance, direction="ahead")
             for lookdistance in lookahead_distances
         ]
         _validate_col_name_columns_exist(obj=self)
 
     @property
@@ -43,15 +46,15 @@
 
     The init_frame must contain columns:
         entity_id_col_name: The name of the column containing the entity ids. Must be a string, and the column's values must be strings which are unique.
         value_timestamp_col_name: The name of the column containing the timestamps of when the event occurs. Must be a string, and the column's values must be datetimes.
     """
 
     init_frame: InitVar[TimestampValueFrame]
-    lookahead_distances: LookDistances
+    lookahead_distances: Sequence[dt.timedelta | tuple[dt.timedelta, dt.timedelta]]
     aggregators: Sequence[Aggregator]
     output_name: str
     column_prefix: str = "outc"
 
     def __post_init__(self, init_frame: TimestampValueFrame):
         self.normalised_lookperiod = [
             _lookdistance_to_normalised_lookperiod(lookdistance=lookdistance, direction="ahead")
```

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/prediction_times.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/prediction_times.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 from __future__ import annotations
 
 from dataclasses import InitVar, dataclass
 from typing import TYPE_CHECKING
 
+import pandas as pd
 import polars as pl
 
 from .._frame_validator import _validate_col_name_columns_exist
 from ..frame_utilities.anyframe_to_lazyframe import _anyframe_to_lazyframe
-from .default_column_names import (
-    default_entity_id_col_name,
-    default_pred_time_col_name,
-    default_prediction_time_uuid_col_name,
-)
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
-    from .meta import InitDF_T
-
 
 @dataclass
 class PredictionTimeFrame:
     """Specification for prediction times, i.e. the times for which predictions are made.
 
     init_df must be a dataframe (pandas or polars) containing columns:
         entity_id_col_name: The name of the column containing the entity ids.
         timestamp_col_name: The name of the column containing the timestamps for when to make a prediction.
     """
 
-    init_df: InitVar[InitDF_T]
-    entity_id_col_name: str = default_entity_id_col_name
-    timestamp_col_name: str = default_pred_time_col_name
-    prediction_time_uuid_col_name: str = default_prediction_time_uuid_col_name
+    init_df: InitVar[pl.LazyFrame | pl.DataFrame | pd.DataFrame]
+    entity_id_col_name: str = "entity_id"
+    timestamp_col_name: str = "pred_timestamp"
+    prediction_time_uuid_col_name: str = "prediction_time_uuid"
     coerce_to_lazy: InitVar[bool] = True
 
-    def __post_init__(self, init_df: InitDF_T, coerce_to_lazy: bool):
+    def __post_init__(
+        self, init_df: pl.LazyFrame | pl.DataFrame | pd.DataFrame, coerce_to_lazy: bool
+    ):
         if coerce_to_lazy:
             self.df = _anyframe_to_lazyframe(init_df)
         else:
             self.df: pl.LazyFrame = init_df
 
         self.df = self.df.with_columns(
             pl.concat_str(
```

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/predictor.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/predictor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
+import datetime as dt
 from dataclasses import InitVar, dataclass
 from typing import TYPE_CHECKING
 
 from .._frame_validator import _validate_col_name_columns_exist
-from .meta import LookDistances, ValueFrame, ValueType, _lookdistance_to_normalised_lookperiod
+from .meta import ValueFrame, _lookdistance_to_normalised_lookperiod
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     import polars as pl
 
     from ..aggregators import Aggregator
@@ -21,20 +22,22 @@
     The value_frame must contain columns:
         entity_id_col_name: The name of the column containing the entity ids.
         value_timestamp_col_name: The name of the column containing the timestamps for each value.
         additional columns containing values to aggregate. The name of the columns will be used for feature naming.
     """
 
     value_frame: ValueFrame
-    lookbehind_distances: InitVar[LookDistances]
+    lookbehind_distances: InitVar[Sequence[dt.timedelta | tuple[dt.timedelta, dt.timedelta]]]
     aggregators: Sequence[Aggregator]
-    fallback: ValueType
+    fallback: int | float | str | None
     column_prefix: str = "pred"
 
-    def __post_init__(self, lookbehind_distances: LookDistances):
+    def __post_init__(
+        self, lookbehind_distances: Sequence[dt.timedelta | tuple[dt.timedelta, dt.timedelta]]
+    ):
         self.normalised_lookperiod = [
             _lookdistance_to_normalised_lookperiod(lookdistance=lookdistance, direction="behind")
             for lookdistance in lookbehind_distances
         ]
         _validate_col_name_columns_exist(obj=self)
 
     @property
```

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/test_from_legacy.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/test_from_legacy.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/test_specs.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/test_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/timedelta.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/timedelta.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Literal
 
 from .._frame_validator import _validate_col_name_columns_exist
-from .meta import ValueFrame, ValueType
+from .meta import ValueFrame
 
 if TYPE_CHECKING:
     import polars as pl
 
     from .timestamp_frame import TimestampValueFrame
 
 
 @dataclass
 class TimeDeltaSpec:
     init_frame: TimestampValueFrame
-    fallback: ValueType
+    fallback: int | float | str | None
     output_name: str
     column_prefix: str = "pred"
     time_format: Literal["seconds", "minutes", "hours", "days", "years"] = "days"
     """Specification for a time delta feature, i.e. the time between a prediction timestamp and a value timestamp.
     Useful for e.g. calculating age or the time since a certain event.
 
     init_frame must contain columns:
```

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/feature_specs/timestamp_frame.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/timestamp_frame.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 from __future__ import annotations
 
 from dataclasses import InitVar, dataclass
-from typing import TYPE_CHECKING
 
+import pandas as pd
 import polars as pl
 
 from .._frame_validator import _validate_col_name_columns_exist
 from ..frame_utilities.anyframe_to_lazyframe import _anyframe_to_lazyframe
-from .default_column_names import default_entity_id_col_name
-
-if TYPE_CHECKING:
-    from .meta import InitDF_T
 
 
 @dataclass
 class TimestampValueFrame:
     """Timestamps, useful for computing e.g. age.
 
     Must contain columns:
         entity_id_col_name: The name of the column containing the entity ids. Must be a string, and the column's values must be strings which are unique.
         value_timestamp_col_name: The name of the column containing the timestamps. Must be a string, and the column's values must be datetimes.
     """
 
-    init_df: InitVar[InitDF_T]
-    entity_id_col_name: str = default_entity_id_col_name
+    init_df: InitVar[pl.LazyFrame | pl.DataFrame | pd.DataFrame]
+    entity_id_col_name: str = "entity_id"
     value_timestamp_col_name: str = "timestamp"
 
-    def __post_init__(self, init_df: InitDF_T):
+    def __post_init__(self, init_df: pl.LazyFrame | pl.DataFrame | pd.DataFrame):
         self.df = _anyframe_to_lazyframe(init_df)
         _validate_col_name_columns_exist(obj=self)
 
     def collect(self) -> pl.DataFrame:
         if isinstance(self.df, pl.DataFrame):
             return self.df
         return self.df.collect()
```

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/flattener.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/flattener.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/process_spec.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/process_spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING
 import datetime as dt
 
 from .feature_specs.static import StaticSpec
 from .feature_specs.timedelta import TimeDeltaSpec
 from .spec_processors.static import process_static_spec
 from .spec_processors.temporal import process_temporal_spec
 from .spec_processors.timedelta import process_timedelta_spec
```

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/static.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/static.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/temporal.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/temporal.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from typing import TYPE_CHECKING, Callable, Union
 
 import polars as pl
 import polars.selectors as cs
 from iterpy.iter import Iter
 
 from .._intermediary_frames import ProcessedFrame, TimeDeltaFrame, TimeMaskedFrame
+from ..feature_specs.meta import ValueFrame
 from ..feature_specs.outcome import BooleanOutcomeSpec, OutcomeSpec
+from ..feature_specs.prediction_times import PredictionTimeFrame
 from ..feature_specs.predictor import PredictorSpec
 from ..frame_utilities._horisontally_concat import horizontally_concatenate_dfs
-from ..feature_specs.prediction_times import PredictionTimeFrame
-from ..feature_specs.meta import ValueFrame, InitDF_T
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from ..aggregators import Aggregator
-    from ..feature_specs.meta import LookPeriod, ValueType
+    from ..feature_specs.meta import LookPeriod
 
 
 def _get_timedelta_frame(
     predictiontime_frame: PredictionTimeFrame, value_frame: ValueFrame
 ) -> TimeDeltaFrame:
     # Join the prediction time dataframe
     if predictiontime_frame.timestamp_col_name == value_frame.value_timestamp_col_name:
@@ -101,15 +101,17 @@
         prediction_time_uuid_col_name=timedelta_frame.prediction_time_uuid_col_name,
         value_col_names=new_colnames,
         timestamp_col_name=timedelta_frame.value_timestamp_col_name,
     )
 
 
 def _aggregate_masked_frame(
-    masked_frame: TimeMaskedFrame, aggregators: Sequence[Aggregator], fallback: ValueType
+    masked_frame: TimeMaskedFrame,
+    aggregators: Sequence[Aggregator],
+    fallback: int | float | str | None,
 ) -> pl.LazyFrame:
     aggregator_expressions = [
         aggregator(value_col_name)
         for aggregator in aggregators
         for value_col_name in masked_frame.value_col_names
     ]
```

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/test_static.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/test_static.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/test_temporal.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/test_temporal.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/spec_processors/timedelta.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/timedelta.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/test_aggregators.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/test_aggregators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/test_flattener.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/test_flattener.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/load_synth_data.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/synth_data_generator/utils.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/testing/utils_for_testing.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/aggregation_fns.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/df_transforms.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/df_transforms.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_specs/group_specs.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_specs/group_specs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import itertools
 from dataclasses import dataclass
 from typing import Dict, List, Sequence, Tuple, Union
 
 import pandas as pd
 from timeseriesflattener.v1.aggregation_fns import AggregationFunType
 from timeseriesflattener.v1.feature_specs.single_specs import AnySpec, OutcomeSpec, PredictorSpec
@@ -14,18 +15,18 @@
     name: str
 
 
 from typing import Protocol
 
 
 class V1PGSProtocol(Protocol):
-    lookbehind_days: Sequence[Union[float, Tuple[float, float]]]
+    lookbehind_days: Sequence[float | Tuple[float, float]]
     named_dataframes: Sequence[NamedDataframe]
     aggregation_fns: Sequence[AggregationFunType]
-    fallback: Sequence[Union[int, float, str]]
+    fallback: Sequence[int | float | str]
     prefix: str = "pred"
 
 
 class PredictorGroupSpec(BaseModel):
     """A group of predictor specifications.
 
     Args:
@@ -105,16 +106,16 @@
         ]
 
 
 GroupSpec = Union[PredictorGroupSpec, OutcomeGroupSpec]
 
 
 def create_feature_combinations_from_dict(
-    dictionary: Dict[str, Union[str, list]],
-) -> List[Dict[str, Union[str, float, int]]]:
+    dictionary: Dict[str, str | list],
+) -> List[Dict[str, str | float | int]]:
     """Create feature combinations from a dictionary of feature specifications.
     Only unpacks the top level of lists.
     Args:
         dictionary (Dict[str]): A dictionary of feature specifications.
     Returns
     -------
         List[Dict[str]]: list of all possible combinations of the arguments.
```

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/feature_specs/single_specs.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_specs/single_specs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from dataclasses import dataclass
 from typing import Tuple, Union
 
 import pandas as pd
 from timeseriesflattener.v1.aggregation_fns import AggregationFunType
 from timeseriesflattener.v1.utils.pydantic_basemodel import BaseModel
 
@@ -17,15 +18,15 @@
                 f"Invalid LookPeriod. The min_days ({self.min_days}) must be smaller than the max_days {self.max_days}."
             )
 
 
 @dataclass(frozen=True)
 class CoercedFloats:
     lookperiod: LookPeriod
-    fallback: Union[float, int]
+    fallback: float | int
 
 
 def can_be_coerced_losslessly_to_int(value: float) -> bool:
     try:
         int_version = int(value)
         return (int_version - value) == 0
     except ValueError:
@@ -75,15 +76,15 @@
 
 
 def get_temporal_col_name(
     prefix: str,
     feature_base_name: str,
     lookperiod: LookPeriod,
     aggregation_fn: AggregationFunType,
-    fallback: Union[float, int],
+    fallback: float | int,
 ) -> str:
     """Get the column name for the temporal feature."""
     coerced = coerce_floats(lookperiod=lookperiod, fallback=fallback)
     lookperiod_str = (
         f"{coerced.lookperiod.max_days!s}"
         if coerced.lookperiod.min_days == 0
         else f"{coerced.lookperiod.min_days!s}_to_{coerced.lookperiod.max_days!s}"
```

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/flattened_dataset.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/flattened_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -720,15 +720,15 @@
             min_timestamp = min(spec.timeseries_df[self.timestamp_col_name])  # type: ignore
 
             if min_timestamp < pd.Timestamp("1971-01-01"):  # type: ignore
                 log.warning(
                     f"{spec.feature_base_name}: Minimum timestamp is {min_timestamp} - perhaps ints were coerced to timestamps?"
                 )
 
-    def add_spec(self, spec: Union[Sequence[AnySpec], AnySpec]):
+    def add_spec(self, spec: Sequence[Union[AnySpec, AnySpec]]):
         """Add a specification to the flattened dataset.
 
         This adds it to a queue of unprocessed specs, which are not processed
         until you call the .compute() or .get_df() methods. This allows us to
         more effectiely parallelise the processing of the specs.
 
         Most of the complexity lies in the OutcomeSpec and PredictorSpec objects.
```

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/flattened_ds_validator.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/flattened_ds_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/logger.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Example of how to setup a logger with sensible defaults."""
 
 import logging
 from pathlib import Path
-from typing import Optional, Union
+from typing import Optional
 
 import coloredlogs
 
 from timeseriesflattener.v1.misc_utils import PROJECT_ROOT
 
 
 def setup_logger(
     name: str,
     level: int = logging.DEBUG,
-    log_file_path: Optional[Union[str, Path]] = None,
+    log_file_path: Optional[str | Path] = None,
     fmt: str = "%(asctime)s [%(levelname)s] %(message)s",
 ) -> logging.Logger:
     """
     Set up a logger with the given name and log level.
 
     Args:
         name (str): The name of the logger. Typically use __name__.
```

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/misc_utils.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/misc_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """A set of misc.
 
 utilities. If this file grows, consider splitting it up.
 """
+from __future__ import annotations
 
 import functools
 import logging
 import os
 from pathlib import Path
-from typing import Any, Callable, Dict, Hashable, List, Union
+from typing import Any, Callable, Dict, Hashable, List
 
 import catalogue
 import pandas as pd
 
 data_loaders = catalogue.create("timeseriesflattener", "data_loaders")
 split_dfs: Dict[str, pd.DataFrame] = {}  #
 
@@ -80,15 +81,15 @@
         .replace(": ", "-")
         .replace("{", "")
         .replace("}", "")
         .replace(", ", "_")
     )
 
 
-def load_dataset_from_file(file_path: Path, nrows: Union[int, None] = None) -> pd.DataFrame:
+def load_dataset_from_file(file_path: Path, nrows: int | None = None) -> pd.DataFrame:
     """Load dataset from file. Handles csv and parquet files based on suffix.
 
     Args:
         file_path (str): File name.
         nrows (int): Number of rows to load.
 
     Returns:
```

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/load_synth_data.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/testing/utils_for_testing.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/utils_for_testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """Utilities for testing."""
+from __future__ import annotations
+
 from io import StringIO
-from typing import Any, List, Optional, Sequence, Union
+from typing import Any, List, Optional, Sequence
+
 
 import numpy as np
 import pandas as pd
 import polars as pl
 from pandas import DataFrame
 from pandas.testing import assert_series_equal
 from timeseriesflattener.v1 import TimeseriesFlattener
@@ -78,27 +81,27 @@
         # Convert all str to float
         df = df.apply(pd.to_numeric, axis=0, errors="coerce")
 
     # Drop "Unnamed" cols
     return df.loc[:, ~df.columns.str.contains("^Unnamed")]
 
 
-def _get_value_cols_based_on_spec(df: pd.DataFrame, spec: AnySpec) -> Union[str, List[str]]:
+def _get_value_cols_based_on_spec(df: pd.DataFrame, spec: AnySpec) -> str | List[str]:
     """Get value columns based on spec. Checks if multiple value columns are present."""
     feature_name = spec.feature_base_name
     value_cols = df.columns[df.columns.str.contains(feature_name)].tolist()
     # to avoid indexing issues
     if len(value_cols) == 1:
         return value_cols[0]
 
     return value_cols
 
 
 def assert_flattened_data_as_expected(
-    prediction_times_df: Union[pd.DataFrame, str],
+    prediction_times_df: pd.DataFrame | str,
     output_spec: AnySpec,
     expected_df: Optional[pd.DataFrame] = None,
     expected_values: Optional[Sequence[Any]] = None,
     drop_pred_times_with_insufficient_look_distance: bool = False,
 ):
     """Flatten spec and assert that flattened data is as expected."""
     if isinstance(prediction_times_df, str):
```

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener/v1/utils/pydantic_basemodel.py` & `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/utils/pydantic_basemodel.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener.egg-info/PKG-INFO` & `timeseriesflattener-2.2.5/src/timeseriesflattener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 2.2.4
+Version: 2.2.5
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.2.4 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.2.5 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener.egg-info/SOURCES.txt` & `timeseriesflattener-2.2.5/src/timeseriesflattener.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 src/timeseriesflattener/test_flattener.py
 src/timeseriesflattener.egg-info/PKG-INFO
 src/timeseriesflattener.egg-info/SOURCES.txt
 src/timeseriesflattener.egg-info/dependency_links.txt
 src/timeseriesflattener.egg-info/requires.txt
 src/timeseriesflattener.egg-info/top_level.txt
 src/timeseriesflattener/feature_specs/__init__.py
-src/timeseriesflattener/feature_specs/default_column_names.py
 src/timeseriesflattener/feature_specs/from_legacy.py
 src/timeseriesflattener/feature_specs/meta.py
 src/timeseriesflattener/feature_specs/outcome.py
 src/timeseriesflattener/feature_specs/prediction_times.py
 src/timeseriesflattener/feature_specs/predictor.py
 src/timeseriesflattener/feature_specs/static.py
 src/timeseriesflattener/feature_specs/test_from_legacy.py
```

### Comparing `timeseriesflattener-2.2.4/src/timeseriesflattener.egg-info/requires.txt` & `timeseriesflattener-2.2.5/src/timeseriesflattener.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.4/tasks.py` & `timeseriesflattener-2.2.5/tasks.py`

 * *Files identical despite different names*

