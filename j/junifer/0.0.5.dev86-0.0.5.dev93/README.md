# Comparing `tmp/junifer-0.0.5.dev86.tar.gz` & `tmp/junifer-0.0.5.dev93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junifer-0.0.5.dev86.tar", last modified: Tue May 14 14:48:37 2024, max compression
+gzip compressed data, was "junifer-0.0.5.dev93.tar", last modified: Wed May 22 13:24:58 2024, max compression
```

## Comparing `junifer-0.0.5.dev86.tar` & `junifer-0.0.5.dev93.tar`

### file list

```diff
@@ -1,465 +1,466 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.950814 junifer-0.0.5.dev86/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.894814 junifer-0.0.5.dev86/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.894814 junifer-0.0.5.dev86/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/.github/ISSUE_TEMPLATE/dataset-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/.github/ISSUE_TEMPLATE/documention-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/.github/ISSUE_TEMPLATE/marker-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.894814 junifer-0.0.5.dev86/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/.github/workflows/ci-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/.github/workflows/docs-preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-14 14:48:37.950814 junifer-0.0.5.dev86/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/conda-env.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.898814 junifer-0.0.5.dev86/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.882814 junifer-0.0.5.dev86/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.898814 junifer-0.0.5.dev86/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.898814 junifer-0.0.5.dev86/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.898814 junifer-0.0.5.dev86/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/_templates/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.902814 junifer-0.0.5.dev86/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/api/configs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/api/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/api/datagrabbers.rst
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/api/datareaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/api/markers.rst
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/api/nilearn.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/api/onthefly.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/api/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/api/preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/api/stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/api/storage.rst
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/api/testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)    25180 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/builtin.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.902814 junifer-0.0.5.dev86/docs/changes/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/changes/contributors.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.902814 junifer-0.0.5.dev86/docs/changes/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/changes/newsfragments/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/changes/newsfragments/115.doc
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/changes/newsfragments/161.feature
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/changes/newsfragments/273.feature
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/changes/newsfragments/323.feature
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/changes/newsfragments/324.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/changes/newsfragments/330.doc
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/changes/newsfragments/331.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/changes/newsfragments/332.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/changes/newsfragments/336.removal
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/changes/newsfragments/339.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/changes/newsfragments/340.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/changes/newsfragments/341.enh
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/changes/newsfragments/342.misc
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/contribution.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.906814 junifer-0.0.5.dev86/docs/extending/
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/extending/coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/extending/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/extending/dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/extending/extension.rst
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/extending/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9619 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/extending/marker.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/extending/masks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/extending/parcellations.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/extending/preprocessor.rst
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/help.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.906814 junifer-0.0.5.dev86/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    62148 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/images/junifer_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/links.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/maintaining.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/redirect.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.906814 junifer-0.0.5.dev86/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/sphinxext/gh_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/starting.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.906814 junifer-0.0.5.dev86/docs/understanding/
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/understanding/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/understanding/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/understanding/datareader.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/understanding/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/understanding/marker.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/understanding/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/understanding/preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/understanding/storage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.906814 junifer-0.0.5.dev86/docs/using/
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/using/codeless.rst
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/using/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/using/masks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/using/queueing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/using/running.rst
--rw-r--r--   0 runner    (1001) docker     (127)    26282 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.906814 junifer-0.0.5.dev86/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/examples/norun_hcpfc_pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/examples/norun_ukbvm_gmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/examples/run_compute_parcel_mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/examples/run_datagrabber_bids_datalad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/examples/run_ets_rss_marker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/examples/run_junifer_julearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/examples/run_run_gmd_mean.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.910814 junifer-0.0.5.dev86/examples/yamls/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/examples/yamls/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/examples/yamls/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/examples/yamls/partly_cloudy_agg_mean_tian.yml
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/examples/yamls/ukb_gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.910814 junifer-0.0.5.dev86/junifer/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-14 14:48:37.000000 junifer-0.0.5.dev86/junifer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.910814 junifer-0.0.5.dev86/junifer/api/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16142 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.910814 junifer-0.0.5.dev86/junifer/api/queue_context/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/queue_context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/queue_context/gnu_parallel_local_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13233 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/queue_context/htcondor_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/queue_context/queue_context_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.910814 junifer-0.0.5.dev86/junifer/api/queue_context/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/queue_context/tests/test_gnu_parallel_local_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/queue_context/tests/test_htcondor_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.910814 junifer-0.0.5.dev86/junifer/api/res/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.914814 junifer-0.0.5.dev86/junifer/api/res/afni/
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/afni/3dAFNItoNIFTI
--rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/afni/3dRSFC
--rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/afni/3dReHo
--rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/afni/afni
--rwxr-xr-x   0 runner    (1001) docker     (127)     1130 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/afni/run_afni_docker.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.914814 junifer-0.0.5.dev86/junifer/api/res/ants/
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/ants/ResampleImage
--rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/ants/antsApplyTransforms
--rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/ants/antsApplyTransformsToPoints
--rwxr-xr-x   0 runner    (1001) docker     (127)     1119 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/ants/run_ants_docker.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.914814 junifer-0.0.5.dev86/junifer/api/res/freesurfer/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/freesurfer/mri_binarize
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/freesurfer/mri_mc
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/freesurfer/mri_pretess
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/freesurfer/mris_convert
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/freesurfer/run_freesurfer_docker.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.914814 junifer-0.0.5.dev86/junifer/api/res/fsl/
--rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/fsl/applywarp
--rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/fsl/flirt
--rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/fsl/img2imgcoord
--rwxr-xr-x   0 runner    (1001) docker     (127)     1122 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/fsl/run_fsl_docker.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/fsl/std2imgcoord
--rwxr-xr-x   0 runner    (1001) docker     (127)      517 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/run_conda.bash
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/run_conda.zsh
--rwxr-xr-x   0 runner    (1001) docker     (127)      507 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/run_venv.bash
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/res/run_venv.zsh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.914814 junifer-0.0.5.dev86/junifer/api/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.914814 junifer-0.0.5.dev86/junifer/api/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/tests/data/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/tests/data/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/tests/data/partly_cloudy_agg_mean_tian.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/tests/test_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10969 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    17753 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.914814 junifer-0.0.5.dev86/junifer/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.918814 junifer-0.0.5.dev86/junifer/configs/juseless/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/configs/juseless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.918814 junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/ixi_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.918814 junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/ucla.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/ukb_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.918814 junifer-0.0.5.dev86/junifer/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.886814 junifer-0.0.5.dev86/junifer/data/VOIs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.922814 junifer-0.0.5.dev86/junifer/data/VOIs/meta/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/AutobiographicalMemory_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/CogAC_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/CogAR_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/Empathy_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/Motor_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/MultiTask_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/Rew_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/ToM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/VigAtt_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/WM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/eMDN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/eSAD_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/VOIs/meta/extDMN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.886814 junifer-0.0.5.dev86/junifer/data/masks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.922814 junifer-0.0.5.dev86/junifer/data/masks/vickery-patil/
--rw-r--r--   0 runner    (1001) docker     (127)    88270 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/masks.py
--rw-r--r--   0 runner    (1001) docker     (127)    65343 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/parcellations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/template_spaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.922814 junifer-0.0.5.dev86/junifer/data/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/tests/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (127)    38222 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/tests/test_parcellations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/tests/test_template_spaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.926814 junifer-0.0.5.dev86/junifer/datagrabber/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.926814 junifer-0.0.5.dev86/junifer/datagrabber/aomic/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/aomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/aomic/id1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/aomic/piop1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/aomic/piop2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.926814 junifer-0.0.5.dev86/junifer/datagrabber/aomic/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/aomic/tests/test_id1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/aomic/tests/test_piop1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/aomic/tests/test_piop2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/datalad_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/dmcc13_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.926814 junifer-0.0.5.dev86/junifer/datagrabber/hcp1200/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/hcp1200/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/hcp1200/datalad_hcp1200.py
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/hcp1200/hcp1200.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.926814 junifer-0.0.5.dev86/junifer/datagrabber/hcp1200/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/hcp1200/tests/test_hcp1200.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)    15273 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/pattern_datalad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.926814 junifer-0.0.5.dev86/junifer/datagrabber/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/tests/test_datagrabber_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/tests/test_datalad_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/tests/test_dmcc13_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/tests/test_multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/tests/test_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/tests/test_pattern_datalad.py
--rw-r--r--   0 runner    (1001) docker     (127)     9406 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datagrabber/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.926814 junifer-0.0.5.dev86/junifer/datareader/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datareader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datareader/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.926814 junifer-0.0.5.dev86/junifer/datareader/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/datareader/tests/test_default_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.926814 junifer-0.0.5.dev86/junifer/external/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.886814 junifer-0.0.5.dev86/junifer/external/h5io/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.930814 junifer-0.0.5.dev86/junifer/external/h5io/h5io/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-14 14:48:34.000000 junifer-0.0.5.dev86/junifer/external/h5io/h5io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28748 2024-05-14 14:48:34.000000 junifer-0.0.5.dev86/junifer/external/h5io/h5io/_h5io.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 14:48:34.000000 junifer-0.0.5.dev86/junifer/external/h5io/h5io/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-14 14:48:34.000000 junifer-0.0.5.dev86/junifer/external/h5io/h5io/chunked_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-14 14:48:34.000000 junifer-0.0.5.dev86/junifer/external/h5io/h5io/chunked_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.930814 junifer-0.0.5.dev86/junifer/external/nilearn/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/external/nilearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16274 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/external/nilearn/junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.930814 junifer-0.0.5.dev86/junifer/external/nilearn/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.930814 junifer-0.0.5.dev86/junifer/markers/
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.930814 junifer-0.0.5.dev86/junifer/markers/complexity/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/complexity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/complexity/complexity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/complexity/hurst_exponent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/complexity/multiscale_entropy_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/complexity/perm_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/complexity/range_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/complexity/range_entropy_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/complexity/sample_entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.934814 junifer-0.0.5.dev86/junifer/markers/complexity/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/complexity/tests/test_complexity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/complexity/tests/test_hurst_exponent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/complexity/tests/test_multiscale_entropy_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/complexity/tests/test_perm_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/complexity/tests/test_range_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/complexity/tests/test_range_entropy_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/complexity/tests/test_sample_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/complexity/tests/test_weighted_perm_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/complexity/weighted_perm_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/ets_rss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.934814 junifer-0.0.5.dev86/junifer/markers/falff/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/falff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/falff/_afni_falff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/falff/_junifer_falff.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/falff/falff_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/falff/falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/falff/falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.934814 junifer-0.0.5.dev86/junifer/markers/falff/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/falff/tests/test_falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/falff/tests/test_falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.934814 junifer-0.0.5.dev86/junifer/markers/functional_connectivity/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/functional_connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/functional_connectivity/functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.934814 junifer-0.0.5.dev86/junifer/markers/functional_connectivity/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     8714 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/parcel_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.938814 junifer-0.0.5.dev86/junifer/markers/reho/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/reho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/reho/_afni_reho.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/reho/_junifer_reho.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/reho/reho_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/reho/reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/reho/reho_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.938814 junifer-0.0.5.dev86/junifer/markers/reho/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/reho/tests/test_reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/reho/tests/test_reho_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/sphere_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.938814 junifer-0.0.5.dev86/junifer/markers/temporal_snr/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/temporal_snr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/temporal_snr/temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/temporal_snr/temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/temporal_snr/temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.938814 junifer-0.0.5.dev86/junifer/markers/temporal_snr/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.938814 junifer-0.0.5.dev86/junifer/markers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/tests/test_ets_rss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/tests/test_marker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/tests/test_markers_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26531 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/tests/test_parcel_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9747 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/tests/test_sphere_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/markers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.938814 junifer-0.0.5.dev86/junifer/onthefly/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/onthefly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/onthefly/read_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.938814 junifer-0.0.5.dev86/junifer/onthefly/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/onthefly/tests/test_read_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.942814 junifer-0.0.5.dev86/junifer/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/pipeline/pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/pipeline/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/pipeline/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.942814 junifer-0.0.5.dev86/junifer/pipeline/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/pipeline/tests/test_pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/pipeline/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/pipeline/tests/test_update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/pipeline/tests/test_workdir_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/pipeline/update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/pipeline/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/pipeline/workdir_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.942814 junifer-0.0.5.dev86/junifer/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/preprocess/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.942814 junifer-0.0.5.dev86/junifer/preprocess/confounds/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/preprocess/confounds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20111 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/preprocess/confounds/fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.942814 junifer-0.0.5.dev86/junifer/preprocess/confounds/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    19973 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.942814 junifer-0.0.5.dev86/junifer/preprocess/smoothing/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/preprocess/smoothing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/preprocess/smoothing/_afni_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/preprocess/smoothing/_fsl_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/preprocess/smoothing/_nilearn_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/preprocess/smoothing/smoothing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.942814 junifer-0.0.5.dev86/junifer/preprocess/smoothing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/preprocess/smoothing/tests/test_smoothing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.942814 junifer-0.0.5.dev86/junifer/preprocess/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/preprocess/tests/test_preprocess_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.942814 junifer-0.0.5.dev86/junifer/preprocess/warping/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/preprocess/warping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/preprocess/warping/_ants_warper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/preprocess/warping/_fsl_warper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/preprocess/warping/space_warper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.942814 junifer-0.0.5.dev86/junifer/preprocess/warping/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/preprocess/warping/tests/test_space_warper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.946814 junifer-0.0.5.dev86/junifer/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    35631 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/storage/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/storage/pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21244 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/storage/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.946814 junifer-0.0.5.dev86/junifer/storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    29338 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/storage/tests/test_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/storage/tests/test_pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    28318 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/storage/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/storage/tests/test_storage_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/storage/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.946814 junifer-0.0.5.dev86/junifer/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.946814 junifer-0.0.5.dev86/junifer/testing/data/
--rw-r--r--   0 runner    (1001) docker     (127)   406849 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/testing/datagrabbers.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/testing/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.946814 junifer-0.0.5.dev86/junifer/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/testing/tests/test_spmauditory_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/testing/tests/test_testing_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.946814 junifer-0.0.5.dev86/junifer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/tests/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.946814 junifer-0.0.5.dev86/junifer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.950814 junifer-0.0.5.dev86/junifer/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/utils/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/utils/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/junifer/utils/tests/test_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.950814 junifer-0.0.5.dev86/junifer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-14 14:48:37.000000 junifer-0.0.5.dev86/junifer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14333 2024-05-14 14:48:37.000000 junifer-0.0.5.dev86/junifer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:48:37.000000 junifer-0.0.5.dev86/junifer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 14:48:37.000000 junifer-0.0.5.dev86/junifer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-14 14:48:37.000000 junifer-0.0.5.dev86/junifer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 14:48:37.000000 junifer-0.0.5.dev86/junifer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:48:37.950814 junifer-0.0.5.dev86/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:48:37.950814 junifer-0.0.5.dev86/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/tools/create_aomic1000_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/tools/create_aomicpiop1_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/tools/create_aomicpiop2_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/tools/create_bids_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/tools/create_bids_example_dataset_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/tools/create_dmcc13_benchmark_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/tools/create_hcp1200_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-14 14:48:33.000000 junifer-0.0.5.dev86/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.225076 junifer-0.0.5.dev93/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.161074 junifer-0.0.5.dev93/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.161074 junifer-0.0.5.dev93/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/.github/ISSUE_TEMPLATE/dataset-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/.github/ISSUE_TEMPLATE/documention-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/.github/ISSUE_TEMPLATE/marker-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.161074 junifer-0.0.5.dev93/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/.github/workflows/ci-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/.github/workflows/docs-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-22 13:24:58.225076 junifer-0.0.5.dev93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/conda-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.165074 junifer-0.0.5.dev93/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.149074 junifer-0.0.5.dev93/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.165074 junifer-0.0.5.dev93/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.165074 junifer-0.0.5.dev93/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.165074 junifer-0.0.5.dev93/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/_templates/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.165074 junifer-0.0.5.dev93/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/api/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/api/datagrabbers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/api/datareaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/api/markers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/api/nilearn.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/api/onthefly.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/api/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/api/preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/api/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/api/storage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/api/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    25180 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/builtin.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.165074 junifer-0.0.5.dev93/docs/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/changes/contributors.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.169074 junifer-0.0.5.dev93/docs/changes/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/changes/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/changes/newsfragments/115.doc
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/changes/newsfragments/161.feature
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/changes/newsfragments/273.feature
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/changes/newsfragments/323.feature
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/changes/newsfragments/324.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/changes/newsfragments/330.doc
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/changes/newsfragments/331.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/changes/newsfragments/332.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/changes/newsfragments/336.removal
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/changes/newsfragments/339.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/changes/newsfragments/340.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/changes/newsfragments/341.enh
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/changes/newsfragments/342.misc
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/changes/newsfragments/343.feature
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/contribution.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.169074 junifer-0.0.5.dev93/docs/extending/
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/extending/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/extending/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/extending/dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/extending/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/extending/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9619 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/extending/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/extending/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/extending/parcellations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/extending/preprocessor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/help.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.169074 junifer-0.0.5.dev93/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    62148 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/images/junifer_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/links.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/maintaining.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/redirect.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.169074 junifer-0.0.5.dev93/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/sphinxext/gh_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/starting.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.173074 junifer-0.0.5.dev93/docs/understanding/
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/understanding/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/understanding/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/understanding/datareader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/understanding/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/understanding/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/understanding/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/understanding/preprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/understanding/storage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.173074 junifer-0.0.5.dev93/docs/using/
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/using/codeless.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/using/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/using/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/using/queueing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/using/running.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    26282 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.173074 junifer-0.0.5.dev93/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/examples/norun_hcpfc_pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/examples/norun_ukbvm_gmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/examples/run_compute_parcel_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/examples/run_datagrabber_bids_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/examples/run_ets_rss_marker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/examples/run_junifer_julearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/examples/run_run_gmd_mean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.173074 junifer-0.0.5.dev93/examples/yamls/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/examples/yamls/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/examples/yamls/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/examples/yamls/partly_cloudy_agg_mean_tian.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/examples/yamls/ukb_gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.173074 junifer-0.0.5.dev93/junifer/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-22 13:24:58.000000 junifer-0.0.5.dev93/junifer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.177075 junifer-0.0.5.dev93/junifer/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16142 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.177075 junifer-0.0.5.dev93/junifer/api/queue_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/queue_context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/queue_context/gnu_parallel_local_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13233 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/queue_context/htcondor_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/queue_context/queue_context_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.177075 junifer-0.0.5.dev93/junifer/api/queue_context/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/queue_context/tests/test_gnu_parallel_local_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/queue_context/tests/test_htcondor_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.177075 junifer-0.0.5.dev93/junifer/api/res/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.181074 junifer-0.0.5.dev93/junifer/api/res/afni/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/afni/3dAFNItoNIFTI
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/afni/3dRSFC
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/afni/3dReHo
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/afni/afni
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1130 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/afni/run_afni_docker.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.181074 junifer-0.0.5.dev93/junifer/api/res/ants/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/ants/ResampleImage
+-rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/ants/antsApplyTransforms
+-rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/ants/antsApplyTransformsToPoints
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1119 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/ants/run_ants_docker.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.181074 junifer-0.0.5.dev93/junifer/api/res/freesurfer/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/freesurfer/mri_binarize
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/freesurfer/mri_mc
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/freesurfer/mri_pretess
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/freesurfer/mris_convert
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/freesurfer/run_freesurfer_docker.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.181074 junifer-0.0.5.dev93/junifer/api/res/fsl/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/fsl/applywarp
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/fsl/flirt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/fsl/img2imgcoord
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1122 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/fsl/run_fsl_docker.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/fsl/std2imgcoord
+-rwxr-xr-x   0 runner    (1001) docker     (127)      517 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/run_conda.bash
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/run_conda.zsh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      507 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/run_venv.bash
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/res/run_venv.zsh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.181074 junifer-0.0.5.dev93/junifer/api/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.181074 junifer-0.0.5.dev93/junifer/api/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/tests/data/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/tests/data/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/tests/data/partly_cloudy_agg_mean_tian.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/tests/test_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10969 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17753 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.181074 junifer-0.0.5.dev93/junifer/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.181074 junifer-0.0.5.dev93/junifer/configs/juseless/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/configs/juseless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.185075 junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/ixi_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.185075 junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/ucla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/ukb_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.185075 junifer-0.0.5.dev93/junifer/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.153074 junifer-0.0.5.dev93/junifer/data/VOIs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.189075 junifer-0.0.5.dev93/junifer/data/VOIs/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/AutobiographicalMemory_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/CogAC_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/CogAR_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/Empathy_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/Motor_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/MultiTask_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/Rew_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/ToM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/VigAtt_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/WM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/eMDN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/eSAD_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/VOIs/meta/extDMN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.153074 junifer-0.0.5.dev93/junifer/data/masks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.189075 junifer-0.0.5.dev93/junifer/data/masks/vickery-patil/
+-rw-r--r--   0 runner    (1001) docker     (127)    88270 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65343 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/parcellations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/template_spaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.189075 junifer-0.0.5.dev93/junifer/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/tests/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38222 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/tests/test_parcellations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/tests/test_template_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.193075 junifer-0.0.5.dev93/junifer/datagrabber/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.193075 junifer-0.0.5.dev93/junifer/datagrabber/aomic/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/aomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/aomic/id1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/aomic/piop1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/aomic/piop2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.193075 junifer-0.0.5.dev93/junifer/datagrabber/aomic/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/aomic/tests/test_id1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/aomic/tests/test_piop1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/aomic/tests/test_piop2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/datalad_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/dmcc13_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.193075 junifer-0.0.5.dev93/junifer/datagrabber/hcp1200/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/hcp1200/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/hcp1200/datalad_hcp1200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/hcp1200/hcp1200.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.193075 junifer-0.0.5.dev93/junifer/datagrabber/hcp1200/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/hcp1200/tests/test_hcp1200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15273 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/pattern_datalad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.197075 junifer-0.0.5.dev93/junifer/datagrabber/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/tests/test_datagrabber_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/tests/test_datalad_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/tests/test_dmcc13_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/tests/test_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/tests/test_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/tests/test_pattern_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9406 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datagrabber/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.197075 junifer-0.0.5.dev93/junifer/datareader/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datareader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datareader/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.197075 junifer-0.0.5.dev93/junifer/datareader/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/datareader/tests/test_default_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.197075 junifer-0.0.5.dev93/junifer/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.153074 junifer-0.0.5.dev93/junifer/external/h5io/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.197075 junifer-0.0.5.dev93/junifer/external/h5io/h5io/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-22 13:24:54.000000 junifer-0.0.5.dev93/junifer/external/h5io/h5io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28748 2024-05-22 13:24:54.000000 junifer-0.0.5.dev93/junifer/external/h5io/h5io/_h5io.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 13:24:54.000000 junifer-0.0.5.dev93/junifer/external/h5io/h5io/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-22 13:24:54.000000 junifer-0.0.5.dev93/junifer/external/h5io/h5io/chunked_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-22 13:24:54.000000 junifer-0.0.5.dev93/junifer/external/h5io/h5io/chunked_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.197075 junifer-0.0.5.dev93/junifer/external/nilearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/external/nilearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16274 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/external/nilearn/junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.197075 junifer-0.0.5.dev93/junifer/external/nilearn/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.197075 junifer-0.0.5.dev93/junifer/markers/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.201075 junifer-0.0.5.dev93/junifer/markers/complexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/complexity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/complexity/complexity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/complexity/hurst_exponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/complexity/multiscale_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/complexity/perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/complexity/range_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/complexity/range_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/complexity/sample_entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.201075 junifer-0.0.5.dev93/junifer/markers/complexity/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/complexity/tests/test_complexity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/complexity/tests/test_hurst_exponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/complexity/tests/test_multiscale_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/complexity/tests/test_perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/complexity/tests/test_range_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/complexity/tests/test_range_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/complexity/tests/test_sample_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/complexity/tests/test_weighted_perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/complexity/weighted_perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/ets_rss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.201075 junifer-0.0.5.dev93/junifer/markers/falff/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/falff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/falff/_afni_falff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/falff/_junifer_falff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/falff/falff_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/falff/falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/falff/falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.205075 junifer-0.0.5.dev93/junifer/markers/falff/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/falff/tests/test_falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/falff/tests/test_falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.205075 junifer-0.0.5.dev93/junifer/markers/functional_connectivity/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/functional_connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/functional_connectivity/functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.205075 junifer-0.0.5.dev93/junifer/markers/functional_connectivity/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8714 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/parcel_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.205075 junifer-0.0.5.dev93/junifer/markers/reho/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/reho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/reho/_afni_reho.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/reho/_junifer_reho.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/reho/reho_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/reho/reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/reho/reho_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.205075 junifer-0.0.5.dev93/junifer/markers/reho/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/reho/tests/test_reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/reho/tests/test_reho_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/sphere_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.209075 junifer-0.0.5.dev93/junifer/markers/temporal_snr/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/temporal_snr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/temporal_snr/temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/temporal_snr/temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/temporal_snr/temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.209075 junifer-0.0.5.dev93/junifer/markers/temporal_snr/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.209075 junifer-0.0.5.dev93/junifer/markers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/tests/test_ets_rss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/tests/test_marker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/tests/test_markers_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26531 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/tests/test_parcel_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9747 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/tests/test_sphere_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/markers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.209075 junifer-0.0.5.dev93/junifer/onthefly/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/onthefly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/onthefly/read_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.209075 junifer-0.0.5.dev93/junifer/onthefly/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/onthefly/tests/test_read_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.209075 junifer-0.0.5.dev93/junifer/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/pipeline/pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/pipeline/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/pipeline/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.213075 junifer-0.0.5.dev93/junifer/pipeline/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/pipeline/tests/test_pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/pipeline/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/pipeline/tests/test_update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/pipeline/tests/test_workdir_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/pipeline/update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/pipeline/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/pipeline/workdir_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.213075 junifer-0.0.5.dev93/junifer/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/preprocess/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.213075 junifer-0.0.5.dev93/junifer/preprocess/confounds/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/preprocess/confounds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20111 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/preprocess/confounds/fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.213075 junifer-0.0.5.dev93/junifer/preprocess/confounds/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    19973 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.213075 junifer-0.0.5.dev93/junifer/preprocess/smoothing/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/preprocess/smoothing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/preprocess/smoothing/_afni_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/preprocess/smoothing/_fsl_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/preprocess/smoothing/_nilearn_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/preprocess/smoothing/smoothing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.213075 junifer-0.0.5.dev93/junifer/preprocess/smoothing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/preprocess/smoothing/tests/test_smoothing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.213075 junifer-0.0.5.dev93/junifer/preprocess/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/preprocess/tests/test_preprocess_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.213075 junifer-0.0.5.dev93/junifer/preprocess/warping/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/preprocess/warping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/preprocess/warping/_ants_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/preprocess/warping/_fsl_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/preprocess/warping/space_warper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.213075 junifer-0.0.5.dev93/junifer/preprocess/warping/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/preprocess/warping/tests/test_space_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.217076 junifer-0.0.5.dev93/junifer/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37951 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/storage/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/storage/pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21244 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/storage/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.217076 junifer-0.0.5.dev93/junifer/storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    31512 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/storage/tests/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/storage/tests/test_pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28318 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/storage/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/storage/tests/test_storage_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/storage/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.217076 junifer-0.0.5.dev93/junifer/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.217076 junifer-0.0.5.dev93/junifer/testing/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   406849 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/testing/datagrabbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/testing/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.221076 junifer-0.0.5.dev93/junifer/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/testing/tests/test_spmauditory_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/testing/tests/test_testing_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.221076 junifer-0.0.5.dev93/junifer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.221076 junifer-0.0.5.dev93/junifer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.221076 junifer-0.0.5.dev93/junifer/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/utils/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/utils/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/junifer/utils/tests/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.221076 junifer-0.0.5.dev93/junifer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-22 13:24:58.000000 junifer-0.0.5.dev93/junifer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14372 2024-05-22 13:24:58.000000 junifer-0.0.5.dev93/junifer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:24:58.000000 junifer-0.0.5.dev93/junifer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-22 13:24:58.000000 junifer-0.0.5.dev93/junifer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-22 13:24:58.000000 junifer-0.0.5.dev93/junifer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 13:24:58.000000 junifer-0.0.5.dev93/junifer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:24:58.225076 junifer-0.0.5.dev93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:24:58.221076 junifer-0.0.5.dev93/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/tools/create_aomic1000_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/tools/create_aomicpiop1_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/tools/create_aomicpiop2_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/tools/create_bids_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/tools/create_bids_example_dataset_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/tools/create_dmcc13_benchmark_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/tools/create_hcp1200_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-22 13:24:53.000000 junifer-0.0.5.dev93/tox.ini
```

### Comparing `junifer-0.0.5.dev86/.github/ISSUE_TEMPLATE/bug-report.yml` & `junifer-0.0.5.dev93/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/.github/ISSUE_TEMPLATE/dataset-request.yml` & `junifer-0.0.5.dev93/.github/ISSUE_TEMPLATE/dataset-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/.github/ISSUE_TEMPLATE/documention-request.yml` & `junifer-0.0.5.dev93/.github/ISSUE_TEMPLATE/documention-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/.github/ISSUE_TEMPLATE/feature-request.yml` & `junifer-0.0.5.dev93/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/.github/ISSUE_TEMPLATE/marker-request.yml` & `junifer-0.0.5.dev93/.github/ISSUE_TEMPLATE/marker-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/.github/workflows/ci-docs.yml` & `junifer-0.0.5.dev93/.github/workflows/ci-docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/.github/workflows/ci.yml` & `junifer-0.0.5.dev93/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/.github/workflows/docs-preview.yml` & `junifer-0.0.5.dev93/.github/workflows/docs-preview.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/.github/workflows/docs.yml` & `junifer-0.0.5.dev93/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/.github/workflows/lint.yml` & `junifer-0.0.5.dev93/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/.github/workflows/pypi.yml` & `junifer-0.0.5.dev93/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/.gitignore` & `junifer-0.0.5.dev93/.gitignore`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/.pre-commit-config.yaml` & `junifer-0.0.5.dev93/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/LICENSE.md` & `junifer-0.0.5.dev93/LICENSE.md`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/PKG-INFO` & `junifer-0.0.5.dev93/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.5.dev86
+Version: 0.0.5.dev93
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: Changelog, https://juaml.github.io/junifer/main/whats_new.html
 Project-URL: Documentation, https://juaml.github.io/junifer
 Project-URL: Homepage, https://juaml.github.io/junifer
```

### Comparing `junifer-0.0.5.dev86/README.md` & `junifer-0.0.5.dev93/README.md`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/codecov.yml` & `junifer-0.0.5.dev93/codecov.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/conda-env.yml` & `junifer-0.0.5.dev93/conda-env.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/Makefile` & `junifer-0.0.5.dev93/docs/Makefile`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/_static/css/custom.css` & `junifer-0.0.5.dev93/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/_templates/versions.html` & `junifer-0.0.5.dev93/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/builtin.rst` & `junifer-0.0.5.dev93/docs/builtin.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/changes/contributors.inc` & `junifer-0.0.5.dev93/docs/changes/contributors.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/conf.py` & `junifer-0.0.5.dev93/docs/conf.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/contribution.rst` & `junifer-0.0.5.dev93/docs/contribution.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/extending/coordinates.rst` & `junifer-0.0.5.dev93/docs/extending/coordinates.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/extending/datagrabber.rst` & `junifer-0.0.5.dev93/docs/extending/datagrabber.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/extending/dependencies.rst` & `junifer-0.0.5.dev93/docs/extending/dependencies.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/extending/extension.rst` & `junifer-0.0.5.dev93/docs/extending/extension.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/extending/index.rst` & `junifer-0.0.5.dev93/docs/extending/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/extending/marker.rst` & `junifer-0.0.5.dev93/docs/extending/marker.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/extending/masks.rst` & `junifer-0.0.5.dev93/docs/extending/masks.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/extending/parcellations.rst` & `junifer-0.0.5.dev93/docs/extending/parcellations.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/extending/preprocessor.rst` & `junifer-0.0.5.dev93/docs/extending/preprocessor.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/faq.rst` & `junifer-0.0.5.dev93/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/help.rst` & `junifer-0.0.5.dev93/docs/help.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/images/junifer_logo.png` & `junifer-0.0.5.dev93/docs/images/junifer_logo.png`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/index.rst` & `junifer-0.0.5.dev93/docs/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/installation.rst` & `junifer-0.0.5.dev93/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/links.inc` & `junifer-0.0.5.dev93/docs/links.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/maintaining.rst` & `junifer-0.0.5.dev93/docs/maintaining.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/sphinxext/gh_substitutions.py` & `junifer-0.0.5.dev93/docs/sphinxext/gh_substitutions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/starting.rst` & `junifer-0.0.5.dev93/docs/starting.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/understanding/data.rst` & `junifer-0.0.5.dev93/docs/understanding/data.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/understanding/datagrabber.rst` & `junifer-0.0.5.dev93/docs/understanding/datagrabber.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/understanding/datareader.rst` & `junifer-0.0.5.dev93/docs/understanding/datareader.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/understanding/index.rst` & `junifer-0.0.5.dev93/docs/understanding/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/understanding/marker.rst` & `junifer-0.0.5.dev93/docs/understanding/marker.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/understanding/pipeline.rst` & `junifer-0.0.5.dev93/docs/understanding/pipeline.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/understanding/preprocess.rst` & `junifer-0.0.5.dev93/docs/understanding/preprocess.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/understanding/storage.rst` & `junifer-0.0.5.dev93/docs/understanding/storage.rst`

 * *Files 8% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 that object else they are kept in memory.
 
 Storage is meant to be used inside the DataGrabber context but you can operate
 on them outside the context as long as the processed data is in the memory and
 the Python runtime has not garbage-collected it.
 
 The :ref:`Markers <marker>` are responsible for defining what *storage kind*
-(``matrix``, ``vector``, ``timeseries``) they support for which
-:ref:`data type <data_types>` by overriding its ``get_output_type`` method. The
-storage object in turn declares and provides implementation for specific
-*storage kind*. For example, :class:`.SQLiteFeatureStorage` supports saving
-``matrix``, ``vector`` and ``timeseries`` via ``store_matrix``, ``store_vector``
-and ``store_timeseries`` methods respectively.
+(``matrix``, ``vector``, ``timeseries``, ``scalar_table``) they support for
+which :ref:`data type <data_types>` by overriding its ``get_output_type``
+method. The storage object in turn declares and provides implementation for
+specific *storage kind*. For example, :class:`.SQLiteFeatureStorage` supports
+saving ``matrix``, ``vector`` and ``timeseries`` via ``store_matrix``,
+``store_vector`` and ``store_timeseries`` methods respectively.
 
 For storage interfaces not supported by ``junifer`` yet, you can either make
 your own ``Storage`` by providing a concrete implementation of
 :class:`.BaseFeatureStorage` or open an issue on `junifer Github`_ and we can
 help you out.
 
 .. _storage_types:
@@ -40,25 +40,32 @@
    :header-rows: 1
 
    * - Storage Type
      - Description
      - Options
      - Reference
    * - ``matrix``
-     - A 2D matrix with row and column names
-     -  ``col_names``, ``row_names``, ``matrix_kind``, ``diagonal``
-     -  :meth:`.BaseFeatureStorage.store_matrix`
+     - A 2D square matrix with row and column names
+     - | ``col_names``, ``row_names``, ``matrix_kind``, ``diagonal``
+       | ``row_header_col_name``
+       | (only for :meth:`.HDF5FeatureStorage.store_matrix`)
+     - :meth:`.BaseFeatureStorage.store_matrix`
    * - ``vector``
      - A 1D row vector of values with column names
      - ``col_names``
-     -  :meth:`.BaseFeatureStorage.store_vector`
+     - :meth:`.BaseFeatureStorage.store_vector`
    * - ``timeseries``
-     - A 2D matrix of values with column names
+     - A 2D square or non-square matrix of scalar values with column names
      - ``col_names``
-     -  :meth:`.BaseFeatureStorage.store_timeseries`
+     - :meth:`.BaseFeatureStorage.store_timeseries`
+   * - ``scalar_table``
+     - | A 2D square or non-square matrix of scalar values with row name, column
+       | name and row header column name
+     - ``col_names``, ``row_names``, ``row_header_col_name``
+     - :meth:`.BaseFeatureStorage.store_scalar_table`
 
 .. _storage_interfaces:
 
 Storage Interfaces
 ------------------
 
 .. list-table::
@@ -72,8 +79,8 @@
    * - :class:`.SQLiteFeatureStorage`
      - ``.sqlite``
      - SQLite
      - ``matrix``, ``vector``, ``timeseries``
    * - :class:`.HDF5FeatureStorage`
      - ``.hdf5``
      - HDF5
-     - ``matrix``, ``vector``, ``timeseries``
+     - ``matrix``, ``vector``, ``timeseries``, ``scalar_table``
```

### Comparing `junifer-0.0.5.dev86/docs/using/codeless.rst` & `junifer-0.0.5.dev93/docs/using/codeless.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/using/index.rst` & `junifer-0.0.5.dev93/docs/using/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/using/masks.rst` & `junifer-0.0.5.dev93/docs/using/masks.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/using/queueing.rst` & `junifer-0.0.5.dev93/docs/using/queueing.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/using/running.rst` & `junifer-0.0.5.dev93/docs/using/running.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/docs/whats_new.rst` & `junifer-0.0.5.dev93/docs/whats_new.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/examples/norun_hcpfc_pearson.py` & `junifer-0.0.5.dev93/examples/norun_hcpfc_pearson.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/examples/norun_ukbvm_gmd.py` & `junifer-0.0.5.dev93/examples/norun_ukbvm_gmd.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/examples/run_compute_parcel_mean.py` & `junifer-0.0.5.dev93/examples/run_compute_parcel_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/examples/run_datagrabber_bids_datalad.py` & `junifer-0.0.5.dev93/examples/run_datagrabber_bids_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/examples/run_ets_rss_marker.py` & `junifer-0.0.5.dev93/examples/run_ets_rss_marker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/examples/run_junifer_julearn.py` & `junifer-0.0.5.dev93/examples/run_junifer_julearn.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/examples/run_run_gmd_mean.py` & `junifer-0.0.5.dev93/examples/run_run_gmd_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/examples/yamls/gmd_mean.yaml` & `junifer-0.0.5.dev93/examples/yamls/gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/examples/yamls/ukb_gmd_mean.yaml` & `junifer-0.0.5.dev93/examples/yamls/ukb_gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/cli.py` & `junifer-0.0.5.dev93/junifer/api/cli.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/decorators.py` & `junifer-0.0.5.dev93/junifer/api/decorators.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/functions.py` & `junifer-0.0.5.dev93/junifer/api/functions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/parser.py` & `junifer-0.0.5.dev93/junifer/api/parser.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/queue_context/gnu_parallel_local_adapter.py` & `junifer-0.0.5.dev93/junifer/api/queue_context/gnu_parallel_local_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/queue_context/htcondor_adapter.py` & `junifer-0.0.5.dev93/junifer/api/queue_context/htcondor_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/queue_context/queue_context_adapter.py` & `junifer-0.0.5.dev93/junifer/api/queue_context/queue_context_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/queue_context/tests/test_gnu_parallel_local_adapter.py` & `junifer-0.0.5.dev93/junifer/api/queue_context/tests/test_gnu_parallel_local_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/queue_context/tests/test_htcondor_adapter.py` & `junifer-0.0.5.dev93/junifer/api/queue_context/tests/test_htcondor_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/res/afni/run_afni_docker.sh` & `junifer-0.0.5.dev93/junifer/api/res/afni/run_afni_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/res/ants/run_ants_docker.sh` & `junifer-0.0.5.dev93/junifer/api/res/ants/run_ants_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/res/freesurfer/run_freesurfer_docker.sh` & `junifer-0.0.5.dev93/junifer/api/res/freesurfer/run_freesurfer_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/res/fsl/run_fsl_docker.sh` & `junifer-0.0.5.dev93/junifer/api/res/fsl/run_fsl_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/res/run_conda.bash` & `junifer-0.0.5.dev93/junifer/api/res/run_conda.bash`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/res/run_conda.zsh` & `junifer-0.0.5.dev93/junifer/api/res/run_conda.zsh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/tests/test_api_utils.py` & `junifer-0.0.5.dev93/junifer/api/tests/test_api_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/tests/test_cli.py` & `junifer-0.0.5.dev93/junifer/api/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/tests/test_functions.py` & `junifer-0.0.5.dev93/junifer/api/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/tests/test_parser.py` & `junifer-0.0.5.dev93/junifer/api/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/api/utils.py` & `junifer-0.0.5.dev93/junifer/api/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py` & `junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/camcan_vbm.py` & `junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/ixi_vbm.py` & `junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py` & `junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py` & `junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py` & `junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/tests/test_ucla.py` & `junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/tests/test_ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py` & `junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/ucla.py` & `junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/configs/juseless/datagrabbers/ukb_vbm.py` & `junifer-0.0.5.dev93/junifer/configs/juseless/datagrabbers/ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/VOIs/meta/AutobiographicalMemory_VOIs.txt` & `junifer-0.0.5.dev93/junifer/data/VOIs/meta/AutobiographicalMemory_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt` & `junifer-0.0.5.dev93/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt` & `junifer-0.0.5.dev93/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv` & `junifer-0.0.5.dev93/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/VOIs/meta/Rew_VOIs.txt` & `junifer-0.0.5.dev93/junifer/data/VOIs/meta/Rew_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/VOIs/meta/WM_VOIs.txt` & `junifer-0.0.5.dev93/junifer/data/VOIs/meta/WM_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/__init__.py` & `junifer-0.0.5.dev93/junifer/data/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/coordinates.py` & `junifer-0.0.5.dev93/junifer/data/coordinates.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz` & `junifer-0.0.5.dev93/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz` & `junifer-0.0.5.dev93/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz` & `junifer-0.0.5.dev93/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/masks.py` & `junifer-0.0.5.dev93/junifer/data/masks.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/parcellations.py` & `junifer-0.0.5.dev93/junifer/data/parcellations.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/template_spaces.py` & `junifer-0.0.5.dev93/junifer/data/template_spaces.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/tests/test_coordinates.py` & `junifer-0.0.5.dev93/junifer/data/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/tests/test_data_utils.py` & `junifer-0.0.5.dev93/junifer/data/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/tests/test_masks.py` & `junifer-0.0.5.dev93/junifer/data/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/tests/test_parcellations.py` & `junifer-0.0.5.dev93/junifer/data/tests/test_parcellations.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/tests/test_template_spaces.py` & `junifer-0.0.5.dev93/junifer/data/tests/test_template_spaces.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/data/utils.py` & `junifer-0.0.5.dev93/junifer/data/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/__init__.py` & `junifer-0.0.5.dev93/junifer/datagrabber/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/aomic/id1000.py` & `junifer-0.0.5.dev93/junifer/datagrabber/aomic/id1000.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/aomic/piop1.py` & `junifer-0.0.5.dev93/junifer/datagrabber/aomic/piop1.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/aomic/piop2.py` & `junifer-0.0.5.dev93/junifer/datagrabber/aomic/piop2.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/aomic/tests/test_id1000.py` & `junifer-0.0.5.dev93/junifer/datagrabber/aomic/tests/test_id1000.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/aomic/tests/test_piop1.py` & `junifer-0.0.5.dev93/junifer/datagrabber/aomic/tests/test_piop1.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/aomic/tests/test_piop2.py` & `junifer-0.0.5.dev93/junifer/datagrabber/aomic/tests/test_piop2.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/base.py` & `junifer-0.0.5.dev93/junifer/datagrabber/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/datalad_base.py` & `junifer-0.0.5.dev93/junifer/datagrabber/datalad_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/dmcc13_benchmark.py` & `junifer-0.0.5.dev93/junifer/datagrabber/dmcc13_benchmark.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/hcp1200/datalad_hcp1200.py` & `junifer-0.0.5.dev93/junifer/datagrabber/hcp1200/datalad_hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/hcp1200/hcp1200.py` & `junifer-0.0.5.dev93/junifer/datagrabber/hcp1200/hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/hcp1200/tests/test_hcp1200.py` & `junifer-0.0.5.dev93/junifer/datagrabber/hcp1200/tests/test_hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/multiple.py` & `junifer-0.0.5.dev93/junifer/datagrabber/multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/pattern.py` & `junifer-0.0.5.dev93/junifer/datagrabber/pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/pattern_datalad.py` & `junifer-0.0.5.dev93/junifer/datagrabber/pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/tests/test_base.py` & `junifer-0.0.5.dev93/junifer/datagrabber/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/tests/test_datagrabber_utils.py` & `junifer-0.0.5.dev93/junifer/datagrabber/tests/test_datagrabber_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/tests/test_datalad_base.py` & `junifer-0.0.5.dev93/junifer/datagrabber/tests/test_datalad_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/tests/test_dmcc13_benchmark.py` & `junifer-0.0.5.dev93/junifer/datagrabber/tests/test_dmcc13_benchmark.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/tests/test_multiple.py` & `junifer-0.0.5.dev93/junifer/datagrabber/tests/test_multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/tests/test_pattern.py` & `junifer-0.0.5.dev93/junifer/datagrabber/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/tests/test_pattern_datalad.py` & `junifer-0.0.5.dev93/junifer/datagrabber/tests/test_pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datagrabber/utils.py` & `junifer-0.0.5.dev93/junifer/datagrabber/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datareader/default.py` & `junifer-0.0.5.dev93/junifer/datareader/default.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/datareader/tests/test_default_reader.py` & `junifer-0.0.5.dev93/junifer/datareader/tests/test_default_reader.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/external/h5io/h5io/_h5io.py` & `junifer-0.0.5.dev93/junifer/external/h5io/h5io/_h5io.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/external/h5io/h5io/chunked_array.py` & `junifer-0.0.5.dev93/junifer/external/h5io/h5io/chunked_array.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/external/h5io/h5io/chunked_list.py` & `junifer-0.0.5.dev93/junifer/external/h5io/h5io/chunked_list.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/external/nilearn/junifer_nifti_spheres_masker.py` & `junifer-0.0.5.dev93/junifer/external/nilearn/junifer_nifti_spheres_masker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py` & `junifer-0.0.5.dev93/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/__init__.py` & `junifer-0.0.5.dev93/junifer/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/base.py` & `junifer-0.0.5.dev93/junifer/markers/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/collection.py` & `junifer-0.0.5.dev93/junifer/markers/collection.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/complexity/__init__.py` & `junifer-0.0.5.dev93/junifer/markers/complexity/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/complexity/complexity_base.py` & `junifer-0.0.5.dev93/junifer/markers/complexity/complexity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/complexity/hurst_exponent.py` & `junifer-0.0.5.dev93/junifer/markers/complexity/hurst_exponent.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/complexity/multiscale_entropy_auc.py` & `junifer-0.0.5.dev93/junifer/markers/complexity/multiscale_entropy_auc.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/complexity/perm_entropy.py` & `junifer-0.0.5.dev93/junifer/markers/complexity/perm_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/complexity/range_entropy.py` & `junifer-0.0.5.dev93/junifer/markers/complexity/range_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/complexity/range_entropy_auc.py` & `junifer-0.0.5.dev93/junifer/markers/complexity/range_entropy_auc.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/complexity/sample_entropy.py` & `junifer-0.0.5.dev93/junifer/markers/complexity/sample_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/complexity/tests/test_hurst_exponent.py` & `junifer-0.0.5.dev93/junifer/markers/complexity/tests/test_hurst_exponent.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/complexity/tests/test_multiscale_entropy_auc.py` & `junifer-0.0.5.dev93/junifer/markers/complexity/tests/test_multiscale_entropy_auc.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/complexity/tests/test_perm_entropy.py` & `junifer-0.0.5.dev93/junifer/markers/complexity/tests/test_perm_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/complexity/tests/test_range_entropy.py` & `junifer-0.0.5.dev93/junifer/markers/complexity/tests/test_range_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/complexity/tests/test_range_entropy_auc.py` & `junifer-0.0.5.dev93/junifer/markers/complexity/tests/test_range_entropy_auc.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/complexity/tests/test_sample_entropy.py` & `junifer-0.0.5.dev93/junifer/markers/complexity/tests/test_sample_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/complexity/tests/test_weighted_perm_entropy.py` & `junifer-0.0.5.dev93/junifer/markers/complexity/tests/test_weighted_perm_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/complexity/weighted_perm_entropy.py` & `junifer-0.0.5.dev93/junifer/markers/complexity/weighted_perm_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/ets_rss.py` & `junifer-0.0.5.dev93/junifer/markers/ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/falff/_afni_falff.py` & `junifer-0.0.5.dev93/junifer/markers/falff/_afni_falff.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/falff/_junifer_falff.py` & `junifer-0.0.5.dev93/junifer/markers/falff/_junifer_falff.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/falff/falff_base.py` & `junifer-0.0.5.dev93/junifer/markers/falff/falff_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/falff/falff_parcels.py` & `junifer-0.0.5.dev93/junifer/markers/falff/falff_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/falff/falff_spheres.py` & `junifer-0.0.5.dev93/junifer/markers/falff/falff_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/falff/tests/test_falff_parcels.py` & `junifer-0.0.5.dev93/junifer/markers/falff/tests/test_falff_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/falff/tests/test_falff_spheres.py` & `junifer-0.0.5.dev93/junifer/markers/falff/tests/test_falff_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py` & `junifer-0.0.5.dev93/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py` & `junifer-0.0.5.dev93/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py` & `junifer-0.0.5.dev93/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/functional_connectivity/functional_connectivity_base.py` & `junifer-0.0.5.dev93/junifer/markers/functional_connectivity/functional_connectivity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/functional_connectivity/functional_connectivity_parcels.py` & `junifer-0.0.5.dev93/junifer/markers/functional_connectivity/functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/functional_connectivity/functional_connectivity_spheres.py` & `junifer-0.0.5.dev93/junifer/markers/functional_connectivity/functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py` & `junifer-0.0.5.dev93/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py` & `junifer-0.0.5.dev93/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py` & `junifer-0.0.5.dev93/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py` & `junifer-0.0.5.dev93/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py` & `junifer-0.0.5.dev93/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py` & `junifer-0.0.5.dev93/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/parcel_aggregation.py` & `junifer-0.0.5.dev93/junifer/markers/parcel_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/reho/_afni_reho.py` & `junifer-0.0.5.dev93/junifer/markers/reho/_afni_reho.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/reho/_junifer_reho.py` & `junifer-0.0.5.dev93/junifer/markers/reho/_junifer_reho.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/reho/reho_base.py` & `junifer-0.0.5.dev93/junifer/markers/reho/reho_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/reho/reho_parcels.py` & `junifer-0.0.5.dev93/junifer/markers/reho/reho_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/reho/reho_spheres.py` & `junifer-0.0.5.dev93/junifer/markers/reho/reho_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/reho/tests/test_reho_parcels.py` & `junifer-0.0.5.dev93/junifer/markers/reho/tests/test_reho_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/reho/tests/test_reho_spheres.py` & `junifer-0.0.5.dev93/junifer/markers/reho/tests/test_reho_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/sphere_aggregation.py` & `junifer-0.0.5.dev93/junifer/markers/sphere_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/temporal_snr/temporal_snr_base.py` & `junifer-0.0.5.dev93/junifer/markers/temporal_snr/temporal_snr_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/temporal_snr/temporal_snr_parcels.py` & `junifer-0.0.5.dev93/junifer/markers/temporal_snr/temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/temporal_snr/temporal_snr_spheres.py` & `junifer-0.0.5.dev93/junifer/markers/temporal_snr/temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py` & `junifer-0.0.5.dev93/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py` & `junifer-0.0.5.dev93/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/tests/test_collection.py` & `junifer-0.0.5.dev93/junifer/markers/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/tests/test_ets_rss.py` & `junifer-0.0.5.dev93/junifer/markers/tests/test_ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/tests/test_marker_utils.py` & `junifer-0.0.5.dev93/junifer/markers/tests/test_marker_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/tests/test_markers_base.py` & `junifer-0.0.5.dev93/junifer/markers/tests/test_markers_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/tests/test_parcel_aggregation.py` & `junifer-0.0.5.dev93/junifer/markers/tests/test_parcel_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/tests/test_sphere_aggregation.py` & `junifer-0.0.5.dev93/junifer/markers/tests/test_sphere_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/markers/utils.py` & `junifer-0.0.5.dev93/junifer/markers/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/onthefly/read_transform.py` & `junifer-0.0.5.dev93/junifer/onthefly/read_transform.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/onthefly/tests/test_read_transform.py` & `junifer-0.0.5.dev93/junifer/onthefly/tests/test_read_transform.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/pipeline/pipeline_step_mixin.py` & `junifer-0.0.5.dev93/junifer/pipeline/pipeline_step_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/pipeline/registry.py` & `junifer-0.0.5.dev93/junifer/pipeline/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/pipeline/singleton.py` & `junifer-0.0.5.dev93/junifer/pipeline/singleton.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/pipeline/tests/test_pipeline_step_mixin.py` & `junifer-0.0.5.dev93/junifer/pipeline/tests/test_pipeline_step_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/pipeline/tests/test_registry.py` & `junifer-0.0.5.dev93/junifer/pipeline/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/pipeline/tests/test_update_meta_mixin.py` & `junifer-0.0.5.dev93/junifer/pipeline/tests/test_update_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/pipeline/tests/test_workdir_manager.py` & `junifer-0.0.5.dev93/junifer/pipeline/tests/test_workdir_manager.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/pipeline/update_meta_mixin.py` & `junifer-0.0.5.dev93/junifer/pipeline/update_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/pipeline/utils.py` & `junifer-0.0.5.dev93/junifer/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/pipeline/workdir_manager.py` & `junifer-0.0.5.dev93/junifer/pipeline/workdir_manager.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/preprocess/base.py` & `junifer-0.0.5.dev93/junifer/preprocess/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/preprocess/confounds/fmriprep_confound_remover.py` & `junifer-0.0.5.dev93/junifer/preprocess/confounds/fmriprep_confound_remover.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py` & `junifer-0.0.5.dev93/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/preprocess/smoothing/_afni_smoothing.py` & `junifer-0.0.5.dev93/junifer/preprocess/smoothing/_afni_smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/preprocess/smoothing/_fsl_smoothing.py` & `junifer-0.0.5.dev93/junifer/preprocess/smoothing/_fsl_smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/preprocess/smoothing/_nilearn_smoothing.py` & `junifer-0.0.5.dev93/junifer/preprocess/smoothing/_nilearn_smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/preprocess/smoothing/smoothing.py` & `junifer-0.0.5.dev93/junifer/preprocess/smoothing/smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/preprocess/smoothing/tests/test_smoothing.py` & `junifer-0.0.5.dev93/junifer/preprocess/smoothing/tests/test_smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/preprocess/tests/test_preprocess_base.py` & `junifer-0.0.5.dev93/junifer/preprocess/tests/test_preprocess_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/preprocess/warping/_ants_warper.py` & `junifer-0.0.5.dev93/junifer/preprocess/warping/_ants_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/preprocess/warping/_fsl_warper.py` & `junifer-0.0.5.dev93/junifer/preprocess/warping/_fsl_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/preprocess/warping/space_warper.py` & `junifer-0.0.5.dev93/junifer/preprocess/warping/space_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/preprocess/warping/tests/test_space_warper.py` & `junifer-0.0.5.dev93/junifer/preprocess/warping/tests/test_space_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/stats.py` & `junifer-0.0.5.dev93/junifer/stats.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/storage/base.py` & `junifer-0.0.5.dev93/junifer/storage/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         )
 
     def store(self, kind: str, **kwargs) -> None:
         """Store extracted features data.
 
         Parameters
         ----------
-        kind : {"matrix", "timeseries", "vector"}
+        kind : {"matrix", "timeseries", "vector", "scalar_table"}
             The storage kind.
         **kwargs
             The keyword arguments.
 
         Raises
         ------
         ValueError
@@ -214,14 +214,18 @@
             self.store_matrix(meta_md5=meta_md5, element=t_element, **kwargs)
         elif kind == "timeseries":
             self.store_timeseries(
                 meta_md5=meta_md5, element=t_element, **kwargs
             )
         elif kind == "vector":
             self.store_vector(meta_md5=meta_md5, element=t_element, **kwargs)
+        elif kind == "scalar_table":
+            self.store_scalar_table(
+                meta_md5=meta_md5, element=t_element, **kwargs
+            )
 
     def store_matrix(
         self,
         meta_md5: str,
         element: Dict,
         data: np.ndarray,
         col_names: Optional[Iterable[str]] = None,
@@ -309,14 +313,46 @@
 
         """
         raise_error(
             msg="Concrete classes need to implement store_timeseries().",
             klass=NotImplementedError,
         )
 
+    def store_scalar_table(
+        self,
+        meta_md5: str,
+        element: Dict,
+        data: np.ndarray,
+        col_names: Optional[Iterable[str]] = None,
+        row_names: Optional[Iterable[str]] = None,
+        row_header_col_name: Optional[str] = "feature",
+    ) -> None:
+        """Store table with scalar values.
+
+        Parameters
+        ----------
+        meta_md5 : str
+            The metadata MD5 hash.
+        element : dict
+            The element as a dictionary.
+        data : numpy.ndarray
+            The timeseries data to store.
+        col_names : list or tuple of str, optional
+            The column labels (default None).
+        row_names : str, optional
+            The row labels (default None).
+        row_header_col_name : str, optional
+            The column name for the row header column (default "feature").
+
+        """
+        raise_error(
+            msg="Concrete classes need to implement store_scalar_table().",
+            klass=NotImplementedError,
+        )
+
     @abstractmethod
     def collect(self) -> None:
         """Collect data."""
         raise_error(
             msg="Concrete classes need to implement collect().",
             klass=NotImplementedError,
         )
```

### Comparing `junifer-0.0.5.dev86/junifer/storage/hdf5.py` & `junifer-0.0.5.dev93/junifer/storage/hdf5.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,16 @@
     -------
     ChunkedArray or ChunkedList
         The chunked array or list.
 
     Raises
     ------
     ValueError
-        If `kind` is not one of ['vector', 'matrix', 'timeseries'].
+        If `kind` is not one of ['vector', 'matrix', 'timeseries',
+        'scalar_table'].
 
     """
     if kind in ["vector", "matrix"]:
         features_data = np.concatenate(chunk_data, axis=-1)
         array_shape = [features_data.shape[0]]
         array_chunk_size = [features_data.shape[0]]
         # Append second dimension for 3D
@@ -73,24 +74,25 @@
         array_chunk_size.append(chunk_size)
         out = ChunkedArray(
             data=features_data,
             shape=tuple(array_shape),
             chunk_size=tuple(array_chunk_size),
             n_chunk=i_chunk,
         )
-    elif kind == "timeseries":
+    elif kind in ["timeseries", "scalar_table"]:
         out = ChunkedList(
             data=chunk_data,
             size=element_count,
             offset=i_chunk * chunk_size,
         )
     else:
         raise_error(
             f"Invalid kind: {kind}. "
-            "Must be one of ['vector', 'matrix', 'timeseries']."
+            "Must be one of ['vector', 'matrix', 'timeseries',"
+            "'scalar_table']."
         )
     return out
 
 
 @register_storage
 class HDF5FeatureStorage(BaseFeatureStorage):
     """Concrete implementation for feature storage via HDF5.
@@ -142,15 +144,15 @@
             logger.info(
                 f"Output directory: '{uri.parent.resolve()}' "
                 "does not exist, creating now"
             )
             uri.parent.mkdir(parents=True, exist_ok=True)
 
         # Available storage kinds
-        storage_types = ["vector", "timeseries", "matrix"]
+        storage_types = ["vector", "timeseries", "matrix", "scalar_table"]
 
         super().__init__(
             uri=uri,
             storage_types=storage_types,
             single_output=single_output,
         )
 
@@ -165,15 +167,15 @@
         Returns
         -------
         list of str
             The list of storage types that can be used as input for this
             storage.
 
         """
-        return ["matrix", "vector", "timeseries"]
+        return ["matrix", "vector", "timeseries", "scalar_table"]
 
     def _fetch_correct_uri_for_io(self, element: Optional[Dict]) -> str:
         """Return proper URI for I/O based on `element`.
 
         If `element` is None, will return `self.uri`.
 
         Parameters
@@ -504,14 +506,34 @@
                 element_idx[hdf_data["row_header_column_name"]].extend(
                     np.arange(n_rows)
                 )
             # Set column headers for dataframe
             columns = hdf_data["column_headers"]
             # Convert data from 3D to 2D
             reshaped_data = np.concatenate(all_data, axis=0)
+        elif hdf_data["kind"] == "scalar_table":
+            # Create dictionary for aggregating index data
+            element_idx = defaultdict(list)
+            all_data = []
+            for idx, element in enumerate(hdf_data["element"]):
+                # Get row count for the element
+                t_data = hdf_data["data"][idx]
+                all_data.append(t_data)
+                n_rows = len(hdf_data["row_headers"])
+                # Set rows for the index
+                for key, val in element.items():
+                    element_idx[key].extend([val] * n_rows)
+                # Add extra column for row header column name
+                element_idx[hdf_data["row_header_column_name"]].extend(
+                    hdf_data["row_headers"]
+                )
+            # Set column headers for dataframe
+            columns = hdf_data["column_headers"]
+            # Convert data from 3D to 2D
+            reshaped_data = np.concatenate(all_data, axis=0)
 
         # Create dataframe for index
         idx_df = pd.DataFrame(data=element_idx)  # type: ignore
         # Create multiindex from dataframe
         hdf_data_idx = pd.MultiIndex.from_frame(df=idx_df)
         logger.debug(
             "Generated pandas.MultiIndex for feature "
@@ -639,15 +661,15 @@
         This method first loads existing data (if any) using
         ``_read_data`` and appends to it the `element` and `data`
         values, and writes them and other information passed via
         `**kwargs` using ``_write_processed_data``.
 
         Parameters
         ----------
-        kind : {"matrix", "vector", "timeseries"}
+        kind : {"matrix", "vector", "timeseries", "scalar_table"}
             The storage kind.
         meta_md5 : str
             The metadata MD5 hash.
         element : list of dict
             The element as list of dictionary.
         data : numpy.ndarray
             The data to store.
@@ -735,16 +757,16 @@
             logger.debug(f"No duplicate elements found for {meta_md5} ...")
 
             logger.debug(
                 f"Existing data found for {meta_md5}, appending to it ..."
             )
 
             t_data = stored_data["data"]
-            if kind == "timeseries":
-                t_data.append(data)
+            if kind in ["timeseries", "scalar_table"]:
+                t_data += data
             else:
                 t_data = np.concatenate((t_data, data), axis=-1)
             # Existing entry; append to existing
             # "element" and "data"
             data_to_write.update(
                 {
                     "element": stored_data["element"] + element,
@@ -917,14 +939,51 @@
             meta_md5=meta_md5,
             element=[element],  # convert to list
             data=[data],  # convert to list
             column_headers=col_names,
             row_header_column_name="timepoint",
         )
 
+    def store_scalar_table(
+        self,
+        meta_md5: str,
+        element: Dict,
+        data: np.ndarray,
+        col_names: Optional[Iterable[str]] = None,
+        row_names: Optional[Iterable[str]] = None,
+        row_header_col_name: Optional[str] = "feature",
+    ) -> None:
+        """Store table with scalar values.
+
+        Parameters
+        ----------
+        meta_md5 : str
+            The metadata MD5 hash.
+        element : dict
+            The element as a dictionary.
+        data : numpy.ndarray
+            The scalar table data to store.
+        col_names : list or tuple of str, optional
+            The column labels (default None).
+        row_names : str, optional
+            The row labels (default None).
+        row_header_col_name : str, optional
+            The column name for the row header column (default "feature").
+
+        """
+        self._store_data(
+            kind="scalar_table",
+            meta_md5=meta_md5,
+            element=[element],  # convert to list
+            data=[data],  # convert to list
+            column_headers=col_names,
+            row_headers=row_names,
+            row_header_column_name=row_header_col_name,
+        )
+
     def collect(self) -> None:
         """Implement data collection.
 
         This method globs the element files and runs a loop
         over them while reading metadata and then runs a loop
         over all the stored features in the metadata, storing
         the metadata and the feature data right after reading.
@@ -1025,15 +1084,15 @@
                         k: v
                         for k, v in t_data.items()
                         if k not in ["data", "element"]
                     }
                     kind = static_data["kind"]
 
                 # Append the "dynamic" data
-                if kind == "timeseries":
+                if kind in ["timeseries", "scalar_table"]:
                     chunk_data.extend(t_data["data"])
                 else:
                     chunk_data.append(t_data["data"])
                 elements.extend(t_data["element"])
 
                 i_file += 1
                 if (i_file % t_chunk_size == 0) or i_file == element_count:
```

### Comparing `junifer-0.0.5.dev86/junifer/storage/pandas_base.py` & `junifer-0.0.5.dev93/junifer/storage/pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/storage/sqlite.py` & `junifer-0.0.5.dev93/junifer/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/storage/tests/test_hdf5.py` & `junifer-0.0.5.dev93/junifer/storage/tests/test_hdf5.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,20 @@
     process_meta,
 )
 
 
 def test_get_valid_inputs() -> None:
     """Test valid inputs."""
     storage = HDF5FeatureStorage(uri="/tmp")
-    assert storage.get_valid_inputs() == ["matrix", "vector", "timeseries"]
+    assert storage.get_valid_inputs() == [
+        "matrix",
+        "vector",
+        "timeseries",
+        "scalar_table",
+    ]
 
 
 def test_single_output(tmp_path: Path) -> None:
     """Test single output setup.
 
     Parameters
     ----------
@@ -804,28 +809,75 @@
         meta_md5=meta_md5, element=element_to_store, meta=meta_to_store
     )
 
     # Data to store
     data = np.array([[10], [20], [30], [40], [50]])
     col_names = ["signal"]
 
-    # Store vector
+    # Store timeseries
     storage.store_timeseries(
         meta_md5=meta_md5,
         element=element_to_store,
         data=data,
         col_names=col_names,
     )
 
     # Read into dataframe
     read_df = storage.read_df(feature_md5=meta_md5)
     # Check if data are equal
     assert_array_equal(read_df.values, data)
 
 
+def test_store_scalar_table(tmp_path: Path) -> None:
+    """Test scalar table store.
+
+    Parameters
+    ----------
+    tmp_path : pathlib.Path
+        The path to the test directory.
+
+    """
+    uri = tmp_path / "test_store_scalar_table.hdf5"
+    storage = HDF5FeatureStorage(uri=uri)
+    # Metadata to store
+    element = {"subject": "test"}
+    meta = {
+        "element": element,
+        "dependencies": ["numpy"],
+        "marker": {"name": "brainprint"},
+        "type": "FreeSurfer",
+    }
+    # Process the metadata
+    meta_md5, meta_to_store, element_to_store = process_meta(meta)
+    # Store metadata
+    storage.store_metadata(
+        meta_md5=meta_md5, element=element_to_store, meta=meta_to_store
+    )
+
+    # Data to store
+    data = np.array([[10, 20], [30, 40], [50, 60]])
+    col_names = ["roi1", "roi2"]
+    row_names = ["ev1", "ev2", "ev3"]
+
+    # Store timeseries
+    storage.store_scalar_table(
+        meta_md5=meta_md5,
+        element=element_to_store,
+        data=data,
+        col_names=col_names,
+        row_names=row_names,
+        row_header_col_name="eigenvalue",
+    )
+
+    # Read into dataframe
+    read_df = storage.read_df(feature_md5=meta_md5)
+    # Check if data are equal
+    assert_array_equal(read_df.values, data)
+
+
 def _create_data_to_store(n_elements: int, kind: str) -> Tuple[str, Dict]:
     """Create data to store.
 
     Parameters
     ----------
     n_elements : int
         The number of elements to create.
@@ -850,21 +902,27 @@
     elif kind == "matrix":
         data_to_store = {
             "data": np.arange(100).reshape(10, 10),
             "row_names": [f"row-{i}" for i in range(10)],
             "col_names": [f"col-{i}" for i in range(10)],
             "matrix_kind": "full",
         }
-    elif kind == "timeseries":
+    elif kind in "timeseries":
         data_to_store = {
             "data": np.arange(20).reshape(2, 10),
             "col_names": [f"col-{i}" for i in range(10)],
         }
-    else:
-        raise ValueError(f"Unknown kind {kind}.")
+    elif kind in "scalar_table":
+        data_to_store = {
+            "data": np.arange(50).reshape(5, 10),
+            "row_names": [f"row-{i}" for i in range(5)],
+            "col_names": [f"col-{i}" for i in range(10)],
+            "row_header_col_name": "row",
+        }
+
     for i in range(n_elements):
         element = {"subject": f"sub-{i // 2}", "session": f"ses-{i % 2}"}
         meta = {
             "element": element,
             "dependencies": ["numpy"],
             "marker": {"name": f"test-{kind}"},
             "type": "BOLD",
@@ -899,14 +957,15 @@
     "n_elements, chunk_size, kind",
     [
         (10, 3, "vector"),
         (10, 5, "vector"),
         (10, 3, "matrix"),
         (10, 5, "matrix"),
         (10, 5, "timeseries"),
+        (10, 5, "scalar_table"),
     ],
 )
 def test_multi_output_store_and_collect(
     tmp_path: Path, n_elements: int, chunk_size: int, kind: str
 ) -> None:
     """Test multi output storing and collection.
 
@@ -926,45 +985,50 @@
     storage = HDF5FeatureStorage(
         uri=uri, single_output=False, chunk_size=chunk_size
     )
 
     meta_md5, all_data = _create_data_to_store(n_elements, kind)
 
     for t_data in all_data:
-        # Store metadata for tables
+        # Store metadata
         storage.store_metadata(
             meta_md5=meta_md5,
             element=t_data["element"],
             meta=t_data["meta"],
         )
+        # Store data
         if kind == "vector":
-            # Store tables
             storage.store_vector(
                 meta_md5=meta_md5,
                 element=t_data["element"],
                 **t_data["data"],
             )
         elif kind == "matrix":
-            # Store tables
             storage.store_matrix(
                 meta_md5=meta_md5,
                 element=t_data["element"],
                 **t_data["data"],
             )
         elif kind == "timeseries":
             storage.store_timeseries(
                 meta_md5=meta_md5,
                 element=t_data["element"],
                 **t_data["data"],
             )
+        elif kind == "scalar_table":
+            storage.store_scalar_table(
+                meta_md5=meta_md5,
+                element=t_data["element"],
+                **t_data["data"],
+            )
     # Check that base URI does not exist yet
     assert not uri.exists()
 
     for t_data in all_data:
-        # Convert element to preifx
+        # Convert element to prefix
         prefix = element_to_prefix(t_data["element"])
         # URIs for data storage
         elem_uri = uri.parent / f"{prefix}{uri.name}"
         # Check URIs for data storage exist
         assert elem_uri.exists()
 
         # Read stored metadata from different files using element
@@ -973,26 +1037,30 @@
         assert read_meta == {meta_md5: t_data["meta"]}
 
     # Collect data
     storage.collect()
     # Check that base URI exists now
     assert uri.exists()
 
-    # # Read unified metadata
+    # Read unified metadata
     read_unified_meta = storage.list_features()
     assert meta_md5 in read_unified_meta
 
     # Check if aggregated metadata are equal
     assert all(x["meta"] == read_unified_meta[meta_md5] for x in all_data)
 
     all_df = storage.read_df(feature_md5=meta_md5)
     if kind == "timeseries":
         data_size = np.sum([x["data"]["data"].shape[0] for x in all_data])
         assert len(all_df) == data_size
         idx_names = [x for x in all_df.index.names if x != "timepoint"]
+    elif kind == "scalar_table":
+        data_size = np.sum([x["data"]["data"].shape[0] for x in all_data])
+        assert len(all_df) == data_size
+        idx_names = [x for x in all_df.index.names if x != "row"]
     else:
         assert len(all_df) == len(all_data)
         idx_names = all_df.index.names
     for t_data in all_data:
         t_series = all_df.loc[tuple([t_data["element"][v] for v in idx_names])]
         if kind == "vector":
             assert_array_equal(t_series.values, t_data["data"]["data"])
@@ -1009,14 +1077,18 @@
             assert_array_equal(t_series.values, flat_data)
             series_names = t_series.index.values.tolist()
             assert series_names == columns
         elif kind == "timeseries":
             assert_array_equal(t_series.values, t_data["data"]["data"])
             series_names = t_series.columns.values.tolist()
             assert series_names == t_data["data"]["col_names"]
+        elif kind == "scalar_table":
+            assert_array_equal(t_series.values, t_data["data"]["data"])
+            series_names = t_series.columns.values.tolist()
+            assert series_names == t_data["data"]["col_names"]
 
 
 def test_collect_error_single_output() -> None:
     """Test error for collect in single output storage."""
     with pytest.raises(
         NotImplementedError,
         match="is not implemented for single output.",
```

### Comparing `junifer-0.0.5.dev86/junifer/storage/tests/test_pandas_base.py` & `junifer-0.0.5.dev93/junifer/storage/tests/test_pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/storage/tests/test_sqlite.py` & `junifer-0.0.5.dev93/junifer/storage/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/storage/tests/test_storage_base.py` & `junifer-0.0.5.dev93/junifer/storage/tests/test_storage_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/storage/tests/test_utils.py` & `junifer-0.0.5.dev93/junifer/storage/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/storage/utils.py` & `junifer-0.0.5.dev93/junifer/storage/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv` & `junifer-0.0.5.dev93/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/testing/datagrabbers.py` & `junifer-0.0.5.dev93/junifer/testing/datagrabbers.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/testing/registry.py` & `junifer-0.0.5.dev93/junifer/testing/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py` & `junifer-0.0.5.dev93/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/testing/tests/test_partlycloudytesting_datagrabber.py` & `junifer-0.0.5.dev93/junifer/testing/tests/test_partlycloudytesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/testing/tests/test_spmauditory_datagrabber.py` & `junifer-0.0.5.dev93/junifer/testing/tests/test_spmauditory_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/testing/tests/test_testing_registry.py` & `junifer-0.0.5.dev93/junifer/testing/tests/test_testing_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/testing/utils.py` & `junifer-0.0.5.dev93/junifer/testing/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/tests/test_stats.py` & `junifer-0.0.5.dev93/junifer/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/utils/helpers.py` & `junifer-0.0.5.dev93/junifer/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/utils/logging.py` & `junifer-0.0.5.dev93/junifer/utils/logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/utils/tests/test_fs.py` & `junifer-0.0.5.dev93/junifer/utils/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/utils/tests/test_helpers.py` & `junifer-0.0.5.dev93/junifer/utils/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer/utils/tests/test_logging.py` & `junifer-0.0.5.dev93/junifer/utils/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/junifer.egg-info/PKG-INFO` & `junifer-0.0.5.dev93/junifer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.5.dev86
+Version: 0.0.5.dev93
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: Changelog, https://juaml.github.io/junifer/main/whats_new.html
 Project-URL: Documentation, https://juaml.github.io/junifer
 Project-URL: Homepage, https://juaml.github.io/junifer
```

### Comparing `junifer-0.0.5.dev86/junifer.egg-info/SOURCES.txt` & `junifer-0.0.5.dev93/junifer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 docs/changes/newsfragments/331.bugfix
 docs/changes/newsfragments/332.bugfix
 docs/changes/newsfragments/336.removal
 docs/changes/newsfragments/339.bugfix
 docs/changes/newsfragments/340.bugfix
 docs/changes/newsfragments/341.enh
 docs/changes/newsfragments/342.misc
+docs/changes/newsfragments/343.feature
 docs/extending/coordinates.rst
 docs/extending/datagrabber.rst
 docs/extending/dependencies.rst
 docs/extending/extension.rst
 docs/extending/index.rst
 docs/extending/marker.rst
 docs/extending/masks.rst
```

### Comparing `junifer-0.0.5.dev86/junifer.egg-info/requires.txt` & `junifer-0.0.5.dev93/junifer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/pyproject.toml` & `junifer-0.0.5.dev93/pyproject.toml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/tools/create_aomic1000_example_dataset.py` & `junifer-0.0.5.dev93/tools/create_aomic1000_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/tools/create_aomicpiop1_example_dataset.py` & `junifer-0.0.5.dev93/tools/create_aomicpiop1_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/tools/create_aomicpiop2_example_dataset.py` & `junifer-0.0.5.dev93/tools/create_aomicpiop2_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/tools/create_bids_example_dataset.py` & `junifer-0.0.5.dev93/tools/create_bids_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/tools/create_bids_example_dataset_sessions.py` & `junifer-0.0.5.dev93/tools/create_bids_example_dataset_sessions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/tools/create_dmcc13_benchmark_example_dataset.py` & `junifer-0.0.5.dev93/tools/create_dmcc13_benchmark_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/tools/create_hcp1200_example_dataset.py` & `junifer-0.0.5.dev93/tools/create_hcp1200_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev86/tox.ini` & `junifer-0.0.5.dev93/tox.ini`

 * *Files identical despite different names*

