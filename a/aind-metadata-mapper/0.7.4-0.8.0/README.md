# Comparing `tmp/aind_metadata_mapper-0.7.4.tar.gz` & `tmp/aind_metadata_mapper-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_metadata_mapper-0.7.4.tar", last modified: Mon May 13 22:23:52 2024, max compression
+gzip compressed data, was "aind_metadata_mapper-0.8.0.tar", last modified: Wed May 22 00:06:41 2024, max compression
```

## Comparing `aind_metadata_mapper-0.7.4.tar` & `aind_metadata_mapper-0.8.0.tar`

### file list

```diff
@@ -1,122 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.140164 aind_metadata_mapper-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.116165 aind_metadata_mapper-0.7.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.120164 aind_metadata_mapper-0.7.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.120164 aind_metadata_mapper-0.7.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-13 22:23:52.140164 aind_metadata_mapper-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.120164 aind_metadata_mapper-0.7.4/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.120164 aind_metadata_mapper-0.7.4/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.124164 aind_metadata_mapper-0.7.4/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/doc_template/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.124164 aind_metadata_mapper-0.7.4/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/examples/bergamo_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.124164 aind_metadata_mapper-0.7.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/scripts/singularity_build.def
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 22:23:52.140164 aind_metadata_mapper-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.116165 aind_metadata_mapper-0.7.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.124164 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 22:23:43.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.124164 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/bergamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23425 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/bergamo/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.124164 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/dynamic_routing/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/dynamic_routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/dynamic_routing/open_ephys_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/dynamic_routing/sync_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/dynamic_routing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.124164 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/ephys/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/ephys/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.128164 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/fib/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/fib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/fib/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/gather_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.128164 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/mesoscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/mesoscope/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.136165 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-13 22:23:52.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-13 22:23:52.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:23:52.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-13 22:23:52.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 22:23:52.000000 aind_metadata_mapper-0.7.4/src/aind_metadata_mapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.128164 aind_metadata_mapper-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.120164 aind_metadata_mapper-0.7.4/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.128164 aind_metadata_mapper-0.7.4/tests/resources/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/bergamo/cropped_neuron50_00001.tif
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/bergamo/example_description0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/bergamo/example_metadata.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/bergamo/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.128164 aind_metadata_mapper-0.7.4/tests/resources/ephys/
--rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/ephys/ephys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/ephys/newscale_main.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/ephys/newscale_surface_finding.csv
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/ephys/settings_main.xml
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/ephys/settings_surface_finding.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.132165 aind_metadata_mapper-0.7.4/tests/resources/fib/
--rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/fib/000000_ophys_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/fib/000000_ophys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/fib/example_from_teensy.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.132165 aind_metadata_mapper-0.7.4/tests/resources/gather_metadata_job/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/gather_metadata_job/example_funding_multiple_response.json
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/gather_metadata_job/example_funding_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/gather_metadata_job/example_procedures_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/gather_metadata_job/example_subject_response.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.132165 aind_metadata_mapper-0.7.4/tests/resources/gather_metadata_job/metadata_files/
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/gather_metadata_job/metadata_files/data_description.json
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/gather_metadata_job/metadata_files/procedures.json
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/gather_metadata_job/metadata_files/processing.json
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/gather_metadata_job/metadata_files/subject.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.132165 aind_metadata_mapper-0.7.4/tests/resources/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
--rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/mesoscope/example_extract.json
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/mesoscope/example_platform.json
--rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/mesoscope/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.136165 aind_metadata_mapper-0.7.4/tests/resources/neuropixels/
--rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/neuropixels/base-missing-probe_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/neuropixels/base_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/neuropixels/mvr.ini
--rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/neuropixels/mvr_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/neuropixels/open-ephys-inferred_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/neuropixels/open-ephys_rig.json
--rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/neuropixels/settings.mislabeled-probes-0.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/neuropixels/settings.mislabeled-probes-1.xml
--rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/neuropixels/settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/neuropixels/sync.yml
--rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/resources/neuropixels/sync_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    13902 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/test_bergamo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:23:52.136165 aind_metadata_mapper-0.7.4/tests/test_dynamic_routing/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/test_dynamic_routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/test_dynamic_routing/test_mvr_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/test_dynamic_routing/test_neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/test_dynamic_routing/test_open_ephys_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/test_dynamic_routing/test_sync_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/test_dynamic_routing/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/test_ephys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/test_fib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18222 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/test_gather_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/test_legacy_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-13 22:23:42.000000 aind_metadata_mapper-0.7.4/tests/test_mesoscope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.526428 aind_metadata_mapper-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.502428 aind_metadata_mapper-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.506428 aind_metadata_mapper-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.506428 aind_metadata_mapper-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-22 00:06:41.526428 aind_metadata_mapper-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.506428 aind_metadata_mapper-0.8.0/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.510428 aind_metadata_mapper-0.8.0/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.510428 aind_metadata_mapper-0.8.0/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/doc_template/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.510428 aind_metadata_mapper-0.8.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/examples/bergamo_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.510428 aind_metadata_mapper-0.8.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/scripts/singularity_build.def
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 00:06:41.526428 aind_metadata_mapper-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.502428 aind_metadata_mapper-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.510428 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 00:06:31.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.510428 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/bergamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23425 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/bergamo/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.510428 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.510428 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/exaspim/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/exaspim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.514428 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/fip/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/fip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/fip/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/gather_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.514428 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/mesoscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/mesoscope/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.514428 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/open_ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/open_ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/open_ephys/rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/open_ephys/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.514428 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/smartspim/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/smartspim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.526428 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-22 00:06:41.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-22 00:06:41.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 00:06:41.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-22 00:06:41.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 00:06:41.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.514428 aind_metadata_mapper-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.506428 aind_metadata_mapper-0.8.0/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.514428 aind_metadata_mapper-0.8.0/tests/resources/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/bergamo/cropped_neuron50_00001.tif
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/bergamo/example_description0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/bergamo/example_metadata.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/bergamo/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.514428 aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/base-missing-probe_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/base_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/mvr.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/mvr_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/sync.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/sync_rig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.518428 aind_metadata_mapper-0.8.0/tests/resources/fip/
+-rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/fip/000000_ophys_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/fip/000000_ophys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/fip/example_from_teensy.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.518428 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/example_funding_multiple_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/example_funding_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/example_procedures_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/example_subject_response.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.518428 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/metadata_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/metadata_files/data_description.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/metadata_files/procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/metadata_files/processing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/metadata_files/subject.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.518428 aind_metadata_mapper-0.8.0/tests/resources/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/mesoscope/example_extract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/mesoscope/example_platform.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/mesoscope/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.522428 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/ephys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/newscale_main.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/newscale_surface_finding.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/open-ephys-inferred_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/open-ephys_rig.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings.mislabeled-probes-0.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings.mislabeled-probes-1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings_main.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings_surface_finding.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.522428 aind_metadata_mapper-0.8.0/tests/test_bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_bergamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_bergamo/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.522428 aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/test_mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/test_neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/test_sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.522428 aind_metadata_mapper-0.8.0/tests/test_fip/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_fip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_fip/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18232 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_gather_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_legacy_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.522428 aind_metadata_mapper-0.8.0/tests/test_mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_mesoscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7761 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_mesoscope/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.522428 aind_metadata_mapper-0.8.0/tests/test_open_ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_open_ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_open_ephys/test_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_open_ephys/test_session.py
```

### Comparing `aind_metadata_mapper-0.7.4/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_mapper-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_mapper-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_mapper-0.8.0/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/.github/workflows/tag_and_publish.yml` & `aind_metadata_mapper-0.8.0/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/.github/workflows/test_and_lint.yml` & `aind_metadata_mapper-0.8.0/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/.gitignore` & `aind_metadata_mapper-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/CONTRIBUTING.md` & `aind_metadata_mapper-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/LICENSE` & `aind_metadata_mapper-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/PKG-INFO` & `aind_metadata_mapper-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.7.4
+Version: 0.8.0
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_metadata_mapper-0.7.4/README.md` & `aind_metadata_mapper-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/doc_template/Makefile` & `aind_metadata_mapper-0.8.0/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/doc_template/make.bat` & `aind_metadata_mapper-0.8.0/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/doc_template/source/_static/dark-logo.svg` & `aind_metadata_mapper-0.8.0/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/doc_template/source/_static/favicon.ico` & `aind_metadata_mapper-0.8.0/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/doc_template/source/_static/light-logo.svg` & `aind_metadata_mapper-0.8.0/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/doc_template/source/conf.py` & `aind_metadata_mapper-0.8.0/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/examples/bergamo_session.py` & `aind_metadata_mapper-0.8.0/examples/bergamo_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/pyproject.toml` & `aind_metadata_mapper-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/bergamo/session.py` & `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/bergamo/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/core.py` & `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/core.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py` & `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py` & `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Base ETL class for neuropixels rigs."""
+"""Base ETL class for dynamic_routing rigs."""
 
 import logging
 from datetime import date
 from pathlib import Path
 from typing import Optional
 
 from aind_data_schema.core.rig import Rig  # type: ignore
@@ -10,15 +10,15 @@
 
 from aind_metadata_mapper.core import BaseEtl
 
 logger = logging.getLogger(__name__)
 
 
 class NeuropixelsRigContext(BaseModel):
-    """Base context for neuropixels rig etl."""
+    """Base context for dynamic_routing rig etl."""
 
     current: Rig
 
 
 class NeuropixelsRigEtl(BaseEtl):
     """Neuropixels rig ETL class. Extracts information from rig-related files
     and transforms them into an aind-data-schema rig.Rig instance.
```

### Comparing `aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/dynamic_routing/open_ephys_rig.py` & `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/open_ephys/rig.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,16 +99,16 @@
         rig_probe_names = [
             probe.name
             for assembly in current.ephys_assemblies
             for probe in assembly.probes
         ]
         if not all(name in rig_probe_names for name in extracted_probe_names):
             logger.warning(
-                "Mismatched probe names in open ephys settings. Attempting to "
-                "infer probe names. extracted: %s, rig: %s"
+                "Mismatched probe names in open open_ephys settings."
+                " Attempting to infer probe names. extracted: %s, rig: %s"
                 % (extracted_probe_names, rig_probe_names)
             )
             if len(extracted_probe_names) != len(rig_probe_names):
                 logger.warning(
                     "Probe count mismatch. Skipping probe inference."
                 )
                 return []
```

### Comparing `aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/dynamic_routing/sync_rig.py` & `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/sync_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/dynamic_routing/utils.py` & `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/utils.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/ephys/session.py` & `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/open_ephys/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Module to write valid ephys schemas"""
+"""Module to write valid open_ephys schemas"""
 
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 
 from aind_data_schema.core.session import Session
 from aind_data_schema_models.modalities import Modality
@@ -16,15 +16,15 @@
 
     stage_logs: [str]
     openephys_logs: [str]
     experiment_data: dict
 
 
 class EphysEtl(BaseEtl):
-    """This class contains the methods to write ephys session"""
+    """This class contains the methods to write open_ephys session"""
 
     def __init__(
         self,
         output_directory: Path,
         stage_logs: [str],
         openephys_logs: [str],
         experiment_data: dict,
@@ -35,27 +35,27 @@
         Parameters
         ----------
         input_source : Union[str, PathLike]
           Can be a string or a Path
         output_directory : Path
           The directory where to save the json files.
         stage_logs : List
-          stage logs of all ephys data streams in a session
+          stage logs of all open_ephys data streams in a session
         openephys_logs : List
-          openephys logs of all ephys data streams in a session
+          openephys logs of all open_ephys data streams in a session
         """
         super().__init__(input_source, output_directory)
         self.stage_logs = stage_logs
         self.openephys_logs = openephys_logs
         self.experiment_data = experiment_data
 
     def _transform(self, extracted_source: ParsedInformation) -> Session:
         """
         Parses params from stage_log and openephys_log and
-        creates partial ephys session model
+        creates partial open_ephys session model
         Parameters
         ----------
         extracted_source : ParsedInformation
 
         Returns
         -------
         Session
@@ -139,13 +139,13 @@
             datetime.strptime(x[-1][0], "%Y/%m/%d %H:%M:%S.%f")
             for x in stage_logs
         ]
         ephys_session["session_end_time"] = max(end_times)
         return Session(**ephys_session)
 
     def _extract(self) -> ParsedInformation:
-        """Extract metadata from ephys session."""
+        """Extract metadata from open_ephys session."""
         return ParsedInformation(
             stage_logs=self.stage_logs,
             openephys_logs=self.openephys_logs,
             experiment_data=self.experiment_data,
         )
```

### Comparing `aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/fib/session.py` & `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/fip/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
             mouse_platform_name=mouse_platform_name,
             active_mouse_platform=active_mouse_platform,
         )
 
         return ophys_session
 
     def _extract(self) -> ParsedMetadata:
-        """Extract metadata from fib session."""
+        """Extract metadata from fip session."""
 
         tensy_str = self.job_settings.string_to_parse
 
         return ParsedMetadata(
             teensy_str=tensy_str,
         )
```

### Comparing `aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/gather_metadata.py` & `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/gather_metadata.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/src/aind_metadata_mapper/mesoscope/session.py` & `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/mesoscope/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/src/aind_metadata_mapper.egg-info/PKG-INFO` & `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.7.4
+Version: 0.8.0
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_metadata_mapper-0.7.4/src/aind_metadata_mapper.egg-info/SOURCES.txt` & `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -28,66 +28,72 @@
 src/aind_metadata_mapper.egg-info/requires.txt
 src/aind_metadata_mapper.egg-info/top_level.txt
 src/aind_metadata_mapper/bergamo/__init__.py
 src/aind_metadata_mapper/bergamo/session.py
 src/aind_metadata_mapper/dynamic_routing/__init__.py
 src/aind_metadata_mapper/dynamic_routing/mvr_rig.py
 src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py
-src/aind_metadata_mapper/dynamic_routing/open_ephys_rig.py
 src/aind_metadata_mapper/dynamic_routing/sync_rig.py
 src/aind_metadata_mapper/dynamic_routing/utils.py
-src/aind_metadata_mapper/ephys/__init__.py
-src/aind_metadata_mapper/ephys/session.py
-src/aind_metadata_mapper/fib/__init__.py
-src/aind_metadata_mapper/fib/session.py
+src/aind_metadata_mapper/exaspim/__init__.py
+src/aind_metadata_mapper/fip/__init__.py
+src/aind_metadata_mapper/fip/session.py
 src/aind_metadata_mapper/mesoscope/__init__.py
 src/aind_metadata_mapper/mesoscope/session.py
+src/aind_metadata_mapper/open_ephys/__init__.py
+src/aind_metadata_mapper/open_ephys/rig.py
+src/aind_metadata_mapper/open_ephys/session.py
+src/aind_metadata_mapper/smartspim/__init__.py
 tests/__init__.py
-tests/test_bergamo.py
-tests/test_ephys.py
-tests/test_fib.py
 tests/test_gather_metadata.py
 tests/test_legacy_core.py
-tests/test_mesoscope.py
 tests/resources/bergamo/cropped_neuron50_00001.tif
 tests/resources/bergamo/example_description0.txt
 tests/resources/bergamo/example_metadata.txt.gz
 tests/resources/bergamo/expected_session.json
-tests/resources/ephys/ephys_session.json
-tests/resources/ephys/newscale_main.csv
-tests/resources/ephys/newscale_surface_finding.csv
-tests/resources/ephys/settings_main.xml
-tests/resources/ephys/settings_surface_finding.xml
-tests/resources/fib/000000_ophys_rig.json
-tests/resources/fib/000000_ophys_session.json
-tests/resources/fib/example_from_teensy.txt
+tests/resources/dynamic_routing/base-missing-probe_rig.json
+tests/resources/dynamic_routing/base_rig.json
+tests/resources/dynamic_routing/mvr.ini
+tests/resources/dynamic_routing/mvr_rig.json
+tests/resources/dynamic_routing/sync.yml
+tests/resources/dynamic_routing/sync_rig.json
+tests/resources/fip/000000_ophys_rig.json
+tests/resources/fip/000000_ophys_session.json
+tests/resources/fip/example_from_teensy.txt
 tests/resources/gather_metadata_job/example_funding_multiple_response.json
 tests/resources/gather_metadata_job/example_funding_response.json
 tests/resources/gather_metadata_job/example_procedures_response.json
 tests/resources/gather_metadata_job/example_subject_response.json
 tests/resources/gather_metadata_job/metadata_files/data_description.json
 tests/resources/gather_metadata_job/metadata_files/procedures.json
 tests/resources/gather_metadata_job/metadata_files/processing.json
 tests/resources/gather_metadata_job/metadata_files/subject.json
 tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
 tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
 tests/resources/mesoscope/0123456789_Face_20240212T091444.json
 tests/resources/mesoscope/example_extract.json
 tests/resources/mesoscope/example_platform.json
 tests/resources/mesoscope/expected_session.json
-tests/resources/neuropixels/base-missing-probe_rig.json
-tests/resources/neuropixels/base_rig.json
-tests/resources/neuropixels/mvr.ini
-tests/resources/neuropixels/mvr_rig.json
-tests/resources/neuropixels/open-ephys-inferred_rig.json
-tests/resources/neuropixels/open-ephys_rig.json
-tests/resources/neuropixels/settings.mislabeled-probes-0.xml
-tests/resources/neuropixels/settings.mislabeled-probes-1.xml
-tests/resources/neuropixels/settings.xml
-tests/resources/neuropixels/sync.yml
-tests/resources/neuropixels/sync_rig.json
+tests/resources/open_ephys/ephys_session.json
+tests/resources/open_ephys/newscale_main.csv
+tests/resources/open_ephys/newscale_surface_finding.csv
+tests/resources/open_ephys/open-ephys-inferred_rig.json
+tests/resources/open_ephys/open-ephys_rig.json
+tests/resources/open_ephys/settings.mislabeled-probes-0.xml
+tests/resources/open_ephys/settings.mislabeled-probes-1.xml
+tests/resources/open_ephys/settings.xml
+tests/resources/open_ephys/settings_main.xml
+tests/resources/open_ephys/settings_surface_finding.xml
+tests/test_bergamo/__init__.py
+tests/test_bergamo/test_session.py
 tests/test_dynamic_routing/__init__.py
 tests/test_dynamic_routing/test_mvr_rig.py
 tests/test_dynamic_routing/test_neuropixels_rig.py
-tests/test_dynamic_routing/test_open_ephys_rig.py
 tests/test_dynamic_routing/test_sync_rig.py
-tests/test_dynamic_routing/utils.py
+tests/test_dynamic_routing/test_utils.py
+tests/test_fip/__init__.py
+tests/test_fip/test_session.py
+tests/test_mesoscope/__init__.py
+tests/test_mesoscope/test_session.py
+tests/test_open_ephys/__init__.py
+tests/test_open_ephys/test_rig.py
+tests/test_open_ephys/test_session.py
```

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/bergamo/cropped_neuron50_00001.tif` & `aind_metadata_mapper-0.8.0/tests/resources/bergamo/cropped_neuron50_00001.tif`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/bergamo/example_description0.txt` & `aind_metadata_mapper-0.8.0/tests/resources/bergamo/example_description0.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/bergamo/example_metadata.txt.gz` & `aind_metadata_mapper-0.8.0/tests/resources/bergamo/example_metadata.txt.gz`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/bergamo/expected_session.json` & `aind_metadata_mapper-0.8.0/tests/resources/bergamo/expected_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/ephys/ephys_session.json` & `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/ephys_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/ephys/newscale_main.csv` & `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/newscale_main.csv`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/ephys/newscale_surface_finding.csv` & `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/newscale_surface_finding.csv`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/ephys/settings_main.xml` & `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings_main.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/ephys/settings_surface_finding.xml` & `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings_surface_finding.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/fib/000000_ophys_rig.json` & `aind_metadata_mapper-0.8.0/tests/resources/fip/000000_ophys_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/fib/000000_ophys_session.json` & `aind_metadata_mapper-0.8.0/tests/resources/fip/000000_ophys_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/gather_metadata_job/example_funding_multiple_response.json` & `aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/example_funding_multiple_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/gather_metadata_job/example_procedures_response.json` & `aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/example_procedures_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/gather_metadata_job/example_subject_response.json` & `aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/example_subject_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/gather_metadata_job/metadata_files/data_description.json` & `aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/metadata_files/data_description.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/gather_metadata_job/metadata_files/procedures.json` & `aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/metadata_files/procedures.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/gather_metadata_job/metadata_files/processing.json` & `aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/metadata_files/processing.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/gather_metadata_job/metadata_files/subject.json` & `aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/metadata_files/subject.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json` & `aind_metadata_mapper-0.8.0/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json` & `aind_metadata_mapper-0.8.0/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/mesoscope/0123456789_Face_20240212T091444.json` & `aind_metadata_mapper-0.8.0/tests/resources/mesoscope/0123456789_Face_20240212T091444.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/mesoscope/example_extract.json` & `aind_metadata_mapper-0.8.0/tests/resources/mesoscope/example_extract.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/mesoscope/example_platform.json` & `aind_metadata_mapper-0.8.0/tests/resources/mesoscope/example_platform.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/mesoscope/expected_session.json` & `aind_metadata_mapper-0.8.0/tests/resources/mesoscope/expected_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/neuropixels/base-missing-probe_rig.json` & `aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/base-missing-probe_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/neuropixels/base_rig.json` & `aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/base_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/neuropixels/mvr.ini` & `aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/mvr.ini`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/neuropixels/mvr_rig.json` & `aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/mvr_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/neuropixels/open-ephys-inferred_rig.json` & `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/open-ephys-inferred_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/neuropixels/open-ephys_rig.json` & `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/open-ephys_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/neuropixels/settings.mislabeled-probes-0.xml` & `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings.mislabeled-probes-0.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/neuropixels/settings.mislabeled-probes-1.xml` & `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings.mislabeled-probes-1.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/neuropixels/settings.xml` & `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/neuropixels/sync.yml` & `aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/sync.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/resources/neuropixels/sync_rig.json` & `aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/sync_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/test_bergamo.py` & `aind_metadata_mapper-0.8.0/tests/test_bergamo/test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,20 @@
 from aind_metadata_mapper.bergamo.session import (
     BergamoEtl,
     JobSettings,
     RawImageInfo,
 )
 
 RESOURCES_DIR = (
-    Path(os.path.dirname(os.path.realpath(__file__))) / "resources" / "bergamo"
+    Path(os.path.dirname(os.path.realpath(__file__)))
+    / ".."
+    / "resources"
+    / "bergamo"
 )
+
 EXAMPLE_MD_PATH = RESOURCES_DIR / "example_metadata.txt.gz"
 EXAMPLE_DES_PATH = RESOURCES_DIR / "example_description0.txt"
 EXAMPLE_IMG_PATH = RESOURCES_DIR / "cropped_neuron50_00001.tif"
 EXPECTED_SESSION = RESOURCES_DIR / "expected_session.json"
 
 
 class TestBergamoEtl(unittest.TestCase):
```

### Comparing `aind_metadata_mapper-0.7.4/tests/test_dynamic_routing/test_mvr_rig.py` & `aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/test_mvr_rig.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 import os
 import unittest
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 
 from aind_metadata_mapper.dynamic_routing.mvr_rig import (  # type: ignore
-     MvrRigEtl,
+    MvrRigEtl,
 )
-from tests.test_dynamic_routing import utils as test_utils
+from tests.test_dynamic_routing import test_utils as test_utils
 
 RESOURCES_DIR = (
     Path(os.path.dirname(os.path.realpath(__file__)))
     / ".."
     / "resources"
-    / "neuropixels"
+    / "dynamic_routing"
 )
 
 
 class TestMvrRigEtl(unittest.TestCase):
-    """Tests dxdiag utilities in for the neuropixels project."""
+    """Tests dxdiag utilities in for the dynamic_routing project."""
 
     def test_transform(self):
         """Test etl transform."""
         etl = MvrRigEtl(
             self.input_source,
             self.output_dir,
             RESOURCES_DIR / "mvr.ini",
```

### Comparing `aind_metadata_mapper-0.7.4/tests/test_dynamic_routing/test_neuropixels_rig.py` & `aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/test_neuropixels_rig.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-"""Tests for the neuropixels open ephys rig ETL with inferred probe mapping."""
+"""Tests for the dynamic_routing neuropixel rig ETL inferred probe mapping."""
 
 import os
 import unittest
 from datetime import date
 from pathlib import Path
 
 from aind_metadata_mapper.dynamic_routing.neuropixels_rig import (
     NeuropixelsRigEtl,
 )
 
 RESOURCES_DIR = (
     Path(os.path.dirname(os.path.realpath(__file__)))
     / ".."
     / "resources"
-    / "neuropixels"
+    / "dynamic_routing"
 )
 
 
 class TestNeuropixelsRig(unittest.TestCase):
-    """Tests dxdiag utilities in for the neuropixels project."""
+    """Tests dxdiag utilities in for the dynamic_routing project."""
 
     def test_update_modification_date(self):
         """Test ETL workflow with inferred probe mapping."""
         etl = NeuropixelsRigEtl(
             RESOURCES_DIR / "base_rig.json",
             Path("./"),
         )
```

### Comparing `aind_metadata_mapper-0.7.4/tests/test_dynamic_routing/test_open_ephys_rig.py` & `aind_metadata_mapper-0.8.0/tests/test_open_ephys/test_rig.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,50 @@
-"""Tests for the neuropixels open ephys rig ETL."""
+"""Tests for the dynamic_routing open open_ephys rig ETL."""
 
 import os
 import unittest
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 
 from aind_data_schema.core.rig import Rig  # type: ignore
-from aind_metadata_mapper.dynamic_routing.open_ephys_rig import (
-    OpenEphysRigEtl,
-)
+
+from aind_metadata_mapper.open_ephys.rig import OpenEphysRigEtl
 
 RESOURCES_DIR = (
-    Path(os.path.dirname(os.path.realpath(__file__)))
-    / ".."
-    / "resources"
-    / "neuropixels"
+    Path(os.path.dirname(os.path.realpath(__file__))) / ".." / "resources"
+)
+
+
+OPEN_EPHYS_RESOURCES_DIR = RESOURCES_DIR / "open_ephys"
+BASE_RIG_PATH = RESOURCES_DIR / "dynamic_routing" / "base_rig.json"
+BASE_RIG_MISSING_PROBE_PATH = (
+    RESOURCES_DIR / "dynamic_routing" / "base-missing-probe_rig.json"
 )
-BASE_RIG_PATH = RESOURCES_DIR / "base_rig.json"
 OUTPUT_DIR = Path(".")  # File writes will be mocked
 
 
 class TestOpenEphysRigEtl(unittest.TestCase):
-    """Tests dxdiag utilities in for the neuropixels project."""
+    """Tests dxdiag utilities in for the dynamic_routing project."""
 
     def load_rig(self, model_path: Path):
         """Convenience function to load a rig model."""
         return Rig.model_validate_json(
             (model_path).read_text(),
         )
 
     def test_transform(self):
         """Tests etl transform."""
-        expected = self.load_rig(RESOURCES_DIR / "open-ephys_rig.json")
+        expected = self.load_rig(
+            OPEN_EPHYS_RESOURCES_DIR / "open-ephys_rig.json"
+        )
         etl = OpenEphysRigEtl(
             BASE_RIG_PATH,
             OUTPUT_DIR,
             open_ephys_settings_sources=[
-                RESOURCES_DIR / "settings.xml",
+                OPEN_EPHYS_RESOURCES_DIR / "settings.xml",
             ],
             probe_manipulator_serial_numbers=[
                 (
                     "Ephys Assembly A",
                     "SN45356",
                 ),
                 (
@@ -73,15 +77,15 @@
     @patch("aind_data_schema.base.AindCoreModel.write_standard_file")
     def test_etl(self, mock_write_standard_file: MagicMock):
         """Test ETL workflow."""
         etl = OpenEphysRigEtl(
             BASE_RIG_PATH,
             OUTPUT_DIR,
             open_ephys_settings_sources=[
-                RESOURCES_DIR / "settings.xml",
+                OPEN_EPHYS_RESOURCES_DIR / "settings.xml",
             ],
             probe_manipulator_serial_numbers=[
                 (
                     "Ephys Assembly A",
                     "SN45356",
                 ),
                 (
@@ -109,20 +113,22 @@
         etl.run_job()
         mock_write_standard_file.assert_called_once_with(
             output_directory=OUTPUT_DIR
         )
 
     def test_transform_no_update(self):
         """Tests etl transform when probe serial numbers dont change."""
-        initial_rig_model_path = RESOURCES_DIR / "open-ephys_rig.json"
+        initial_rig_model_path = (
+            OPEN_EPHYS_RESOURCES_DIR / "open-ephys_rig.json"
+        )
         etl = OpenEphysRigEtl(
             initial_rig_model_path,
             OUTPUT_DIR,
             open_ephys_settings_sources=[
-                RESOURCES_DIR / "settings.xml",
+                OPEN_EPHYS_RESOURCES_DIR / "settings.xml",
             ],
         )
         extracted = etl._extract()
         transformed = etl._transform(extracted)
         initial_rig_model = self.load_rig(initial_rig_model_path)
         self.assertEqual(initial_rig_model.rig_id, transformed.rig_id)
 
@@ -147,16 +153,16 @@
     @patch("aind_data_schema.base.AindCoreModel.write_standard_file")
     def test_etl_inferred_mapping(self, mock_write_standard_file: MagicMock):
         """Test ETL workflow with inferred probe mapping."""
         etl = OpenEphysRigEtl(
             BASE_RIG_PATH,
             OUTPUT_DIR,
             open_ephys_settings_sources=[
-                RESOURCES_DIR / "settings.mislabeled-probes-0.xml",
-                RESOURCES_DIR / "settings.mislabeled-probes-1.xml",
+                OPEN_EPHYS_RESOURCES_DIR / "settings.mislabeled-probes-0.xml",
+                OPEN_EPHYS_RESOURCES_DIR / "settings.mislabeled-probes-1.xml",
             ],
             probe_manipulator_serial_numbers=[
                 (
                     "Ephys Assembly A",
                     "SN45356",
                 ),
                 (
@@ -188,19 +194,19 @@
 
     @patch("aind_data_schema.base.AindCoreModel.write_standard_file")
     def test_etl_inferred_mapping_mismatched_probe_count(
         self, mock_write_standard_file: MagicMock
     ):
         """Test ETL workflow with mismatched probe count."""
         etl = OpenEphysRigEtl(
-            RESOURCES_DIR / "base-missing-probe_rig.json",
+            BASE_RIG_MISSING_PROBE_PATH,
             OUTPUT_DIR,
             open_ephys_settings_sources=[
-                RESOURCES_DIR / "settings.mislabeled-probes-0.xml",
-                RESOURCES_DIR / "settings.mislabeled-probes-1.xml",
+                OPEN_EPHYS_RESOURCES_DIR / "settings.mislabeled-probes-0.xml",
+                OPEN_EPHYS_RESOURCES_DIR / "settings.mislabeled-probes-1.xml",
             ],
             probe_manipulator_serial_numbers=[
                 (
                     "Ephys Assembly A",
                     "SN45356",
                 ),
                 (
```

### Comparing `aind_metadata_mapper-0.7.4/tests/test_dynamic_routing/utils.py` & `aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/test_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""Utilities for neuropixels etl tests."""
+"""Utilities for dynamic_routing etl tests."""
 import os
 from pathlib import Path
 from typing import Tuple
 
 from aind_data_schema.core.rig import Rig  # type: ignore
 
 RESOURCES_DIR = (
     Path(os.path.dirname(os.path.realpath(__file__)))
     / ".."
     / "resources"
-    / "neuropixels"
+    / "dynamic_routing"
 )
 
 FORWARD_CAMERA_ASSEMBLY_NAME = "Forward"
 FORWARD_CAMERA_NAME = f"{FORWARD_CAMERA_ASSEMBLY_NAME} camera"
 EYE_CAMERA_ASSEMBLY_NAME = "Eye"
 EYE_CAMERA_NAME = f"{EYE_CAMERA_ASSEMBLY_NAME} camera"
 SIDE_CAMERA_ASSEMBLY_NAME = "Side"
 SIDE_CAMERA_NAME = f"{SIDE_CAMERA_ASSEMBLY_NAME} camera"
 
 
 def setup_neuropixels_etl_resources(
     expected_json: Path,
 ) -> Tuple[Path, Path, Rig]:
-    """Sets test resources neuropixels etl.
+    """Sets test resources dynamic_routing etl.
 
     Parameters
     ----------
     expected_json: Path
       paths to etl resources to move to input dir
 
     Returns
```

### Comparing `aind_metadata_mapper-0.7.4/tests/test_ephys.py` & `aind_metadata_mapper-0.8.0/tests/test_open_ephys/test_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,42 @@
-"""Tests parsing of session information from ephys rig."""
+"""Tests parsing of session information from open_ephys rig."""
 
 import csv
 import json
 import os
 import unittest
 import zoneinfo
 from pathlib import Path
 from xml.dom import minidom
 
 from aind_data_schema.core.session import Session
 
-from aind_metadata_mapper.ephys.session import EphysEtl
+from aind_metadata_mapper.open_ephys.session import EphysEtl
 
 RESOURCES_DIR = (
-    Path(os.path.dirname(os.path.realpath(__file__))) / "resources" / "ephys"
+    Path(os.path.dirname(os.path.realpath(__file__)))
+    / ".."
+    / "resources"
+    / "open_ephys"
 )
+
 EXAMPLE_STAGE_LOGS = [
     RESOURCES_DIR / "newscale_main.csv",
     RESOURCES_DIR / "newscale_surface_finding.csv",
 ]
 EXAMPLE_OPENEPHYS_LOGS = [
     RESOURCES_DIR / "settings_main.xml",
     RESOURCES_DIR / "settings_surface_finding.xml",
 ]
 
 EXPECTED_SESSION = RESOURCES_DIR / "ephys_session.json"
 
 
 class TestEphysSession(unittest.TestCase):
-    """Test methods in ephys session module."""
+    """Test methods in open_ephys session module."""
 
     maxDiff = None  # show full diff without truncation
 
     @classmethod
     def setUpClass(cls):
         """Load record object and user settings before running tests."""
         # TODO: Add visual stimulus
```

### Comparing `aind_metadata_mapper-0.7.4/tests/test_fib.py` & `aind_metadata_mapper-0.8.0/tests/test_fip/test_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-"""Tests parsing of session information from fib rig."""
+"""Tests parsing of session information from fip rig."""
 
 import json
 import os
 import unittest
 import zoneinfo
 from datetime import datetime
 from pathlib import Path
 
 from aind_data_schema.core.session import Session
 
-from aind_metadata_mapper.fib.session import FIBEtl, JobSettings
+from aind_metadata_mapper.fip.session import FIBEtl, JobSettings
 
 RESOURCES_DIR = (
-    Path(os.path.dirname(os.path.realpath(__file__))) / "resources" / "fib"
+    Path(os.path.dirname(os.path.realpath(__file__)))
+    / ".."
+    / "resources"
+    / "fip"
 )
+
 EXAMPLE_MD_PATH = RESOURCES_DIR / "example_from_teensy.txt"
 EXPECTED_SESSION = RESOURCES_DIR / "000000_ophys_session.json"
 
 
 class TestSchemaWriter(unittest.TestCase):
     """Test methods in SchemaWriter class."""
```

### Comparing `aind_metadata_mapper-0.7.4/tests/test_gather_metadata.py` & `aind_metadata_mapper-0.8.0/tests/test_gather_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
             software_version="0.0.15",
             start_date_time=datetime(
                 2020, 10, 10, 10, 10, 10, tzinfo=timezone.utc
             ),
             end_date_time=datetime(
                 2020, 10, 10, 11, 10, 10, tzinfo=timezone.utc
             ),
-            input_location="/source/ephys",
+            input_location="/source/open_ephys",
             output_location="/tmp/stage",
             code_url=(
                 "https://github.com/AllenNeuralDynamics/"
                 "aind-data-transformation"
             ),
             parameters={},
             outputs={},
@@ -389,15 +389,15 @@
             software_version="0.0.15",
             start_date_time=datetime(
                 2020, 10, 10, 10, 10, 10, tzinfo=timezone.utc
             ),
             end_date_time=datetime(
                 2020, 10, 10, 11, 10, 10, tzinfo=timezone.utc
             ),
-            input_location="/source/ephys",
+            input_location="/source/open_ephys",
             output_location="/tmp/stage",
             code_url=(
                 "https://github.com/AllenNeuralDynamics/"
                 "aind-data-transformation"
             ),
             parameters={},
             outputs={},
```

### Comparing `aind_metadata_mapper-0.7.4/tests/test_legacy_core.py` & `aind_metadata_mapper-0.8.0/tests/test_legacy_core.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.4/tests/test_mesoscope.py` & `aind_metadata_mapper-0.8.0/tests/test_mesoscope/test_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from aind_data_schema.core.session import Session
 from PIL import Image
 
 from aind_metadata_mapper.mesoscope.session import JobSettings, MesoscopeEtl
 
 RESOURCES_DIR = (
     Path(os.path.dirname(os.path.realpath(__file__)))
+    / ".."
     / "resources"
     / "mesoscope"
 )
 
 EXAMPLE_EXTRACT = RESOURCES_DIR / "example_extract.json"
 EXAMPLE_SESSION = RESOURCES_DIR / "expected_session.json"
 EXAMPLE_PLATFORM = RESOURCES_DIR / "example_platform.json"
```

