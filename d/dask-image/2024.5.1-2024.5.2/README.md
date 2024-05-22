# Comparing `tmp/dask_image-2024.5.1.tar.gz` & `tmp/dask_image-2024.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask_image-2024.5.1.tar", last modified: Tue May 21 04:35:59 2024, max compression
+gzip compressed data, was "dask_image-2024.5.2.tar", last modified: Tue May 21 06:41:02 2024, max compression
```

## Comparing `dask_image-2024.5.1.tar` & `dask_image-2024.5.2.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.901791 dask_image-2024.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-21 04:35:50.000000 dask_image-2024.5.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 04:35:50.000000 dask_image-2024.5.1/.coveralls.yml
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-21 04:35:50.000000 dask_image-2024.5.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-21 04:35:50.000000 dask_image-2024.5.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.885791 dask_image-2024.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-21 04:35:50.000000 dask_image-2024.5.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-21 04:35:50.000000 dask_image-2024.5.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-21 04:35:50.000000 dask_image-2024.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.885791 dask_image-2024.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-21 04:35:50.000000 dask_image-2024.5.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-21 04:35:50.000000 dask_image-2024.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-21 04:35:50.000000 dask_image-2024.5.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-21 04:35:50.000000 dask_image-2024.5.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-05-21 04:35:50.000000 dask_image-2024.5.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    24469 2024-05-21 04:35:50.000000 dask_image-2024.5.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-21 04:35:50.000000 dask_image-2024.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-21 04:35:50.000000 dask_image-2024.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-21 04:35:50.000000 dask_image-2024.5.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-21 04:35:59.901791 dask_image-2024.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-21 04:35:50.000000 dask_image-2024.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.885791 dask_image-2024.5.1/continuous_integration/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-21 04:35:50.000000 dask_image-2024.5.1/continuous_integration/environment-3.10.yml
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-21 04:35:50.000000 dask_image-2024.5.1/continuous_integration/environment-3.11.yml
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-21 04:35:50.000000 dask_image-2024.5.1/continuous_integration/environment-3.12.yml
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-21 04:35:50.000000 dask_image-2024.5.1/continuous_integration/environment-3.9.yml
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-21 04:35:50.000000 dask_image-2024.5.1/continuous_integration/environment-doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-21 04:35:50.000000 dask_image-2024.5.1/continuous_integration/environment-latest.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.885791 dask_image-2024.5.1/continuous_integration/gpuci/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-21 04:35:50.000000 dask_image-2024.5.1/continuous_integration/gpuci/axis.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-21 04:35:50.000000 dask_image-2024.5.1/continuous_integration/gpuci/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.885791 dask_image-2024.5.1/dask_image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-21 04:35:59.000000 dask_image-2024.5.1/dask_image/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.889791 dask_image-2024.5.1/dask_image/dispatch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/dispatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/dispatch/_dispatch_ndfilters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/dispatch/_dispatch_ndinterp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/dispatch/_dispatch_ndmorph.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/dispatch/_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/dispatch/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.889791 dask_image-2024.5.1/dask_image/imread/
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/imread/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.889791 dask_image-2024.5.1/dask_image/ndfilters/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndfilters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndfilters/_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndfilters/_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndfilters/_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndfilters/_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndfilters/_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndfilters/_order.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndfilters/_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndfilters/_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndfilters/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.889791 dask_image-2024.5.1/dask_image/ndfourier/
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndfourier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndfourier/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.889791 dask_image-2024.5.1/dask_image/ndinterp/
--rw-r--r--   0 runner    (1001) docker     (127)    17746 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndinterp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.889791 dask_image-2024.5.1/dask_image/ndmeasure/
--rw-r--r--   0 runner    (1001) docker     (127)    24228 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndmeasure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.889791 dask_image-2024.5.1/dask_image/ndmeasure/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndmeasure/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndmeasure/_utils/_find_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndmeasure/_utils/_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.893791 dask_image-2024.5.1/dask_image/ndmorph/
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndmorph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndmorph/_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-21 04:35:50.000000 dask_image-2024.5.1/dask_image/ndmorph/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.897791 dask_image-2024.5.1/dask_image.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-21 04:35:59.000000 dask_image-2024.5.1/dask_image.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-21 04:35:59.000000 dask_image-2024.5.1/dask_image.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 04:35:59.000000 dask_image-2024.5.1/dask_image.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 04:35:59.000000 dask_image-2024.5.1/dask_image.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-21 04:35:59.000000 dask_image-2024.5.1/dask_image.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 04:35:59.000000 dask_image-2024.5.1/dask_image.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.893791 dask_image-2024.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-21 04:35:50.000000 dask_image-2024.5.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 04:35:50.000000 dask_image-2024.5.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 04:35:50.000000 dask_image-2024.5.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     9205 2024-05-21 04:35:50.000000 dask_image-2024.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 04:35:50.000000 dask_image-2024.5.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-21 04:35:50.000000 dask_image-2024.5.1/docs/coverage.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 04:35:50.000000 dask_image-2024.5.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-21 04:35:50.000000 dask_image-2024.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-21 04:35:50.000000 dask_image-2024.5.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-05-21 04:35:50.000000 dask_image-2024.5.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-21 04:35:50.000000 dask_image-2024.5.1/docs/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.893791 dask_image-2024.5.1/docs/release/
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-05-21 04:35:50.000000 dask_image-2024.5.1/docs/release/generate_release_notes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-21 04:35:50.000000 dask_image-2024.5.1/docs/release/release_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-21 04:35:50.000000 dask_image-2024.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 04:35:59.901791 dask_image-2024.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.893791 dask_image-2024.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.881791 dask_image-2024.5.1/tests/test_dask_image/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.893791 dask_image-2024.5.1/tests/test_dask_image/test_imread/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_imread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_imread/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_imread/test_cupy_imread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.897791 dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test__conv.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test__diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test__edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test__gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test__generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test__order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test__smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test__threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test__utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test_cupy_ndfilters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test_cupy_threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.897791 dask_image-2024.5.1/tests/test_dask_image/test_ndfourier/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndfourier/test__utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndfourier/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.897791 dask_image-2024.5.1/tests/test_dask_image/test_ndinterp/
--rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndinterp/test_affine_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndinterp/test_rotate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndinterp/test_spline_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.897791 dask_image-2024.5.1/tests/test_dask_image/test_ndmeasure/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndmeasure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndmeasure/test__utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26183 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndmeasure/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndmeasure/test_find_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 04:35:59.897791 dask_image-2024.5.1/tests/test_dask_image/test_ndmorph/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndmorph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndmorph/test__utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndmorph/test_cupy_ndmorph.py
--rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-05-21 04:35:50.000000 dask_image-2024.5.1/tests/test_dask_image/test_ndmorph/test_ndmorph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.615897 dask_image-2024.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-21 06:40:53.000000 dask_image-2024.5.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 06:40:53.000000 dask_image-2024.5.2/.coveralls.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-21 06:40:53.000000 dask_image-2024.5.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-21 06:40:53.000000 dask_image-2024.5.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.599897 dask_image-2024.5.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-21 06:40:53.000000 dask_image-2024.5.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-21 06:40:53.000000 dask_image-2024.5.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-21 06:40:53.000000 dask_image-2024.5.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.599897 dask_image-2024.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-21 06:40:53.000000 dask_image-2024.5.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-21 06:40:53.000000 dask_image-2024.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-21 06:40:53.000000 dask_image-2024.5.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-21 06:40:53.000000 dask_image-2024.5.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-05-21 06:40:53.000000 dask_image-2024.5.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    24469 2024-05-21 06:40:53.000000 dask_image-2024.5.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-21 06:40:53.000000 dask_image-2024.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-21 06:40:53.000000 dask_image-2024.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-21 06:40:53.000000 dask_image-2024.5.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-21 06:41:02.615897 dask_image-2024.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-21 06:40:53.000000 dask_image-2024.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.599897 dask_image-2024.5.2/continuous_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-21 06:40:53.000000 dask_image-2024.5.2/continuous_integration/environment-3.10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-21 06:40:53.000000 dask_image-2024.5.2/continuous_integration/environment-3.11.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-21 06:40:53.000000 dask_image-2024.5.2/continuous_integration/environment-3.12.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-21 06:40:53.000000 dask_image-2024.5.2/continuous_integration/environment-3.9.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-21 06:40:53.000000 dask_image-2024.5.2/continuous_integration/environment-doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-21 06:40:53.000000 dask_image-2024.5.2/continuous_integration/environment-latest.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.599897 dask_image-2024.5.2/continuous_integration/gpuci/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-21 06:40:53.000000 dask_image-2024.5.2/continuous_integration/gpuci/axis.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-21 06:40:53.000000 dask_image-2024.5.2/continuous_integration/gpuci/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.599897 dask_image-2024.5.2/dask_image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-21 06:41:02.000000 dask_image-2024.5.2/dask_image/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.603897 dask_image-2024.5.2/dask_image/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/dispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/dispatch/_dispatch_ndfilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/dispatch/_dispatch_ndinterp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/dispatch/_dispatch_ndmorph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/dispatch/_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/dispatch/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.603897 dask_image-2024.5.2/dask_image/imread/
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/imread/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.603897 dask_image-2024.5.2/dask_image/ndfilters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndfilters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndfilters/_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndfilters/_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndfilters/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndfilters/_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndfilters/_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndfilters/_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndfilters/_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndfilters/_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndfilters/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.603897 dask_image-2024.5.2/dask_image/ndfourier/
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndfourier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndfourier/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.603897 dask_image-2024.5.2/dask_image/ndinterp/
+-rw-r--r--   0 runner    (1001) docker     (127)    17746 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndinterp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.603897 dask_image-2024.5.2/dask_image/ndmeasure/
+-rw-r--r--   0 runner    (1001) docker     (127)    24228 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndmeasure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.603897 dask_image-2024.5.2/dask_image/ndmeasure/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndmeasure/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndmeasure/_utils/_find_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndmeasure/_utils/_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.603897 dask_image-2024.5.2/dask_image/ndmorph/
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndmorph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndmorph/_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-21 06:40:53.000000 dask_image-2024.5.2/dask_image/ndmorph/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.611897 dask_image-2024.5.2/dask_image.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-21 06:41:02.000000 dask_image-2024.5.2/dask_image.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-21 06:41:02.000000 dask_image-2024.5.2/dask_image.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 06:41:02.000000 dask_image-2024.5.2/dask_image.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 06:41:02.000000 dask_image-2024.5.2/dask_image.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-21 06:41:02.000000 dask_image-2024.5.2/dask_image.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 06:41:02.000000 dask_image-2024.5.2/dask_image.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.607897 dask_image-2024.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-21 06:40:53.000000 dask_image-2024.5.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 06:40:53.000000 dask_image-2024.5.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 06:40:53.000000 dask_image-2024.5.2/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9205 2024-05-21 06:40:53.000000 dask_image-2024.5.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 06:40:53.000000 dask_image-2024.5.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-21 06:40:53.000000 dask_image-2024.5.2/docs/coverage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 06:40:53.000000 dask_image-2024.5.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-21 06:40:53.000000 dask_image-2024.5.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-21 06:40:53.000000 dask_image-2024.5.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-05-21 06:40:53.000000 dask_image-2024.5.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-21 06:40:53.000000 dask_image-2024.5.2/docs/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.607897 dask_image-2024.5.2/docs/release/
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-05-21 06:40:53.000000 dask_image-2024.5.2/docs/release/generate_release_notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-21 06:40:53.000000 dask_image-2024.5.2/docs/release/release_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-21 06:40:53.000000 dask_image-2024.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 06:41:02.615897 dask_image-2024.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.607897 dask_image-2024.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.595897 dask_image-2024.5.2/tests/test_dask_image/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.607897 dask_image-2024.5.2/tests/test_dask_image/test_imread/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_imread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_imread/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_imread/test_cupy_imread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.611897 dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test__conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test__diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test__edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test__gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test__generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test__order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test__smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test__threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test__utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test_cupy_ndfilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test_cupy_threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.611897 dask_image-2024.5.2/tests/test_dask_image/test_ndfourier/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndfourier/test__utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndfourier/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.611897 dask_image-2024.5.2/tests/test_dask_image/test_ndinterp/
+-rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndinterp/test_affine_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndinterp/test_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndinterp/test_spline_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.611897 dask_image-2024.5.2/tests/test_dask_image/test_ndmeasure/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndmeasure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndmeasure/test__utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26183 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndmeasure/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndmeasure/test_find_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:41:02.611897 dask_image-2024.5.2/tests/test_dask_image/test_ndmorph/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndmorph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndmorph/test__utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndmorph/test_cupy_ndmorph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-05-21 06:40:53.000000 dask_image-2024.5.2/tests/test_dask_image/test_ndmorph/test_ndmorph.py
```

### Comparing `dask_image-2024.5.1/.coveragerc` & `dask_image-2024.5.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/.github/workflows/test_and_deploy.yml` & `dask_image-2024.5.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/.gitignore` & `dask_image-2024.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/CONTRIBUTING.rst` & `dask_image-2024.5.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/HISTORY.rst` & `dask_image-2024.5.2/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/LICENSE.txt` & `dask_image-2024.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/Makefile` & `dask_image-2024.5.2/Makefile`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/PKG-INFO` & `dask_image-2024.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-image
-Version: 2024.5.1
+Version: 2024.5.2
 Summary: Distributed image processing
 Author: dask-image contributors. see https://github.com/dask/dask-image/graphs/contributors
 License: BSD-3-Clause
 Project-URL: Homepage, https://image.dask.org
 Project-URL: Issue Tracker, https://github.com/dask/dask-image/issues
 Project-URL: Source Code, https://github.com/dask/dask-image
 Keywords: dask-image,dask,image
```

### Comparing `dask_image-2024.5.1/README.rst` & `dask_image-2024.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/continuous_integration/environment-doc.yml` & `dask_image-2024.5.2/continuous_integration/environment-doc.yml`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/continuous_integration/gpuci/build.sh` & `dask_image-2024.5.2/continuous_integration/gpuci/build.sh`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 . /opt/conda/etc/profile.d/conda.sh
 rapids-mamba-retry env update -n dask_image -f "$WORKSPACE/continuous_integration/environment-$PYTHON_VER.yml"
 
 rapids-logger "Activate conda env"
 conda activate dask_image
 
 rapids-logger "Install cupy"
-python -m pip install cupy-cuda112 -f https://pip.cupy.dev/pre
+python -m pip install cupy-cuda11x -f https://pip.cupy.dev/pre
 
 rapids-logger "Install dask-image"
 python -m pip install .
 
 rapids-logger "Check Python versions"
 python --version
```

### Comparing `dask_image-2024.5.1/dask_image/dispatch/_dispatch_ndfilters.py` & `dask_image-2024.5.2/dask_image/dispatch/_dispatch_ndfilters.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/dispatch/_dispatch_ndinterp.py` & `dask_image-2024.5.2/dask_image/dispatch/_dispatch_ndinterp.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/dispatch/_dispatch_ndmorph.py` & `dask_image-2024.5.2/dask_image/dispatch/_dispatch_ndmorph.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/dispatch/_dispatcher.py` & `dask_image-2024.5.2/dask_image/dispatch/_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/dispatch/_utils.py` & `dask_image-2024.5.2/dask_image/dispatch/_utils.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/imread/__init__.py` & `dask_image-2024.5.2/dask_image/imread/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndfilters/__init__.py` & `dask_image-2024.5.2/dask_image/ndfilters/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndfilters/_conv.py` & `dask_image-2024.5.2/dask_image/ndfilters/_conv.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndfilters/_edge.py` & `dask_image-2024.5.2/dask_image/ndfilters/_edge.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndfilters/_gaussian.py` & `dask_image-2024.5.2/dask_image/ndfilters/_gaussian.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndfilters/_generic.py` & `dask_image-2024.5.2/dask_image/ndfilters/_generic.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndfilters/_order.py` & `dask_image-2024.5.2/dask_image/ndfilters/_order.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndfilters/_smooth.py` & `dask_image-2024.5.2/dask_image/ndfilters/_smooth.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndfilters/_threshold.py` & `dask_image-2024.5.2/dask_image/ndfilters/_threshold.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndfilters/_utils.py` & `dask_image-2024.5.2/dask_image/ndfilters/_utils.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndfourier/__init__.py` & `dask_image-2024.5.2/dask_image/ndfourier/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndfourier/_utils.py` & `dask_image-2024.5.2/dask_image/ndfourier/_utils.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndinterp/__init__.py` & `dask_image-2024.5.2/dask_image/ndinterp/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndmeasure/__init__.py` & `dask_image-2024.5.2/dask_image/ndmeasure/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndmeasure/_utils/__init__.py` & `dask_image-2024.5.2/dask_image/ndmeasure/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndmeasure/_utils/_find_objects.py` & `dask_image-2024.5.2/dask_image/ndmeasure/_utils/_find_objects.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndmeasure/_utils/_label.py` & `dask_image-2024.5.2/dask_image/ndmeasure/_utils/_label.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndmorph/__init__.py` & `dask_image-2024.5.2/dask_image/ndmorph/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndmorph/_ops.py` & `dask_image-2024.5.2/dask_image/ndmorph/_ops.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image/ndmorph/_utils.py` & `dask_image-2024.5.2/dask_image/ndmorph/_utils.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/dask_image.egg-info/PKG-INFO` & `dask_image-2024.5.2/dask_image.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-image
-Version: 2024.5.1
+Version: 2024.5.2
 Summary: Distributed image processing
 Author: dask-image contributors. see https://github.com/dask/dask-image/graphs/contributors
 License: BSD-3-Clause
 Project-URL: Homepage, https://image.dask.org
 Project-URL: Issue Tracker, https://github.com/dask/dask-image/issues
 Project-URL: Source Code, https://github.com/dask/dask-image
 Keywords: dask-image,dask,image
```

### Comparing `dask_image-2024.5.1/dask_image.egg-info/SOURCES.txt` & `dask_image-2024.5.2/dask_image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/docs/Makefile` & `dask_image-2024.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/docs/conf.py` & `dask_image-2024.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/docs/coverage.rst` & `dask_image-2024.5.2/docs/coverage.rst`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/docs/index.rst` & `dask_image-2024.5.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/docs/installation.rst` & `dask_image-2024.5.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/docs/make.bat` & `dask_image-2024.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/docs/quickstart.rst` & `dask_image-2024.5.2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/docs/release/generate_release_notes.py` & `dask_image-2024.5.2/docs/release/generate_release_notes.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/docs/release/release_guide.rst` & `dask_image-2024.5.2/docs/release/release_guide.rst`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/pyproject.toml` & `dask_image-2024.5.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
 [project.urls]
 "Homepage" = "https://image.dask.org"
 "Issue Tracker" = "https://github.com/dask/dask-image/issues"
 "Source Code" = "https://github.com/dask/dask-image"
 
 [tool.setuptools_scm]
+version_scheme = "no-guess-dev"
 version_file = "dask_image/_version.py"
 
 [tool.setuptools]
 include-package-data = true
 zip-safe = false
 license-files = [
     "LICENSE.txt",
```

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_imread/test_core.py` & `dask_image-2024.5.2/tests/test_dask_image/test_imread/test_core.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_imread/test_cupy_imread.py` & `dask_image-2024.5.2/tests/test_dask_image/test_imread/test_cupy_imread.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test__conv.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test__conv.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test__diff.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test__diff.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test__edge.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test__edge.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test__gaussian.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test__gaussian.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test__generic.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test__generic.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test__order.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test__order.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test__smooth.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test__smooth.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test__threshold.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test__threshold.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test__utils.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test__utils.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test_cupy_ndfilters.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test_cupy_ndfilters.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndfilters/test_cupy_threshold.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndfilters/test_cupy_threshold.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndfourier/test__utils.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndfourier/test__utils.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndfourier/test_core.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndfourier/test_core.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndinterp/test_affine_transformation.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndinterp/test_affine_transformation.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndinterp/test_rotate.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndinterp/test_rotate.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndinterp/test_spline_filter.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndinterp/test_spline_filter.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndmeasure/test__utils.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndmeasure/test__utils.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndmeasure/test_core.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndmeasure/test_core.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndmeasure/test_find_objects.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndmeasure/test_find_objects.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndmorph/test__utils.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndmorph/test__utils.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndmorph/test_cupy_ndmorph.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndmorph/test_cupy_ndmorph.py`

 * *Files identical despite different names*

### Comparing `dask_image-2024.5.1/tests/test_dask_image/test_ndmorph/test_ndmorph.py` & `dask_image-2024.5.2/tests/test_dask_image/test_ndmorph/test_ndmorph.py`

 * *Files identical despite different names*

