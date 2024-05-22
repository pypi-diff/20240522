# Comparing `tmp/libcst-1.3.0.tar.gz` & `tmp/libcst-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libcst-1.3.0.tar", last modified: Wed Apr  3 19:41:06 2024, max compression
+gzip compressed data, was "libcst-1.3.1.tar", last modified: Wed Apr  3 20:57:16 2024, max compression
```

## Comparing `libcst-1.3.0.tar` & `libcst-1.3.1.tar`

### file list

```diff
@@ -1,503 +1,503 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.497963 libcst-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.417963 libcst-1.3.0/.cargo/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 19:40:02.000000 libcst-1.3.0/.cargo/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-03 19:40:02.000000 libcst-1.3.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-03 19:40:02.000000 libcst-1.3.0/.fixit.config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-04-03 19:40:02.000000 libcst-1.3.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 19:40:02.000000 libcst-1.3.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.417963 libcst-1.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 19:40:02.000000 libcst-1.3.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-03 19:40:02.000000 libcst-1.3.0/.github/build-matrix.json
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-03 19:40:02.000000 libcst-1.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.417963 libcst-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-03 19:40:02.000000 libcst-1.3.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-03 19:40:02.000000 libcst-1.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-03 19:40:02.000000 libcst-1.3.0/.github/workflows/pypi_upload.yml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 19:40:02.000000 libcst-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-03 19:40:02.000000 libcst-1.3.0/.pyre_configuration
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-03 19:40:02.000000 libcst-1.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-03 19:40:02.000000 libcst-1.3.0/.watchmanconfig
--rw-r--r--   0 runner    (1001) docker     (127)    40809 2024-04-03 19:40:02.000000 libcst-1.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-03 19:40:02.000000 libcst-1.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-03 19:40:02.000000 libcst-1.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-03 19:40:02.000000 libcst-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-03 19:40:02.000000 libcst-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17200 2024-04-03 19:41:06.497963 libcst-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-04-03 19:40:02.000000 libcst-1.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 19:40:02.000000 libcst-1.3.0/apt.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 19:40:02.000000 libcst-1.3.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.409963 libcst-1.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.421963 libcst-1.3.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.421963 libcst-1.3.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.421963 libcst-1.3.0/docs/source/_static/img/
--rw-r--r--   0 runner    (1001) docker     (127)   108465 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/_static/img/python_scopes.png
--rw-r--r--   0 runner    (1001) docker     (127)    30400 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/_static/img/python_scopes.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.425963 libcst-1.3.0/docs/source/_static/logo/
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/_static/logo/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/_static/logo/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/_static/logo/favicon_16px.png
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/_static/logo/favicon_32px.png
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/_static/logo/horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/_static/logo/horizontal_white.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/_static/logo/horizontal_white_sidebar.png
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/_static/logo/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/_static/logo/icon_white.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/_static/logo/vertical.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/_static/logo/vertical_white.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.425963 libcst-1.3.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/best_practices.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/codemods.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/codemods_tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9553 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/experimental.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/helpers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/matchers.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/matchers_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/metadata_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/motivation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/nodes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/parser.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/scope_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9873 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/visitors.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-04-03 19:40:02.000000 libcst-1.3.0/docs/source/why_libcst.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.429963 libcst-1.3.0/libcst/
--rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_add_slots.py
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_batched_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_flatten_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_maybe_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_metadata_dependent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.429963 libcst-1.3.0/libcst/_nodes/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19437 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/deep_equals.py
--rw-r--r--   0 runner    (1001) docker     (127)   141869 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    31193 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/op.py
--rw-r--r--   0 runner    (1001) docker     (127)   143870 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.441963 libcst-1.3.0/libcst/_nodes/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_assert.py
--rw-r--r--   0 runner    (1001) docker     (127)    16051 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)    45724 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_atom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_await.py
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_binary_op.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_boolean_op.py
--rw-r--r--   0 runner    (1001) docker     (127)    22698 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    17662 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_classdef.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13640 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_cst_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_del.py
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_dict_comp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_else.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_empty_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_flatten_behavior.py
--rw-r--r--   0 runner    (1001) docker     (127)     7665 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_for.py
--rw-r--r--   0 runner    (1001) docker     (127)    97662 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_funcdef.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_global.py
--rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_ifexp.py
--rw-r--r--   0 runner    (1001) docker     (127)    29777 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_indented_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    40904 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_leaf_small_statements.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    22302 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_matrix_multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_namedexpr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_newline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_nonlocal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_removal_behavior.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_return.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    21237 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_simple_comp.py
--rw-r--r--   0 runner    (1001) docker     (127)    13989 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_simple_statement.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_simple_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_simple_whitespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_small_statement.py
--rw-r--r--   0 runner    (1001) docker     (127)    16758 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_subscript.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_trailing_whitespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    25792 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_try.py
--rw-r--r--   0 runner    (1001) docker     (127)    11237 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_type_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_unary_op.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_while.py
--rw-r--r--   0 runner    (1001) docker     (127)    13850 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_with.py
--rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/tests/test_yield.py
--rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_nodes/whitespace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.441963 libcst-1.3.0/libcst/_parser/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/base_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.445963 libcst-1.3.0/libcst/_parser/conversions/
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/conversions/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/conversions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53078 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/conversions/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/conversions/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    13365 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/conversions/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    47301 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/conversions/statement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/conversions/terminals.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/custom_itertools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/detect_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/grammar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.445963 libcst-1.3.0/libcst/_parser/parso/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/parso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.445963 libcst-1.3.0/libcst/_parser/parso/pgen2/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/parso/pgen2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13727 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/parso/pgen2/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/parso/pgen2/grammar_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.445963 libcst-1.3.0/libcst/_parser/parso/python/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/parso/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/parso/python/py_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/parso/python/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    44145 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/parso/python/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.445963 libcst-1.3.0/libcst/_parser/parso/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/parso/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/parso/tests/test_fstring.py
--rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/parso/tests/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/parso/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7565 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/parso/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/production_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/py_whitespace_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/python_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.445963 libcst-1.3.0/libcst/_parser/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14086 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/tests/test_detect_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/tests/test_footer_behavior.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/tests/test_node_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/tests/test_parse_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/tests/test_version_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     9447 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/tests/test_whitespace_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    83462 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/tests/test_wrapped_tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.449963 libcst-1.3.0/libcst/_parser/types/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/types/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/types/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/types/partials.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/types/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/types/py_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/types/py_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/types/py_whitespace_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.449963 libcst-1.3.0/libcst/_parser/types/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/types/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/types/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/types/token.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/types/whitespace_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/whitespace_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_parser/wrapped_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_position.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_removal_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_type_enforce.py
--rw-r--r--   0 runner    (1001) docker     (127)   194662 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_typed_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_typed_visitor_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 19:41:06.000000 libcst-1.3.0/libcst/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/_visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.449963 libcst-1.3.0/libcst/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codegen/gather.py
--rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codegen/gen_matcher_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codegen/gen_type_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codegen/gen_visitor_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codegen/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.449963 libcst-1.3.0/libcst/codegen/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codegen/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codegen/tests/test_codegen_clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codegen/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.453963 libcst-1.3.0/libcst/codemod/
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24326 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/_dummy_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/_visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.453963 libcst-1.3.0/libcst/codemod/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/add_pyre_directive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/add_trailing_commas.py
--rw-r--r--   0 runner    (1001) docker     (127)    16027 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/convert_format_to_fstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/convert_namedtuple_to_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/convert_percent_format_to_fstring.py
--rw-r--r--   0 runner    (1001) docker     (127)    32486 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/convert_type_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/ensure_import_present.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/fix_pyre_directives.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/noop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/remove_pyre_directive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    16702 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/strip_strings_from_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.457963 libcst-1.3.0/libcst/codemod/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/tests/test_add_pyre_directive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/tests/test_add_trailing_commas.py
--rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/tests/test_convert_format_to_fstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/tests/test_convert_namedtuple_to_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/tests/test_convert_percent_format_to_fstring.py
--rw-r--r--   0 runner    (1001) docker     (127)    13941 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/tests/test_convert_type_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/tests/test_ensure_import_present.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/tests/test_fix_pyre_directives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/tests/test_noop.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/tests/test_remove_pyre_directive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/tests/test_remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    15932 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/tests/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/tests/test_strip_strings_from_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/tests/test_unnecessary_format_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/commands/unnecessary_format_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.457963 libcst-1.3.0/libcst/codemod/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/tests/codemod_formatter_error_input.py.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/tests/test_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/tests/test_codemod_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/tests/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.461963 libcst-1.3.0/libcst/codemod/visitors/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19494 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/_add_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    50925 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/_apply_type_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/_gather_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/_gather_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/_gather_global_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/_gather_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/_gather_string_annotation_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/_gather_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    20494 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/_remove_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.461963 libcst-1.3.0/libcst/codemod/visitors/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23717 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/tests/test_add_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    55792 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/tests/test_apply_type_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/tests/test_gather_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/tests/test_gather_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/tests/test_gather_global_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/tests/test_gather_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/tests/test_gather_string_annotation_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/tests/test_gather_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    23816 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/codemod/visitors/tests/test_remove_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.461963 libcst-1.3.0/libcst/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19403 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/helpers/_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/helpers/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/helpers/module.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/helpers/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.465963 libcst-1.3.0/libcst/helpers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/helpers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/helpers/tests/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    10669 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/helpers/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/helpers/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)    11776 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/helpers/tests/test_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.465963 libcst-1.3.0/libcst/matchers/
--rw-r--r--   0 runner    (1001) docker     (127)   561418 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/matchers/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    79068 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/matchers/_matcher_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10414 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/matchers/_return_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    34453 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/matchers/_visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.465963 libcst-1.3.0/libcst/matchers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/matchers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35211 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/matchers/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    15761 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/matchers/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/matchers/tests/test_findall.py
--rw-r--r--   0 runner    (1001) docker     (127)    53908 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/matchers/tests/test_matchers.py
--rw-r--r--   0 runner    (1001) docker     (127)    23189 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/matchers/tests/test_matchers_with_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/matchers/tests/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (127)    20190 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/matchers/tests/test_visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.469963 libcst-1.3.0/libcst/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/accessor_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/expression_context_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/file_path_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/full_repo_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/name_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/parent_node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/position_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/reentrant_codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)    47962 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/scope_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/span_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.473963 libcst-1.3.0/libcst/metadata/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/tests/test_accessor_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/tests/test_base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/tests/test_expression_context_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/tests/test_file_path_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/tests/test_full_repo_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/tests/test_metadata_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/tests/test_metadata_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19965 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/tests/test_name_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/tests/test_parent_node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/tests/test_position_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/tests/test_reentrant_codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)    86437 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/tests/test_scope_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/tests/test_span_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/tests/test_type_inference_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/type_inference_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/metadata/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.473963 libcst-1.3.0/libcst/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.473963 libcst-1.3.0/libcst/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tests/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.473963 libcst-1.3.0/libcst/tests/pyre/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tests/pyre/.pyre_configuration
--rw-r--r--   0 runner    (1001) docker     (127)     9016 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tests/pyre/simple_class.json
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tests/pyre/simple_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tests/test_add_slots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tests/test_batched_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tests/test_deep_clone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tests/test_deep_replace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tests/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tests/test_fuzz.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tests/test_pyre_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tests/test_roundtrip.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tests/test_tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25736 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tests/test_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tests/test_type_enforce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tests/test_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    31443 2024-04-03 19:40:02.000000 libcst-1.3.0/libcst/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.493963 libcst-1.3.0/libcst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17200 2024-04-03 19:41:06.000000 libcst-1.3.0/libcst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16090 2024-04-03 19:41:06.000000 libcst-1.3.0/libcst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:41:06.000000 libcst-1.3.0/libcst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:41:06.000000 libcst-1.3.0/libcst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-03 19:41:06.000000 libcst-1.3.0/libcst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 19:41:06.000000 libcst-1.3.0/libcst.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.477963 libcst-1.3.0/native/
--rw-r--r--   0 runner    (1001) docker     (127)    26565 2024-04-03 19:40:02.000000 libcst-1.3.0/native/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 19:40:02.000000 libcst-1.3.0/native/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.477963 libcst-1.3.0/native/libcst/
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)    32411 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/Grammar
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.477963 libcst-1.3.0/native/libcst/benches/
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/benches/parser_benchmark.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.477963 libcst-1.3.0/native/libcst/src/
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/bin.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.481963 libcst-1.3.0/native/libcst/src/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/nodes/codegen.rs
--rw-r--r--   0 runner    (1001) docker     (127)    80129 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/nodes/expression.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/nodes/inflate_helpers.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/nodes/macros.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/nodes/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/nodes/module.rs
--rw-r--r--   0 runner    (1001) docker     (127)    50731 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/nodes/op.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/nodes/parser_config.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/nodes/py_cached.rs
--rw-r--r--   0 runner    (1001) docker     (127)   113875 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/nodes/statement.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/nodes/test_utils.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/nodes/traits.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/nodes/whitespace.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.481963 libcst-1.3.0/native/libcst/src/parser/
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/parser/errors.rs
--rw-r--r--   0 runner    (1001) docker     (127)   113160 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/parser/grammar.rs
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/parser/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/parser/numbers.rs
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/py.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.481963 libcst-1.3.0/native/libcst/src/tokenizer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.481963 libcst-1.3.0/native/libcst/src/tokenizer/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/tokenizer/core/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/tokenizer/core/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    49168 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/tokenizer/core/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/tokenizer/core/string_types.rs
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/tokenizer/debug_utils.rs
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/tokenizer/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/tokenizer/operators.rs
--rw-r--r--   0 runner    (1001) docker     (127)    23922 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/tokenizer/tests.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.481963 libcst-1.3.0/native/libcst/src/tokenizer/text_position/
--rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/tokenizer/text_position/char_width.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/tokenizer/text_position/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)    16117 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/src/tokenizer/whitespace_parser.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.481963 libcst-1.3.0/native/libcst/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.489963 libcst-1.3.0/native/libcst/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/big_binary_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/class_craziness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/dangling_indent.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/decorated_function_without_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/dysfunctional_del.py
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/expr.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/expr_statement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/fun_with_func_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/global_nonlocal.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/import.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/indents_but_no_eol_before_eof.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/just_a_comment_without_nl.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/malicious_match.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/mixed_newlines.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/pep646.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/raise.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/smol_statements.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/spacious_spaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/starry_tries.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/suicidal_slices.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/super_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/terrible_tries.py
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/trailing_comment_without_nl.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/trailing_whitespace.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/tuple_shenanigans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/type_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/vast_emptiness.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/with_wickedness.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/fixtures/wonky_walrus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst/tests/parser_roundtrip.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.489963 libcst-1.3.0/native/libcst_derive/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst_derive/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst_derive/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.489963 libcst-1.3.0/native/libcst_derive/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst_derive/src/codegen.rs
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst_derive/src/cstnode.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst_derive/src/inflate.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst_derive/src/into_py.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst_derive/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst_derive/src/parenthesized_node.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.413963 libcst-1.3.0/native/libcst_derive/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.489963 libcst-1.3.0/native/libcst_derive/tests/pass/
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst_derive/tests/pass/minimal_cst.rs
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-03 19:40:02.000000 libcst-1.3.0/native/libcst_derive/tests/pass/simple.rs
--rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-04-03 19:40:02.000000 libcst-1.3.0/native/roundtrip.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-03 19:40:02.000000 libcst-1.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.489963 libcst-1.3.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-03 19:40:02.000000 libcst-1.3.0/scripts/check_copyright.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-03 19:40:02.000000 libcst-1.3.0/scripts/regenerate-fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:41:06.497963 libcst-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-03 19:40:02.000000 libcst-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.489963 libcst-1.3.0/stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 19:40:02.000000 libcst-1.3.0/stubs/hypothesis.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 19:40:02.000000 libcst-1.3.0/stubs/hypothesmith.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.493963 libcst-1.3.0/stubs/libcst/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-03 19:40:02.000000 libcst-1.3.0/stubs/libcst/native.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:06.493963 libcst-1.3.0/stubs/libcst_native/
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-03 19:40:02.000000 libcst-1.3.0/stubs/libcst_native/parser_config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-03 19:40:02.000000 libcst-1.3.0/stubs/libcst_native/token_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-03 19:40:02.000000 libcst-1.3.0/stubs/libcst_native/tokenize.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-03 19:40:02.000000 libcst-1.3.0/stubs/libcst_native/whitespace_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-03 19:40:02.000000 libcst-1.3.0/stubs/libcst_native/whitespace_state.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 19:40:02.000000 libcst-1.3.0/stubs/setuptools.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-03 19:40:02.000000 libcst-1.3.0/stubs/tokenize.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 19:40:02.000000 libcst-1.3.0/stubs/typing_inspect.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.175547 libcst-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.099547 libcst-1.3.1/.cargo/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 20:56:08.000000 libcst-1.3.1/.cargo/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-03 20:56:08.000000 libcst-1.3.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-03 20:56:08.000000 libcst-1.3.1/.fixit.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-04-03 20:56:08.000000 libcst-1.3.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 20:56:08.000000 libcst-1.3.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.099547 libcst-1.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 20:56:08.000000 libcst-1.3.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-03 20:56:08.000000 libcst-1.3.1/.github/build-matrix.json
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-03 20:56:08.000000 libcst-1.3.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.099547 libcst-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-03 20:56:08.000000 libcst-1.3.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-03 20:56:08.000000 libcst-1.3.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-03 20:56:08.000000 libcst-1.3.1/.github/workflows/pypi_upload.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 20:56:08.000000 libcst-1.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-03 20:56:08.000000 libcst-1.3.1/.pyre_configuration
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-03 20:56:08.000000 libcst-1.3.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-03 20:56:08.000000 libcst-1.3.1/.watchmanconfig
+-rw-r--r--   0 runner    (1001) docker     (127)    40957 2024-04-03 20:56:08.000000 libcst-1.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-03 20:56:08.000000 libcst-1.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-03 20:56:08.000000 libcst-1.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-03 20:56:08.000000 libcst-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-03 20:56:08.000000 libcst-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17200 2024-04-03 20:57:16.171547 libcst-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-04-03 20:56:08.000000 libcst-1.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 20:56:08.000000 libcst-1.3.1/apt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 20:56:08.000000 libcst-1.3.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.087547 libcst-1.3.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.103547 libcst-1.3.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.103547 libcst-1.3.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.103547 libcst-1.3.1/docs/source/_static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   108465 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/_static/img/python_scopes.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30400 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/_static/img/python_scopes.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.103547 libcst-1.3.1/docs/source/_static/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/_static/logo/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/_static/logo/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/_static/logo/favicon_16px.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/_static/logo/favicon_32px.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/_static/logo/horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/_static/logo/horizontal_white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/_static/logo/horizontal_white_sidebar.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/_static/logo/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/_static/logo/icon_white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/_static/logo/vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/_static/logo/vertical_white.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.103547 libcst-1.3.1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/best_practices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/codemods.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/codemods_tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9553 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/experimental.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/matchers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/matchers_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/metadata_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/motivation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/nodes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/parser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/scope_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9873 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/visitors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-04-03 20:56:08.000000 libcst-1.3.1/docs/source/why_libcst.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.107547 libcst-1.3.1/libcst/
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_add_slots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_batched_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_flatten_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_maybe_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_metadata_dependent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.111547 libcst-1.3.1/libcst/_nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19437 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/deep_equals.py
+-rw-r--r--   0 runner    (1001) docker     (127)   141869 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31193 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/op.py
+-rw-r--r--   0 runner    (1001) docker     (127)   143870 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.119547 libcst-1.3.1/libcst/_nodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16051 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45724 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_await.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_binary_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_boolean_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22698 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17662 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_classdef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13640 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_cst_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_del.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_dict_comp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_else.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_empty_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_flatten_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7665 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_for.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97662 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_funcdef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_ifexp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29777 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_indented_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40904 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_leaf_small_statements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22302 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_matrix_multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_namedexpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_newline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_nonlocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_removal_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21237 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_simple_comp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13989 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_simple_statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_simple_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_simple_whitespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_small_statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16758 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_subscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_trailing_whitespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25792 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_try.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11237 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_type_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_unary_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_while.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13850 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_with.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/tests/test_yield.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_nodes/whitespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.123547 libcst-1.3.1/libcst/_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/base_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.123547 libcst-1.3.1/libcst/_parser/conversions/
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/conversions/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/conversions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53078 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/conversions/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/conversions/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13365 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/conversions/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47301 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/conversions/statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/conversions/terminals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/custom_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/detect_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/grammar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.123547 libcst-1.3.1/libcst/_parser/parso/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/parso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.123547 libcst-1.3.1/libcst/_parser/parso/pgen2/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/parso/pgen2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13727 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/parso/pgen2/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/parso/pgen2/grammar_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.123547 libcst-1.3.1/libcst/_parser/parso/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/parso/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/parso/python/py_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/parso/python/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44145 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/parso/python/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.123547 libcst-1.3.1/libcst/_parser/parso/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/parso/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/parso/tests/test_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/parso/tests/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/parso/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7565 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/parso/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/production_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/py_whitespace_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/python_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.127547 libcst-1.3.1/libcst/_parser/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14086 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/tests/test_detect_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/tests/test_footer_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/tests/test_node_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/tests/test_parse_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/tests/test_version_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9447 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/tests/test_whitespace_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83462 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/tests/test_wrapped_tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.127547 libcst-1.3.1/libcst/_parser/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/types/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/types/partials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/types/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/types/py_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/types/py_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/types/py_whitespace_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.127547 libcst-1.3.1/libcst/_parser/types/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/types/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/types/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/types/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/types/whitespace_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/whitespace_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_parser/wrapped_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_removal_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_type_enforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)   194662 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_typed_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_typed_visitor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 20:57:15.000000 libcst-1.3.1/libcst/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.131547 libcst-1.3.1/libcst/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codegen/gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codegen/gen_matcher_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codegen/gen_type_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codegen/gen_visitor_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codegen/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.131547 libcst-1.3.1/libcst/codegen/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codegen/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codegen/tests/test_codegen_clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codegen/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.131547 libcst-1.3.1/libcst/codemod/
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24326 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/_dummy_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/_visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.135547 libcst-1.3.1/libcst/codemod/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/add_pyre_directive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/add_trailing_commas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16027 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/convert_format_to_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/convert_namedtuple_to_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/convert_percent_format_to_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32486 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/convert_type_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/ensure_import_present.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/fix_pyre_directives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/noop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/remove_pyre_directive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16702 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/strip_strings_from_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.135547 libcst-1.3.1/libcst/codemod/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/tests/test_add_pyre_directive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/tests/test_add_trailing_commas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/tests/test_convert_format_to_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/tests/test_convert_namedtuple_to_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/tests/test_convert_percent_format_to_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13941 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/tests/test_convert_type_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/tests/test_ensure_import_present.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/tests/test_fix_pyre_directives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/tests/test_noop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/tests/test_remove_pyre_directive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/tests/test_remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15932 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/tests/test_strip_strings_from_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/tests/test_unnecessary_format_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/commands/unnecessary_format_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.139546 libcst-1.3.1/libcst/codemod/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/tests/codemod_formatter_error_input.py.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/tests/test_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/tests/test_codemod_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/tests/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.139546 libcst-1.3.1/libcst/codemod/visitors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19494 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/_add_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50925 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/_apply_type_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/_gather_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/_gather_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/_gather_global_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/_gather_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/_gather_string_annotation_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/_gather_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20494 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/_remove_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.139546 libcst-1.3.1/libcst/codemod/visitors/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23717 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/tests/test_add_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55792 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/tests/test_apply_type_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/tests/test_gather_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/tests/test_gather_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/tests/test_gather_global_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/tests/test_gather_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/tests/test_gather_string_annotation_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/tests/test_gather_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23816 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/codemod/visitors/tests/test_remove_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.143547 libcst-1.3.1/libcst/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19403 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/helpers/_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/helpers/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/helpers/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/helpers/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.143547 libcst-1.3.1/libcst/helpers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/helpers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/helpers/tests/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10669 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/helpers/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/helpers/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11776 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/helpers/tests/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.143547 libcst-1.3.1/libcst/matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)   561418 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/matchers/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79068 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/matchers/_matcher_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10414 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/matchers/_return_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34453 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/matchers/_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.147547 libcst-1.3.1/libcst/matchers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/matchers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35211 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/matchers/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15761 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/matchers/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/matchers/tests/test_findall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53908 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/matchers/tests/test_matchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23189 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/matchers/tests/test_matchers_with_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/matchers/tests/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20190 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/matchers/tests/test_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.147547 libcst-1.3.1/libcst/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/accessor_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/expression_context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/file_path_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/full_repo_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/name_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/parent_node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/position_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/reentrant_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47962 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/scope_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/span_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.151547 libcst-1.3.1/libcst/metadata/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/tests/test_accessor_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/tests/test_base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/tests/test_expression_context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/tests/test_file_path_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/tests/test_full_repo_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/tests/test_metadata_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/tests/test_metadata_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19965 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/tests/test_name_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/tests/test_parent_node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/tests/test_position_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/tests/test_reentrant_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86437 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/tests/test_scope_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/tests/test_span_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/tests/test_type_inference_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/type_inference_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/metadata/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.151547 libcst-1.3.1/libcst/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.155547 libcst-1.3.1/libcst/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tests/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.155547 libcst-1.3.1/libcst/tests/pyre/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tests/pyre/.pyre_configuration
+-rw-r--r--   0 runner    (1001) docker     (127)     9016 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tests/pyre/simple_class.json
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tests/pyre/simple_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tests/test_add_slots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tests/test_batched_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tests/test_deep_clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tests/test_deep_replace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tests/test_fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tests/test_pyre_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tests/test_roundtrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tests/test_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25736 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tests/test_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tests/test_type_enforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tests/test_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31443 2024-04-03 20:56:08.000000 libcst-1.3.1/libcst/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.171547 libcst-1.3.1/libcst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17200 2024-04-03 20:57:15.000000 libcst-1.3.1/libcst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16090 2024-04-03 20:57:16.000000 libcst-1.3.1/libcst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:57:15.000000 libcst-1.3.1/libcst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:57:15.000000 libcst-1.3.1/libcst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-03 20:57:15.000000 libcst-1.3.1/libcst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 20:57:15.000000 libcst-1.3.1/libcst.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.155547 libcst-1.3.1/native/
+-rw-r--r--   0 runner    (1001) docker     (127)    26565 2024-04-03 20:56:08.000000 libcst-1.3.1/native/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 20:56:08.000000 libcst-1.3.1/native/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.155547 libcst-1.3.1/native/libcst/
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    32411 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/Grammar
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.155547 libcst-1.3.1/native/libcst/benches/
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/benches/parser_benchmark.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.155547 libcst-1.3.1/native/libcst/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/bin.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.159546 libcst-1.3.1/native/libcst/src/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/nodes/codegen.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    80129 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/nodes/expression.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/nodes/inflate_helpers.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/nodes/macros.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/nodes/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/nodes/module.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    50731 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/nodes/op.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/nodes/parser_config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/nodes/py_cached.rs
+-rw-r--r--   0 runner    (1001) docker     (127)   113875 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/nodes/statement.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/nodes/test_utils.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/nodes/traits.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/nodes/whitespace.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.159546 libcst-1.3.1/native/libcst/src/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/parser/errors.rs
+-rw-r--r--   0 runner    (1001) docker     (127)   113160 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/parser/grammar.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/parser/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/parser/numbers.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/py.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.159546 libcst-1.3.1/native/libcst/src/tokenizer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.159546 libcst-1.3.1/native/libcst/src/tokenizer/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/tokenizer/core/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/tokenizer/core/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    49168 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/tokenizer/core/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/tokenizer/core/string_types.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/tokenizer/debug_utils.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/tokenizer/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/tokenizer/operators.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    23922 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/tokenizer/tests.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.159546 libcst-1.3.1/native/libcst/src/tokenizer/text_position/
+-rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/tokenizer/text_position/char_width.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/tokenizer/text_position/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    16117 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/src/tokenizer/whitespace_parser.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.159546 libcst-1.3.1/native/libcst/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.167547 libcst-1.3.1/native/libcst/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/big_binary_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/class_craziness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/dangling_indent.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/decorated_function_without_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/dysfunctional_del.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/expr_statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/fun_with_func_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/global_nonlocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/import.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/indents_but_no_eol_before_eof.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/just_a_comment_without_nl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/malicious_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/mixed_newlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/pep646.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/smol_statements.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/spacious_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/starry_tries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/suicidal_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/super_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/terrible_tries.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/trailing_comment_without_nl.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/trailing_whitespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/tuple_shenanigans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/type_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/vast_emptiness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/with_wickedness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/fixtures/wonky_walrus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst/tests/parser_roundtrip.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.167547 libcst-1.3.1/native/libcst_derive/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst_derive/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst_derive/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.167547 libcst-1.3.1/native/libcst_derive/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst_derive/src/codegen.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst_derive/src/cstnode.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst_derive/src/inflate.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst_derive/src/into_py.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst_derive/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst_derive/src/parenthesized_node.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.095547 libcst-1.3.1/native/libcst_derive/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.167547 libcst-1.3.1/native/libcst_derive/tests/pass/
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst_derive/tests/pass/minimal_cst.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-03 20:56:08.000000 libcst-1.3.1/native/libcst_derive/tests/pass/simple.rs
+-rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-04-03 20:56:08.000000 libcst-1.3.1/native/roundtrip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-03 20:56:08.000000 libcst-1.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.167547 libcst-1.3.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-03 20:56:08.000000 libcst-1.3.1/scripts/check_copyright.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-03 20:56:08.000000 libcst-1.3.1/scripts/regenerate-fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:57:16.175547 libcst-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-03 20:56:08.000000 libcst-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.167547 libcst-1.3.1/stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 20:56:08.000000 libcst-1.3.1/stubs/hypothesis.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 20:56:08.000000 libcst-1.3.1/stubs/hypothesmith.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.167547 libcst-1.3.1/stubs/libcst/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-03 20:56:08.000000 libcst-1.3.1/stubs/libcst/native.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:57:16.171547 libcst-1.3.1/stubs/libcst_native/
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-03 20:56:08.000000 libcst-1.3.1/stubs/libcst_native/parser_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-03 20:56:08.000000 libcst-1.3.1/stubs/libcst_native/token_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-03 20:56:08.000000 libcst-1.3.1/stubs/libcst_native/tokenize.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-03 20:56:08.000000 libcst-1.3.1/stubs/libcst_native/whitespace_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-03 20:56:08.000000 libcst-1.3.1/stubs/libcst_native/whitespace_state.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 20:56:08.000000 libcst-1.3.1/stubs/setuptools.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-03 20:56:08.000000 libcst-1.3.1/stubs/tokenize.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 20:56:08.000000 libcst-1.3.1/stubs/typing_inspect.pyi
```

### Comparing `libcst-1.3.0/.flake8` & `libcst-1.3.1/.flake8`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/.github/build-matrix.json` & `libcst-1.3.1/.github/build-matrix.json`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/.github/workflows/build.yml` & `libcst-1.3.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/.github/workflows/ci.yml` & `libcst-1.3.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/.github/workflows/pypi_upload.yml` & `libcst-1.3.1/.github/workflows/pypi_upload.yml`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/CHANGELOG.md` & `libcst-1.3.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# 1.3.1 - 2024-04-03
+
+## Fixed
+* ImportError due to missing `mypy_extensions` dependency by @zsol in https://github.com/Instagram/LibCST/pull/1128
+
 # 1.3.0 - 2024-04-03
 
 ## Updated
 * Removed dependencies on `typing_extensions` and `typing_inspect` by @zsol in https://github.com/Instagram/LibCST/pull/1126
 
 # 1.2.0 - 2024-02-19
```

### Comparing `libcst-1.3.0/CODE_OF_CONDUCT.md` & `libcst-1.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/CONTRIBUTING.md` & `libcst-1.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/LICENSE` & `libcst-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/PKG-INFO` & `libcst-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libcst
-Version: 1.3.0
+Version: 1.3.1
 Summary: A concrete syntax tree with AST-like properties for Python 3.0 through 3.12 programs.
 License: All contributions towards LibCST are MIT licensed.
         
         Some Python files have been derived from the standard library and are therefore
         PSF licensed. Modifications on these files are dual licensed (both MIT and
         PSF). These files are:
```

### Comparing `libcst-1.3.0/README.rst` & `libcst-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/_static/img/python_scopes.png` & `libcst-1.3.1/docs/source/_static/img/python_scopes.png`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/_static/img/python_scopes.svg` & `libcst-1.3.1/docs/source/_static/img/python_scopes.svg`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/_static/logo/favicon.ico` & `libcst-1.3.1/docs/source/_static/logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/_static/logo/favicon.svg` & `libcst-1.3.1/docs/source/_static/logo/favicon.svg`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/_static/logo/favicon_16px.png` & `libcst-1.3.1/docs/source/_static/logo/favicon_16px.png`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/_static/logo/favicon_32px.png` & `libcst-1.3.1/docs/source/_static/logo/favicon_32px.png`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/_static/logo/horizontal.svg` & `libcst-1.3.1/docs/source/_static/logo/horizontal.svg`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/_static/logo/horizontal_white.svg` & `libcst-1.3.1/docs/source/_static/logo/horizontal_white.svg`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/_static/logo/horizontal_white_sidebar.png` & `libcst-1.3.1/docs/source/_static/logo/horizontal_white_sidebar.png`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/_static/logo/icon.svg` & `libcst-1.3.1/docs/source/_static/logo/icon.svg`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/_static/logo/icon_white.svg` & `libcst-1.3.1/docs/source/_static/logo/icon_white.svg`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/_static/logo/vertical.svg` & `libcst-1.3.1/docs/source/_static/logo/vertical.svg`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/_static/logo/vertical_white.svg` & `libcst-1.3.1/docs/source/_static/logo/vertical_white.svg`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/best_practices.rst` & `libcst-1.3.1/docs/source/best_practices.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/codemods.rst` & `libcst-1.3.1/docs/source/codemods.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/codemods_tutorial.rst` & `libcst-1.3.1/docs/source/codemods_tutorial.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/conf.py` & `libcst-1.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/helpers.rst` & `libcst-1.3.1/docs/source/helpers.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/index.rst` & `libcst-1.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/matchers.rst` & `libcst-1.3.1/docs/source/matchers.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/matchers_tutorial.ipynb` & `libcst-1.3.1/docs/source/matchers_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/metadata.rst` & `libcst-1.3.1/docs/source/metadata.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/metadata_tutorial.ipynb` & `libcst-1.3.1/docs/source/metadata_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/motivation.rst` & `libcst-1.3.1/docs/source/motivation.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/nodes.rst` & `libcst-1.3.1/docs/source/nodes.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/parser.rst` & `libcst-1.3.1/docs/source/parser.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/scope_tutorial.ipynb` & `libcst-1.3.1/docs/source/scope_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/tutorial.ipynb` & `libcst-1.3.1/docs/source/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/visitors.rst` & `libcst-1.3.1/docs/source/visitors.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/docs/source/why_libcst.rst` & `libcst-1.3.1/docs/source/why_libcst.rst`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/__init__.py` & `libcst-1.3.1/libcst/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_add_slots.py` & `libcst-1.3.1/libcst/_add_slots.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_batched_visitor.py` & `libcst-1.3.1/libcst/_batched_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_exceptions.py` & `libcst-1.3.1/libcst/_exceptions.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_flatten_sentinel.py` & `libcst-1.3.1/libcst/_flatten_sentinel.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_maybe_sentinel.py` & `libcst-1.3.1/libcst/_maybe_sentinel.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_metadata_dependent.py` & `libcst-1.3.1/libcst/_metadata_dependent.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/base.py` & `libcst-1.3.1/libcst/_nodes/base.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/deep_equals.py` & `libcst-1.3.1/libcst/_nodes/deep_equals.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/expression.py` & `libcst-1.3.1/libcst/_nodes/expression.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/internal.py` & `libcst-1.3.1/libcst/_nodes/internal.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/module.py` & `libcst-1.3.1/libcst/_nodes/module.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/op.py` & `libcst-1.3.1/libcst/_nodes/op.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/statement.py` & `libcst-1.3.1/libcst/_nodes/statement.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/base.py` & `libcst-1.3.1/libcst/_nodes/tests/base.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_assert.py` & `libcst-1.3.1/libcst/_nodes/tests/test_assert.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_assign.py` & `libcst-1.3.1/libcst/_nodes/tests/test_assign.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_atom.py` & `libcst-1.3.1/libcst/_nodes/tests/test_atom.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_attribute.py` & `libcst-1.3.1/libcst/_nodes/tests/test_attribute.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_await.py` & `libcst-1.3.1/libcst/_nodes/tests/test_await.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_binary_op.py` & `libcst-1.3.1/libcst/_nodes/tests/test_binary_op.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_boolean_op.py` & `libcst-1.3.1/libcst/_nodes/tests/test_boolean_op.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_call.py` & `libcst-1.3.1/libcst/_nodes/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_classdef.py` & `libcst-1.3.1/libcst/_nodes/tests/test_classdef.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_comment.py` & `libcst-1.3.1/libcst/_nodes/tests/test_comment.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_comparison.py` & `libcst-1.3.1/libcst/_nodes/tests/test_comparison.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_cst_node.py` & `libcst-1.3.1/libcst/_nodes/tests/test_cst_node.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_del.py` & `libcst-1.3.1/libcst/_nodes/tests/test_del.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_dict.py` & `libcst-1.3.1/libcst/_nodes/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_dict_comp.py` & `libcst-1.3.1/libcst/_nodes/tests/test_dict_comp.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_docstring.py` & `libcst-1.3.1/libcst/_nodes/tests/test_docstring.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_else.py` & `libcst-1.3.1/libcst/_nodes/tests/test_else.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_empty_line.py` & `libcst-1.3.1/libcst/_nodes/tests/test_empty_line.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_flatten_behavior.py` & `libcst-1.3.1/libcst/_nodes/tests/test_flatten_behavior.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_for.py` & `libcst-1.3.1/libcst/_nodes/tests/test_for.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_funcdef.py` & `libcst-1.3.1/libcst/_nodes/tests/test_funcdef.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_global.py` & `libcst-1.3.1/libcst/_nodes/tests/test_global.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_if.py` & `libcst-1.3.1/libcst/_nodes/tests/test_if.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_ifexp.py` & `libcst-1.3.1/libcst/_nodes/tests/test_ifexp.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_import.py` & `libcst-1.3.1/libcst/_nodes/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_indented_block.py` & `libcst-1.3.1/libcst/_nodes/tests/test_indented_block.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_lambda.py` & `libcst-1.3.1/libcst/_nodes/tests/test_lambda.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_leaf_small_statements.py` & `libcst-1.3.1/libcst/_nodes/tests/test_leaf_small_statements.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_list.py` & `libcst-1.3.1/libcst/_nodes/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_match.py` & `libcst-1.3.1/libcst/_nodes/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_matrix_multiply.py` & `libcst-1.3.1/libcst/_nodes/tests/test_matrix_multiply.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_module.py` & `libcst-1.3.1/libcst/_nodes/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_namedexpr.py` & `libcst-1.3.1/libcst/_nodes/tests/test_namedexpr.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_newline.py` & `libcst-1.3.1/libcst/_nodes/tests/test_newline.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_nonlocal.py` & `libcst-1.3.1/libcst/_nodes/tests/test_nonlocal.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_number.py` & `libcst-1.3.1/libcst/_nodes/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_raise.py` & `libcst-1.3.1/libcst/_nodes/tests/test_raise.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_removal_behavior.py` & `libcst-1.3.1/libcst/_nodes/tests/test_removal_behavior.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_return.py` & `libcst-1.3.1/libcst/_nodes/tests/test_return.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_set.py` & `libcst-1.3.1/libcst/_nodes/tests/test_set.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_simple_comp.py` & `libcst-1.3.1/libcst/_nodes/tests/test_simple_comp.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_simple_statement.py` & `libcst-1.3.1/libcst/_nodes/tests/test_simple_statement.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_simple_string.py` & `libcst-1.3.1/libcst/_nodes/tests/test_simple_string.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_simple_whitespace.py` & `libcst-1.3.1/libcst/_nodes/tests/test_simple_whitespace.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_small_statement.py` & `libcst-1.3.1/libcst/_nodes/tests/test_small_statement.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_subscript.py` & `libcst-1.3.1/libcst/_nodes/tests/test_subscript.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_trailing_whitespace.py` & `libcst-1.3.1/libcst/_nodes/tests/test_trailing_whitespace.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_try.py` & `libcst-1.3.1/libcst/_nodes/tests/test_try.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_tuple.py` & `libcst-1.3.1/libcst/_nodes/tests/test_tuple.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_type_alias.py` & `libcst-1.3.1/libcst/_nodes/tests/test_type_alias.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_unary_op.py` & `libcst-1.3.1/libcst/_nodes/tests/test_unary_op.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_while.py` & `libcst-1.3.1/libcst/_nodes/tests/test_while.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_with.py` & `libcst-1.3.1/libcst/_nodes/tests/test_with.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/tests/test_yield.py` & `libcst-1.3.1/libcst/_nodes/tests/test_yield.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_nodes/whitespace.py` & `libcst-1.3.1/libcst/_nodes/whitespace.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/base_parser.py` & `libcst-1.3.1/libcst/_parser/base_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/conversions/README.md` & `libcst-1.3.1/libcst/_parser/conversions/README.md`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/conversions/expression.py` & `libcst-1.3.1/libcst/_parser/conversions/expression.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/conversions/module.py` & `libcst-1.3.1/libcst/_parser/conversions/module.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/conversions/params.py` & `libcst-1.3.1/libcst/_parser/conversions/params.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/conversions/statement.py` & `libcst-1.3.1/libcst/_parser/conversions/statement.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/conversions/terminals.py` & `libcst-1.3.1/libcst/_parser/conversions/terminals.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/custom_itertools.py` & `libcst-1.3.1/libcst/_parser/custom_itertools.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/detect_config.py` & `libcst-1.3.1/libcst/_parser/detect_config.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/entrypoints.py` & `libcst-1.3.1/libcst/_parser/entrypoints.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/grammar.py` & `libcst-1.3.1/libcst/_parser/grammar.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/parso/pgen2/generator.py` & `libcst-1.3.1/libcst/_parser/parso/pgen2/generator.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/parso/pgen2/grammar_parser.py` & `libcst-1.3.1/libcst/_parser/parso/pgen2/grammar_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/parso/python/py_token.py` & `libcst-1.3.1/libcst/_parser/parso/python/py_token.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/parso/python/token.py` & `libcst-1.3.1/libcst/_parser/parso/python/token.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/parso/python/tokenize.py` & `libcst-1.3.1/libcst/_parser/parso/python/tokenize.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/parso/tests/test_fstring.py` & `libcst-1.3.1/libcst/_parser/parso/tests/test_fstring.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/parso/tests/test_tokenize.py` & `libcst-1.3.1/libcst/_parser/parso/tests/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/parso/tests/test_utils.py` & `libcst-1.3.1/libcst/_parser/parso/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/parso/utils.py` & `libcst-1.3.1/libcst/_parser/parso/utils.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/production_decorator.py` & `libcst-1.3.1/libcst/_parser/production_decorator.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/py_whitespace_parser.py` & `libcst-1.3.1/libcst/_parser/py_whitespace_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/python_parser.py` & `libcst-1.3.1/libcst/_parser/python_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/tests/test_config.py` & `libcst-1.3.1/libcst/_parser/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/tests/test_detect_config.py` & `libcst-1.3.1/libcst/_parser/tests/test_detect_config.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/tests/test_footer_behavior.py` & `libcst-1.3.1/libcst/_parser/tests/test_footer_behavior.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/tests/test_node_identity.py` & `libcst-1.3.1/libcst/_parser/tests/test_node_identity.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/tests/test_parse_errors.py` & `libcst-1.3.1/libcst/_parser/tests/test_parse_errors.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/tests/test_version_compare.py` & `libcst-1.3.1/libcst/_parser/tests/test_version_compare.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/tests/test_whitespace_parser.py` & `libcst-1.3.1/libcst/_parser/tests/test_whitespace_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/tests/test_wrapped_tokenize.py` & `libcst-1.3.1/libcst/_parser/tests/test_wrapped_tokenize.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/types/config.py` & `libcst-1.3.1/libcst/_parser/types/config.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/types/conversions.py` & `libcst-1.3.1/libcst/_parser/types/conversions.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/types/partials.py` & `libcst-1.3.1/libcst/_parser/types/partials.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/types/py_config.py` & `libcst-1.3.1/libcst/_parser/types/py_config.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/types/py_token.py` & `libcst-1.3.1/libcst/_parser/types/py_token.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/types/py_whitespace_state.py` & `libcst-1.3.1/libcst/_parser/types/py_whitespace_state.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/types/tests/test_config.py` & `libcst-1.3.1/libcst/_parser/types/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/whitespace_parser.py` & `libcst-1.3.1/libcst/_parser/whitespace_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_parser/wrapped_tokenize.py` & `libcst-1.3.1/libcst/_parser/wrapped_tokenize.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_position.py` & `libcst-1.3.1/libcst/_position.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_removal_sentinel.py` & `libcst-1.3.1/libcst/_removal_sentinel.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_tabs.py` & `libcst-1.3.1/libcst/_tabs.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_type_enforce.py` & `libcst-1.3.1/libcst/_type_enforce.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_typed_visitor.py` & `libcst-1.3.1/libcst/_typed_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_typed_visitor_base.py` & `libcst-1.3.1/libcst/_typed_visitor_base.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/_visitors.py` & `libcst-1.3.1/libcst/_visitors.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codegen/gather.py` & `libcst-1.3.1/libcst/codegen/gather.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codegen/gen_matcher_classes.py` & `libcst-1.3.1/libcst/codegen/gen_matcher_classes.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codegen/gen_type_mapping.py` & `libcst-1.3.1/libcst/codegen/gen_type_mapping.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codegen/gen_visitor_functions.py` & `libcst-1.3.1/libcst/codegen/gen_visitor_functions.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codegen/generate.py` & `libcst-1.3.1/libcst/codegen/generate.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codegen/tests/test_codegen_clean.py` & `libcst-1.3.1/libcst/codegen/tests/test_codegen_clean.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codegen/transforms.py` & `libcst-1.3.1/libcst/codegen/transforms.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/__init__.py` & `libcst-1.3.1/libcst/codemod/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/_cli.py` & `libcst-1.3.1/libcst/codemod/_cli.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/_codemod.py` & `libcst-1.3.1/libcst/codemod/_codemod.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/_command.py` & `libcst-1.3.1/libcst/codemod/_command.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/_context.py` & `libcst-1.3.1/libcst/codemod/_context.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/_dummy_pool.py` & `libcst-1.3.1/libcst/codemod/_dummy_pool.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/_runner.py` & `libcst-1.3.1/libcst/codemod/_runner.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/_testing.py` & `libcst-1.3.1/libcst/codemod/_testing.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/_visitor.py` & `libcst-1.3.1/libcst/codemod/_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/add_pyre_directive.py` & `libcst-1.3.1/libcst/codemod/commands/add_pyre_directive.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/add_trailing_commas.py` & `libcst-1.3.1/libcst/codemod/commands/add_trailing_commas.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/convert_format_to_fstring.py` & `libcst-1.3.1/libcst/codemod/commands/convert_format_to_fstring.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/convert_namedtuple_to_dataclass.py` & `libcst-1.3.1/libcst/codemod/commands/convert_namedtuple_to_dataclass.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/convert_percent_format_to_fstring.py` & `libcst-1.3.1/libcst/codemod/commands/convert_percent_format_to_fstring.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/convert_type_comments.py` & `libcst-1.3.1/libcst/codemod/commands/convert_type_comments.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/ensure_import_present.py` & `libcst-1.3.1/libcst/codemod/commands/ensure_import_present.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/fix_pyre_directives.py` & `libcst-1.3.1/libcst/codemod/commands/fix_pyre_directives.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/remove_pyre_directive.py` & `libcst-1.3.1/libcst/codemod/commands/remove_pyre_directive.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/remove_unused_imports.py` & `libcst-1.3.1/libcst/codemod/commands/remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/rename.py` & `libcst-1.3.1/libcst/codemod/commands/rename.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/strip_strings_from_types.py` & `libcst-1.3.1/libcst/codemod/commands/strip_strings_from_types.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/tests/test_add_pyre_directive.py` & `libcst-1.3.1/libcst/codemod/commands/tests/test_add_pyre_directive.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/tests/test_add_trailing_commas.py` & `libcst-1.3.1/libcst/codemod/commands/tests/test_add_trailing_commas.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/tests/test_convert_format_to_fstring.py` & `libcst-1.3.1/libcst/codemod/commands/tests/test_convert_format_to_fstring.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/tests/test_convert_namedtuple_to_dataclass.py` & `libcst-1.3.1/libcst/codemod/commands/tests/test_convert_namedtuple_to_dataclass.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/tests/test_convert_percent_format_to_fstring.py` & `libcst-1.3.1/libcst/codemod/commands/tests/test_convert_percent_format_to_fstring.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/tests/test_convert_type_comments.py` & `libcst-1.3.1/libcst/codemod/commands/tests/test_convert_type_comments.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/tests/test_ensure_import_present.py` & `libcst-1.3.1/libcst/codemod/commands/tests/test_ensure_import_present.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/tests/test_fix_pyre_directives.py` & `libcst-1.3.1/libcst/codemod/commands/tests/test_fix_pyre_directives.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/tests/test_noop.py` & `libcst-1.3.1/libcst/codemod/commands/tests/test_noop.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/tests/test_remove_pyre_directive.py` & `libcst-1.3.1/libcst/codemod/commands/tests/test_remove_pyre_directive.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/tests/test_remove_unused_imports.py` & `libcst-1.3.1/libcst/codemod/commands/tests/test_remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/tests/test_rename.py` & `libcst-1.3.1/libcst/codemod/commands/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/tests/test_strip_strings_from_types.py` & `libcst-1.3.1/libcst/codemod/commands/tests/test_strip_strings_from_types.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/tests/test_unnecessary_format_string.py` & `libcst-1.3.1/libcst/codemod/commands/tests/test_unnecessary_format_string.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/commands/unnecessary_format_string.py` & `libcst-1.3.1/libcst/codemod/commands/unnecessary_format_string.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/tests/test_codemod.py` & `libcst-1.3.1/libcst/codemod/tests/test_codemod.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/tests/test_codemod_cli.py` & `libcst-1.3.1/libcst/codemod/tests/test_codemod_cli.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/tests/test_metadata.py` & `libcst-1.3.1/libcst/codemod/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/tests/test_runner.py` & `libcst-1.3.1/libcst/codemod/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/__init__.py` & `libcst-1.3.1/libcst/codemod/visitors/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/_add_imports.py` & `libcst-1.3.1/libcst/codemod/visitors/_add_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/_apply_type_annotations.py` & `libcst-1.3.1/libcst/codemod/visitors/_apply_type_annotations.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/_gather_comments.py` & `libcst-1.3.1/libcst/codemod/visitors/_gather_comments.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/_gather_exports.py` & `libcst-1.3.1/libcst/codemod/visitors/_gather_exports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/_gather_global_names.py` & `libcst-1.3.1/libcst/codemod/visitors/_gather_global_names.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/_gather_imports.py` & `libcst-1.3.1/libcst/codemod/visitors/_gather_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/_gather_string_annotation_names.py` & `libcst-1.3.1/libcst/codemod/visitors/_gather_string_annotation_names.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/_gather_unused_imports.py` & `libcst-1.3.1/libcst/codemod/visitors/_gather_unused_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/_imports.py` & `libcst-1.3.1/libcst/codemod/visitors/_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/_remove_imports.py` & `libcst-1.3.1/libcst/codemod/visitors/_remove_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/tests/test_add_imports.py` & `libcst-1.3.1/libcst/codemod/visitors/tests/test_add_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/tests/test_apply_type_annotations.py` & `libcst-1.3.1/libcst/codemod/visitors/tests/test_apply_type_annotations.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/tests/test_gather_comments.py` & `libcst-1.3.1/libcst/codemod/visitors/tests/test_gather_comments.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/tests/test_gather_exports.py` & `libcst-1.3.1/libcst/codemod/visitors/tests/test_gather_exports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/tests/test_gather_global_names.py` & `libcst-1.3.1/libcst/codemod/visitors/tests/test_gather_global_names.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/tests/test_gather_imports.py` & `libcst-1.3.1/libcst/codemod/visitors/tests/test_gather_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/tests/test_gather_string_annotation_names.py` & `libcst-1.3.1/libcst/codemod/visitors/tests/test_gather_string_annotation_names.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/tests/test_gather_unused_imports.py` & `libcst-1.3.1/libcst/codemod/visitors/tests/test_gather_unused_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/codemod/visitors/tests/test_remove_imports.py` & `libcst-1.3.1/libcst/codemod/visitors/tests/test_remove_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/helpers/__init__.py` & `libcst-1.3.1/libcst/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/helpers/_template.py` & `libcst-1.3.1/libcst/helpers/_template.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/helpers/common.py` & `libcst-1.3.1/libcst/helpers/common.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/helpers/expression.py` & `libcst-1.3.1/libcst/helpers/expression.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/helpers/module.py` & `libcst-1.3.1/libcst/helpers/module.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/helpers/paths.py` & `libcst-1.3.1/libcst/helpers/paths.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/helpers/tests/test_expression.py` & `libcst-1.3.1/libcst/helpers/tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/helpers/tests/test_module.py` & `libcst-1.3.1/libcst/helpers/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/helpers/tests/test_paths.py` & `libcst-1.3.1/libcst/helpers/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/helpers/tests/test_template.py` & `libcst-1.3.1/libcst/helpers/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/matchers/__init__.py` & `libcst-1.3.1/libcst/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/matchers/_decorators.py` & `libcst-1.3.1/libcst/matchers/_decorators.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/matchers/_matcher_base.py` & `libcst-1.3.1/libcst/matchers/_matcher_base.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/matchers/_return_types.py` & `libcst-1.3.1/libcst/matchers/_return_types.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/matchers/_visitors.py` & `libcst-1.3.1/libcst/matchers/_visitors.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/matchers/tests/test_decorators.py` & `libcst-1.3.1/libcst/matchers/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/matchers/tests/test_extract.py` & `libcst-1.3.1/libcst/matchers/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/matchers/tests/test_findall.py` & `libcst-1.3.1/libcst/matchers/tests/test_findall.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/matchers/tests/test_matchers.py` & `libcst-1.3.1/libcst/matchers/tests/test_matchers.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/matchers/tests/test_matchers_with_metadata.py` & `libcst-1.3.1/libcst/matchers/tests/test_matchers_with_metadata.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/matchers/tests/test_replace.py` & `libcst-1.3.1/libcst/matchers/tests/test_replace.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/matchers/tests/test_visitors.py` & `libcst-1.3.1/libcst/matchers/tests/test_visitors.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/__init__.py` & `libcst-1.3.1/libcst/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/accessor_provider.py` & `libcst-1.3.1/libcst/metadata/accessor_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/base_provider.py` & `libcst-1.3.1/libcst/metadata/base_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/expression_context_provider.py` & `libcst-1.3.1/libcst/metadata/expression_context_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/file_path_provider.py` & `libcst-1.3.1/libcst/metadata/file_path_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/full_repo_manager.py` & `libcst-1.3.1/libcst/metadata/full_repo_manager.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/name_provider.py` & `libcst-1.3.1/libcst/metadata/name_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/parent_node_provider.py` & `libcst-1.3.1/libcst/metadata/parent_node_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/position_provider.py` & `libcst-1.3.1/libcst/metadata/position_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/reentrant_codegen.py` & `libcst-1.3.1/libcst/metadata/reentrant_codegen.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/scope_provider.py` & `libcst-1.3.1/libcst/metadata/scope_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/span_provider.py` & `libcst-1.3.1/libcst/metadata/span_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/tests/test_accessor_provider.py` & `libcst-1.3.1/libcst/metadata/tests/test_accessor_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/tests/test_base_provider.py` & `libcst-1.3.1/libcst/metadata/tests/test_base_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/tests/test_expression_context_provider.py` & `libcst-1.3.1/libcst/metadata/tests/test_expression_context_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/tests/test_file_path_provider.py` & `libcst-1.3.1/libcst/metadata/tests/test_file_path_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/tests/test_full_repo_manager.py` & `libcst-1.3.1/libcst/metadata/tests/test_full_repo_manager.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/tests/test_metadata_provider.py` & `libcst-1.3.1/libcst/metadata/tests/test_metadata_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/tests/test_metadata_wrapper.py` & `libcst-1.3.1/libcst/metadata/tests/test_metadata_wrapper.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/tests/test_name_provider.py` & `libcst-1.3.1/libcst/metadata/tests/test_name_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/tests/test_parent_node_provider.py` & `libcst-1.3.1/libcst/metadata/tests/test_parent_node_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/tests/test_position_provider.py` & `libcst-1.3.1/libcst/metadata/tests/test_position_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/tests/test_reentrant_codegen.py` & `libcst-1.3.1/libcst/metadata/tests/test_reentrant_codegen.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/tests/test_scope_provider.py` & `libcst-1.3.1/libcst/metadata/tests/test_scope_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/tests/test_span_provider.py` & `libcst-1.3.1/libcst/metadata/tests/test_span_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/tests/test_type_inference_provider.py` & `libcst-1.3.1/libcst/metadata/tests/test_type_inference_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/metadata/type_inference_provider.py` & `libcst-1.3.1/libcst/metadata/type_inference_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import json
 import subprocess
 from pathlib import Path
-from typing import Dict, List, Mapping, Optional, Sequence, Tuple
-
-from mypy_extensions import TypedDict
+from typing import Dict, List, Mapping, Optional, Sequence, Tuple, TypedDict
 
 import libcst as cst
 from libcst._position import CodePosition, CodeRange
 from libcst.metadata.base_provider import BatchableMetadataProvider
 from libcst.metadata.position_provider import PositionProvider
```

### Comparing `libcst-1.3.0/libcst/metadata/wrapper.py` & `libcst-1.3.1/libcst/metadata/wrapper.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/testing/utils.py` & `libcst-1.3.1/libcst/testing/utils.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/tests/pyre/simple_class.json` & `libcst-1.3.1/libcst/tests/pyre/simple_class.json`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/tests/pyre/simple_class.py` & `libcst-1.3.1/libcst/tests/pyre/simple_class.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/tests/test_add_slots.py` & `libcst-1.3.1/libcst/tests/test_add_slots.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/tests/test_batched_visitor.py` & `libcst-1.3.1/libcst/tests/test_batched_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/tests/test_deep_clone.py` & `libcst-1.3.1/libcst/tests/test_deep_clone.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/tests/test_deep_replace.py` & `libcst-1.3.1/libcst/tests/test_deep_replace.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/tests/test_e2e.py` & `libcst-1.3.1/libcst/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/tests/test_exceptions.py` & `libcst-1.3.1/libcst/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/tests/test_fuzz.py` & `libcst-1.3.1/libcst/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/tests/test_pyre_integration.py` & `libcst-1.3.1/libcst/tests/test_pyre_integration.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/tests/test_roundtrip.py` & `libcst-1.3.1/libcst/tests/test_roundtrip.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/tests/test_tabs.py` & `libcst-1.3.1/libcst/tests/test_tabs.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/tests/test_tool.py` & `libcst-1.3.1/libcst/tests/test_tool.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/tests/test_type_enforce.py` & `libcst-1.3.1/libcst/tests/test_type_enforce.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/tests/test_visitor.py` & `libcst-1.3.1/libcst/tests/test_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst/tool.py` & `libcst-1.3.1/libcst/tool.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/libcst.egg-info/PKG-INFO` & `libcst-1.3.1/libcst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libcst
-Version: 1.3.0
+Version: 1.3.1
 Summary: A concrete syntax tree with AST-like properties for Python 3.0 through 3.12 programs.
 License: All contributions towards LibCST are MIT licensed.
         
         Some Python files have been derived from the standard library and are therefore
         PSF licensed. Modifications on these files are dual licensed (both MIT and
         PSF). These files are:
```

### Comparing `libcst-1.3.0/libcst.egg-info/SOURCES.txt` & `libcst-1.3.1/libcst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/Cargo.lock` & `libcst-1.3.1/native/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
 name = "libc"
 version = "0.2.149"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a08173bc88b7955d1b3145aa561539096c421ac8debde8cbc3612ec635fee29b"
 
 [[package]]
 name = "libcst"
-version = "1.3.0"
+version = "1.3.1"
 dependencies = [
  "chic",
  "criterion",
  "difference",
  "itertools 0.11.0",
  "libcst_derive",
  "memchr",
@@ -369,15 +369,15 @@
  "rayon",
  "regex",
  "thiserror",
 ]
 
 [[package]]
 name = "libcst_derive"
-version = "1.3.0"
+version = "1.3.1"
 dependencies = [
  "quote",
  "syn 2.0.41",
  "trybuild",
 ]
 
 [[package]]
```

### Comparing `libcst-1.3.0/native/libcst/Cargo.toml` & `libcst-1.3.1/native/libcst/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 [package]
 name = "libcst"
-version = "1.3.0"
+version = "1.3.1"
 authors = ["LibCST Developers"]
 edition = "2018"
 rust-version = "1.70"
 description = "A Python parser and Concrete Syntax Tree library."
 license-file = "LICENSE"
 repository = "https://github.com/Instagram/LibCST"
 documentation = "https://libcst.rtfd.org"
@@ -38,15 +38,15 @@
 paste = "1.0.9"
 pyo3 = { version = "0.20", optional = true }
 thiserror = "1.0.37"
 peg = "0.8.1"
 chic = "1.2.2"
 regex = "1.9.3"
 memchr = "2.5.0"
-libcst_derive = { path = "../libcst_derive", version = "1.3.0" }
+libcst_derive = { path = "../libcst_derive", version = "1.3.1" }
 
 [dev-dependencies]
 criterion = { version = "0.5.1", features = ["html_reports"] }
 difference = "2.0.0"
 rayon = "1.7.0"
 itertools = "0.11.0"
```

### Comparing `libcst-1.3.0/native/libcst/Grammar` & `libcst-1.3.1/native/libcst/Grammar`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/LICENSE` & `libcst-1.3.1/native/libcst/LICENSE`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/README.md` & `libcst-1.3.1/native/libcst/README.md`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/benches/parser_benchmark.rs` & `libcst-1.3.1/native/libcst/benches/parser_benchmark.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/bin.rs` & `libcst-1.3.1/native/libcst/src/bin.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/lib.rs` & `libcst-1.3.1/native/libcst/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/nodes/codegen.rs` & `libcst-1.3.1/native/libcst/src/nodes/codegen.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/nodes/expression.rs` & `libcst-1.3.1/native/libcst/src/nodes/expression.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/nodes/inflate_helpers.rs` & `libcst-1.3.1/native/libcst/src/nodes/inflate_helpers.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/nodes/macros.rs` & `libcst-1.3.1/native/libcst/src/nodes/macros.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/nodes/mod.rs` & `libcst-1.3.1/native/libcst/src/nodes/mod.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/nodes/module.rs` & `libcst-1.3.1/native/libcst/src/nodes/module.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/nodes/op.rs` & `libcst-1.3.1/native/libcst/src/nodes/op.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/nodes/parser_config.rs` & `libcst-1.3.1/native/libcst/src/nodes/parser_config.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/nodes/py_cached.rs` & `libcst-1.3.1/native/libcst/src/nodes/py_cached.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/nodes/statement.rs` & `libcst-1.3.1/native/libcst/src/nodes/statement.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/nodes/test_utils.rs` & `libcst-1.3.1/native/libcst/src/nodes/test_utils.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/nodes/traits.rs` & `libcst-1.3.1/native/libcst/src/nodes/traits.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/nodes/whitespace.rs` & `libcst-1.3.1/native/libcst/src/nodes/whitespace.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/parser/errors.rs` & `libcst-1.3.1/native/libcst/src/parser/errors.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/parser/grammar.rs` & `libcst-1.3.1/native/libcst/src/parser/grammar.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/parser/numbers.rs` & `libcst-1.3.1/native/libcst/src/parser/numbers.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/py.rs` & `libcst-1.3.1/native/libcst/src/py.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/tokenizer/core/LICENSE` & `libcst-1.3.1/native/libcst/src/tokenizer/core/LICENSE`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/tokenizer/core/mod.rs` & `libcst-1.3.1/native/libcst/src/tokenizer/core/mod.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/tokenizer/core/string_types.rs` & `libcst-1.3.1/native/libcst/src/tokenizer/core/string_types.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/tokenizer/operators.rs` & `libcst-1.3.1/native/libcst/src/tokenizer/operators.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/tokenizer/tests.rs` & `libcst-1.3.1/native/libcst/src/tokenizer/tests.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/tokenizer/text_position/char_width.rs` & `libcst-1.3.1/native/libcst/src/tokenizer/text_position/char_width.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/tokenizer/text_position/mod.rs` & `libcst-1.3.1/native/libcst/src/tokenizer/text_position/mod.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/src/tokenizer/whitespace_parser.rs` & `libcst-1.3.1/native/libcst/src/tokenizer/whitespace_parser.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/tests/fixtures/big_binary_operator.py` & `libcst-1.3.1/native/libcst/tests/fixtures/big_binary_operator.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/tests/fixtures/comments.py` & `libcst-1.3.1/native/libcst/tests/fixtures/comments.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/tests/fixtures/expr.py` & `libcst-1.3.1/native/libcst/tests/fixtures/expr.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/tests/fixtures/fun_with_func_defs.py` & `libcst-1.3.1/native/libcst/tests/fixtures/fun_with_func_defs.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/tests/fixtures/malicious_match.py` & `libcst-1.3.1/native/libcst/tests/fixtures/malicious_match.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/tests/fixtures/pep646.py` & `libcst-1.3.1/native/libcst/tests/fixtures/pep646.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/tests/fixtures/super_strings.py` & `libcst-1.3.1/native/libcst/tests/fixtures/super_strings.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/tests/fixtures/type_parameters.py` & `libcst-1.3.1/native/libcst/tests/fixtures/type_parameters.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/tests/fixtures/with_wickedness.py` & `libcst-1.3.1/native/libcst/tests/fixtures/with_wickedness.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst/tests/parser_roundtrip.rs` & `libcst-1.3.1/native/libcst/tests/parser_roundtrip.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst_derive/LICENSE` & `libcst-1.3.1/native/libcst_derive/LICENSE`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst_derive/src/codegen.rs` & `libcst-1.3.1/native/libcst_derive/src/codegen.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst_derive/src/cstnode.rs` & `libcst-1.3.1/native/libcst_derive/src/cstnode.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst_derive/src/inflate.rs` & `libcst-1.3.1/native/libcst_derive/src/inflate.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst_derive/src/into_py.rs` & `libcst-1.3.1/native/libcst_derive/src/into_py.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst_derive/src/lib.rs` & `libcst-1.3.1/native/libcst_derive/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst_derive/src/parenthesized_node.rs` & `libcst-1.3.1/native/libcst_derive/src/parenthesized_node.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst_derive/tests/pass/minimal_cst.rs` & `libcst-1.3.1/native/libcst_derive/tests/pass/minimal_cst.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/native/libcst_derive/tests/pass/simple.rs` & `libcst-1.3.1/native/libcst_derive/tests/pass/simple.rs`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/pyproject.toml` & `libcst-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/scripts/check_copyright.py` & `libcst-1.3.1/scripts/check_copyright.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/scripts/regenerate-fixtures.py` & `libcst-1.3.1/scripts/regenerate-fixtures.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/setup.py` & `libcst-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/stubs/libcst_native/parser_config.pyi` & `libcst-1.3.1/stubs/libcst_native/parser_config.pyi`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/stubs/libcst_native/token_type.pyi` & `libcst-1.3.1/stubs/libcst_native/token_type.pyi`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/stubs/libcst_native/tokenize.pyi` & `libcst-1.3.1/stubs/libcst_native/tokenize.pyi`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/stubs/libcst_native/whitespace_parser.pyi` & `libcst-1.3.1/stubs/libcst_native/whitespace_parser.pyi`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/stubs/libcst_native/whitespace_state.pyi` & `libcst-1.3.1/stubs/libcst_native/whitespace_state.pyi`

 * *Files identical despite different names*

### Comparing `libcst-1.3.0/stubs/tokenize.pyi` & `libcst-1.3.1/stubs/tokenize.pyi`

 * *Files identical despite different names*

