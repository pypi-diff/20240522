# Comparing `tmp/nbwipers-0.3.5.tar.gz` & `tmp/nbwipers-0.3.6.tar.gz`

## Comparing `nbwipers-0.3.5.tar` & `nbwipers-0.3.6.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0        0        0     1081 1970-01-01 00:00:00.000000 nbwipers-0.3.5/Cargo.toml
--rw-r--r--   0     1001      127     6082 2024-03-17 00:57:04.000000 nbwipers-0.3.5/.github/workflows/release.yml
--rw-r--r--   0     1001      127     1012 2024-03-17 00:57:04.000000 nbwipers-0.3.5/.github/workflows/testing.yml
--rw-r--r--   0     1001      127      725 2024-03-17 00:57:04.000000 nbwipers-0.3.5/.gitignore
--rw-r--r--   0     1001      127       96 2024-03-17 00:57:04.000000 nbwipers-0.3.5/.markdownlint.jsonc
--rw-r--r--   0     1001      127      474 2024-03-17 00:57:04.000000 nbwipers-0.3.5/.pre-commit-config.yaml
--rw-r--r--   0     1001      127      252 2024-03-17 00:57:04.000000 nbwipers-0.3.5/.pre-commit-hooks.yaml
--rw-r--r--   0     1001      127     1870 2024-03-17 00:57:04.000000 nbwipers-0.3.5/CHANGELOG.md
--rw-r--r--   0     1001      127    42555 2024-03-17 00:57:04.000000 nbwipers-0.3.5/Cargo.lock
--rw-r--r--   0     1001      127     7439 2024-03-17 00:57:04.000000 nbwipers-0.3.5/CommandLineHelp.md
--rw-r--r--   0     1001      127     3628 2024-03-17 00:57:04.000000 nbwipers-0.3.5/LICENSE
--rw-r--r--   0     1001      127     6807 2024-03-17 00:57:04.000000 nbwipers-0.3.5/README.md
--rw-r--r--   0     1001      127      364 2024-03-17 00:57:04.000000 nbwipers-0.3.5/justfile
--rw-r--r--   0     1001      127     5265 2024-03-17 00:57:04.000000 nbwipers-0.3.5/src/cell_impl.rs
--rw-r--r--   0     1001      127     5330 2024-03-17 00:57:04.000000 nbwipers-0.3.5/src/check.rs
--rw-r--r--   0     1001      127     8293 2024-03-17 00:57:04.000000 nbwipers-0.3.5/src/cli.rs
--rw-r--r--   0     1001      127     3506 2024-03-17 00:57:04.000000 nbwipers-0.3.5/src/config.rs
--rw-r--r--   0     1001      127     5671 2024-03-17 00:57:04.000000 nbwipers-0.3.5/src/extra_keys.rs
--rw-r--r--   0     1001      127     3970 2024-03-17 00:57:04.000000 nbwipers-0.3.5/src/files.rs
--rw-r--r--   0     1001      127     8324 2024-03-17 00:57:04.000000 nbwipers-0.3.5/src/install/attributes.rs
--rw-r--r--   0     1001      127     5320 2024-03-17 00:57:04.000000 nbwipers-0.3.5/src/install/gitconfig.rs
--rw-r--r--   0     1001      127     5706 2024-03-17 00:57:04.000000 nbwipers-0.3.5/src/install/mod.rs
--rw-r--r--   0     1001      127     5782 2024-03-17 00:57:04.000000 nbwipers-0.3.5/src/main.rs
--rw-r--r--   0     1001      127     5629 2024-03-17 00:57:04.000000 nbwipers-0.3.5/src/schema.rs
--rw-r--r--   0     1001      127      772 2024-03-17 00:57:04.000000 nbwipers-0.3.5/src/settings.rs
--rw-r--r--   0     1001      127     6201 2024-03-17 00:57:04.000000 nbwipers-0.3.5/src/strip.rs
--rw-r--r--   0     1001      127     5454 2024-03-17 00:57:04.000000 nbwipers-0.3.5/src/utils.rs
--rw-r--r--   0     1001      127     1180 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_drop_empty_cells.ipynb
--rw-r--r--   0     1001      127      716 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_drop_empty_cells.ipynb.expected
--rw-r--r--   0     1001      127       40 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_drop_empty_cells.toml
--rw-r--r--   0     1001      127     1052 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_drop_empty_cells_dontdrop.ipynb.expected
--rw-r--r--   0     1001      127     1808 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_drop_tagged_cells.ipynb
--rw-r--r--   0     1001      127     1333 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_drop_tagged_cells.ipynb.expected
--rw-r--r--   0     1001      127       45 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_drop_tagged_cells.toml
--rw-r--r--   0     1001      127     1686 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_drop_tagged_cells_dontdrop.ipynb.expected
--rw-r--r--   0     1001      127     1137 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_execution_timing.ipynb
--rw-r--r--   0     1001      127      700 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_execution_timing.ipynb.expected
--rw-r--r--   0     1001      127      435 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_keep_metadata_keys.ipynb
--rw-r--r--   0     1001      127      409 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_keep_metadata_keys.ipynb.expected
--rw-r--r--   0     1001      127       96 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_keep_metadata_keys.toml
--rw-r--r--   0     1001      127     2097 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_max_size.ipynb
--rw-r--r--   0     1001      127     1645 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_max_size.ipynb.expected
--rw-r--r--   0     1001      127     1624 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_max_size.ipynb.expected_sequential_id
--rw-r--r--   0     1001      127     1745 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_metadata.ipynb
--rw-r--r--   0     1001      127     1520 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_metadata.ipynb.expected
--rw-r--r--   0     1001      127      889 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_exception.ipynb
--rw-r--r--   0     1001      127     1152 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_extra_keys.ipynb.expected
--rw-r--r--   0     1001      127       79 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_extra_keys.toml
--rw-r--r--   0     1001      127     1505 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_keep_count.ipynb.expected
--rw-r--r--   0     1001      127       35 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_keep_count.toml
--rw-r--r--   0     1001      127     1688 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_keep_output.ipynb.expected
--rw-r--r--   0     1001      127       36 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_keep_output.toml
--rw-r--r--   0     1001      127     1670 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_keep_output_keep_count.ipynb.expected
--rw-r--r--   0     1001      127       55 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_keep_output_keep_count.toml
--rw-r--r--   0     1001      127     1266 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_notebook.ipynb
--rw-r--r--   0     1001      127     1266 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_notebook.ipynb.expected
--rw-r--r--   0     1001      127     1871 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_period.ipynb
--rw-r--r--   0     1001      127      352 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_period.ipynb.expected
--rw-r--r--   0     1001      127      145 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_period.toml
--rw-r--r--   0     1001      127     1770 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_nbformat45.ipynb
--rw-r--r--   0     1001      127     1273 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_nbformat45.ipynb.expected
--rw-r--r--   0     1001      127     1238 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_nbformat45.ipynb.expected_sequential_id
--rw-r--r--   0     1001      127       32 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_nbformat45.toml
--rw-r--r--   0     1001      127       31 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_nbformat45_sequential.toml
--rw-r--r--   0     1001      127     1056 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_strip_init_cells.ipynb
--rw-r--r--   0     1001      127      870 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_strip_init_cells.ipynb.expected
--rw-r--r--   0     1001      127       39 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_strip_init_cells.toml
--rw-r--r--   0     1001      127      716 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_unicode.ipynb
--rw-r--r--   0     1001      127      584 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_unicode.ipynb.expected
--rw-r--r--   0     1001      127     1106 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_widgets.ipynb
--rw-r--r--   0     1001      127      783 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/e2e_notebooks/test_widgets.ipynb.expected
--rw-r--r--   0     1001      127    13862 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/integration_test.rs
--rw-r--r--   0     1001      127     8141 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/notebook_test.rs
--rw-r--r--   0     1001      127     1430 2024-03-17 00:57:04.000000 nbwipers-0.3.5/tests/test_nbformat2.ipynb
--rw-r--r--   0     1001      127      432 2024-03-17 00:57:04.000000 nbwipers-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     7336 1970-01-01 00:00:00.000000 nbwipers-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1207 1970-01-01 00:00:00.000000 nbwipers-0.3.6/Cargo.toml
+-rw-r--r--   0     1001      127       23 2024-05-22 17:06:39.000000 nbwipers-0.3.6/.gitattributes
+-rw-r--r--   0     1001      127     6082 2024-05-22 17:06:39.000000 nbwipers-0.3.6/.github/workflows/release.yml
+-rw-r--r--   0     1001      127     1012 2024-05-22 17:06:39.000000 nbwipers-0.3.6/.github/workflows/testing.yml
+-rw-r--r--   0     1001      127      725 2024-05-22 17:06:39.000000 nbwipers-0.3.6/.gitignore
+-rw-r--r--   0     1001      127       96 2024-05-22 17:06:39.000000 nbwipers-0.3.6/.markdownlint.jsonc
+-rw-r--r--   0     1001      127      473 2024-05-22 17:06:39.000000 nbwipers-0.3.6/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      252 2024-05-22 17:06:39.000000 nbwipers-0.3.6/.pre-commit-hooks.yaml
+-rw-r--r--   0     1001      127     1870 2024-05-22 17:06:39.000000 nbwipers-0.3.6/CHANGELOG.md
+-rw-r--r--   0     1001      127    42568 2024-05-22 17:06:39.000000 nbwipers-0.3.6/Cargo.lock
+-rw-r--r--   0     1001      127     7439 2024-05-22 17:06:39.000000 nbwipers-0.3.6/CommandLineHelp.md
+-rw-r--r--   0     1001      127     3628 2024-05-22 17:06:39.000000 nbwipers-0.3.6/LICENSE
+-rw-r--r--   0     1001      127     6807 2024-05-22 17:06:39.000000 nbwipers-0.3.6/README.md
+-rw-r--r--   0     1001      127      401 2024-05-22 17:06:39.000000 nbwipers-0.3.6/justfile
+-rw-r--r--   0     1001      127     5242 2024-05-22 17:06:39.000000 nbwipers-0.3.6/src/cell_impl.rs
+-rw-r--r--   0     1001      127     5274 2024-05-22 17:06:39.000000 nbwipers-0.3.6/src/check.rs
+-rw-r--r--   0     1001      127     8293 2024-05-22 17:06:39.000000 nbwipers-0.3.6/src/cli.rs
+-rw-r--r--   0     1001      127     3506 2024-05-22 17:06:39.000000 nbwipers-0.3.6/src/config.rs
+-rw-r--r--   0     1001      127     5725 2024-05-22 17:06:39.000000 nbwipers-0.3.6/src/extra_keys.rs
+-rw-r--r--   0     1001      127     3886 2024-05-22 17:06:39.000000 nbwipers-0.3.6/src/files.rs
+-rw-r--r--   0     1001      127     8324 2024-05-22 17:06:39.000000 nbwipers-0.3.6/src/install/attributes.rs
+-rw-r--r--   0     1001      127     5301 2024-05-22 17:06:39.000000 nbwipers-0.3.6/src/install/gitconfig.rs
+-rw-r--r--   0     1001      127     5654 2024-05-22 17:06:39.000000 nbwipers-0.3.6/src/install/mod.rs
+-rw-r--r--   0     1001      127     5894 2024-05-22 17:06:39.000000 nbwipers-0.3.6/src/main.rs
+-rw-r--r--   0     1001      127     5653 2024-05-22 17:06:39.000000 nbwipers-0.3.6/src/schema.rs
+-rw-r--r--   0     1001      127      772 2024-05-22 17:06:39.000000 nbwipers-0.3.6/src/settings.rs
+-rw-r--r--   0     1001      127     6199 2024-05-22 17:06:39.000000 nbwipers-0.3.6/src/strip.rs
+-rw-r--r--   0     1001      127     5454 2024-05-22 17:06:39.000000 nbwipers-0.3.6/src/utils.rs
+-rw-r--r--   0     1001      127     1180 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_drop_empty_cells.ipynb
+-rw-r--r--   0     1001      127      716 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_drop_empty_cells.ipynb.expected
+-rw-r--r--   0     1001      127       40 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_drop_empty_cells.toml
+-rw-r--r--   0     1001      127     1052 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_drop_empty_cells_dontdrop.ipynb.expected
+-rw-r--r--   0     1001      127     1808 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_drop_tagged_cells.ipynb
+-rw-r--r--   0     1001      127     1333 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_drop_tagged_cells.ipynb.expected
+-rw-r--r--   0     1001      127       45 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_drop_tagged_cells.toml
+-rw-r--r--   0     1001      127     1686 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_drop_tagged_cells_dontdrop.ipynb.expected
+-rw-r--r--   0     1001      127     1137 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_execution_timing.ipynb
+-rw-r--r--   0     1001      127      700 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_execution_timing.ipynb.expected
+-rw-r--r--   0     1001      127      435 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_keep_metadata_keys.ipynb
+-rw-r--r--   0     1001      127      409 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_keep_metadata_keys.ipynb.expected
+-rw-r--r--   0     1001      127       96 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_keep_metadata_keys.toml
+-rw-r--r--   0     1001      127     2101 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_max_size.ipynb
+-rw-r--r--   0     1001      127     1645 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_max_size.ipynb.expected
+-rw-r--r--   0     1001      127     1624 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_max_size.sequential_id.ipynb.expected
+-rw-r--r--   0     1001      127     1745 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_metadata.ipynb
+-rw-r--r--   0     1001      127     1520 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_metadata.ipynb.expected
+-rw-r--r--   0     1001      127      889 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_exception.ipynb
+-rw-r--r--   0     1001      127     1152 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_extra_keys.ipynb.expected
+-rw-r--r--   0     1001      127       79 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_extra_keys.toml
+-rw-r--r--   0     1001      127     1505 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_keep_count.ipynb.expected
+-rw-r--r--   0     1001      127       35 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_keep_count.toml
+-rw-r--r--   0     1001      127     1688 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_keep_output.ipynb.expected
+-rw-r--r--   0     1001      127       36 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_keep_output.toml
+-rw-r--r--   0     1001      127     1670 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_keep_output_keep_count.ipynb.expected
+-rw-r--r--   0     1001      127       55 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_keep_output_keep_count.toml
+-rw-r--r--   0     1001      127     1266 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_notebook.ipynb
+-rw-r--r--   0     1001      127     1266 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_notebook.ipynb.expected
+-rw-r--r--   0     1001      127     1871 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_period.ipynb
+-rw-r--r--   0     1001      127      352 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_period.ipynb.expected
+-rw-r--r--   0     1001      127      145 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_period.toml
+-rw-r--r--   0     1001      127     1770 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_nbformat45.ipynb
+-rw-r--r--   0     1001      127     1273 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_nbformat45.ipynb.expected
+-rw-r--r--   0     1001      127     1238 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_nbformat45.sequential_id.ipynb.expected
+-rw-r--r--   0     1001      127       32 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_nbformat45.toml
+-rw-r--r--   0     1001      127       31 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_nbformat45_sequential.toml
+-rw-r--r--   0     1001      127     1056 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_strip_init_cells.ipynb
+-rw-r--r--   0     1001      127      870 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_strip_init_cells.ipynb.expected
+-rw-r--r--   0     1001      127       39 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_strip_init_cells.toml
+-rw-r--r--   0     1001      127      716 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_unicode.ipynb
+-rw-r--r--   0     1001      127      584 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_unicode.ipynb.expected
+-rw-r--r--   0     1001      127     1106 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_widgets.ipynb
+-rw-r--r--   0     1001      127      783 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/e2e_notebooks/test_widgets.ipynb.expected
+-rw-r--r--   0     1001      127    13862 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/integration_test.rs
+-rw-r--r--   0     1001      127     8141 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/notebook_test.rs
+-rw-r--r--   0     1001      127     1430 2024-05-22 17:06:39.000000 nbwipers-0.3.6/tests/test_nbformat2.ipynb
+-rw-r--r--   0     1001      127      432 2024-05-22 17:06:39.000000 nbwipers-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     7384 1970-01-01 00:00:00.000000 nbwipers-0.3.6/PKG-INFO
```

### Comparing `nbwipers-0.3.5/Cargo.toml` & `nbwipers-0.3.6/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [package]
 name = "nbwipers"
-version = "0.3.5"
+version = "0.3.6"
 edition = "2021"
 license = "MIT"
 description = "Wipe clean your Jupyter Notebooks!"
 repository = "https://github.com/felixgwilliams/nbwipers"
 homepage = "https://github.com/felixgwilliams/nbwipers"
 readme = "README.md"
+categories = ["command-line-utilities", "development-tools"]
+keywords = ["python", "notebook", "jupyter", "ci", "pre-commit"]
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 anyhow = "1.0.79"
 bstr = "1.9.0"
 clap = { version = "4.4.18", features = ["derive"] }
 clap-markdown = { version = "0.1.3", optional = true }
 colored = "2.1.0"
 gix-attributes = "0.22.0"
-gix-config = { version = "0.36.0" }
-gix-discover = "0.31.0"
+gix-config = { version = "0.37.0" }
+gix-discover = "0.32.0"
 gix-path = "0.10.5"
 ignore = "0.4.22"
 inquire = "0.7.0"
-itertools = "0.12.1"
+itertools = "0.13.0"
 path-absolutize = { version = "3.1.1", features = ["once_cell_cache"] }
 rayon = "1.8.1"
 rustc-hash = "1.1.0"
 serde = { version = "1.0.196", features = ["derive"] }
 serde_json = { version = "1.0.113", features = ["preserve_order"] }
 serde_with = "3.6.0"
 thiserror = "1.0.56"
```

### Comparing `nbwipers-0.3.5/.github/workflows/release.yml` & `nbwipers-0.3.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/.github/workflows/testing.yml` & `nbwipers-0.3.6/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/.gitignore` & `nbwipers-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/CHANGELOG.md` & `nbwipers-0.3.6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/Cargo.lock` & `nbwipers-0.3.6/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -356,17 +356,17 @@
 name = "faster-hex"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2a2b11eda1d40935b26cf18f6833c526845ae8c41e58d09af6adeb6f0269183"
 
 [[package]]
 name = "fastrand"
-version = "2.0.1"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
@@ -386,17 +386,17 @@
 checksum = "c31b6d751ae2c7f11320402d34e41349dd1016f8d5d45e48c4312bc8625af50c"
 dependencies = [
  "byteorder",
 ]
 
 [[package]]
 name = "gix-actor"
-version = "0.31.0"
+version = "0.31.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3eb3230825b44deba727ec2e9c886c4ab350d34333ae17555973ceb5e5261471"
+checksum = "d69c59d392c7e6c94385b6fd6089d6df0fe945f32b4357687989f3aee253cd7f"
 dependencies = [
  "bstr",
  "gix-date",
  "gix-utils",
  "itoa",
  "thiserror",
  "winnow",
@@ -417,17 +417,17 @@
  "smallvec",
  "thiserror",
  "unicode-bom",
 ]
 
 [[package]]
 name = "gix-config"
-version = "0.36.0"
+version = "0.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62129c75e4b6229fe15fb9838cdc00c655e87105b651e4edd7c183fc5288b5d1"
+checksum = "53fafe42957e11d98e354a66b6bd70aeea00faf2f62dd11164188224a507c840"
 dependencies = [
  "bstr",
  "gix-config-value",
  "gix-features",
  "gix-glob",
  "gix-path",
  "gix-ref",
@@ -451,61 +451,62 @@
  "gix-path",
  "libc",
  "thiserror",
 ]
 
 [[package]]
 name = "gix-date"
-version = "0.8.5"
+version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "180b130a4a41870edfbd36ce4169c7090bca70e195da783dea088dd973daa59c"
+checksum = "367ee9093b0c2b04fd04c5c7c8b6a1082713534eab537597ae343663a518fa99"
 dependencies = [
  "bstr",
  "itoa",
  "thiserror",
  "time",
 ]
 
 [[package]]
 name = "gix-discover"
-version = "0.31.0"
+version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64bab49087ed3710caf77e473dc0efc54ca33d8ccc6441359725f121211482b1"
+checksum = "fc27c699b63da66b50d50c00668bc0b7e90c3a382ef302865e891559935f3dbf"
 dependencies = [
  "bstr",
  "dunce",
  "gix-fs",
  "gix-hash",
  "gix-path",
  "gix-ref",
  "gix-sec",
  "thiserror",
 ]
 
 [[package]]
 name = "gix-features"
-version = "0.38.1"
+version = "0.38.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db4254037d20a247a0367aa79333750146a369719f0c6617fec4f5752cc62b37"
+checksum = "ac7045ac9fe5f9c727f38799d002a7ed3583cd777e3322a7c4b43e3cf437dc69"
 dependencies = [
  "gix-hash",
  "gix-trace",
  "gix-utils",
  "libc",
  "prodash",
  "sha1_smol",
  "walkdir",
 ]
 
 [[package]]
 name = "gix-fs"
-version = "0.10.1"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "634b8a743b0aae03c1a74ee0ea24e8c5136895efac64ce52b3ea106e1c6f0613"
+checksum = "3f78f7d6dcda7a5809efd73a33b145e3dce7421c460df21f32126f9732736b0c"
 dependencies = [
+ "fastrand",
  "gix-features",
  "gix-utils",
 ]
 
 [[package]]
 name = "gix-glob"
 version = "0.16.2"
@@ -526,28 +527,28 @@
 dependencies = [
  "faster-hex",
  "thiserror",
 ]
 
 [[package]]
 name = "gix-lock"
-version = "13.1.0"
+version = "14.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "886490a07b1d6433aa91262a99d430a91cc8b9a1f758ac1282e132f1098a9342"
+checksum = "e3bc7fe297f1f4614774989c00ec8b1add59571dc9b024b4c00acb7dedd4e19d"
 dependencies = [
  "gix-tempfile",
  "gix-utils",
  "thiserror",
 ]
 
 [[package]]
 name = "gix-object"
-version = "0.42.0"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03e9e56e790cdd548dee951019b4f0575a00cdd95092d34ceddeb3294b34ef08"
+checksum = "1fe2dc4a41191c680c942e6ebd630c8107005983c4679214fdb1007dcf5ae1df"
 dependencies = [
  "bstr",
  "gix-actor",
  "gix-date",
  "gix-features",
  "gix-hash",
  "gix-utils",
@@ -580,17 +581,17 @@
  "bstr",
  "gix-utils",
  "thiserror",
 ]
 
 [[package]]
 name = "gix-ref"
-version = "0.43.0"
+version = "0.44.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd4aba68b925101cb45d6df328979af0681364579db889098a0de75b36c77b65"
+checksum = "0b36752b448647acd59c9668fdd830b16d07db1e6d9c3b3af105c1605a6e23d9"
 dependencies = [
  "gix-actor",
  "gix-date",
  "gix-features",
  "gix-fs",
  "gix-hash",
  "gix-lock",
@@ -614,17 +615,17 @@
  "gix-path",
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "gix-tempfile"
-version = "13.1.0"
+version = "14.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "439f4da9657aec7434cde3c2510dcdb0a35f2031233ff67ae986269c788966d7"
+checksum = "d3b0e276cd08eb2a22e9f286a4f13a222a01be2defafa8621367515375644b99"
 dependencies = [
  "gix-fs",
  "libc",
  "once_cell",
  "parking_lot",
  "tempfile",
 ]
@@ -633,27 +634,27 @@
 name = "gix-trace"
 version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b838b2db8f62c9447d483a4c28d251b67fee32741a82cb4d35e9eb4e9fdc5ab"
 
 [[package]]
 name = "gix-utils"
-version = "0.1.11"
+version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0066432d4c277f9877f091279a597ea5331f68ca410efc874f0bdfb1cd348f92"
+checksum = "35192df7fd0fa112263bad8021e2df7167df4cc2a6e6d15892e1e55621d3d4dc"
 dependencies = [
  "fastrand",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "gix-validate"
-version = "0.8.4"
+version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e39fc6e06044985eac19dd34d474909e517307582e462b2eb4c8fa51b6241545"
+checksum = "82c27dd34a49b1addf193c92070bcbf3beaf6e10f16a78544de6372e146a0acf"
 dependencies = [
  "bstr",
  "thiserror",
 ]
 
 [[package]]
 name = "globset"
@@ -783,17 +784,17 @@
  "once_cell",
  "unicode-segmentation",
  "unicode-width",
 ]
 
 [[package]]
 name = "itertools"
-version = "0.12.1"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
+checksum = "413ee7dfc52ee1a4949ceeb7dbc8a33f2d6c088194d9f922fb8318faf1f01186"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
 version = "1.0.10"
@@ -877,15 +878,15 @@
  "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "nbwipers"
-version = "0.3.5"
+version = "0.3.6"
 dependencies = [
  "anyhow",
  "bstr",
  "clap",
  "clap-markdown",
  "colored",
  "gix-attributes",
```

### Comparing `nbwipers-0.3.5/CommandLineHelp.md` & `nbwipers-0.3.6/CommandLineHelp.md`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/LICENSE` & `nbwipers-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/README.md` & `nbwipers-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/src/cell_impl.rs` & `nbwipers-0.3.6/src/cell_impl.rs`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 use serde_json::Value;
 
 use crate::schema::{Cell, CodeCell, SourceValue};
 
 impl SourceValue {
     fn is_empty(&self) -> bool {
         match self {
-            SourceValue::String(ref s) => s.trim().is_empty(),
-            SourceValue::StringArray(ref s_vec) => s_vec.iter().all(|s| s.trim().is_empty()),
+            Self::String(ref s) => s.trim().is_empty(),
+            Self::StringArray(ref s_vec) => s_vec.iter().all(|s| s.trim().is_empty()),
         }
     }
 }
 
 impl CodeCell {
     pub fn is_clear_outputs(&self) -> bool {
         self.outputs.is_empty()
@@ -61,72 +61,72 @@
         } else {
             false
         }
     }
 }
 
 impl Cell {
-    pub fn as_codecell(&self) -> Option<&CodeCell> {
-        if let Cell::Code(codecell) = self {
+    pub const fn as_codecell(&self) -> Option<&CodeCell> {
+        if let Self::Code(codecell) = self {
             Some(codecell)
         } else {
             None
         }
     }
     pub fn as_codecell_mut(&mut self) -> Option<&mut CodeCell> {
-        if let Cell::Code(codecell) = self {
+        if let Self::Code(codecell) = self {
             Some(codecell)
         } else {
             None
         }
     }
     pub fn is_clear_id(&self, cell_number: usize) -> bool {
         let id = self.get_id();
         id.is_none() || id.as_ref().is_some_and(|id| id == &cell_number.to_string())
     }
 
-    pub fn get_source(&self) -> &SourceValue {
+    pub const fn get_source(&self) -> &SourceValue {
         match self {
-            Cell::Code(ref c) => &c.source,
-            Cell::Markdown(ref c) => &c.source,
-            Cell::Raw(ref c) => &c.source,
+            Self::Code(ref c) => &c.source,
+            Self::Markdown(ref c) => &c.source,
+            Self::Raw(ref c) => &c.source,
         }
     }
 
-    pub fn get_metadata(&self) -> &Value {
+    pub const fn get_metadata(&self) -> &Value {
         match self {
-            Cell::Code(ref c) => &c.metadata,
-            Cell::Markdown(ref c) => &c.metadata,
-            Cell::Raw(ref c) => &c.metadata,
+            Self::Code(ref c) => &c.metadata,
+            Self::Markdown(ref c) => &c.metadata,
+            Self::Raw(ref c) => &c.metadata,
         }
     }
     pub fn get_metadata_mut(&mut self) -> &mut Value {
         match self {
-            Cell::Code(ref mut c) => &mut c.metadata,
-            Cell::Markdown(ref mut c) => &mut c.metadata,
-            Cell::Raw(ref mut c) => &mut c.metadata,
+            Self::Code(ref mut c) => &mut c.metadata,
+            Self::Markdown(ref mut c) => &mut c.metadata,
+            Self::Raw(ref mut c) => &mut c.metadata,
         }
     }
-    pub fn get_id(&self) -> &Option<String> {
+    pub const fn get_id(&self) -> &Option<String> {
         match self {
-            Cell::Code(ref c) => &c.id,
-            Cell::Markdown(ref c) => &c.id,
-            Cell::Raw(ref c) => &c.id,
+            Self::Code(ref c) => &c.id,
+            Self::Markdown(ref c) => &c.id,
+            Self::Raw(ref c) => &c.id,
         }
     }
     pub fn set_id(&mut self, new_id: Option<String>) -> Option<String> {
         let prev_id = match self {
-            Cell::Code(c) => c.id.clone(),
-            Cell::Markdown(c) => c.id.clone(),
-            Cell::Raw(c) => c.id.clone(),
+            Self::Code(c) => c.id.clone(),
+            Self::Markdown(c) => c.id.clone(),
+            Self::Raw(c) => c.id.clone(),
         };
         match self {
-            Cell::Code(ref mut c) => c.id = new_id,
-            Cell::Markdown(ref mut c) => c.id = new_id,
-            Cell::Raw(ref mut c) => c.id = new_id,
+            Self::Code(ref mut c) => c.id = new_id,
+            Self::Markdown(ref mut c) => c.id = new_id,
+            Self::Raw(ref mut c) => c.id = new_id,
         };
         prev_id
     }
 
     pub fn should_drop(
         &self,
         drop_empty_cells: bool,
@@ -140,21 +140,19 @@
         }
         let tags = self
             .get_metadata()
             .as_object()
             .and_then(|x| x.get("tags"))
             .and_then(|x| x.as_array());
 
-        if let Some(tags) = tags {
+        tags.map_or(false, |tags| {
             tags.iter()
                 .filter_map(|v| v.as_str())
                 .any(|s| drop_tagged_cells.contains(s))
-        } else {
-            false
-        }
+        })
     }
 }
 
 #[cfg(test)]
 mod tests {
     use serde_json::json;
```

### Comparing `nbwipers-0.3.5/src/check.rs` & `nbwipers-0.3.6/src/check.rs`

 * *Files 12% similar despite different names*

```diff
@@ -55,34 +55,34 @@
     #[serde(flatten)]
     pub result: &'a CheckResult,
 }
 
 impl Display for CheckResult {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         match self {
-            CheckResult::IOError { error } => write!(f, "IO Error: {error}"),
-            CheckResult::InvalidNotebook { error } => write!(f, "Invalid notebook: {error}"),
-            CheckResult::DropCells { cell_number } => {
+            Self::IOError { error } => write!(f, "IO Error: {error}"),
+            Self::InvalidNotebook { error } => write!(f, "Invalid notebook: {error}"),
+            Self::DropCells { cell_number } => {
                 write!(f, "cell: {cell_number}: Found cell to be dropped")
             }
-            CheckResult::StripMeta { extra_key } => {
+            Self::StripMeta { extra_key } => {
                 write!(f, "Found notebook metadata: {extra_key}")
             }
 
-            CheckResult::CellStripMeta {
+            Self::CellStripMeta {
                 cell_number,
                 extra_key,
             } => write!(f, "cell {cell_number}: Found cell metadata {extra_key}"),
-            CheckResult::ClearCount { cell_number } => {
+            Self::ClearCount { cell_number } => {
                 write!(f, "cell {cell_number}: Found cell with execution count")
             }
-            CheckResult::ClearId { cell_number } => {
+            Self::ClearId { cell_number } => {
                 write!(f, "cell {cell_number}: Found cell with Id")
             }
-            CheckResult::ClearOutput { cell_number } => {
+            Self::ClearOutput { cell_number } => {
                 write!(f, "cell {cell_number}: Found cell with output")
             }
         }
     }
 }
 
 pub fn check_nb(nb: &RawNotebook, settings: &Settings) -> Vec<CheckResult> {
```

### Comparing `nbwipers-0.3.5/src/cli.rs` & `nbwipers-0.3.6/src/cli.rs`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/src/config.rs` & `nbwipers-0.3.6/src/config.rs`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/src/extra_keys.rs` & `nbwipers-0.3.6/src/extra_keys.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-use std::str::FromStr;
+use std::{fmt::Display, str::FromStr};
 
 use serde::{de, Deserialize};
 use thiserror::Error;
 
 #[derive(Debug, Clone, PartialEq, Eq, Hash)]
 pub enum ExtraKey {
     CellMeta(StripKey),
     Metadata(StripKey),
 }
 
 impl ExtraKey {
-    pub fn get_parts(&self) -> &Vec<String> {
+    pub const fn get_parts(&self) -> &Vec<String> {
         match self {
-            ExtraKey::Metadata(ref c) | ExtraKey::CellMeta(ref c) => &c.parts,
+            Self::Metadata(ref c) | Self::CellMeta(ref c) => &c.parts,
         }
     }
 }
 
-impl ToString for ExtraKey {
-    fn to_string(&self) -> String {
+impl Display for ExtraKey {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         match self {
-            Self::CellMeta(cellmeta) => format!("cell.metadata.{}", cellmeta.parts.join(".")),
-            Self::Metadata(meta) => format!("metadata.{}", meta.parts.join(".")),
+            Self::CellMeta(cellmeta) => write!(f, "cell.metadata.{}", cellmeta.parts.join(".")),
+            Self::Metadata(meta) => write!(f, "metadata.{}", meta.parts.join(".")),
         }
     }
 }
 
 #[derive(Debug, Clone, PartialEq, Eq, Hash)]
 pub struct StripKey {
     pub(crate) parts: Vec<String>,
 }
 
-#[derive(Debug, PartialEq, Clone, Copy, Error)]
+#[derive(Debug, PartialEq, Eq, Clone, Copy, Error)]
 pub enum ExtraKeyParseError {
     #[error("Key must start with `cell.metadata` or `metadata`")]
     NotCellOrMetadata,
     #[error("Empty Subkey")]
     EmptySubKey,
     #[error("Empty Key")]
     Empty,
 }
 
 impl StripKey {
     pub fn try_from_slice(parts: &[&str]) -> Result<Self, ExtraKeyParseError> {
         if parts.is_empty() || parts == [""] {
             Err(ExtraKeyParseError::EmptySubKey)
         } else {
-            Ok(StripKey {
+            Ok(Self {
                 parts: parts.iter().map(|x| String::from(*x)).collect(),
             })
         }
     }
 }
 
 impl FromStr for ExtraKey {
```

### Comparing `nbwipers-0.3.5/src/files.rs` & `nbwipers-0.3.6/src/files.rs`

 * *Files 9% similar despite different names*

```diff
@@ -13,31 +13,26 @@
 
 use crate::schema::RawNotebook;
 
 // normalize_path and relative_path are from Ruff, used under the MIT license
 
 fn normalize_path<P: AsRef<Path>>(path: P) -> PathBuf {
     let path = path.as_ref();
-    if let Ok(path) = path.absolutize() {
-        path.to_path_buf()
-    } else {
-        #[cfg(not(tarpaulin_include))]
-        path.to_path_buf()
-    }
+    path.absolutize()
+        .map_or_else(|_| path.to_path_buf(), |path| path.to_path_buf())
 }
 pub fn relativize_path<P: AsRef<Path>>(path: P) -> String {
     let path = path.as_ref();
 
     let cwd = path_absolutize::path_dedot::CWD.as_path();
 
-    if let Ok(path) = path.strip_prefix(cwd) {
-        format!("{}", path.display())
-    } else {
-        format!("{}", path.display())
-    }
+    path.strip_prefix(cwd).map_or_else(
+        |_| format!("{}", path.display()),
+        |path| format!("{}", path.display()),
+    )
 }
 
 pub enum FoundNotebooks {
     Stdin,
     NoFiles,
     Files(Vec<PathBuf>),
 }
@@ -45,15 +40,15 @@
 pub fn find_notebooks(paths: &[PathBuf]) -> Result<FoundNotebooks, Error> {
     if paths == [Path::new("-")] {
         return Ok(FoundNotebooks::Stdin);
     }
     let paths: Vec<PathBuf> = paths.iter().map(normalize_path).unique().collect();
     let (first_path, rest_paths) = paths
         .split_first()
-        .ok_or(anyhow!("Please provide at least one path"))?;
+        .ok_or_else(|| anyhow!("Please provide at least one path"))?;
 
     let mut builder = WalkBuilder::new(first_path);
     for path in rest_paths {
         builder.add(path);
     }
     builder.standard_filters(true);
     builder.hidden(false);
@@ -112,16 +107,15 @@
     #[error("File IO error")]
     IO(#[from] std::io::Error),
     #[error("JSON write error")]
     Serde(#[from] serde_json::Error),
 }
 
 pub fn read_nb_stdin() -> Result<RawNotebook, NBReadError> {
-    let handle = stdin().lock();
-    let out = serde_json::from_reader(handle)?;
+    let out = serde_json::from_reader(stdin().lock())?;
     Ok(out)
 }
 
 #[allow(clippy::unwrap_used)]
 #[cfg(test)]
 mod tests {
     use std::env::current_dir;
```

### Comparing `nbwipers-0.3.5/src/install/attributes.rs` & `nbwipers-0.3.6/src/install/attributes.rs`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/src/install/gitconfig.rs` & `nbwipers-0.3.6/src/install/gitconfig.rs`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 use bstr::BStr;
 
 use crate::cli::GitConfigType;
 
 pub fn install_config(config_file: Option<&Path>, config_type: GitConfigType) -> Result<(), Error> {
     let cur_exe = std::env::current_exe()?;
     let source = config_type.into();
-    let cur_exe_str = match cur_exe.to_str() {
-        Some(s) => Ok(s),
-        #[cfg(not(tarpaulin_include))]
-        None => Err(anyhow!("Executable path cannot be converted to unicode")),
-    }?
-    .replace('\\', "/");
+    let cur_exe_str = cur_exe
+        .to_str()
+        .map_or_else(
+            || Err(anyhow!("Executable path cannot be converted to unicode")),
+            Ok,
+        )?
+        .replace('\\', "/");
     let file_path = resolve_config_file(config_file, config_type)?;
 
     let mut file = if file_path.is_file() {
         gix_config::File::from_path_no_includes(file_path.clone(), source)?
     } else {
         if let Some(parent) = file_path.parent() {
             fs::create_dir_all(parent)?;
```

### Comparing `nbwipers-0.3.5/src/install/mod.rs` & `nbwipers-0.3.6/src/install/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 use gitconfig::{check_install_config_file, resolve_config_file};
 pub use gitconfig::{install_config, uninstall_config};
 use gix_config::File;
 
 impl From<GitConfigType> for Source {
     fn from(value: GitConfigType) -> Self {
         match value {
-            GitConfigType::Global => Source::User,
-            GitConfigType::System => Source::System,
-            GitConfigType::Local => Source::Local,
+            GitConfigType::Global => Self::User,
+            GitConfigType::System => Self::System,
+            GitConfigType::Local => Self::Local,
         }
     }
 }
 
 fn get_git_repo_and_work_tree() -> Result<(PathBuf, Option<PathBuf>), Error> {
     let cur_dir = std::env::current_dir()?;
     let (git_dir, _) = gix_discover::upwards(&cur_dir)?;
@@ -41,15 +41,15 @@
 #[derive(Debug, Clone, PartialEq, Eq, Default)]
 struct InstallStatus {
     pub nbstripout: InstallToolStatus,
     pub nbwipers: InstallToolStatus,
 }
 
 impl InstallToolStatus {
-    fn is_installed(&self) -> bool {
+    const fn is_installed(&self) -> bool {
         self.diff && self.filter
     }
 }
 // impl From<InstallToolStatus> for bool {
 //     fn from(value: InstallToolStatus) -> Self {
 //         value.diff & value.filter
 //     }
@@ -57,17 +57,17 @@
 // impl From<InstallStatus> for bool {
 //     fn from(value: InstallStatus) -> Self {
 //         (value.nbstripout | value.nbwipers).into()
 //     }
 // }
 
 impl BitAnd for InstallToolStatus {
-    type Output = InstallToolStatus;
+    type Output = Self;
     fn bitand(self, rhs: Self) -> Self::Output {
-        InstallToolStatus {
+        Self {
             diff: self.diff & rhs.diff,
             filter: self.filter & rhs.filter,
         }
     }
 }
 
 // impl BitOr for InstallToolStatus {
@@ -86,17 +86,17 @@
 //         InstallStatus {
 //             nbstripout: self.nbstripout | rhs.nbstripout,
 //             nbwipers: self.nbwipers | rhs.nbwipers,
 //         }
 //     }
 // }
 impl BitAnd for InstallStatus {
-    type Output = InstallStatus;
+    type Output = Self;
     fn bitand(self, rhs: Self) -> Self::Output {
-        InstallStatus {
+        Self {
             nbstripout: self.nbstripout & rhs.nbstripout,
             nbwipers: self.nbwipers & rhs.nbwipers,
         }
     }
 }
 
 impl BitOrAssign for InstallToolStatus {
@@ -132,15 +132,15 @@
         bail!("Neither nbstripout nor nbwipers are installed.")
     }
 }
 pub fn check_install_some_type(config_type: GitConfigType) -> Result<(), Error> {
     let attr_install_status = check_install_attr_files(&[config_type])?;
 
     let file_path = resolve_config_file(None, config_type)?;
-    let config_file = File::from_path_no_includes(file_path.clone(), config_type.into())?;
+    let config_file = File::from_path_no_includes(file_path, config_type.into())?;
     let config_install_status = check_install_config_file(&config_file);
 
     combine_install_status(attr_install_status, config_install_status)
 }
 pub fn check_install_none_type() -> Result<(), Error> {
     let config_types = vec![
         GitConfigType::Local,
```

### Comparing `nbwipers-0.3.5/src/main.rs` & `nbwipers-0.3.6/src/main.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-#![warn(clippy::all, clippy::pedantic)]
+#![warn(clippy::all, clippy::pedantic, clippy::nursery, clippy::cargo)]
 #![allow(clippy::module_name_repetitions)]
 #![warn(clippy::unwrap_used)]
 #![warn(missing_docs)]
+#![allow(clippy::multiple_crate_versions)] // can't do anything about these
 
 /*! nbwipers is a command line tool to wipe clean Jupyter Notebooks
  *
  *
  */
 
 use std::path::{Path, PathBuf};
@@ -141,19 +142,19 @@
 
 fn uninstall(cmd: &UninstallCommand) -> Result<(), Error> {
     install::uninstall_config(cmd.git_config_file.as_deref(), cmd.config_type)?;
     install::uninstall_attributes(cmd.config_type, cmd.attribute_file.as_deref())
 }
 
 fn check_install(cmd: &CheckInstallCommand) -> Result<(), Error> {
-    let check_result = if let Some(config_type) = cmd.config_type {
-        install::check_install_some_type(config_type)
-    } else {
-        install::check_install_none_type()
-    };
+    let check_result = cmd
+        .config_type
+        .map_or_else(install::check_install_none_type, |config_type| {
+            install::check_install_some_type(config_type)
+        });
     if install::check_should_exit_zero(cmd.exit_zero) {
         Ok(())
     } else {
         check_result
     }
 }
```

### Comparing `nbwipers-0.3.5/src/schema.rs` & `nbwipers-0.3.6/src/schema.rs`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 /// The schema declarations in this file are taken from Ruff, used under the MIT license
 
 /// The root of the JSON of a Jupyter Notebook
 ///
 /// Generated by <https://app.quicktype.io/> from
 /// <https://github.com/jupyter/nbformat/blob/16b53251aabf472ad9406ddb1f78b0421c014eeb/nbformat/v4/nbformat.v4.schema.json>
 /// Jupyter Notebook v4.5 JSON schema.
-#[derive(Clone, Debug, Serialize, Deserialize, PartialEq)]
+#[derive(Clone, Debug, Serialize, Deserialize, PartialEq, Eq)]
 #[serde(deny_unknown_fields)]
 pub struct RawNotebook {
     /// Array of cells of the current notebook.
     pub cells: Vec<Cell>,
     /// Notebook root-level metadata.
     pub metadata: Value,
     /// Notebook format (major number). Incremented between backwards incompatible changes to the
@@ -21,57 +21,57 @@
     pub nbformat: i64,
     /// Notebook format (minor number). Incremented for backward compatible changes to the
     /// notebook format.
     pub nbformat_minor: i64,
 }
 
 /// String identifying the type of cell.
-#[derive(Debug, Serialize, Deserialize, Clone, PartialEq)]
+#[derive(Debug, Serialize, Deserialize, Clone, PartialEq, Eq)]
 #[serde(tag = "cell_type")]
 pub enum Cell {
     #[serde(rename = "code")]
     Code(CodeCell),
     #[serde(rename = "markdown")]
     Markdown(MarkdownCell),
     #[serde(rename = "raw")]
     Raw(RawCell),
 }
 
 /// Notebook raw nbconvert cell.
 #[skip_serializing_none]
-#[derive(Clone, Debug, Serialize, Deserialize, PartialEq)]
+#[derive(Clone, Debug, Serialize, Deserialize, PartialEq, Eq)]
 #[serde(deny_unknown_fields)]
 pub struct RawCell {
     pub attachments: Option<Value>,
     /// Technically, id isn't required (it's not even present) in schema v4.0 through v4.4, but
     /// it's required in v4.5. Main issue is that pycharm creates notebooks without an id
     /// <https://youtrack.jetbrains.com/issue/PY-59438/Jupyter-notebooks-created-with-PyCharm-are-missing-the-id-field-in-cells-in-the-.ipynb-json>
     pub id: Option<String>,
     /// Cell-level metadata.
     pub metadata: Value,
     pub source: SourceValue,
 }
 
 /// Notebook markdown cell.
 #[skip_serializing_none]
-#[derive(Clone, Debug, Serialize, Deserialize, PartialEq)]
+#[derive(Clone, Debug, Serialize, Deserialize, PartialEq, Eq)]
 #[serde(deny_unknown_fields)]
 pub struct MarkdownCell {
     pub attachments: Option<Value>,
     /// Technically, id isn't required (it's not even present) in schema v4.0 through v4.4, but
     /// it's required in v4.5. Main issue is that pycharm creates notebooks without an id
     /// <https://youtrack.jetbrains.com/issue/PY-59438/Jupyter-notebooks-created-with-PyCharm-are-missing-the-id-field-in-cells-in-the-.ipynb-json>
     pub id: Option<String>,
     /// Cell-level metadata.
     pub metadata: Value,
     pub source: SourceValue,
 }
 
 /// Notebook code cell.
-#[derive(Clone, Debug, Serialize, Deserialize, PartialEq)]
+#[derive(Clone, Debug, Serialize, Deserialize, PartialEq, Eq)]
 #[serde(deny_unknown_fields)]
 pub struct CodeCell {
     /// The code cell's prompt number. Will be null if the cell has not been run.
     pub execution_count: Option<i64>,
     /// Technically, id isn't required (it's not even present) in schema v4.0 through v4.4, but
     /// it's required in v4.5. Main issue is that pycharm creates notebooks without an id
     /// <https://youtrack.jetbrains.com/issue/PY-59438/Jupyter-notebooks-created-with-PyCharm-are-missing-the-id-field-in-cells-in-the-.ipynb-json>
@@ -86,15 +86,15 @@
 
 /// mimetype output (e.g. text/plain), represented as either an array of strings or a
 /// string.
 ///
 /// Contents of the cell, represented as an array of lines.
 ///
 /// The stream's text output, represented as an array of strings.
-#[derive(Clone, Debug, Serialize, Deserialize, PartialEq)]
+#[derive(Clone, Debug, Serialize, Deserialize, PartialEq, Eq)]
 #[serde(untagged)]
 pub enum SourceValue {
     String(String),
     StringArray(Vec<String>),
 }
 
 #[allow(clippy::unwrap_used)]
```

### Comparing `nbwipers-0.3.5/src/settings.rs` & `nbwipers-0.3.6/src/settings.rs`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/src/strip.rs` & `nbwipers-0.3.6/src/strip.rs`

 * *Files 2% similar despite different names*

```diff
@@ -168,26 +168,26 @@
             Self::ReadError(e) => write!(f, "Read error: {e}"),
             Self::WriteError(e) => write!(f, "Write error: {e}"),
         }
     }
 }
 
 impl StripSuccess {
-    pub fn from_stripped(stripped: bool) -> Self {
+    pub const fn from_stripped(stripped: bool) -> Self {
         if stripped {
             Self::Stripped
         } else {
             Self::NoChange
         }
     }
 }
 
 impl StripResult {
-    pub fn is_err(&self) -> bool {
-        matches!(self, StripResult::ReadError(_) | StripResult::WriteError(_))
+    pub const fn is_err(&self) -> bool {
+        matches!(self, Self::ReadError(_) | Self::WriteError(_))
     }
 }
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[test]
```

### Comparing `nbwipers-0.3.5/src/utils.rs` & `nbwipers-0.3.6/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_drop_empty_cells.ipynb` & `nbwipers-0.3.6/tests/e2e_notebooks/test_drop_empty_cells.ipynb`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_drop_empty_cells.ipynb.expected` & `nbwipers-0.3.6/tests/e2e_notebooks/test_drop_empty_cells.ipynb.expected`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_drop_empty_cells_dontdrop.ipynb.expected` & `nbwipers-0.3.6/tests/e2e_notebooks/test_drop_empty_cells_dontdrop.ipynb.expected`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_drop_tagged_cells.ipynb` & `nbwipers-0.3.6/tests/e2e_notebooks/test_drop_tagged_cells.ipynb`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_drop_tagged_cells.ipynb.expected` & `nbwipers-0.3.6/tests/e2e_notebooks/test_drop_tagged_cells.ipynb.expected`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_drop_tagged_cells_dontdrop.ipynb.expected` & `nbwipers-0.3.6/tests/e2e_notebooks/test_drop_tagged_cells_dontdrop.ipynb.expected`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_execution_timing.ipynb` & `nbwipers-0.3.6/tests/e2e_notebooks/test_execution_timing.ipynb`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_execution_timing.ipynb.expected` & `nbwipers-0.3.6/tests/e2e_notebooks/test_execution_timing.ipynb.expected`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_max_size.ipynb` & `nbwipers-0.3.6/tests/e2e_notebooks/test_max_size.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555556%*

 * *Differences: {"'cells'": '{1: {\'source\': [\'print("a" * 10)\']}, 2: {\'source\': [\'print("a" * 100)\']}}'}*

```diff
@@ -24,15 +24,15 @@
                     "output_type": "stream",
                     "text": [
                         "aaaaaaaaaa\n"
                     ]
                 }
             ],
             "source": [
-                "print(\"a\"*10)"
+                "print(\"a\" * 10)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "89ff455b",
             "metadata": {
@@ -47,15 +47,15 @@
                     "output_type": "stream",
                     "text": [
                         "aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa\n"
                     ]
                 }
             ],
             "source": [
-                "print(\"a\"*100)"
+                "print(\"a\" * 100)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
```

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_max_size.ipynb.expected` & `nbwipers-0.3.6/tests/e2e_notebooks/test_max_size.ipynb.expected`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_max_size.ipynb.expected_sequential_id` & `nbwipers-0.3.6/tests/e2e_notebooks/test_max_size.sequential_id.ipynb.expected`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_metadata.ipynb` & `nbwipers-0.3.6/tests/e2e_notebooks/test_metadata.ipynb`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_metadata.ipynb.expected` & `nbwipers-0.3.6/tests/e2e_notebooks/test_metadata.ipynb.expected`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_exception.ipynb` & `nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_exception.ipynb`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_extra_keys.ipynb.expected` & `nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_extra_keys.ipynb.expected`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_keep_count.ipynb.expected` & `nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_keep_count.ipynb.expected`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_keep_output.ipynb.expected` & `nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_keep_output.ipynb.expected`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_keep_output_keep_count.ipynb.expected` & `nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_keep_output_keep_count.ipynb.expected`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_notebook.ipynb` & `nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_notebook.ipynb.expected` & `nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_notebook.ipynb.expected`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_metadata_period.ipynb` & `nbwipers-0.3.6/tests/e2e_notebooks/test_metadata_period.ipynb`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_nbformat45.ipynb` & `nbwipers-0.3.6/tests/e2e_notebooks/test_nbformat45.ipynb`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_nbformat45.ipynb.expected` & `nbwipers-0.3.6/tests/e2e_notebooks/test_nbformat45.ipynb.expected`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_nbformat45.ipynb.expected_sequential_id` & `nbwipers-0.3.6/tests/e2e_notebooks/test_nbformat45.sequential_id.ipynb.expected`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_strip_init_cells.ipynb` & `nbwipers-0.3.6/tests/e2e_notebooks/test_strip_init_cells.ipynb`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_strip_init_cells.ipynb.expected` & `nbwipers-0.3.6/tests/e2e_notebooks/test_strip_init_cells.ipynb.expected`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_unicode.ipynb` & `nbwipers-0.3.6/tests/e2e_notebooks/test_unicode.ipynb`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_unicode.ipynb.expected` & `nbwipers-0.3.6/tests/e2e_notebooks/test_unicode.ipynb.expected`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_widgets.ipynb` & `nbwipers-0.3.6/tests/e2e_notebooks/test_widgets.ipynb`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/e2e_notebooks/test_widgets.ipynb.expected` & `nbwipers-0.3.6/tests/e2e_notebooks/test_widgets.ipynb.expected`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/integration_test.rs` & `nbwipers-0.3.6/tests/integration_test.rs`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/tests/notebook_test.rs` & `nbwipers-0.3.6/tests/notebook_test.rs`

 * *Files 0% similar despite different names*

```diff
@@ -225,20 +225,20 @@
         &["-c", "tests/e2e_notebooks/test_nbformat45.toml"],
     );
 }
 #[test]
 fn test_nbformat45_expected_sequential_id() {
     test_expected(
         "tests/e2e_notebooks/test_nbformat45.ipynb",
-        "tests/e2e_notebooks/test_nbformat45.ipynb.expected_sequential_id",
+        "tests/e2e_notebooks/test_nbformat45.sequential_id.ipynb.expected",
         &["--drop-id"],
     );
     test_expected(
         "tests/e2e_notebooks/test_nbformat45.ipynb",
-        "tests/e2e_notebooks/test_nbformat45.ipynb.expected_sequential_id",
+        "tests/e2e_notebooks/test_nbformat45.sequential_id.ipynb.expected",
         &["-c", "tests/e2e_notebooks/test_nbformat45_sequential.toml"],
     );
 }
 #[test]
 fn test_unicode() {
     test_expected(
         "tests/e2e_notebooks/test_unicode.ipynb",
```

### Comparing `nbwipers-0.3.5/tests/test_nbformat2.ipynb` & `nbwipers-0.3.6/tests/test_nbformat2.ipynb`

 * *Files identical despite different names*

### Comparing `nbwipers-0.3.5/PKG-INFO` & `nbwipers-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.3
 Name: nbwipers
-Version: 0.3.5
+Version: 0.3.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Wipe clean your Jupyter Notebooks!
+Keywords: python,notebook,jupyter,ci,pre-commit
 Home-Page: https://github.com/felixgwilliams/nbwipers
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/felixgwilliams/nbwipers
 
 # nbwipers
```

