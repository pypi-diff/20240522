# Comparing `tmp/erlab-2.5.2.tar.gz` & `tmp/erlab-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlab-2.5.2.tar", last modified: Thu May 16 02:14:48 2024, max compression
+gzip compressed data, was "erlab-2.5.3.tar", last modified: Wed May 22 08:43:07 2024, max compression
```

## Comparing `erlab-2.5.2.tar` & `erlab-2.5.3.tar`

### file list

```diff
@@ -1,199 +1,200 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.428651 erlab-2.5.2/
--rw-r--r--   0 root         (0) root         (0)       74 2024-05-16 02:14:39.000000 erlab-2.5.2/.codecov.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.376652 erlab-2.5.2/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.384652 erlab-2.5.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)     2200 2024-05-16 02:14:39.000000 erlab-2.5.2/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 root         (0) root         (0)      206 2024-05-16 02:14:39.000000 erlab-2.5.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)     1071 2024-05-16 02:14:39.000000 erlab-2.5.2/.github/ISSUE_TEMPLATE/feature-request.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.384652 erlab-2.5.2/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1668 2024-05-16 02:14:39.000000 erlab-2.5.2/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     2535 2024-05-16 02:14:39.000000 erlab-2.5.2/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2898 2024-05-16 02:14:39.000000 erlab-2.5.2/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1022 2024-05-16 02:14:39.000000 erlab-2.5.2/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      793 2024-05-16 02:14:39.000000 erlab-2.5.2/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)   128259 2024-05-16 02:14:44.000000 erlab-2.5.2/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2024-05-16 02:14:39.000000 erlab-2.5.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    48973 2024-05-16 02:14:48.428651 erlab-2.5.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1473 2024-05-16 02:14:39.000000 erlab-2.5.2/PythonInterface.ipf
--rw-r--r--   0 root         (0) root         (0)     5552 2024-05-16 02:14:39.000000 erlab-2.5.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.384652 erlab-2.5.2/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      726 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/environment.yml
--rw-r--r--   0 root         (0) root         (0)      804 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.388652 erlab-2.5.2/docs/source/
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/bibliography.rst
--rw-r--r--   0 root         (0) root         (0)    18220 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)    15203 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      106 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/erlab.accessors.rst
--rw-r--r--   0 root         (0) root         (0)      101 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/erlab.analysis.rst
--rw-r--r--   0 root         (0) root         (0)      485 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/erlab.constants.rst
--rw-r--r--   0 root         (0) root         (0)      116 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/erlab.interactive.rst
--rw-r--r--   0 root         (0) root         (0)       81 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/erlab.io.rst
--rw-r--r--   0 root         (0) root         (0)      236 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/erlab.lattice.rst
--rw-r--r--   0 root         (0) root         (0)      224 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/erlab.parallel.rst
--rw-r--r--   0 root         (0) root         (0)      174 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/erlab.plotting.rst
--rw-r--r--   0 root         (0) root         (0)     5039 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/getting-started.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.396652 erlab-2.5.2/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)   328062 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/images/flowchart_multiple.pdf
--rw-r--r--   0 root         (0) root         (0)   328737 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/images/flowchart_single.pdf
--rw-r--r--   0 root         (0) root         (0)   996803 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/images/imagetool_dark.png
--rw-r--r--   0 root         (0) root         (0)   966547 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/images/imagetool_light.png
--rw-r--r--   0 root         (0) root         (0)   709231 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/images/ktool_1_dark.png
--rw-r--r--   0 root         (0) root         (0)   694078 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/images/ktool_1_light.png
--rw-r--r--   0 root         (0) root         (0)   703343 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/images/ktool_2_dark.png
--rw-r--r--   0 root         (0) root         (0)   686688 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/images/ktool_2_light.png
--rw-r--r--   0 root         (0) root         (0)     3119 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.396652 erlab-2.5.2/docs/source/pyplots/
--rw-r--r--   0 root         (0) root         (0)     2604 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/pyplots/norms.py
--rw-r--r--   0 root         (0) root         (0)     1470 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/reference.rst
--rw-r--r--   0 root         (0) root         (0)     3099 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/refs.bib
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.400652 erlab-2.5.2/docs/source/user-guide/
--rw-r--r--   0 root         (0) root         (0)    42435 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/user-guide/curve-fitting.ipynb
--rw-r--r--   0 root         (0) root         (0)     2598 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/user-guide/imagetool.rst
--rw-r--r--   0 root         (0) root         (0)     1291 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/user-guide/index.rst
--rw-r--r--   0 root         (0) root         (0)    12039 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/user-guide/indexing.ipynb
--rw-r--r--   0 root         (0) root         (0)    54817 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/user-guide/io.ipynb
--rw-r--r--   0 root         (0) root         (0)    10710 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/user-guide/kconv.ipynb
--rw-r--r--   0 root         (0) root         (0)    27572 2024-05-16 02:14:39.000000 erlab-2.5.2/docs/source/user-guide/plotting.ipynb
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-16 02:14:39.000000 erlab-2.5.2/environment.yml
--rw-r--r--   0 root         (0) root         (0)     5938 2024-05-16 02:14:39.000000 erlab-2.5.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      299 2024-05-16 02:14:39.000000 erlab-2.5.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 02:14:48.428651 erlab-2.5.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.380652 erlab-2.5.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.400652 erlab-2.5.2/src/erlab/
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-16 02:14:44.000000 erlab-2.5.2/src/erlab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.400652 erlab-2.5.2/src/erlab/accessors/
--rw-r--r--   0 root         (0) root         (0)      897 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/accessors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26123 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/accessors/fit.py
--rw-r--r--   0 root         (0) root         (0)    30007 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/accessors/kspace.py
--rw-r--r--   0 root         (0) root         (0)    14898 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/accessors/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.404652 erlab-2.5.2/src/erlab/analysis/
--rw-r--r--   0 root         (0) root         (0)      880 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5322 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/analysis/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.404652 erlab-2.5.2/src/erlab/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)      168 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/analysis/fit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.404652 erlab-2.5.2/src/erlab/analysis/fit/functions/
--rw-r--r--   0 root         (0) root         (0)      957 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/analysis/fit/functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10779 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/analysis/fit/functions/dynamic.py
--rw-r--r--   0 root         (0) root         (0)     9594 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/analysis/fit/functions/general.py
--rw-r--r--   0 root         (0) root         (0)     6905 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/analysis/fit/minuit.py
--rw-r--r--   0 root         (0) root         (0)    12746 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/analysis/fit/models.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/analysis/fit/spline.py
--rw-r--r--   0 root         (0) root         (0)    20223 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/analysis/gold.py
--rw-r--r--   0 root         (0) root         (0)    27520 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/analysis/image.py
--rw-r--r--   0 root         (0) root         (0)    14968 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/analysis/interpolate.py
--rw-r--r--   0 root         (0) root         (0)    10276 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/analysis/kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.404652 erlab-2.5.2/src/erlab/analysis/mask/
--rw-r--r--   0 root         (0) root         (0)     5397 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/analysis/mask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8505 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/analysis/mask/polygon.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/analysis/transform.py
--rw-r--r--   0 root         (0) root         (0)     5443 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/analysis/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.404652 erlab-2.5.2/src/erlab/characterization/
--rw-r--r--   0 root         (0) root         (0)      232 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2152 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.408652 erlab-2.5.2/src/erlab/interactive/
--rw-r--r--   0 root         (0) root         (0)      526 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14181 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/bzplot.py
--rw-r--r--   0 root         (0) root         (0)    21371 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/colors.py
--rw-r--r--   0 root         (0) root         (0)    23038 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/curvefittingtool.py
--rw-r--r--   0 root         (0) root         (0)    11816 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/derivative.py
--rw-r--r--   0 root         (0) root         (0)    16300 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/dtool.ui
--rw-r--r--   0 root         (0) root         (0)    19376 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/fermiedge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.408652 erlab-2.5.2/src/erlab/interactive/imagetool/
--rw-r--r--   0 root         (0) root         (0)    17431 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/imagetool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.412652 erlab-2.5.2/src/erlab/interactive/imagetool/_deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/imagetool/_deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52053 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
--rw-r--r--   0 root         (0) root         (0)   114641 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
--rw-r--r--   0 root         (0) root         (0)    27909 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/imagetool/controls.py
--rw-r--r--   0 root         (0) root         (0)    57841 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/imagetool/core.py
--rw-r--r--   0 root         (0) root         (0)    14551 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/imagetool/fastbinning.py
--rw-r--r--   0 root         (0) root         (0)    25642 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/imagetool/slicer.py
--rw-r--r--   0 root         (0) root         (0)    16014 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/kspace.py
--rw-r--r--   0 root         (0) root         (0)    19321 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/ktool.ui
--rw-r--r--   0 root         (0) root         (0)     2749 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/masktool.py
--rw-r--r--   0 root         (0) root         (0)    56647 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/interactive/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.412652 erlab-2.5.2/src/erlab/io/
--rw-r--r--   0 root         (0) root         (0)     2194 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.412652 erlab-2.5.2/src/erlab/io/characterization/
--rw-r--r--   0 root         (0) root         (0)      170 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/io/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3058 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/io/characterization/resistance.py
--rw-r--r--   0 root         (0) root         (0)     1981 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/io/characterization/xrd.py
--rw-r--r--   0 root         (0) root         (0)    43727 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/io/dataloader.py
--rw-r--r--   0 root         (0) root         (0)    12460 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/io/exampledata.py
--rw-r--r--   0 root         (0) root         (0)     6998 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/io/igor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.412652 erlab-2.5.2/src/erlab/io/plugins/
--rw-r--r--   0 root         (0) root         (0)      900 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/io/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3811 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/io/plugins/da30.py
--rw-r--r--   0 root         (0) root         (0)     1142 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/io/plugins/kriss.py
--rw-r--r--   0 root         (0) root         (0)     8166 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/io/plugins/merlin.py
--rw-r--r--   0 root         (0) root         (0)     7667 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/io/plugins/ssrl52.py
--rw-r--r--   0 root         (0) root         (0)     6737 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/io/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2528 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/lattice.py
--rw-r--r--   0 root         (0) root         (0)     1522 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.416652 erlab-2.5.2/src/erlab/plotting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.416652 erlab-2.5.2/src/erlab/plotting/IgorCT/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/IgorCT/Blue-White.txt
--rw-r--r--   0 root         (0) root         (0)     3456 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/IgorCT/BlueHot.ibw
--rw-r--r--   0 root         (0) root         (0)     3526 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
--rw-r--r--   0 root         (0) root         (0)     3530 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
--rw-r--r--   0 root         (0) root         (0)     3531 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/IgorCT/ColdWarm.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw
--rw-r--r--   0 root         (0) root         (0)     1920 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/IgorCT/ametrine.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/IgorCT/isolum.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/IgorCT/morgenstemning.ibw
--rw-r--r--   0 root         (0) root         (0)     2113 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30848 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/annotations.py
--rw-r--r--   0 root         (0) root         (0)    18686 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/atoms.py
--rw-r--r--   0 root         (0) root         (0)     4420 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/bz.py
--rw-r--r--   0 root         (0) root         (0)    39811 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     2248 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/erplot.py
--rw-r--r--   0 root         (0) root         (0)    38540 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/general.py
--rw-r--r--   0 root         (0) root         (0)     2739 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/plot3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.420652 erlab-2.5.2/src/erlab/plotting/stylelib/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/stylelib/fira.mplstyle
--rw-r--r--   0 root         (0) root         (0)     6826 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/stylelib/firalight.mplstyle
--rw-r--r--   0 root         (0) root         (0)    14358 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/stylelib/khan.mplstyle
--rw-r--r--   0 root         (0) root         (0)     9160 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/stylelib/nature.mplstyle
--rw-r--r--   0 root         (0) root         (0)      630 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/stylelib/poster.mplstyle
--rw-r--r--   0 root         (0) root         (0)     7023 2024-05-16 02:14:39.000000 erlab-2.5.2/src/erlab/plotting/stylelib/times.mplstyle
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.424651 erlab-2.5.2/src/erlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    48973 2024-05-16 02:14:48.000000 erlab-2.5.2/src/erlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5265 2024-05-16 02:14:48.000000 erlab-2.5.2/src/erlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 02:14:48.000000 erlab-2.5.2/src/erlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      667 2024-05-16 02:14:48.000000 erlab-2.5.2/src/erlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-16 02:14:48.000000 erlab-2.5.2/src/erlab.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.420652 erlab-2.5.2/templates/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-05-16 02:14:39.000000 erlab-2.5.2/templates/.macros.j2
--rw-r--r--   0 root         (0) root         (0)      161 2024-05-16 02:14:39.000000 erlab-2.5.2/templates/.release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)      423 2024-05-16 02:14:39.000000 erlab-2.5.2/templates/CHANGELOG.md.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.420652 erlab-2.5.2/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.420652 erlab-2.5.2/tests/accessors/
--rw-r--r--   0 root         (0) root         (0)     5855 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/accessors/test_fit.py
--rw-r--r--   0 root         (0) root         (0)     4150 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/accessors/test_kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.420652 erlab-2.5.2/tests/analysis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.420652 erlab-2.5.2/tests/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)     4497 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/analysis/fit/test_functions_dynamic.py
--rw-r--r--   0 root         (0) root         (0)     4794 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/analysis/fit/test_functions_general.py
--rw-r--r--   0 root         (0) root         (0)     1087 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/analysis/fit/test_minuit.py
--rw-r--r--   0 root         (0) root         (0)     6035 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/analysis/fit/test_models.py
--rw-r--r--   0 root         (0) root         (0)     1020 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/analysis/test_fastbinning.py
--rw-r--r--   0 root         (0) root         (0)     1525 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/analysis/test_gold.py
--rw-r--r--   0 root         (0) root         (0)     5228 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/analysis/test_image.py
--rw-r--r--   0 root         (0) root         (0)     3909 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/analysis/test_image_savgol.py
--rw-r--r--   0 root         (0) root         (0)     3126 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/analysis/test_interpolate.py
--rw-r--r--   0 root         (0) root         (0)     1513 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/analysis/test_kspace.py
--rw-r--r--   0 root         (0) root         (0)      718 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/analysis/test_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.424651 erlab-2.5.2/tests/interactive/
--rw-r--r--   0 root         (0) root         (0)     4374 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/interactive/test_imagetool.py
--rw-r--r--   0 root         (0) root         (0)     4352 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/interactive/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.424651 erlab-2.5.2/tests/io/
--rw-r--r--   0 root         (0) root         (0)    10032 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/io/test_dataloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 02:14:48.424651 erlab-2.5.2/tests/plotting/
--rw-r--r--   0 root         (0) root         (0)     1305 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/plotting/test_annotations.py
--rw-r--r--   0 root         (0) root         (0)     1400 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/plotting/test_atoms.py
--rw-r--r--   0 root         (0) root         (0)     2015 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/plotting/test_colors.py
--rw-r--r--   0 root         (0) root         (0)     2642 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/plotting/test_general.py
--rw-r--r--   0 root         (0) root         (0)      295 2024-05-16 02:14:39.000000 erlab-2.5.2/tests/test_constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.476373 erlab-2.5.3/
+-rw-r--r--   0 root         (0) root         (0)       74 2024-05-22 08:42:58.000000 erlab-2.5.3/.codecov.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.428373 erlab-2.5.3/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.436373 erlab-2.5.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)     2200 2024-05-22 08:42:58.000000 erlab-2.5.3/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-22 08:42:58.000000 erlab-2.5.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-22 08:42:58.000000 erlab-2.5.3/.github/ISSUE_TEMPLATE/feature-request.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.436373 erlab-2.5.3/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1668 2024-05-22 08:42:58.000000 erlab-2.5.3/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     2535 2024-05-22 08:42:58.000000 erlab-2.5.3/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-05-22 08:42:58.000000 erlab-2.5.3/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1022 2024-05-22 08:42:58.000000 erlab-2.5.3/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      793 2024-05-22 08:42:58.000000 erlab-2.5.3/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)   129359 2024-05-22 08:43:03.000000 erlab-2.5.3/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-05-22 08:42:58.000000 erlab-2.5.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    48973 2024-05-22 08:43:07.476373 erlab-2.5.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-05-22 08:42:58.000000 erlab-2.5.3/PythonInterface.ipf
+-rw-r--r--   0 root         (0) root         (0)     5552 2024-05-22 08:42:58.000000 erlab-2.5.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.436373 erlab-2.5.3/docs/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      726 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      804 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.440373 erlab-2.5.3/docs/source/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/bibliography.rst
+-rw-r--r--   0 root         (0) root         (0)    18220 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)    15203 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/erlab.accessors.rst
+-rw-r--r--   0 root         (0) root         (0)      101 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/erlab.analysis.rst
+-rw-r--r--   0 root         (0) root         (0)      485 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/erlab.constants.rst
+-rw-r--r--   0 root         (0) root         (0)      116 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/erlab.interactive.rst
+-rw-r--r--   0 root         (0) root         (0)       81 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/erlab.io.rst
+-rw-r--r--   0 root         (0) root         (0)      236 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/erlab.lattice.rst
+-rw-r--r--   0 root         (0) root         (0)      224 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/erlab.parallel.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/erlab.plotting.rst
+-rw-r--r--   0 root         (0) root         (0)     5039 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/getting-started.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.448373 erlab-2.5.3/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)   328062 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/images/flowchart_multiple.pdf
+-rw-r--r--   0 root         (0) root         (0)   328737 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/images/flowchart_single.pdf
+-rw-r--r--   0 root         (0) root         (0)   996803 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/images/imagetool_dark.png
+-rw-r--r--   0 root         (0) root         (0)   966547 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/images/imagetool_light.png
+-rw-r--r--   0 root         (0) root         (0)   709231 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/images/ktool_1_dark.png
+-rw-r--r--   0 root         (0) root         (0)   694078 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/images/ktool_1_light.png
+-rw-r--r--   0 root         (0) root         (0)   703343 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/images/ktool_2_dark.png
+-rw-r--r--   0 root         (0) root         (0)   686688 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/images/ktool_2_light.png
+-rw-r--r--   0 root         (0) root         (0)     3119 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.448373 erlab-2.5.3/docs/source/pyplots/
+-rw-r--r--   0 root         (0) root         (0)     2604 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/pyplots/norms.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     3099 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/refs.bib
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.452373 erlab-2.5.3/docs/source/user-guide/
+-rw-r--r--   0 root         (0) root         (0)    42435 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/user-guide/curve-fitting.ipynb
+-rw-r--r--   0 root         (0) root         (0)     2598 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/user-guide/imagetool.rst
+-rw-r--r--   0 root         (0) root         (0)     1291 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/user-guide/index.rst
+-rw-r--r--   0 root         (0) root         (0)    12039 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/user-guide/indexing.ipynb
+-rw-r--r--   0 root         (0) root         (0)    54817 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/user-guide/io.ipynb
+-rw-r--r--   0 root         (0) root         (0)    10710 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/user-guide/kconv.ipynb
+-rw-r--r--   0 root         (0) root         (0)    27572 2024-05-22 08:42:58.000000 erlab-2.5.3/docs/source/user-guide/plotting.ipynb
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-22 08:42:58.000000 erlab-2.5.3/environment.yml
+-rw-r--r--   0 root         (0) root         (0)     5938 2024-05-22 08:42:58.000000 erlab-2.5.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      299 2024-05-22 08:42:58.000000 erlab-2.5.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 08:43:07.476373 erlab-2.5.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.432373 erlab-2.5.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.452373 erlab-2.5.3/src/erlab/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-22 08:43:03.000000 erlab-2.5.3/src/erlab/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.452373 erlab-2.5.3/src/erlab/accessors/
+-rw-r--r--   0 root         (0) root         (0)      897 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/accessors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26366 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/accessors/fit.py
+-rw-r--r--   0 root         (0) root         (0)    30007 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/accessors/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    14898 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/accessors/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.456373 erlab-2.5.3/src/erlab/analysis/
+-rw-r--r--   0 root         (0) root         (0)      880 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5322 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/analysis/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.456373 erlab-2.5.3/src/erlab/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/analysis/fit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.456373 erlab-2.5.3/src/erlab/analysis/fit/functions/
+-rw-r--r--   0 root         (0) root         (0)      957 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/analysis/fit/functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10779 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/analysis/fit/functions/dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     9594 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/analysis/fit/functions/general.py
+-rw-r--r--   0 root         (0) root         (0)     6905 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/analysis/fit/minuit.py
+-rw-r--r--   0 root         (0) root         (0)    12774 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/analysis/fit/models.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/analysis/fit/spline.py
+-rw-r--r--   0 root         (0) root         (0)    20223 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/analysis/gold.py
+-rw-r--r--   0 root         (0) root         (0)    27520 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/analysis/image.py
+-rw-r--r--   0 root         (0) root         (0)    14968 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/analysis/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/analysis/kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.456373 erlab-2.5.3/src/erlab/analysis/mask/
+-rw-r--r--   0 root         (0) root         (0)     5397 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/analysis/mask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8505 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/analysis/mask/polygon.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/analysis/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5443 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/analysis/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.456373 erlab-2.5.3/src/erlab/characterization/
+-rw-r--r--   0 root         (0) root         (0)      232 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.460373 erlab-2.5.3/src/erlab/interactive/
+-rw-r--r--   0 root         (0) root         (0)      725 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14181 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/bzplot.py
+-rw-r--r--   0 root         (0) root         (0)    21371 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/colors.py
+-rw-r--r--   0 root         (0) root         (0)    23038 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/curvefittingtool.py
+-rw-r--r--   0 root         (0) root         (0)    11816 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/derivative.py
+-rw-r--r--   0 root         (0) root         (0)    16300 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/dtool.ui
+-rw-r--r--   0 root         (0) root         (0)    19376 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/fermiedge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.460373 erlab-2.5.3/src/erlab/interactive/imagetool/
+-rw-r--r--   0 root         (0) root         (0)    17433 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/imagetool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.460373 erlab-2.5.3/src/erlab/interactive/imagetool/_deprecated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/imagetool/_deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52053 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
+-rw-r--r--   0 root         (0) root         (0)   114641 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
+-rw-r--r--   0 root         (0) root         (0)    27909 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/imagetool/controls.py
+-rw-r--r--   0 root         (0) root         (0)    57841 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/imagetool/core.py
+-rw-r--r--   0 root         (0) root         (0)    14551 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/imagetool/fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)    25642 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/imagetool/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    16014 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    19321 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/ktool.ui
+-rw-r--r--   0 root         (0) root         (0)     2749 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/masktool.py
+-rw-r--r--   0 root         (0) root         (0)    56647 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/interactive/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.464373 erlab-2.5.3/src/erlab/io/
+-rw-r--r--   0 root         (0) root         (0)     2194 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.464373 erlab-2.5.3/src/erlab/io/characterization/
+-rw-r--r--   0 root         (0) root         (0)      170 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/io/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/io/characterization/resistance.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/io/characterization/xrd.py
+-rw-r--r--   0 root         (0) root         (0)    43727 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/io/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)    12460 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/io/exampledata.py
+-rw-r--r--   0 root         (0) root         (0)     6998 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/io/igor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.464373 erlab-2.5.3/src/erlab/io/plugins/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/io/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3811 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/io/plugins/da30.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/io/plugins/kriss.py
+-rw-r--r--   0 root         (0) root         (0)     6974 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/io/plugins/maestro.py
+-rw-r--r--   0 root         (0) root         (0)     8167 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/io/plugins/merlin.py
+-rw-r--r--   0 root         (0) root         (0)     7667 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/io/plugins/ssrl52.py
+-rw-r--r--   0 root         (0) root         (0)     7123 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/io/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2528 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/lattice.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.468373 erlab-2.5.3/src/erlab/plotting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.468373 erlab-2.5.3/src/erlab/plotting/IgorCT/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/IgorCT/Blue-White.txt
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/IgorCT/BlueHot.ibw
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/IgorCT/ColdWarm.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/IgorCT/PlanetEarth.ibw
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/IgorCT/ametrine.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/IgorCT/isolum.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/IgorCT/morgenstemning.ibw
+-rw-r--r--   0 root         (0) root         (0)     2113 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30848 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/annotations.py
+-rw-r--r--   0 root         (0) root         (0)    18686 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/atoms.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/bz.py
+-rw-r--r--   0 root         (0) root         (0)    39811 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/colors.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/erplot.py
+-rw-r--r--   0 root         (0) root         (0)    38540 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/general.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/plot3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.468373 erlab-2.5.3/src/erlab/plotting/stylelib/
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/stylelib/fira.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/stylelib/firalight.mplstyle
+-rw-r--r--   0 root         (0) root         (0)    14358 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/stylelib/khan.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/stylelib/nature.mplstyle
+-rw-r--r--   0 root         (0) root         (0)      630 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/stylelib/poster.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-05-22 08:42:58.000000 erlab-2.5.3/src/erlab/plotting/stylelib/times.mplstyle
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.476373 erlab-2.5.3/src/erlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    48973 2024-05-22 08:43:07.000000 erlab-2.5.3/src/erlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5297 2024-05-22 08:43:07.000000 erlab-2.5.3/src/erlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 08:43:07.000000 erlab-2.5.3/src/erlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      667 2024-05-22 08:43:07.000000 erlab-2.5.3/src/erlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-22 08:43:07.000000 erlab-2.5.3/src/erlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.472373 erlab-2.5.3/templates/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-05-22 08:42:58.000000 erlab-2.5.3/templates/.macros.j2
+-rw-r--r--   0 root         (0) root         (0)      161 2024-05-22 08:42:58.000000 erlab-2.5.3/templates/.release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)      423 2024-05-22 08:42:58.000000 erlab-2.5.3/templates/CHANGELOG.md.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.472373 erlab-2.5.3/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.472373 erlab-2.5.3/tests/accessors/
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/accessors/test_fit.py
+-rw-r--r--   0 root         (0) root         (0)     4150 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/accessors/test_kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.472373 erlab-2.5.3/tests/analysis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.472373 erlab-2.5.3/tests/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)     4497 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/analysis/fit/test_functions_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     4794 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/analysis/fit/test_functions_general.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/analysis/fit/test_minuit.py
+-rw-r--r--   0 root         (0) root         (0)     6035 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/analysis/fit/test_models.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/analysis/test_fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/analysis/test_gold.py
+-rw-r--r--   0 root         (0) root         (0)     5228 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/analysis/test_image.py
+-rw-r--r--   0 root         (0) root         (0)     3909 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/analysis/test_image_savgol.py
+-rw-r--r--   0 root         (0) root         (0)     3126 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/analysis/test_interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/analysis/test_kspace.py
+-rw-r--r--   0 root         (0) root         (0)      718 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/analysis/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.472373 erlab-2.5.3/tests/interactive/
+-rw-r--r--   0 root         (0) root         (0)     4374 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/interactive/test_imagetool.py
+-rw-r--r--   0 root         (0) root         (0)     4352 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/interactive/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.472373 erlab-2.5.3/tests/io/
+-rw-r--r--   0 root         (0) root         (0)    10032 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/io/test_dataloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:43:07.476373 erlab-2.5.3/tests/plotting/
+-rw-r--r--   0 root         (0) root         (0)     1305 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/plotting/test_annotations.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/plotting/test_atoms.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/plotting/test_colors.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/plotting/test_general.py
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-22 08:42:58.000000 erlab-2.5.3/tests/test_constants.py
```

### Comparing `erlab-2.5.2/.github/ISSUE_TEMPLATE/bug-report.yml` & `erlab-2.5.3/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/.github/ISSUE_TEMPLATE/feature-request.yml` & `erlab-2.5.3/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/.github/workflows/pr.yml` & `erlab-2.5.3/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/.github/workflows/release.yml` & `erlab-2.5.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/.gitignore` & `erlab-2.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/.pre-commit-config.yaml` & `erlab-2.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/.readthedocs.yaml` & `erlab-2.5.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/CHANGELOG.md` & `erlab-2.5.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 # CHANGELOG
 
 
 
+## v2.5.3 (2024-05-22)
+
+### Fix
+
+* (**io.utilities**) `get_files` now only list files, not directories ([`60f9230`](https://github.com/kmnhan/erlabpy/commit/60f92307f94484361e0ba11b10a52be4c4cc05a1))
+
+* (**accessors.fit**) add `make_params` call before determining param names, closes #38 ([`f1d161d`](https://github.com/kmnhan/erlabpy/commit/f1d161de089b93e16b2947b126ac075764d98f75))
+
+* (**analysis.fit**) make some models more robust to DataArray input ([`afe5ddd`](https://github.com/kmnhan/erlabpy/commit/afe5ddd9d1e6796ba0261a147c2733d607916d81))
+
+### Refactor
+
+* add loader for ALS BL7 MAESTRO `.h5` files ([`4f33402`](https://github.com/kmnhan/erlabpy/commit/4f3340228ae2e1cbd8baf57d5d426043f5e28688))
+
+* (**interactive**) add informative error message for missing Qt bindings ([`560615b`](https://github.com/kmnhan/erlabpy/commit/560615bb89d2646965d1a2a967133f0df08e3f6e))
+
+* (**io**) rename some internal variables and reorder ([`76fe284`](https://github.com/kmnhan/erlabpy/commit/76fe284b4bc9f1e0c3cb94857a65599b07ee04df))
+
+  Also added a check for astropy in FITS file related utility.
+
+
 ## v2.5.2 (2024-05-16)
 
 ### Ci
 
 * (**github**) re-enable parallel tests and tweak coverage ([`0fd910f`](https://github.com/kmnhan/erlabpy/commit/0fd910f63d576942fbf8d66d71c468b00157ca19))
 
 * (**github**) disable `.pyc` generation ([`54c7dd1`](https://github.com/kmnhan/erlabpy/commit/54c7dd1262db8fc3744cc154fe434672d2a7313b))
```

### Comparing `erlab-2.5.2/LICENSE` & `erlab-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/PKG-INFO` & `erlab-2.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.5.2
+Version: 2.5.3
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `erlab-2.5.2/PythonInterface.ipf` & `erlab-2.5.3/PythonInterface.ipf`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/README.md` & `erlab-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/Makefile` & `erlab-2.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/environment.yml` & `erlab-2.5.3/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/make.bat` & `erlab-2.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/conf.py` & `erlab-2.5.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/contributing.rst` & `erlab-2.5.3/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/getting-started.rst` & `erlab-2.5.3/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/images/flowchart_multiple.pdf` & `erlab-2.5.3/docs/source/images/flowchart_multiple.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/images/flowchart_single.pdf` & `erlab-2.5.3/docs/source/images/flowchart_single.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/images/imagetool_dark.png` & `erlab-2.5.3/docs/source/images/imagetool_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/images/imagetool_light.png` & `erlab-2.5.3/docs/source/images/imagetool_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/images/ktool_1_dark.png` & `erlab-2.5.3/docs/source/images/ktool_1_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/images/ktool_1_light.png` & `erlab-2.5.3/docs/source/images/ktool_1_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/images/ktool_2_dark.png` & `erlab-2.5.3/docs/source/images/ktool_2_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/images/ktool_2_light.png` & `erlab-2.5.3/docs/source/images/ktool_2_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/index.rst` & `erlab-2.5.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/pyplots/norms.py` & `erlab-2.5.3/docs/source/pyplots/norms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/reference.rst` & `erlab-2.5.3/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/refs.bib` & `erlab-2.5.3/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/user-guide/curve-fitting.ipynb` & `erlab-2.5.3/docs/source/user-guide/curve-fitting.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/user-guide/imagetool.rst` & `erlab-2.5.3/docs/source/user-guide/imagetool.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/user-guide/index.rst` & `erlab-2.5.3/docs/source/user-guide/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/user-guide/indexing.ipynb` & `erlab-2.5.3/docs/source/user-guide/indexing.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/user-guide/io.ipynb` & `erlab-2.5.3/docs/source/user-guide/io.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/user-guide/kconv.ipynb` & `erlab-2.5.3/docs/source/user-guide/kconv.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/docs/source/user-guide/plotting.ipynb` & `erlab-2.5.3/docs/source/user-guide/plotting.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/pyproject.toml` & `erlab-2.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/accessors/__init__.py` & `erlab-2.5.3/src/erlab/accessors/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/accessors/fit.py` & `erlab-2.5.3/src/erlab/accessors/fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,14 +309,17 @@
         # Broadcast all coords with each other
         coords_ = xr.broadcast(*coords_)
         coords_ = [
             coord.broadcast_like(self._obj, exclude=preserved_dims) for coord in coords_
         ]
         n_coords = len(coords_)
 
+        # Call make_params before getting parameter names as it may add param hints
+        model.make_params()
+
         # Get the parameter names
         param_names: list[str] = model.param_names
         n_params = len(param_names)
 
         # Define the statistics to extract from the fit result
         stat_names = [
             "nfev",
@@ -440,14 +443,16 @@
                     stats = np.array(
                         [
                             s if s is not None else np.nan
                             for s in [getattr(modres, s) for s in stat_names]
                         ]
                     )
 
+                    # Fill in covariance matrix entries, entries for non-varying
+                    # parameters are left as NaN
                     if modres.covar is not None:
                         var_names = modres.var_names
                         for vi in range(modres.nvarys):
                             i = param_names.index(var_names[vi])
                             for vj in range(modres.nvarys):
                                 j = param_names.index(var_names[vj])
                                 pcov[i, j] = modres.covar[vi, vj]
```

### Comparing `erlab-2.5.2/src/erlab/accessors/kspace.py` & `erlab-2.5.3/src/erlab/accessors/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/accessors/utils.py` & `erlab-2.5.3/src/erlab/accessors/utils.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/analysis/__init__.py` & `erlab-2.5.3/src/erlab/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/analysis/correlation.py` & `erlab-2.5.3/src/erlab/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/analysis/fit/functions/__init__.py` & `erlab-2.5.3/src/erlab/analysis/fit/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/analysis/fit/functions/dynamic.py` & `erlab-2.5.3/src/erlab/analysis/fit/functions/dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/analysis/fit/functions/general.py` & `erlab-2.5.3/src/erlab/analysis/fit/functions/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/analysis/fit/minuit.py` & `erlab-2.5.3/src/erlab/analysis/fit/minuit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/analysis/fit/models.py` & `erlab-2.5.3/src/erlab/analysis/fit/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
     def __init__(self, degree=9, **kwargs):
         kwargs.setdefault("name", f"Poly{degree}")
         super().__init__(PolynomialFunction(degree), **kwargs)
 
     def guess(self, data, x=None, **kwargs):
         pars = self.make_params()
         if x is None:
-            pars["c0"].set(value=data.mean())
+            pars["c0"].set(value=float(data.mean()))
             for i in range(1, self.func.degree + 1):
                 pars[f"{self.prefix}c{i}"].set(value=0.0)
         else:
             out = np.polyfit(x, data, self.func.degree)
             for i, coef in enumerate(out[::-1]):
                 pars[f"{self.prefix}c{i}"].set(value=coef)
         return lmfit.models.update_param_vals(pars, self.prefix, **kwargs)
@@ -265,28 +265,28 @@
         if self.func.convolve:
             self.set_param_hint("resolution", min=0.0)
 
     def guess(self, data, x=None, **kwargs):
         pars = self.make_params()
         # !TODO: better guesses
         if self.func.fd:
-            pars[f"{self.prefix}offset"].set(value=data[x >= 0].mean())
+            pars[f"{self.prefix}offset"].set(value=float(data[x >= 0].mean()))
 
         poly1 = PolynomialModel(1).guess(data, x)
         pars[f"{self.prefix}lin_bkg"].set(poly1["c1"].value)
         pars[f"{self.prefix}const_bkg"].set(poly1["c0"].value)
 
         # for i, func in enumerate(self.func.peak_funcs):
         # self.func.peak_argnames
 
-        xrange = x.max() - x.min()
+        xrange = float(x.max() - x.min())
 
         for i in range(self.func.npeaks):  # Number of peaks
             pars[f"{self.prefix}p{i}_center"].set(value=0.0)
-            pars[f"{self.prefix}p{i}_height"].set(value=data.mean())
+            pars[f"{self.prefix}p{i}_height"].set(value=float(data.mean()))
             pars[f"{self.prefix}p{i}_width"].set(value=0.1 * xrange)
 
         return lmfit.models.update_param_vals(pars, self.prefix, **kwargs)
 
     def eval_components(self, params=None, **kwargs):
         key = self._prefix
         if len(key) < 1:
```

### Comparing `erlab-2.5.2/src/erlab/analysis/fit/spline.py` & `erlab-2.5.3/src/erlab/analysis/fit/spline.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/analysis/gold.py` & `erlab-2.5.3/src/erlab/analysis/gold.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/analysis/image.py` & `erlab-2.5.3/src/erlab/analysis/image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/analysis/interpolate.py` & `erlab-2.5.3/src/erlab/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/analysis/kspace.py` & `erlab-2.5.3/src/erlab/analysis/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/analysis/mask/__init__.py` & `erlab-2.5.3/src/erlab/analysis/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/analysis/mask/polygon.py` & `erlab-2.5.3/src/erlab/analysis/mask/polygon.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/analysis/transform.py` & `erlab-2.5.3/src/erlab/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/analysis/utilities.py` & `erlab-2.5.3/src/erlab/analysis/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/constants.py` & `erlab-2.5.3/src/erlab/constants.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/interactive/__init__.py` & `erlab-2.5.3/src/erlab/interactive/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,11 +19,20 @@
    derivative
    utilities
 
 """
 
 __all__ = ["dtool", "goldtool", "itool", "ktool"]
 
+
+try:
+    import qtpy  # noqa: F401
+except ImportError as e:
+    raise ImportError(
+        "A Qt binding is required for interactive tools. "
+        "Please install PySide6 or PyQt6"
+    ) from e
+
 from erlab.interactive.derivative import dtool
 from erlab.interactive.fermiedge import goldtool
 from erlab.interactive.imagetool import itool
 from erlab.interactive.kspace import ktool
```

### Comparing `erlab-2.5.2/src/erlab/interactive/bzplot.py` & `erlab-2.5.3/src/erlab/interactive/bzplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/interactive/colors.py` & `erlab-2.5.3/src/erlab/interactive/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/interactive/curvefittingtool.py` & `erlab-2.5.3/src/erlab/interactive/curvefittingtool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/interactive/derivative.py` & `erlab-2.5.3/src/erlab/interactive/derivative.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/interactive/dtool.ui` & `erlab-2.5.3/src/erlab/interactive/dtool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/interactive/fermiedge.py` & `erlab-2.5.3/src/erlab/interactive/fermiedge.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/interactive/imagetool/__init__.py` & `erlab-2.5.3/src/erlab/interactive/imagetool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from erlab.interactive.imagetool.controls import (
     ItoolBinningControls,
     ItoolColormapControls,
     ItoolCrosshairControls,
 )
 from erlab.interactive.imagetool.core import ImageSlicerArea, SlicerLinkProxy
 from erlab.interactive.utilities import DictMenuBar, copy_to_clipboard
-from erlab.io.plugins.merlin import BL403Loader
+from erlab.io.plugins.merlin import MERLINLoader
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Collection
 
     from erlab.interactive.imagetool.slicer import ArraySlicer
 
 
@@ -435,15 +435,15 @@
     def _copy_cursor_val(self):
         copy_to_clipboard(str(self.slicer_area.array_slicer._values))
 
     def _copy_cursor_idx(self):
         copy_to_clipboard(str(self.slicer_area.array_slicer._indices))
 
     def _open_file(self):
-        merlin_loader = cast(BL403Loader, erlab.io.loaders["merlin"])
+        merlin_loader = cast(MERLINLoader, erlab.io.loaders["merlin"])
         valid_loaders: dict[str, tuple[Callable, dict]] = {
             "xarray HDF5 Files (*.h5)": (erlab.io.load_hdf5, {}),
             "ALS BL4.0.3 Raw Data (*.pxt)": (merlin_loader.load, {}),
             "ALS BL4.0.3 Live (*.ibw)": (merlin_loader.load_live, {}),
             "DA30 Raw Data (*.ibw *.pxt *.zip)": (erlab.io.loaders["da30"].load, {}),
             "SSRL BL5-2 Raw Data (*.h5)": (erlab.io.loaders["ssrl52"].load, {}),
             "NetCDF Files (*.nc *.nc4 *.cdf)": (xr.load_dataarray, {}),
```

### Comparing `erlab-2.5.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py` & `erlab-2.5.3/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py` & `erlab-2.5.3/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/interactive/imagetool/controls.py` & `erlab-2.5.3/src/erlab/interactive/imagetool/controls.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/interactive/imagetool/core.py` & `erlab-2.5.3/src/erlab/interactive/imagetool/core.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/interactive/imagetool/fastbinning.py` & `erlab-2.5.3/src/erlab/interactive/imagetool/fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/interactive/imagetool/slicer.py` & `erlab-2.5.3/src/erlab/interactive/imagetool/slicer.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/interactive/kspace.py` & `erlab-2.5.3/src/erlab/interactive/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/interactive/ktool.ui` & `erlab-2.5.3/src/erlab/interactive/ktool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/interactive/masktool.py` & `erlab-2.5.3/src/erlab/interactive/masktool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/interactive/utilities.py` & `erlab-2.5.3/src/erlab/interactive/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/io/__init__.py` & `erlab-2.5.3/src/erlab/io/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/io/characterization/resistance.py` & `erlab-2.5.3/src/erlab/io/characterization/resistance.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,18 +101,16 @@
         delimiter="\t",
         skip_header=3,
         usecols=[2, 3, 4, 5, 6, 7],
         **kwargs,
     )
     ds = xr.Dataset(
         data_vars={
-            "time": ("temp", data[:, 0]),
-            "res": ("temp", data[:, 2]),
-            "curr": ("temp", data[:, 3]),
-            "temp_err": ("temp", data[:, 4]),
-            "res_err": ("temp", data[:, 5]),
-        },
-        coords={
-            "temp": data[:, 1],
+            "temp": ("time", data[:, 1]),
+            "res": ("time", data[:, 2]),
+            "curr": ("time", data[:, 3]),
+            "temp_err": ("time", data[:, 4]),
+            "res_err": ("time", data[:, 5]),
         },
+        coords={"time": data[:, 0]},
     )
     return ds
```

### Comparing `erlab-2.5.2/src/erlab/io/characterization/xrd.py` & `erlab-2.5.3/src/erlab/io/characterization/xrd.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/io/dataloader.py` & `erlab-2.5.3/src/erlab/io/dataloader.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -877,29 +877,14 @@
                     data_list,
                     dim=next(iter(coord_dict.keys())),
                     coords="different",
                 )
             except:  # noqa: E722
                 return data_list
 
-    def post_process_general(
-        self, data: xr.DataArray | xr.Dataset | list[xr.DataArray]
-    ) -> xr.DataArray | xr.Dataset | list[xr.DataArray]:
-        if isinstance(data, xr.DataArray):
-            return self.post_process(data)
-
-        elif isinstance(data, list):
-            return [self.post_process(d) for d in data]
-
-        elif isinstance(data, xr.Dataset):
-            return xr.Dataset(
-                {k: self.post_process(v) for k, v in data.data_vars.items()},
-                attrs=data.attrs,
-            )
-
     def process_keys(
         self, data: xr.DataArray, key_mapping: dict[str, str] | None = None
     ) -> xr.DataArray:
         if key_mapping is None:
             key_mapping = self.name_map_reversed
 
         # Rename coordinates
@@ -931,14 +916,29 @@
         data = self.process_keys(data)
         data = data.assign_attrs(
             self.additional_attrs | {"data_loader_name": str(self.name)}
         )
         data = data.assign_coords(self.additional_coords)
         return data
 
+    def post_process_general(
+        self, data: xr.DataArray | xr.Dataset | list[xr.DataArray]
+    ) -> xr.DataArray | xr.Dataset | list[xr.DataArray]:
+        if isinstance(data, xr.DataArray):
+            return self.post_process(data)
+
+        elif isinstance(data, list):
+            return [self.post_process(d) for d in data]
+
+        elif isinstance(data, xr.Dataset):
+            return xr.Dataset(
+                {k: self.post_process(v) for k, v in data.data_vars.items()},
+                attrs=data.attrs,
+            )
+
     @classmethod
     def validate(
         cls, data: xr.DataArray | xr.Dataset | list[xr.DataArray | xr.Dataset]
     ) -> None:
         """Validate the input data to ensure it is in the correct format.
 
         Checks for the presence of all required coordinates and attributes. If the data
```

### Comparing `erlab-2.5.2/src/erlab/io/exampledata.py` & `erlab-2.5.3/src/erlab/io/exampledata.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/io/igor.py` & `erlab-2.5.3/src/erlab/io/igor.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/io/plugins/__init__.py` & `erlab-2.5.3/src/erlab/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/io/plugins/da30.py` & `erlab-2.5.3/src/erlab/io/plugins/da30.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/io/plugins/kriss.py` & `erlab-2.5.3/src/erlab/io/plugins/kriss.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/io/plugins/merlin.py` & `erlab-2.5.3/src/erlab/io/plugins/merlin.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import xarray as xr
 
 import erlab.io.utilities
 from erlab.io.dataloader import LoaderBase
 from erlab.io.igor import load_experiment, load_wave
 
 
-class BL403Loader(LoaderBase):
+class MERLINLoader(LoaderBase):
     name = "merlin"
 
     aliases = ("ALS_BL4", "als_bl4", "BL403", "bl403")
 
     name_map: ClassVar[dict] = {
         "alpha": "deg",
         "beta": ["Polar", "Polar Compens"],
```

### Comparing `erlab-2.5.2/src/erlab/io/plugins/ssrl52.py` & `erlab-2.5.3/src/erlab/io/plugins/ssrl52.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/io/utilities.py` & `erlab-2.5.3/src/erlab/io/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     "load_hdf5",
     "open_hdf5",
     "save_as_hdf5",
     "save_as_netcdf",
     "showfitsinfo",
 ]
 
+import importlib.util
 import os
 import warnings
 from collections.abc import Sequence
 
 import numpy as np
 import numpy.typing as npt
 import xarray as xr
@@ -21,32 +22,37 @@
 
     Parameters
     ----------
     path
         Local path to ``.fits`` file.
 
     """
+    if not importlib.util.find_spec("astropy"):
+        raise ImportError("`astropy` needs to be installed to handle FITS files")
+
     from astropy.io import fits
 
     with fits.open(path, ignore_missing_end=True) as hdul:
         hdul.verify("silentfix+warn")
         hdul.info()
         for i in range(len(hdul)):
             # print(f'\nColumns in {i:d}: {hdul[i].columns.names!r}')
             print(f"\nHeaders in {i:d}:\n{hdul[i].header!r}")
 
 
 def get_files(
     directory,
-    extensions: Sequence[str] | None = None,
+    extensions: Sequence[str] | str | None = None,
     contains: str | None = None,
     notcontains: str | None = None,
 ) -> list[str]:
     """Return a list of files in a directory with the given extensions.
 
+    Directories are ignored.
+
     Parameters
     ----------
     directory
         Target directory.
     extensions
         List of extensions to filter for. If not provided, all files are returned.
     contains
@@ -58,17 +64,24 @@
     -------
     files : list of str
         List of files in the directory.
 
     """
     files = []
 
+    if isinstance(extensions, str):
+        extensions = [extensions]
+
     for f in os.listdir(directory):
-        if extensions is not None and os.path.splitext(f)[1] not in extensions:
+        if os.path.isdir(os.path.join(directory, f)):
             continue
+        if extensions is not None:
+            ext = os.path.splitext(f)[1]
+            if ext == "" or ext not in extensions:
+                continue
         if contains is not None and contains not in f:
             continue
         if notcontains is not None and notcontains in f:
             continue
         files.append(os.path.join(directory, f))
 
     return files
```

### Comparing `erlab-2.5.2/src/erlab/lattice.py` & `erlab-2.5.3/src/erlab/lattice.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/parallel.py` & `erlab-2.5.3/src/erlab/parallel.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/IgorCT/Blue-White.txt` & `erlab-2.5.3/src/erlab/plotting/IgorCT/Blue-White.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/IgorCT/BlueHot.ibw` & `erlab-2.5.3/src/erlab/plotting/IgorCT/BlueHot.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw` & `erlab-2.5.3/src/erlab/plotting/IgorCT/CTBlueWhite.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw` & `erlab-2.5.3/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw` & `erlab-2.5.3/src/erlab/plotting/IgorCT/CTRedTemperature.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/IgorCT/ColdWarm.ibw` & `erlab-2.5.3/src/erlab/plotting/IgorCT/ColdWarm.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw` & `erlab-2.5.3/src/erlab/plotting/IgorCT/PlanetEarth.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/IgorCT/ametrine.ibw` & `erlab-2.5.3/src/erlab/plotting/IgorCT/ametrine.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/IgorCT/isolum.ibw` & `erlab-2.5.3/src/erlab/plotting/IgorCT/isolum.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/IgorCT/morgenstemning.ibw` & `erlab-2.5.3/src/erlab/plotting/IgorCT/morgenstemning.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/__init__.py` & `erlab-2.5.3/src/erlab/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/annotations.py` & `erlab-2.5.3/src/erlab/plotting/annotations.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/atoms.py` & `erlab-2.5.3/src/erlab/plotting/atoms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/bz.py` & `erlab-2.5.3/src/erlab/plotting/bz.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/colors.py` & `erlab-2.5.3/src/erlab/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/erplot.py` & `erlab-2.5.3/src/erlab/plotting/erplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/general.py` & `erlab-2.5.3/src/erlab/plotting/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/plot3d.py` & `erlab-2.5.3/src/erlab/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/stylelib/fira.mplstyle` & `erlab-2.5.3/src/erlab/plotting/stylelib/fira.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/stylelib/firalight.mplstyle` & `erlab-2.5.3/src/erlab/plotting/stylelib/firalight.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/stylelib/khan.mplstyle` & `erlab-2.5.3/src/erlab/plotting/stylelib/khan.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/stylelib/nature.mplstyle` & `erlab-2.5.3/src/erlab/plotting/stylelib/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/stylelib/poster.mplstyle` & `erlab-2.5.3/src/erlab/plotting/stylelib/poster.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab/plotting/stylelib/times.mplstyle` & `erlab-2.5.3/src/erlab/plotting/stylelib/times.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/src/erlab.egg-info/PKG-INFO` & `erlab-2.5.3/src/erlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.5.2
+Version: 2.5.3
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `erlab-2.5.2/src/erlab.egg-info/SOURCES.txt` & `erlab-2.5.3/src/erlab.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 src/erlab/io/utilities.py
 src/erlab/io/characterization/__init__.py
 src/erlab/io/characterization/resistance.py
 src/erlab/io/characterization/xrd.py
 src/erlab/io/plugins/__init__.py
 src/erlab/io/plugins/da30.py
 src/erlab/io/plugins/kriss.py
+src/erlab/io/plugins/maestro.py
 src/erlab/io/plugins/merlin.py
 src/erlab/io/plugins/ssrl52.py
 src/erlab/plotting/__init__.py
 src/erlab/plotting/annotations.py
 src/erlab/plotting/atoms.py
 src/erlab/plotting/bz.py
 src/erlab/plotting/colors.py
```

### Comparing `erlab-2.5.2/src/erlab.egg-info/requires.txt` & `erlab-2.5.3/src/erlab.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/templates/.macros.j2` & `erlab-2.5.3/templates/.macros.j2`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/accessors/test_fit.py` & `erlab-2.5.3/tests/accessors/test_fit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/accessors/test_kspace.py` & `erlab-2.5.3/tests/accessors/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/analysis/fit/test_functions_dynamic.py` & `erlab-2.5.3/tests/analysis/fit/test_functions_dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/analysis/fit/test_functions_general.py` & `erlab-2.5.3/tests/analysis/fit/test_functions_general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/analysis/fit/test_minuit.py` & `erlab-2.5.3/tests/analysis/fit/test_minuit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/analysis/fit/test_models.py` & `erlab-2.5.3/tests/analysis/fit/test_models.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/analysis/test_fastbinning.py` & `erlab-2.5.3/tests/analysis/test_fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/analysis/test_gold.py` & `erlab-2.5.3/tests/analysis/test_gold.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/analysis/test_image.py` & `erlab-2.5.3/tests/analysis/test_image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/analysis/test_image_savgol.py` & `erlab-2.5.3/tests/analysis/test_image_savgol.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/analysis/test_interpolate.py` & `erlab-2.5.3/tests/analysis/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/analysis/test_kspace.py` & `erlab-2.5.3/tests/analysis/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/analysis/test_utilities.py` & `erlab-2.5.3/tests/analysis/test_utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/interactive/test_imagetool.py` & `erlab-2.5.3/tests/interactive/test_imagetool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/interactive/test_tools.py` & `erlab-2.5.3/tests/interactive/test_tools.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/io/test_dataloader.py` & `erlab-2.5.3/tests/io/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/plotting/test_annotations.py` & `erlab-2.5.3/tests/plotting/test_annotations.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/plotting/test_atoms.py` & `erlab-2.5.3/tests/plotting/test_atoms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/plotting/test_colors.py` & `erlab-2.5.3/tests/plotting/test_colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.2/tests/plotting/test_general.py` & `erlab-2.5.3/tests/plotting/test_general.py`

 * *Files identical despite different names*

