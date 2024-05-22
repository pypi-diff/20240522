# Comparing `tmp/dvcx-0.83.1.tar.gz` & `tmp/dvcx-0.83.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.83.1.tar", last modified: Tue May 21 13:21:45 2024, max compression
+gzip compressed data, was "dvcx-0.83.2.tar", last modified: Wed May 22 12:48:21 2024, max compression
```

## Comparing `dvcx-0.83.1.tar` & `dvcx-0.83.2.tar`

### file list

```diff
@@ -1,252 +1,252 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.369377 dvcx-0.83.1/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-21 13:21:40.000000 dvcx-0.83.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-21 13:21:40.000000 dvcx-0.83.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.325377 dvcx-0.83.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.325377 dvcx-0.83.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-21 13:21:40.000000 dvcx-0.83.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-21 13:21:40.000000 dvcx-0.83.1/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-21 13:21:40.000000 dvcx-0.83.1/.github/ISSUE_TEMPLATE/epic-or-story.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-21 13:21:40.000000 dvcx-0.83.1/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-21 13:21:40.000000 dvcx-0.83.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.325377 dvcx-0.83.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-21 13:21:40.000000 dvcx-0.83.1/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-21 13:21:40.000000 dvcx-0.83.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-21 13:21:40.000000 dvcx-0.83.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-21 13:21:40.000000 dvcx-0.83.1/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-21 13:21:40.000000 dvcx-0.83.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-21 13:21:40.000000 dvcx-0.83.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.325377 dvcx-0.83.1/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-21 13:21:40.000000 dvcx-0.83.1/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-21 13:21:40.000000 dvcx-0.83.1/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-21 13:21:40.000000 dvcx-0.83.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-21 13:21:40.000000 dvcx-0.83.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-21 13:21:40.000000 dvcx-0.83.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.325377 dvcx-0.83.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-21 13:21:40.000000 dvcx-0.83.1/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-21 13:21:40.000000 dvcx-0.83.1/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-21 13:21:40.000000 dvcx-0.83.1/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-21 13:21:45.369377 dvcx-0.83.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-21 13:21:40.000000 dvcx-0.83.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.325377 dvcx-0.83.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-21 13:21:40.000000 dvcx-0.83.1/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.329377 dvcx-0.83.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/llm-claude-aggregate-query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/llm-claude-simple-query.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/llm-claude.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.329377 dvcx-0.83.1/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.333377 dvcx-0.83.1/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.333377 dvcx-0.83.1/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-21 13:21:40.000000 dvcx-0.83.1/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-21 13:21:40.000000 dvcx-0.83.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-21 13:21:40.000000 dvcx-0.83.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:21:45.369377 dvcx-0.83.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.317377 dvcx-0.83.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.337377 dvcx-0.83.1/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-21 13:21:45.000000 dvcx-0.83.1/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.337377 dvcx-0.83.1/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72918 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.341377 dvcx-0.83.1/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11915 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/client/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.341377 dvcx-0.83.1/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    46796 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    11067 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/data_storage/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24927 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    31922 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    17314 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.345377 dvcx-0.83.1/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/feature_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/tar_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/webdataset_laion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.349377 dvcx-0.83.1/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    61364 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/query/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/query/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.349377 dvcx-0.83.1/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.349377 dvcx-0.83.1/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.349377 dvcx-0.83.1/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.353377 dvcx-0.83.1/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/sql/functions/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.353377 dvcx-0.83.1/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-05-21 13:21:40.000000 dvcx-0.83.1/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.365377 dvcx-0.83.1/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-21 13:21:45.000000 dvcx-0.83.1/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-21 13:21:45.000000 dvcx-0.83.1/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:21:45.000000 dvcx-0.83.1/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-21 13:21:45.000000 dvcx-0.83.1/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-21 13:21:45.000000 dvcx-0.83.1/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 13:21:45.000000 dvcx-0.83.1/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.353377 dvcx-0.83.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.353377 dvcx-0.83.1/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16483 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.357377 dvcx-0.83.1/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35078 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   112963 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    28908 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/func/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/func/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.357377 dvcx-0.83.1/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/scripts/name_len_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/scripts/name_len_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/test_cli_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/test_query_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.361377 dvcx-0.83.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.365377 dvcx-0.83.1/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/lib/test_cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/lib/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/lib/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/lib/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/lib/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/lib/test_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/lib/test_webdataset_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.365377 dvcx-0.83.1/tests/unit/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:45.365377 dvcx-0.83.1/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/sql/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_catalog_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_dataset_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/unit/test_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-21 13:21:40.000000 dvcx-0.83.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.152004 dvcx-0.83.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-22 12:48:14.000000 dvcx-0.83.2/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 12:48:14.000000 dvcx-0.83.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.108004 dvcx-0.83.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.108004 dvcx-0.83.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-22 12:48:14.000000 dvcx-0.83.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-22 12:48:14.000000 dvcx-0.83.2/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-22 12:48:14.000000 dvcx-0.83.2/.github/ISSUE_TEMPLATE/epic-or-story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-22 12:48:14.000000 dvcx-0.83.2/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-22 12:48:14.000000 dvcx-0.83.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.108004 dvcx-0.83.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-22 12:48:14.000000 dvcx-0.83.2/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-22 12:48:14.000000 dvcx-0.83.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-22 12:48:14.000000 dvcx-0.83.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-22 12:48:14.000000 dvcx-0.83.2/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-22 12:48:14.000000 dvcx-0.83.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-22 12:48:14.000000 dvcx-0.83.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.108004 dvcx-0.83.2/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-22 12:48:14.000000 dvcx-0.83.2/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-22 12:48:14.000000 dvcx-0.83.2/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-22 12:48:14.000000 dvcx-0.83.2/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-22 12:48:14.000000 dvcx-0.83.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 12:48:14.000000 dvcx-0.83.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.112004 dvcx-0.83.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-22 12:48:14.000000 dvcx-0.83.2/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-22 12:48:14.000000 dvcx-0.83.2/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-22 12:48:14.000000 dvcx-0.83.2/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-22 12:48:21.152004 dvcx-0.83.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-22 12:48:14.000000 dvcx-0.83.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.112004 dvcx-0.83.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-22 12:48:14.000000 dvcx-0.83.2/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.116004 dvcx-0.83.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/llm-claude-aggregate-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/llm-claude-simple-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/llm-claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.116004 dvcx-0.83.2/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.116004 dvcx-0.83.2/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.116004 dvcx-0.83.2/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-22 12:48:14.000000 dvcx-0.83.2/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-22 12:48:14.000000 dvcx-0.83.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:48:21.152004 dvcx-0.83.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.104004 dvcx-0.83.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.120004 dvcx-0.83.2/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-22 12:48:20.000000 dvcx-0.83.2/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.124004 dvcx-0.83.2/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72918 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.124004 dvcx-0.83.2/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11915 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.124004 dvcx-0.83.2/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46796 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24927 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31922 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16819 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.128004 dvcx-0.83.2/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/feature_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/tar_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.132004 dvcx-0.83.2/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61232 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/query/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/query/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.132004 dvcx-0.83.2/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.132004 dvcx-0.83.2/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.132004 dvcx-0.83.2/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.132004 dvcx-0.83.2/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/functions/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.132004 dvcx-0.83.2/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.148004 dvcx-0.83.2/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-22 12:48:21.000000 dvcx-0.83.2/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-22 12:48:21.000000 dvcx-0.83.2/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:48:21.000000 dvcx-0.83.2/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-22 12:48:21.000000 dvcx-0.83.2/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-22 12:48:21.000000 dvcx-0.83.2/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 12:48:21.000000 dvcx-0.83.2/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.136004 dvcx-0.83.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.136004 dvcx-0.83.2/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16448 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.136004 dvcx-0.83.2/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35078 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112876 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28908 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/func/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.140004 dvcx-0.83.2/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/scripts/name_len_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/scripts/name_len_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/test_cli_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/test_query_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.144004 dvcx-0.83.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.144004 dvcx-0.83.2/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/test_cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.144004 dvcx-0.83.2/tests/unit/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.148004 dvcx-0.83.2/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/sql/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_dataset_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/utils.py
```

### Comparing `dvcx-0.83.1/.cruft.json` & `dvcx-0.83.2/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/.github/ISSUE_TEMPLATE/bug_report.md` & `dvcx-0.83.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/.github/ISSUE_TEMPLATE/epic-or-story.md` & `dvcx-0.83.2/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/.github/workflows/benchmarks.yml` & `dvcx-0.83.2/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/.github/workflows/release.yml` & `dvcx-0.83.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/.github/workflows/tests.yml` & `dvcx-0.83.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/.gitignore` & `dvcx-0.83.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/.pre-commit-config.yaml` & `dvcx-0.83.2/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -34,7 +34,16 @@
   - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
     rev: v2.13.0
     hooks:
       - id: pretty-format-toml
         args: [--autofix, --no-sort]
       - id: pretty-format-yaml
         args: [--autofix, --indent, '2', '--offset', '2', --preserve-quotes]
+  - repo: local
+    hooks:
+      - id: mypy
+        name: mypy
+        entry: mypy
+        files: '^src/|^tests/'
+        language: system
+        types: [python]
+        require_serial: true
```

### Comparing `dvcx-0.83.1/CODE_OF_CONDUCT.rst` & `dvcx-0.83.2/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/CONTRIBUTING.rst` & `dvcx-0.83.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/LICENSE` & `dvcx-0.83.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/LICENSES/Apache-2.0.txt` & `dvcx-0.83.2/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/LICENSES/BSD-3-Clause.txt` & `dvcx-0.83.2/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/LICENSES/Python-2.0.txt` & `dvcx-0.83.2/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/PKG-INFO` & `dvcx-0.83.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.83.1
+Version: 0.83.2
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.83.1/README.rst` & `dvcx-0.83.2/README.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/docs/udfs.md` & `dvcx-0.83.2/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/blip2_image_desc_lib.py` & `dvcx-0.83.2/examples/blip2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/clip.py` & `dvcx-0.83.2/examples/clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/common_sql_functions.py` & `dvcx-0.83.2/examples/common_sql_functions.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/dir_expansion.py` & `dvcx-0.83.2/examples/dir_expansion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/hf_pipeline.py` & `dvcx-0.83.2/examples/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/llava2_image_desc_lib.py` & `dvcx-0.83.2/examples/llava2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/llm-claude-aggregate-query.py` & `dvcx-0.83.2/examples/llm-claude-aggregate-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/llm-claude-simple-query.py` & `dvcx-0.83.2/examples/llm-claude-simple-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/llm-claude.py` & `dvcx-0.83.2/examples/llm-claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/loader.py` & `dvcx-0.83.2/examples/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/neurips/README` & `dvcx-0.83.2/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/neurips/distance_to_query.py` & `dvcx-0.83.2/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/neurips/llm_chat.py` & `dvcx-0.83.2/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/neurips/single_query.py` & `dvcx-0.83.2/examples/neurips/single_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/neurips/text_loaders.py` & `dvcx-0.83.2/examples/neurips/text_loaders.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/openai_image_desc_lib.py` & `dvcx-0.83.2/examples/openai_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/openimage-detect.py` & `dvcx-0.83.2/examples/openimage-detect.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/pose_detection.py` & `dvcx-0.83.2/examples/pose_detection.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/torch-loader.py` & `dvcx-0.83.2/examples/torch-loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/udfs/batching.py` & `dvcx-0.83.2/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/udfs/image_transformation.py` & `dvcx-0.83.2/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/udfs/parallel.py` & `dvcx-0.83.2/examples/udfs/parallel.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/udfs/simple.py` & `dvcx-0.83.2/examples/udfs/simple.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/udfs/stateful.py` & `dvcx-0.83.2/examples/udfs/stateful.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/udfs/stateful_similarity.py` & `dvcx-0.83.2/examples/udfs/stateful_similarity.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/unstructured-text.py` & `dvcx-0.83.2/examples/unstructured-text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/wds.py` & `dvcx-0.83.2/examples/wds.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/wds_filtered.py` & `dvcx-0.83.2/examples/wds_filtered.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/wds_meta.py` & `dvcx-0.83.2/examples/wds_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/zalando/zalando_clip.py` & `dvcx-0.83.2/examples/zalando/zalando_clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.83.2/examples/zalando/zalando_dir_as_class.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/noxfile.py` & `dvcx-0.83.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/pyproject.toml` & `dvcx-0.83.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/asyn.py` & `dvcx-0.83.2/src/dvcx/asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/cache.py` & `dvcx-0.83.2/src/dvcx/cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/catalog/catalog.py` & `dvcx-0.83.2/src/dvcx/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/catalog/datasource.py` & `dvcx-0.83.2/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/catalog/loader.py` & `dvcx-0.83.2/src/dvcx/catalog/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/cli.py` & `dvcx-0.83.2/src/dvcx/cli.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/cli_utils.py` & `dvcx-0.83.2/src/dvcx/cli_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/client/azure.py` & `dvcx-0.83.2/src/dvcx/client/azure.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/client/fileslice.py` & `dvcx-0.83.2/src/dvcx/client/fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/client/fsspec.py` & `dvcx-0.83.2/src/dvcx/client/fsspec.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/client/gcs.py` & `dvcx-0.83.2/src/dvcx/client/gcs.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/client/local.py` & `dvcx-0.83.2/src/dvcx/client/local.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/client/s3.py` & `dvcx-0.83.2/src/dvcx/client/s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/config.py` & `dvcx-0.83.2/src/dvcx/config.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/data_storage/db_engine.py` & `dvcx-0.83.2/src/dvcx/data_storage/db_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/data_storage/id_generator.py` & `dvcx-0.83.2/src/dvcx/data_storage/id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/data_storage/metastore.py` & `dvcx-0.83.2/src/dvcx/data_storage/metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/data_storage/schema.py` & `dvcx-0.83.2/src/dvcx/data_storage/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,14 @@
 
     @classmethod
     def dataset_default_columns(cls) -> list[sa.Column]:
         return [
             sa.Column("id", Int, primary_key=True),
             sa.Column("vtype", String, nullable=False, index=True),
             sa.Column("dir_type", Int, index=True),
-            sa.Column("parent_id", Int, index=True),
             sa.Column("parent", String, index=True),
             sa.Column("name", String, nullable=False, index=True),
             sa.Column("checksum", String),
             sa.Column("etag", String),
             sa.Column("version", String),
             sa.Column("is_latest", Boolean),
             sa.Column("last_modified", DateTime(timezone=True)),
```

### Comparing `dvcx-0.83.1/src/dvcx/data_storage/serializer.py` & `dvcx-0.83.2/src/dvcx/data_storage/serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/data_storage/sqlite.py` & `dvcx-0.83.2/src/dvcx/data_storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/data_storage/warehouse.py` & `dvcx-0.83.2/src/dvcx/data_storage/warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/dataset.py` & `dvcx-0.83.2/src/dvcx/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -485,15 +485,14 @@
 
 
 @attrs.define
 class DatasetRow:
     id: int
     vtype: str
     dir_type: int
-    parent_id: Optional[int]
     parent: str
     name: str
     checksum: str
     etag: str
     version: str
     is_latest: bool
     last_modified: Optional[datetime]
@@ -502,18 +501,14 @@
     owner_id: str
     anno: Optional[str]
     random: int
     location: Optional[str]
     source: "StorageURI"
     custom: Optional[dict] = attrs.field(factory=dict)
 
-    @property
-    def path(self) -> str:
-        return f"{self.parent}/{self.name}" if self.parent else self.name
-
     @classmethod
     def from_result_row(cls, columns: list[str], values: Iterable[Any]) -> "DatasetRow":
         row = dict(zip(columns, values))
         return cls.from_dict(row)
 
     @classmethod
     def from_dict(cls, row: dict[str, Any]) -> "DatasetRow":
@@ -524,22 +519,14 @@
             core_fields["last_modified"] = isoparse(core_fields["last_modified"])
         custom_fields = {
             key: value for (key, value) in row.items() if key not in core_fields
         }
         core_fields["custom"] = custom_fields
         return cls(**core_fields)
 
-    def for_insert(self) -> dict[str, Any]:
-        """Prepares data for insert"""
-        d = attrs.asdict(self)
-        del d["id"]  # id will be autogenerated in DB
-        del d["parent_id"]  # parent_id is deprecated
-        d.update(d.pop("custom", {}))
-        return d
-
     def __getitem__(self, col):
         if hasattr(self, col):
             return getattr(self, col)
         if self.custom and col in self.custom:
             return self.custom[col]
         raise KeyError
 
@@ -555,17 +542,15 @@
         )
 
     def to_preview(self):
         return {
             "id": self.id,
             "vtype": self.vtype,
             "dir_type": self.dir_type,
-            "parent_id": self.parent_id,
             "parent": self.parent,
-            "path": self.path,
             "name": self.name,
             "checksum": self.checksum,
             "etag": self.etag,
             "version": self.version,
             "is_latest": self.is_latest,
             "last_modified": (
                 self.last_modified.isoformat() if self.last_modified else None
```

### Comparing `dvcx-0.83.1/src/dvcx/error.py` & `dvcx-0.83.2/src/dvcx/error.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/cached_stream.py` & `dvcx-0.83.2/src/dvcx/lib/cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/claude.py` & `dvcx-0.83.2/src/dvcx/lib/claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/dataset.py` & `dvcx-0.83.2/src/dvcx/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/feature.py` & `dvcx-0.83.2/src/dvcx/lib/feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/feature_types.py` & `dvcx-0.83.2/src/dvcx/lib/feature_types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/feature_udf.py` & `dvcx-0.83.2/src/dvcx/lib/feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/file.py` & `dvcx-0.83.2/src/dvcx/lib/file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.83.2/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.83.2/src/dvcx/lib/hf_image_to_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.83.2/src/dvcx/lib/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/image.py` & `dvcx-0.83.2/src/dvcx/lib/image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/image_transform.py` & `dvcx-0.83.2/src/dvcx/lib/image_transform.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.83.2/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/pytorch.py` & `dvcx-0.83.2/src/dvcx/lib/pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/reader.py` & `dvcx-0.83.2/src/dvcx/lib/reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/tar_file.py` & `dvcx-0.83.2/src/dvcx/lib/tar_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/text.py` & `dvcx-0.83.2/src/dvcx/lib/text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/udf.py` & `dvcx-0.83.2/src/dvcx/lib/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/unstructured.py` & `dvcx-0.83.2/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/utils.py` & `dvcx-0.83.2/src/dvcx/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/webdataset.py` & `dvcx-0.83.2/src/dvcx/lib/webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/webdataset_laion.py` & `dvcx-0.83.2/src/dvcx/lib/webdataset_laion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.83.2/src/dvcx/lib/webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/listing.py` & `dvcx-0.83.2/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/node.py` & `dvcx-0.83.2/src/dvcx/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 
 
 @attrs.define
 class Node:
     id: int = 0
     vtype: str = ""
     dir_type: Optional[int] = None
-    parent_id: Optional[int] = None
     parent: str = ""
     name: str = ""
     checksum: str = ""
     etag: str = ""
     version: Optional[str] = None
     is_latest: bool = True
     last_modified: Optional[datetime] = None
```

### Comparing `dvcx-0.83.1/src/dvcx/nodes_fetcher.py` & `dvcx-0.83.2/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/nodes_thread_pool.py` & `dvcx-0.83.2/src/dvcx/nodes_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/progress.py` & `dvcx-0.83.2/src/dvcx/progress.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/query/batch.py` & `dvcx-0.83.2/src/dvcx/query/batch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/query/builtins.py` & `dvcx-0.83.2/src/dvcx/query/builtins.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/query/dataset.py` & `dvcx-0.83.2/src/dvcx/query/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1654,22 +1654,18 @@
                 **kwargs,
             )
             version = version or dataset.latest_version
 
             dr = self.catalog.warehouse.dataset_rows(dataset)
 
             # Exclude the id column and let the db create it to avoid unique
-            # constraint violations, and parent_id is not used in datasets.
-            cols = [
-                col.name
-                for col in dr.get_table().c
-                if col.name not in ("id", "parent_id")
-            ]
+            # constraint violations.
+            cols = [col.name for col in dr.get_table().c if col.name != "id"]
 
-            q = query.exclude(("id", "parent_id"))
+            q = query.exclude(("id",))
 
             if q._order_by_clauses:
                 # ensuring we have id sorted by order by clause if it exists in a query
                 q = q.add_columns(
                     f.row_number().over(order_by=q._order_by_clauses).label("id")
                 )
                 cols.append("id")
```

### Comparing `dvcx-0.83.1/src/dvcx/query/dispatch.py` & `dvcx-0.83.2/src/dvcx/query/dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/query/params.py` & `dvcx-0.83.2/src/dvcx/query/params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/query/schema.py` & `dvcx-0.83.2/src/dvcx/query/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/query/session.py` & `dvcx-0.83.2/src/dvcx/query/session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/query/udf.py` & `dvcx-0.83.2/src/dvcx/query/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/remote/studio.py` & `dvcx-0.83.2/src/dvcx/remote/studio.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,14 @@
         return response
 
     def dataset_rows_chunk(
         self, name: str, version: int, offset: int
     ) -> Response[DatasetRowsData]:
         def _parse_row(row):
             row["id"] = int(row["id"])
-            row["parent_id"] = int(row["parent_id"])
             return row
 
         req_data = {"dataset_name": name, "dataset_version": version}
         response = self._send_request_msgpack(
             "dataset-rows",
             {**req_data, "offset": offset, "limit": DATASET_ROWS_CHUNK_SIZE},
         )
```

### Comparing `dvcx-0.83.1/src/dvcx/sql/default/base.py` & `dvcx-0.83.2/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/sql/functions/array.py` & `dvcx-0.83.2/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/sql/functions/path.py` & `dvcx-0.83.2/src/dvcx/sql/functions/path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/sql/selectable.py` & `dvcx-0.83.2/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/sql/sqlite/base.py` & `dvcx-0.83.2/src/dvcx/sql/sqlite/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/sql/sqlite/types.py` & `dvcx-0.83.2/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/sql/types.py` & `dvcx-0.83.2/src/dvcx/sql/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/sql/utils.py` & `dvcx-0.83.2/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/storage.py` & `dvcx-0.83.2/src/dvcx/storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx/utils.py` & `dvcx-0.83.2/src/dvcx/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,14 @@
                 "checksum",
                 "dir_type",
                 "etag",
                 "is_latest",
                 "last_modified",
                 "owner_id",
                 "owner_name",
-                "parent_id",
                 "size",
                 "version",
                 "vtype",
             ],
             inplace=True,
             errors="ignore",
         )
```

### Comparing `dvcx-0.83.1/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.83.2/src/dvcx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.83.1
+Version: 0.83.2
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.83.1/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.83.2/src/dvcx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/src/dvcx.egg-info/requires.txt` & `dvcx-0.83.2/src/dvcx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/benchmarks/conftest.py` & `dvcx-0.83.2/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/conftest.py` & `dvcx-0.83.2/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -511,15 +511,14 @@
         DatasetRow.from_dict(
             {
                 "id": i,
                 "location": "",
                 "source": "s3://my-bucket",
                 "dir_type": 0,
                 "vtype": "",
-                "parent_id": None,
                 "parent": "input/text_emd_1m",
                 "version": "7e589b7d-382c-49a5-931f-2b999c930c5e",
                 "is_latest": True,
                 "name": f"dql_1m_meta_text_emd.parquet_3_{i}_0.snappy.parquet",
                 "etag": f"72b35c8e9b8eed1636c91eb94241c2f8-{i}",
                 "owner_id": "owner",
                 "owner_name": "aws-iterative-sandbox",
```

### Comparing `dvcx-0.83.1/tests/data.py` & `dvcx-0.83.2/tests/data.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/func/test_catalog.py` & `dvcx-0.83.2/tests/func/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/func/test_client.py` & `dvcx-0.83.2/tests/func/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/func/test_dataset_query.py` & `dvcx-0.83.2/tests/func/test_dataset_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,15 +459,15 @@
         )
         result = new_query.results(row_factory=lambda c, v: dict(zip(c, v)))
         dataset_record = catalog.get_dataset(ds_name)
         assert dataset_record.status == DatasetStatus.COMPLETE
     else:
         result = q.results(row_factory=lambda c, v: dict(zip(c, v)))
     assert len(result) == 4
-    assert len(result[0]) == 23
+    assert len(result[0]) == 22
     cols = {"size10x", "size1000x", "s2", "s3", "s4"}
     new_data = [[v for k, v in r.items() if k in cols] for r in result]
     assert new_data == [
         [130, 13000, 26, 39, 52],
         [40, 4000, 8, 12, 16],
         [40, 4000, 8, 12, 16],
         [30, 3000, 6, 9, 12],
@@ -490,15 +490,15 @@
         q.save(ds_name)
         new_query = DatasetQuery(name=ds_name, catalog=catalog).order_by(C.name.desc())
         result = new_query.results()
         dataset_record = catalog.get_dataset(ds_name)
         assert dataset_record.status == DatasetStatus.COMPLETE
     else:
         result = q.results()
-    assert [r[5] for r in result] == ["dog4", "dog3", "dog2", "dog1", "description"]
+    assert [r[4] for r in result] == ["dog4", "dog3", "dog2", "dog1", "description"]
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
@@ -1925,15 +1925,14 @@
 
 def create_subobject(row, name: str, size: int):
     """Create a subobject with this row as its parent."""
     return {
         # Values that depend on the parent object.
         "vtype": "fake",
         "dir_type": 0,
-        "parent_id": None,
         # Inherited values.
         "owner_name": row.owner_name,
         "owner_id": row.owner_id,
         "is_latest": row.is_latest,
         "source": row.source,
         # User-provided values.
         "name": name,
@@ -2772,18 +2771,17 @@
     ds_queries = []
     for ds_name in ("ds1", "ds2"):
         ds = metastore.get_dataset(ds_name)
         dr = warehouse.dataset_rows(ds)
         dq = dr.select().order_by(dr.c.parent, dr.c.name)
         ds_queries.append(dq)
 
-    ignore_cols = ["id", "parent_id"]
     ds1, ds2 = (
         [
-            {k: v for k, v in zip(DATASET_CORE_COLUMN_NAMES, r) if k not in ignore_cols}
+            {k: v for k, v in zip(DATASET_CORE_COLUMN_NAMES, r) if k != "id"}
             for r in warehouse.db.execute(q)
         ]
         for q in ds_queries
     )
 
     # everything except the id field should match
     assert ds1 == ds2
@@ -3636,11 +3634,11 @@
 def test_missing_default_columns(cloud_test_catalog):
     catalog = cloud_test_catalog.catalog
     path = f"{cloud_test_catalog.src_uri}/cats"
     with pytest.raises(RuntimeError) as exc_info:
         DatasetQuery(path=path, catalog=catalog).select(C.name).save("cats", version=1)
 
     assert str(exc_info.value) == (
-        "Missing default columns from final query: id, vtype, dir_type, parent_id, "
+        "Missing default columns from final query: id, vtype, dir_type, "
         "parent, checksum, etag, version, is_latest, last_modified, size, "
         "owner_name, owner_id, anno, random, location, source"
     )
```

### Comparing `dvcx-0.83.1/tests/func/test_datasets.py` & `dvcx-0.83.2/tests/func/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/func/test_ls.py` & `dvcx-0.83.2/tests/func/test_ls.py`

 * *Files 3% similar despite different names*

```diff
@@ -277,15 +277,14 @@
 
 owner_id = "a13a3ff923430363b098ce9c769e450724e74e646332b08ca6b3ac4f96dae083"
 REMOTE_DATA: dict[str, list[dict[str, Any]]] = {
     "": [
         {
             "id": 816,
             "dir_type": 1,
-            "parent_id": None,
             "name": "cats",
             "checksum": "",
             "etag": "",
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2023, 1, 17, 21, 39, 0, 88564),
             "size": 0,
@@ -294,15 +293,14 @@
             "path_str": "{src}/cats",
             "anno": None,
             "path": [],
         },
         {
             "id": 825,
             "dir_type": 1,
-            "parent_id": None,
             "name": "dogs",
             "checksum": "",
             "etag": "",
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2023, 1, 17, 21, 39, 0, 88567),
             "size": 0,
@@ -311,15 +309,14 @@
             "path_str": "{src}/dogs",
             "anno": None,
             "path": [],
         },
         {
             "id": None,
             "dir_type": 0,
-            "parent_id": None,
             "name": "description",
             "checksum": "",
             "etag": "20664550afa2654017377ceb266a1f82",
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2022, 2, 10, 3, 39, 9),
             "size": 350496,
@@ -330,15 +327,14 @@
             "path": [],
         },
     ],
     "dogs/others": [
         {
             "id": None,
             "dir_type": 0,
-            "parent_id": None,
             "name": "dog4",
             "checksum": "",
             "etag": "c4e42ce24d92bb5b4c4be9a99b237502",
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2022, 6, 28, 22, 39, 1),
             "size": 32975,
@@ -349,15 +345,14 @@
             "path": [],
         },
     ],
     "dogs": [
         {
             "id": None,
             "dir_type": 0,
-            "parent_id": None,
             "name": "dog1",
             "checksum": "",
             "etag": "44a632238558e0aa4c54bdb901bf9cff",
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2022, 6, 28, 22, 39, 1),
             "size": 101,
@@ -366,15 +361,14 @@
             "path_str": "{src}/dogs/dog1",
             "anno": None,
             "path": [],
         },
         {
             "id": None,
             "dir_type": 0,
-            "parent_id": None,
             "name": "dog2",
             "checksum": "",
             "etag": "76556c960239c50e5a8f8569daf85355",
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2022, 6, 28, 22, 39, 1),
             "size": 29759,
@@ -383,15 +377,14 @@
             "path_str": "{src}/dogs/dog2",
             "anno": None,
             "path": [],
         },
         {
             "id": None,
             "dir_type": 0,
-            "parent_id": None,
             "name": "dog3",
             "checksum": "",
             "etag": "b1c99fedcf77bf5fa62984e93db1955c",
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2022, 6, 28, 22, 39, 1),
             "size": 102,
```

### Comparing `dvcx-0.83.1/tests/func/test_pull.py` & `dvcx-0.83.2/tests/func/test_pull.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 
         adapted["id"] = 1
         adapted["vtype"] = b""
         adapted["location"] = b""
         adapted["source"] = b"s3://dogs"
         adapted["dir_type"] = DirType.FILE
         adapted["random"] = 1
-        adapted["parent_id"] = 1
         return adapted
 
     dog_entries = [_adapt_row(e) for e in dog_entries]
     df = pd.DataFrame.from_records(dog_entries)
     buffer = io.BytesIO()
     df.to_parquet(buffer, engine="auto")
```

### Comparing `dvcx-0.83.1/tests/func/test_pytorch.py` & `dvcx-0.83.2/tests/func/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/func/test_query.py` & `dvcx-0.83.2/tests/func/test_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/scripts/name_len_normal.py` & `dvcx-0.83.2/tests/scripts/name_len_normal.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/scripts/name_len_slow.py` & `dvcx-0.83.2/tests/scripts/name_len_slow.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/test_cli_e2e.py` & `dvcx-0.83.2/tests/test_cli_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/test_query_e2e.py` & `dvcx-0.83.2/tests/test_query_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/lib/test_cached_stream.py` & `dvcx-0.83.2/tests/unit/lib/test_cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/lib/test_feature.py` & `dvcx-0.83.2/tests/unit/lib/test_feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/lib/test_feature_udf.py` & `dvcx-0.83.2/tests/unit/lib/test_feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/lib/test_file.py` & `dvcx-0.83.2/tests/unit/lib/test_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/lib/test_image.py` & `dvcx-0.83.2/tests/unit/lib/test_image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/lib/test_reader.py` & `dvcx-0.83.2/tests/unit/lib/test_reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/lib/test_text.py` & `dvcx-0.83.2/tests/unit/lib/test_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/lib/test_webdataset.py` & `dvcx-0.83.2/tests/unit/lib/test_webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/lib/test_webdataset_meta.py` & `dvcx-0.83.2/tests/unit/lib/test_webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/sql/test_array.py` & `dvcx-0.83.2/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/sql/test_conditional.py` & `dvcx-0.83.2/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/sql/test_path.py` & `dvcx-0.83.2/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/sql/test_selectable.py` & `dvcx-0.83.2/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/sql/test_string.py` & `dvcx-0.83.2/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_asyn.py` & `dvcx-0.83.2/tests/unit/test_asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_cache.py` & `dvcx-0.83.2/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_catalog.py` & `dvcx-0.83.2/tests/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_catalog_loader.py` & `dvcx-0.83.2/tests/unit/test_catalog_loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_cli_parsing.py` & `dvcx-0.83.2/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_client.py` & `dvcx-0.83.2/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_client_s3.py` & `dvcx-0.83.2/tests/unit/test_client_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 
 def make_size_node(node_id, dir_type, parent, name, size):
     return Node(
         node_id,
         "",  # vtype
         dir_type,
-        None,  # parent_id
         parent,
         name,
         size=size,
     )
 
 
 class FakeCache:
```

### Comparing `dvcx-0.83.1/tests/unit/test_data_storage.py` & `dvcx-0.83.2/tests/unit/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_database_engine.py` & `dvcx-0.83.2/tests/unit/test_database_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_dataset.py` & `dvcx-0.83.2/tests/unit/test_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
     assert result.string == (
         "\n"
         'CREATE TABLE IF NOT EXISTS "ds-1" (\n'
         "\tid INTEGER NOT NULL, \n"
         "\tvtype VARCHAR NOT NULL, \n"
         "\tdir_type INTEGER, \n"
-        "\tparent_id INTEGER, \n"
         "\tparent VARCHAR, \n"
         "\tname VARCHAR NOT NULL, \n"
         "\tchecksum VARCHAR, \n"
         "\tetag VARCHAR, \n"
         "\tversion VARCHAR, \n"
         "\tis_latest BOOLEAN, \n"
         "\tlast_modified DATETIME, \n"
```

### Comparing `dvcx-0.83.1/tests/unit/test_dataset_row.py` & `dvcx-0.83.2/tests/unit/test_dataset_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 
 def test_dataset_row_from_dict():
     row = DatasetRow(
         id=37,
         vtype="",
         dir_type=1,
-        parent_id=None,
         parent="000002",
         name="0000020572.json",
         checksum="",
         etag="c16a68901b0a3222beccaa53c34a6c0c",
         version="",
         is_latest=True,
         last_modified=datetime.datetime(2022, 12, 27, 1, 16, 57),
```

### Comparing `dvcx-0.83.1/tests/unit/test_dispatch.py` & `dvcx-0.83.2/tests/unit/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_fileslice.py` & `dvcx-0.83.2/tests/unit/test_fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_id_generator.py` & `dvcx-0.83.2/tests/unit/test_id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_listing.py` & `dvcx-0.83.2/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_metastore.py` & `dvcx-0.83.2/tests/unit/test_metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_query_params.py` & `dvcx-0.83.2/tests/unit/test_query_params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_serializer.py` & `dvcx-0.83.2/tests/unit/test_serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_session.py` & `dvcx-0.83.2/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_storage.py` & `dvcx-0.83.2/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_udf.py` & `dvcx-0.83.2/tests/unit/test_udf.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     row = DatasetRow(
         id=6,
         vtype="",
         dir_type=1,
         parent="",
         name="obj",
         checksum="",
-        parent_id=None,
         last_modified=None,
         anno={},
         etag="",
         version="",
         is_latest=True,
         size=7,
         owner_name="",
@@ -44,15 +43,14 @@
     row = DatasetRow(
         id=6,
         vtype="",
         dir_type=1,
         parent="",
         name="obj",
         checksum="",
-        parent_id=None,
         last_modified=None,
         anno={},
         etag="",
         version="",
         is_latest=True,
         size=7,
         owner_name="",
@@ -76,15 +74,14 @@
         row = DatasetRow(
             id=row_id,
             vtype="",
             dir_type=1,
             parent="",
             name="obj",
             checksum="",
-            parent_id=None,
             last_modified=None,
             anno={},
             etag="",
             version="",
             is_latest=True,
             size=size,
             owner_name="",
@@ -119,15 +116,14 @@
         row = DatasetRow(
             id=5,
             vtype="",
             dir_type=1,
             parent="",
             name="obj",
             checksum="",
-            parent_id=None,
             last_modified=None,
             anno={},
             etag="",
             version="",
             is_latest=True,
             size=size,
             owner_name="",
```

### Comparing `dvcx-0.83.1/tests/unit/test_utils.py` & `dvcx-0.83.2/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/unit/test_warehouse.py` & `dvcx-0.83.2/tests/unit/test_warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.1/tests/utils.py` & `dvcx-0.83.2/tests/utils.py`

 * *Files identical despite different names*

