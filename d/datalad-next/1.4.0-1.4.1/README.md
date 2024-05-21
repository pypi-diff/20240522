# Comparing `tmp/datalad_next-1.4.0.tar.gz` & `tmp/datalad_next-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalad_next-1.4.0.tar", last modified: Fri May 17 19:27:07 2024, max compression
+gzip compressed data, was "datalad_next-1.4.1.tar", last modified: Tue May 21 22:17:30 2024, max compression
```

## Comparing `datalad_next-1.4.0.tar` & `datalad_next-1.4.1.tar`

### file list

```diff
@@ -1,354 +1,356 @@
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.642464 datalad_next-1.4.0/
--rw-rw-r--   0 mih       (1000) mih       (1000)     4809 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.all-contributorsrc
--rw-rw-r--   0 mih       (1000) mih       (1000)    16333 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.appveyor.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)      265 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.codeclimate.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)       46 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.codespell-exclude
--rw-rw-r--   0 mih       (1000) mih       (1000)       79 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.codespellrc
--rw-rw-r--   0 mih       (1000) mih       (1000)      286 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.coveragerc
--rw-rw-r--   0 mih       (1000) mih       (1000)       38 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.gitattributes
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/.github/
--rw-rw-r--   0 mih       (1000) mih       (1000)      657 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/.github/workflows/
--rw-rw-r--   0 mih       (1000) mih       (1000)      377 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.github/workflows/codespell.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)      613 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.github/workflows/docbuild.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)     1523 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.github/workflows/mypy.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)     2830 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.github/workflows/update-contributors.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)      123 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.gitignore
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.noannex
--rw-rw-r--   0 mih       (1000) mih       (1000)     2394 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.zenodo.json
--rw-rw-r--   0 mih       (1000) mih       (1000)    58894 2024-05-17 19:26:55.000000 datalad_next-1.4.0/CHANGELOG.md
--rw-rw-r--   0 mih       (1000) mih       (1000)     2451 2024-05-17 19:26:55.000000 datalad_next-1.4.0/CITATION.cff
--rw-rw-r--   0 mih       (1000) mih       (1000)     8180 2024-05-17 19:26:55.000000 datalad_next-1.4.0/CONTRIBUTING.md
--rw-rw-r--   0 mih       (1000) mih       (1000)       55 2024-05-17 19:26:55.000000 datalad_next-1.4.0/CONTRIBUTORS
--rw-rw-r--   0 mih       (1000) mih       (1000)     1609 2024-05-17 19:26:55.000000 datalad_next-1.4.0/LICENSE
--rw-rw-r--   0 mih       (1000) mih       (1000)      124 2024-05-17 19:26:55.000000 datalad_next-1.4.0/MANIFEST.in
--rw-rw-r--   0 mih       (1000) mih       (1000)      506 2024-05-17 19:26:55.000000 datalad_next-1.4.0/Makefile
--rw-r--r--   0 mih       (1000) mih       (1000)    19945 2024-05-17 19:27:07.642464 datalad_next-1.4.0/PKG-INFO
--rw-rw-r--   0 mih       (1000) mih       (1000)    18914 2024-05-17 19:26:55.000000 datalad_next-1.4.0/README.md
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/_datalad_buildsupport/
--rw-rw-r--   0 mih       (1000) mih       (1000)      529 2024-05-17 19:26:55.000000 datalad_next-1.4.0/_datalad_buildsupport/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    10699 2024-05-17 19:26:55.000000 datalad_next-1.4.0/_datalad_buildsupport/formatters.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8520 2024-05-17 19:26:55.000000 datalad_next-1.4.0/_datalad_buildsupport/setup.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/changelog.d/
--rw-rw-r--   0 mih       (1000) mih       (1000)      234 2024-05-17 19:26:55.000000 datalad_next-1.4.0/changelog.d/README
--rw-rw-r--   0 mih       (1000) mih       (1000)      312 2024-05-17 19:26:55.000000 datalad_next-1.4.0/changelog.d/scriv.ini
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/changelog.d/templates/
--rw-rw-r--   0 mih       (1000) mih       (1000)       74 2024-05-17 19:26:55.000000 datalad_next-1.4.0/changelog.d/templates/entry_title.md.j2
--rw-rw-r--   0 mih       (1000) mih       (1000)      349 2024-05-17 19:26:55.000000 datalad_next-1.4.0/changelog.d/templates/new_fragment.md.j2
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/
--rw-rw-r--   0 mih       (1000) mih       (1000)     4028 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      497 2024-05-17 19:27:07.642464 datalad_next-1.4.0/datalad_next/_version.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/annexbackends/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexbackends/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    10375 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexbackends/base.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/annexbackends/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexbackends/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1978 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexbackends/tests/test_base.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2429 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexbackends/xdlra.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/annexremotes/
--rw-rw-r--   0 mih       (1000) mih       (1000)     3639 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexremotes/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    23285 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexremotes/archivist.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/annexremotes/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexremotes/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     9576 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexremotes/tests/test_archivist.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    16906 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexremotes/tests/test_uncurl.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    22959 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexremotes/uncurl.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/archive_operations/
--rw-rw-r--   0 mih       (1000) mih       (1000)      870 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/archive_operations/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3181 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/archive_operations/base.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3828 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/archive_operations/tarfile.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/archive_operations/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/archive_operations/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2670 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/archive_operations/tests/test_tarfile.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3111 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/archive_operations/tests/test_zipfile.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4315 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/archive_operations/zipfile.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/commands/
--rw-rw-r--   0 mih       (1000) mih       (1000)     3702 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    26365 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/create_sibling_webdav.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    19186 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/credentials.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    14081 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/download.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    17496 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/ls_file_collection.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4426 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/results.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    14601 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/status.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/commands/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    15000 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/tests/test_create_sibling_webdav.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     6160 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/tests/test_credentials.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     9133 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/tests/test_download.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8333 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/tests/test_ls_file_collection.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1766 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/tests/test_results.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1819 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/tests/test_status.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    31754 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/tests/test_tree.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    46335 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/tree.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/config/
--rw-rw-r--   0 mih       (1000) mih       (1000)      244 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/config/__init__.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/config/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/config/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      325 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/config/tests/test_core.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5747 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/config/tests/test_utils.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3904 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/config/utils.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2197 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/conftest.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/constraints/
--rw-rw-r--   0 mih       (1000) mih       (1000)     3490 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8724 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/base.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    16694 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/basic.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    18795 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/compound.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4774 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/dataset.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    12974 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/exceptions.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3881 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/formats.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5669 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/git.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    18669 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/parameter.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     7361 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/parameter_legacy.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/constraints/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4416 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/tests/test_base.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     9875 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/tests/test_basic.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    11946 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/tests/test_cmdarg_validation.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     9523 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/tests/test_compound.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1807 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/tests/test_exceptions.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    14738 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/tests/test_special_purpose.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2072 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/tests/test_tutorial.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1047 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/utils.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/consts/
--rw-rw-r--   0 mih       (1000) mih       (1000)      775 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/consts/__init__.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/credman/
--rw-rw-r--   0 mih       (1000) mih       (1000)      232 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/credman/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    43876 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/credman/manager.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/credman/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/credman/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    15102 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/credman/tests/test_credman.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/datasets/
--rw-rw-r--   0 mih       (1000) mih       (1000)     1788 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/datasets/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1805 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/datasets/annexrepo.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/exceptions/
--rw-rw-r--   0 mih       (1000) mih       (1000)      779 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/exceptions/__init__.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/gitremotes/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/gitremotes/__init__.py
--rwxrwxr-x   0 mih       (1000) mih       (1000)    52669 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/gitremotes/datalad_annex.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/gitremotes/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/gitremotes/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    14941 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/gitremotes/tests/test_datalad_annex.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/iter_collections/
--rw-rw-r--   0 mih       (1000) mih       (1000)     2182 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    14857 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/annexworktree.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2183 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/directory.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    18526 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/gitdiff.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    20038 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/gitstatus.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4529 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/gittree.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    13158 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/gitworktree.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3475 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tarfile.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/iter_collections/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4939 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/test_iterannexworktree.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2844 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/test_iterdir.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    12436 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itergitdiff.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    10920 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itergitstatus.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3353 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itergittree.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8321 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itergitworktree.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3357 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itertar.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2454 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/test_iterzip.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      994 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/test_utils.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3663 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/utils.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2812 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/zipfile.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/iterable_subprocess/
--rw-rw-r--   0 mih       (1000) mih       (1000)       20 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/.coveragerc
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.622464 datalad_next-1.4.0/datalad_next/iterable_subprocess/.github/
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/iterable_subprocess/.github/workflows/
--rw-rw-r--   0 mih       (1000) mih       (1000)      993 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/.github/workflows/deploy-package-to-pypi.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)      819 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/.github/workflows/test.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)     1799 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/.gitignore
--rw-rw-r--   0 mih       (1000) mih       (1000)     1091 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/LICENSE
--rw-rw-r--   0 mih       (1000) mih       (1000)     3710 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/README.md
--rw-rw-r--   0 mih       (1000) mih       (1000)      859 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)       15 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/codecov.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)     7086 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/iterable_subprocess.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      736 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/pyproject.toml
--rw-rw-r--   0 mih       (1000) mih       (1000)    11706 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/test_iterable_subprocess.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.634464 datalad_next-1.4.0/datalad_next/itertools/
--rw-rw-r--   0 mih       (1000) mih       (1000)      523 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4520 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/align_pattern.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5286 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/decode_bytes.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5703 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/itemize.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4065 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/load_json.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8378 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/reroute.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.634464 datalad_next-1.4.0/datalad_next/itertools/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2048 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/tests/test_align_pattern.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1078 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/tests/test_decode_bytes.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1225 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/tests/test_itemize.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1381 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/tests/test_load_json.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1588 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/tests/test_reroute.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.634464 datalad_next-1.4.0/datalad_next/patches/
--rw-rw-r--   0 mih       (1000) mih       (1000)     2009 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2252 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/add_method_url2transport_path.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4173 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/annexrepo.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2075 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/cli_configoverrides.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1326 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/commanderror.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      491 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/common_cfg.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     6849 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/configuration.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5443 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/create_sibling_ghlike.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    16127 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/create_sibling_gitlab.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     6224 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/customremotes_main.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1173 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/distribution_dataset.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      434 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/enabled.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    37392 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/fix_ria_ora_tests.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    11068 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/interface_utils.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      646 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/patch_ria_ora.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    17041 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/push_optimize.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    10128 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/push_to_export_remote.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    35692 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/replace_create_sibling_ria.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    41308 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/replace_ora_remote.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    13580 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/replace_sshremoteio.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8093 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/ria_utils.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3067 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/run.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2424 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/siblings.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2525 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/ssh_exec.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4330 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/sshconnector.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      827 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/test_keyring.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.634464 datalad_next-1.4.0/datalad_next/patches/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1607 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_add_method_url2transport_path.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2347 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_annex_progress_logging.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      615 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_cli_configoverrides.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      721 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_commanderror.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1798 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_configuration.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1465 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_create_sibling_ghlike.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    17167 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_create_sibling_gitlab.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1421 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_push.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     7798 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_push_to_export_remote.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1436 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_replace_ora_remote.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      977 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_ria.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      839 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_run.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3393 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_sshremoteio.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2129 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/update.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.634464 datalad_next-1.4.0/datalad_next/repo_utils/
--rw-rw-r--   0 mih       (1000) mih       (1000)      267 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/repo_utils/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1240 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/repo_utils/annex.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.634464 datalad_next-1.4.0/datalad_next/repo_utils/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/repo_utils/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      610 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/repo_utils/tests/test_annex.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1098 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/repo_utils/tests/test_head.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1909 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/repo_utils/worktree.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.634464 datalad_next-1.4.0/datalad_next/runners/
--rw-rw-r--   0 mih       (1000) mih       (1000)     3001 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/runners/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     6380 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/runners/git.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4167 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/runners/iter_subproc.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      887 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/runners/protocols.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/runners/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/runners/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1190 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/runners/tests/test_git.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      946 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/runners/tests/test_iter_subproc.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/shell/
--rw-rw-r--   0 mih       (1000) mih       (1000)     7843 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/shell/__init__.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/shell/operations/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/shell/operations/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3070 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/shell/operations/common.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    11452 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/shell/operations/posix.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    10989 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/shell/response_generators.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    27832 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/shell/shell.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/shell/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/shell/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3835 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/shell/tests/test_response_generators.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    18189 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/shell/tests/test_shell.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)     1081 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    24864 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/tests/fixtures.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      156 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/tests/marker.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      142 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/tests/test_common_cfg.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      120 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/tests/test_register.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      486 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/tests/test_testutils.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     9422 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/tests/utils.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/types/
--rw-rw-r--   0 mih       (1000) mih       (1000)      267 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/types/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1523 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/types/annexkey.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5417 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/types/archivist.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      266 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/types/enums.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/types/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/types/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      905 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/types/tests/test_annexkey.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2020 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/types/tests/test_archivist.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/uis/
--rw-rw-r--   0 mih       (1000) mih       (1000)      337 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/uis/__init__.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/url_operations/
--rw-rw-r--   0 mih       (1000) mih       (1000)     1419 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8076 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/any.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    14899 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/base.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2091 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/exceptions.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     9046 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/file.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    11849 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/http.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    14741 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/ssh.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/url_operations/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2041 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/tests/test_any.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3443 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/tests/test_file.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5066 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/tests/test_http.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4598 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/tests/test_ssh.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/utils/
--rw-rw-r--   0 mih       (1000) mih       (1000)     2778 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      134 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/consts.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      326 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/credman.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3927 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/deprecate.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2667 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/http_helpers.py
--rw-rw-r--   0 mih       (1000) mih       (1000)       37 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/log.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1737 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/multihash.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      857 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/patch.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    15257 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/requests_auth.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5859 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/specialremote.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/utils/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5673 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/tests/test_deprecated.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      543 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/tests/test_multihash.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      240 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/tests/test_paramdictator.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1486 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/tests/test_parse_www_authenticate.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      483 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/tests/test_patch.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next.egg-info/
--rw-r--r--   0 mih       (1000) mih       (1000)    19945 2024-05-17 19:27:07.000000 datalad_next-1.4.0/datalad_next.egg-info/PKG-INFO
--rw-rw-r--   0 mih       (1000) mih       (1000)    10974 2024-05-17 19:27:07.000000 datalad_next-1.4.0/datalad_next.egg-info/SOURCES.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)        1 2024-05-17 19:27:07.000000 datalad_next-1.4.0/datalad_next.egg-info/dependency_links.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)      342 2024-05-17 19:27:07.000000 datalad_next-1.4.0/datalad_next.egg-info/entry_points.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)      167 2024-05-17 19:27:07.000000 datalad_next-1.4.0/datalad_next.egg-info/requires.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)       13 2024-05-17 19:27:07.000000 datalad_next-1.4.0/datalad_next.egg-info/top_level.txt
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/docs/
--rw-rw-r--   0 mih       (1000) mih       (1000)      658 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/CODEOWNERS
--rw-rw-r--   0 mih       (1000) mih       (1000)     7496 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/Makefile
--rw-rw-r--   0 mih       (1000) mih       (1000)     1755 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/README.md
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/docs/policy/
--rw-rw-r--   0 mih       (1000) mih       (1000)      826 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/policy/release-management.md
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.642464 datalad_next-1.4.0/docs/source/
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.642464 datalad_next-1.4.0/docs/source/_static/
--rw-rw-r--   0 mih       (1000) mih       (1000)      958 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/_static/datalad_logo.png
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.622464 datalad_next-1.4.0/docs/source/_templates/
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.642464 datalad_next-1.4.0/docs/source/_templates/autosummary/
--rw-rw-r--   0 mih       (1000) mih       (1000)      116 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/_templates/autosummary/class.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      436 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/_templates/autosummary/module.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      142 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/annex-backends.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      179 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/annex-specialremotes.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      218 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/api.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      306 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/cmd.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)     4843 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/conf.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.642464 datalad_next-1.4.0/docs/source/developer_guide/
--rw-rw-r--   0 mih       (1000) mih       (1000)     3431 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/developer_guide/constraints.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      497 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/developer_guide/contributing.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      314 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/developer_guide/index.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      140 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/git-remote-helpers.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)     3476 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/index.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      690 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/patches.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      744 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/pyutils.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)       60 2024-05-17 19:26:55.000000 datalad_next-1.4.0/pyproject.toml
--rw-rw-r--   0 mih       (1000) mih       (1000)      554 2024-05-17 19:26:55.000000 datalad_next-1.4.0/readthedocs.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)      128 2024-05-17 19:26:55.000000 datalad_next-1.4.0/requirements-devel.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)     1419 2024-05-17 19:27:07.642464 datalad_next-1.4.0/setup.cfg
--rwxrwxr-x   0 mih       (1000) mih       (1000)      364 2024-05-17 19:26:55.000000 datalad_next-1.4.0/setup.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.622464 datalad_next-1.4.0/tools/
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.642464 datalad_next-1.4.0/tools/appveyor/
--rw-rw-r--   0 mih       (1000) mih       (1000)      291 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/chmod600.bat
--rwxrwxr-x   0 mih       (1000) mih       (1000)      311 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/docker-load-httpbin
--rwxrwxr-x   0 mih       (1000) mih       (1000)      124 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/enable-ssh-login
--rw-rw-r--   0 mih       (1000) mih       (1000)      101 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/env_setup.bat
--rwxrwxr-x   0 mih       (1000) mih       (1000)      399 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/install-git-annex
--rwxrwxr-x   0 mih       (1000) mih       (1000)      331 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/install-syspkgs
--rwxrwxr-x   0 mih       (1000) mih       (1000)     1464 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/setup-sshd
--rw-rw-r--   0 mih       (1000) mih       (1000)     1054 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/setup-sshd.bat
--rwxrwxr-x   0 mih       (1000) mih       (1000)      330 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/verify-ssh-access
--rw-rw-r--   0 mih       (1000) mih       (1000)      343 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/verify-ssh-access.bat
--rw-rw-r--   0 mih       (1000) mih       (1000)    86677 2024-05-17 19:26:55.000000 datalad_next-1.4.0/versioneer.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.254108 datalad_next-1.4.1/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4809 2024-05-21 22:17:23.000000 datalad_next-1.4.1/.all-contributorsrc
+-rw-rw-r--   0 mih       (1000) mih       (1000)    16333 2024-05-21 22:17:23.000000 datalad_next-1.4.1/.appveyor.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)      489 2024-05-21 22:17:23.000000 datalad_next-1.4.1/.changelog.md.j2
+-rw-rw-r--   0 mih       (1000) mih       (1000)      265 2024-05-21 22:17:23.000000 datalad_next-1.4.1/.codeclimate.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)       46 2024-05-21 22:17:23.000000 datalad_next-1.4.1/.codespell-exclude
+-rw-rw-r--   0 mih       (1000) mih       (1000)       79 2024-05-21 22:17:23.000000 datalad_next-1.4.1/.codespellrc
+-rw-rw-r--   0 mih       (1000) mih       (1000)      286 2024-05-21 22:17:23.000000 datalad_next-1.4.1/.coveragerc
+-rw-rw-r--   0 mih       (1000) mih       (1000)       38 2024-05-21 22:17:23.000000 datalad_next-1.4.1/.gitattributes
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.234108 datalad_next-1.4.1/.github/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      657 2024-05-21 22:17:23.000000 datalad_next-1.4.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.234108 datalad_next-1.4.1/.github/workflows/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      377 2024-05-21 22:17:23.000000 datalad_next-1.4.1/.github/workflows/codespell.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)      796 2024-05-21 22:17:23.000000 datalad_next-1.4.1/.github/workflows/conventional-commits.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)      613 2024-05-21 22:17:23.000000 datalad_next-1.4.1/.github/workflows/docbuild.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1523 2024-05-21 22:17:23.000000 datalad_next-1.4.1/.github/workflows/mypy.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2830 2024-05-21 22:17:23.000000 datalad_next-1.4.1/.github/workflows/update-contributors.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)      123 2024-05-21 22:17:23.000000 datalad_next-1.4.1/.gitignore
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/.noannex
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2394 2024-05-21 22:17:23.000000 datalad_next-1.4.1/.zenodo.json
+-rw-rw-r--   0 mih       (1000) mih       (1000)    59263 2024-05-21 22:17:23.000000 datalad_next-1.4.1/CHANGELOG.md
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2451 2024-05-21 22:17:23.000000 datalad_next-1.4.1/CITATION.cff
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8328 2024-05-21 22:17:23.000000 datalad_next-1.4.1/CONTRIBUTING.md
+-rw-rw-r--   0 mih       (1000) mih       (1000)       55 2024-05-21 22:17:23.000000 datalad_next-1.4.1/CONTRIBUTORS
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1609 2024-05-21 22:17:23.000000 datalad_next-1.4.1/LICENSE
+-rw-rw-r--   0 mih       (1000) mih       (1000)      124 2024-05-21 22:17:23.000000 datalad_next-1.4.1/MANIFEST.in
+-rw-rw-r--   0 mih       (1000) mih       (1000)      506 2024-05-21 22:17:23.000000 datalad_next-1.4.1/Makefile
+-rw-r--r--   0 mih       (1000) mih       (1000)    20512 2024-05-21 22:17:30.254108 datalad_next-1.4.1/PKG-INFO
+-rw-rw-r--   0 mih       (1000) mih       (1000)    19481 2024-05-21 22:17:23.000000 datalad_next-1.4.1/README.md
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.234108 datalad_next-1.4.1/_datalad_buildsupport/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      529 2024-05-21 22:17:23.000000 datalad_next-1.4.1/_datalad_buildsupport/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    10699 2024-05-21 22:17:23.000000 datalad_next-1.4.1/_datalad_buildsupport/formatters.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8520 2024-05-21 22:17:23.000000 datalad_next-1.4.1/_datalad_buildsupport/setup.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.234108 datalad_next-1.4.1/changelog.d/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      234 2024-05-21 22:17:23.000000 datalad_next-1.4.1/changelog.d/README
+-rw-rw-r--   0 mih       (1000) mih       (1000)      312 2024-05-21 22:17:23.000000 datalad_next-1.4.1/changelog.d/scriv.ini
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.234108 datalad_next-1.4.1/changelog.d/templates/
+-rw-rw-r--   0 mih       (1000) mih       (1000)       74 2024-05-21 22:17:23.000000 datalad_next-1.4.1/changelog.d/templates/entry_title.md.j2
+-rw-rw-r--   0 mih       (1000) mih       (1000)      349 2024-05-21 22:17:23.000000 datalad_next-1.4.1/changelog.d/templates/new_fragment.md.j2
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.234108 datalad_next-1.4.1/datalad_next/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4028 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      497 2024-05-21 22:17:30.254108 datalad_next-1.4.1/datalad_next/_version.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.238108 datalad_next-1.4.1/datalad_next/annexbackends/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/annexbackends/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    10375 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/annexbackends/base.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.238108 datalad_next-1.4.1/datalad_next/annexbackends/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/annexbackends/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1978 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/annexbackends/tests/test_base.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2429 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/annexbackends/xdlra.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.238108 datalad_next-1.4.1/datalad_next/annexremotes/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3639 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/annexremotes/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    23285 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/annexremotes/archivist.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.238108 datalad_next-1.4.1/datalad_next/annexremotes/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/annexremotes/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9576 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/annexremotes/tests/test_archivist.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    16906 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/annexremotes/tests/test_uncurl.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    22959 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/annexremotes/uncurl.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.238108 datalad_next-1.4.1/datalad_next/archive_operations/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      870 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/archive_operations/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3181 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/archive_operations/base.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3828 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/archive_operations/tarfile.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.238108 datalad_next-1.4.1/datalad_next/archive_operations/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/archive_operations/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2677 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/archive_operations/tests/test_tarfile.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3120 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/archive_operations/tests/test_zipfile.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4315 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/archive_operations/zipfile.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.238108 datalad_next-1.4.1/datalad_next/commands/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3702 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/commands/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    26365 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/commands/create_sibling_webdav.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    19186 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/commands/credentials.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    14081 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/commands/download.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    17496 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/commands/ls_file_collection.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4426 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/commands/results.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    14601 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/commands/status.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.238108 datalad_next-1.4.1/datalad_next/commands/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/commands/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    15000 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/commands/tests/test_create_sibling_webdav.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     6160 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/commands/tests/test_credentials.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9133 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/commands/tests/test_download.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8333 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/commands/tests/test_ls_file_collection.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1766 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/commands/tests/test_results.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1819 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/commands/tests/test_status.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    31754 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/commands/tests/test_tree.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    46335 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/commands/tree.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.238108 datalad_next-1.4.1/datalad_next/config/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      244 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/config/__init__.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.238108 datalad_next-1.4.1/datalad_next/config/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/config/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      325 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/config/tests/test_core.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5747 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/config/tests/test_utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3904 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/config/utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2197 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/conftest.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.238108 datalad_next-1.4.1/datalad_next/constraints/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3490 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8724 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/base.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    16694 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/basic.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    18795 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/compound.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4774 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/dataset.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    12974 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/exceptions.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3881 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/formats.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5669 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/git.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    18669 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/parameter.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     7361 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/parameter_legacy.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.242108 datalad_next-1.4.1/datalad_next/constraints/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4416 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/tests/test_base.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9875 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/tests/test_basic.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    11946 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/tests/test_cmdarg_validation.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9523 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/tests/test_compound.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1807 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/tests/test_exceptions.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    14738 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/tests/test_special_purpose.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2072 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/tests/test_tutorial.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1047 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/constraints/utils.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.242108 datalad_next-1.4.1/datalad_next/consts/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      775 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/consts/__init__.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.242108 datalad_next-1.4.1/datalad_next/credman/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      232 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/credman/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    43876 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/credman/manager.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.242108 datalad_next-1.4.1/datalad_next/credman/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/credman/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    15102 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/credman/tests/test_credman.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.242108 datalad_next-1.4.1/datalad_next/datasets/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1788 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/datasets/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1805 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/datasets/annexrepo.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.242108 datalad_next-1.4.1/datalad_next/exceptions/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      779 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/exceptions/__init__.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.242108 datalad_next-1.4.1/datalad_next/gitremotes/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/gitremotes/__init__.py
+-rwxrwxr-x   0 mih       (1000) mih       (1000)    52669 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/gitremotes/datalad_annex.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.242108 datalad_next-1.4.1/datalad_next/gitremotes/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/gitremotes/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    14941 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/gitremotes/tests/test_datalad_annex.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.242108 datalad_next-1.4.1/datalad_next/iter_collections/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2182 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    14857 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/annexworktree.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2183 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/directory.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    18536 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/gitdiff.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    20171 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/gitstatus.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4529 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/gittree.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    13158 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/gitworktree.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3475 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/tarfile.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.242108 datalad_next-1.4.1/datalad_next/iter_collections/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4939 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/tests/test_iterannexworktree.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2844 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/tests/test_iterdir.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    12436 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/tests/test_itergitdiff.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    10920 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/tests/test_itergitstatus.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3353 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/tests/test_itergittree.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8321 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/tests/test_itergitworktree.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3357 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/tests/test_itertar.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2454 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/tests/test_iterzip.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      994 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/tests/test_utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3663 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2812 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iter_collections/zipfile.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.242108 datalad_next-1.4.1/datalad_next/iterable_subprocess/
+-rw-rw-r--   0 mih       (1000) mih       (1000)       20 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iterable_subprocess/.coveragerc
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.230108 datalad_next-1.4.1/datalad_next/iterable_subprocess/.github/
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.242108 datalad_next-1.4.1/datalad_next/iterable_subprocess/.github/workflows/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      993 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iterable_subprocess/.github/workflows/deploy-package-to-pypi.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)      819 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iterable_subprocess/.github/workflows/test.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1799 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iterable_subprocess/.gitignore
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1091 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iterable_subprocess/LICENSE
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3710 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iterable_subprocess/README.md
+-rw-rw-r--   0 mih       (1000) mih       (1000)      859 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iterable_subprocess/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)       15 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iterable_subprocess/codecov.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)     7086 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iterable_subprocess/iterable_subprocess.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      736 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iterable_subprocess/pyproject.toml
+-rw-rw-r--   0 mih       (1000) mih       (1000)    11706 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/iterable_subprocess/test_iterable_subprocess.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.242108 datalad_next-1.4.1/datalad_next/itertools/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      523 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/itertools/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4520 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/itertools/align_pattern.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5286 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/itertools/decode_bytes.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5703 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/itertools/itemize.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4065 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/itertools/load_json.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8378 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/itertools/reroute.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.246108 datalad_next-1.4.1/datalad_next/itertools/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/itertools/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2048 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/itertools/tests/test_align_pattern.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1078 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/itertools/tests/test_decode_bytes.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1225 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/itertools/tests/test_itemize.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1381 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/itertools/tests/test_load_json.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1588 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/itertools/tests/test_reroute.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.246108 datalad_next-1.4.1/datalad_next/patches/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2009 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2252 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/add_method_url2transport_path.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4173 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/annexrepo.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2075 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/cli_configoverrides.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1326 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/commanderror.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      491 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/common_cfg.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     6849 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/configuration.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5443 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/create_sibling_ghlike.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    16127 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/create_sibling_gitlab.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     6224 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/customremotes_main.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1173 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/distribution_dataset.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      434 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/enabled.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    37392 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/fix_ria_ora_tests.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    11068 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/interface_utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      953 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/patch_ria_ora.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    17041 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/push_optimize.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    10128 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/push_to_export_remote.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    35692 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/replace_create_sibling_ria.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    41308 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/replace_ora_remote.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    13580 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/replace_sshremoteio.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8093 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/ria_utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3067 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/run.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2424 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/siblings.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2525 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/ssh_exec.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4330 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/sshconnector.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      827 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/test_keyring.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.246108 datalad_next-1.4.1/datalad_next/patches/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1607 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/tests/test_add_method_url2transport_path.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2347 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/tests/test_annex_progress_logging.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      615 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/tests/test_cli_configoverrides.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      721 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/tests/test_commanderror.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1798 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/tests/test_configuration.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1465 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/tests/test_create_sibling_ghlike.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    17167 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/tests/test_create_sibling_gitlab.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1421 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/tests/test_push.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     7798 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/tests/test_push_to_export_remote.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1436 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/tests/test_replace_ora_remote.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      977 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/tests/test_ria.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      839 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/tests/test_run.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3393 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/tests/test_sshremoteio.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2129 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/patches/update.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.246108 datalad_next-1.4.1/datalad_next/repo_utils/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      267 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/repo_utils/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1240 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/repo_utils/annex.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.246108 datalad_next-1.4.1/datalad_next/repo_utils/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/repo_utils/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      610 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/repo_utils/tests/test_annex.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1098 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/repo_utils/tests/test_head.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1909 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/repo_utils/worktree.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.250108 datalad_next-1.4.1/datalad_next/runners/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3001 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/runners/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     6380 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/runners/git.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4167 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/runners/iter_subproc.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      887 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/runners/protocols.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.250108 datalad_next-1.4.1/datalad_next/runners/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/runners/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1190 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/runners/tests/test_git.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      946 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/runners/tests/test_iter_subproc.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.250108 datalad_next-1.4.1/datalad_next/shell/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     7843 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/shell/__init__.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.250108 datalad_next-1.4.1/datalad_next/shell/operations/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/shell/operations/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3070 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/shell/operations/common.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    11452 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/shell/operations/posix.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    10989 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/shell/response_generators.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    27832 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/shell/shell.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.250108 datalad_next-1.4.1/datalad_next/shell/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/shell/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3835 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/shell/tests/test_response_generators.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    18189 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/shell/tests/test_shell.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.250108 datalad_next-1.4.1/datalad_next/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1081 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    24864 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/tests/fixtures.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      156 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/tests/marker.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      142 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/tests/test_common_cfg.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      120 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/tests/test_register.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      486 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/tests/test_testutils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9436 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/tests/utils.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.250108 datalad_next-1.4.1/datalad_next/types/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      267 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/types/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1523 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/types/annexkey.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5417 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/types/archivist.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      266 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/types/enums.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.250108 datalad_next-1.4.1/datalad_next/types/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/types/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      905 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/types/tests/test_annexkey.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2020 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/types/tests/test_archivist.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.250108 datalad_next-1.4.1/datalad_next/uis/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      337 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/uis/__init__.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.250108 datalad_next-1.4.1/datalad_next/url_operations/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1419 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/url_operations/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8076 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/url_operations/any.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    14899 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/url_operations/base.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2091 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/url_operations/exceptions.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9046 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/url_operations/file.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    11849 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/url_operations/http.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    14741 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/url_operations/ssh.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.250108 datalad_next-1.4.1/datalad_next/url_operations/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/url_operations/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2041 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/url_operations/tests/test_any.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3443 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/url_operations/tests/test_file.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5066 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/url_operations/tests/test_http.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4598 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/url_operations/tests/test_ssh.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.250108 datalad_next-1.4.1/datalad_next/utils/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2778 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/utils/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      134 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/utils/consts.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      326 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/utils/credman.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3927 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/utils/deprecate.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2667 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/utils/http_helpers.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)       37 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/utils/log.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1737 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/utils/multihash.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      857 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/utils/patch.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    15257 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/utils/requests_auth.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5859 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/utils/specialremote.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.254108 datalad_next-1.4.1/datalad_next/utils/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/utils/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5673 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/utils/tests/test_deprecated.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      543 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/utils/tests/test_multihash.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      240 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/utils/tests/test_paramdictator.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1486 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/utils/tests/test_parse_www_authenticate.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      483 2024-05-21 22:17:23.000000 datalad_next-1.4.1/datalad_next/utils/tests/test_patch.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.238108 datalad_next-1.4.1/datalad_next.egg-info/
+-rw-r--r--   0 mih       (1000) mih       (1000)    20512 2024-05-21 22:17:30.000000 datalad_next-1.4.1/datalad_next.egg-info/PKG-INFO
+-rw-rw-r--   0 mih       (1000) mih       (1000)    11034 2024-05-21 22:17:30.000000 datalad_next-1.4.1/datalad_next.egg-info/SOURCES.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)        1 2024-05-21 22:17:30.000000 datalad_next-1.4.1/datalad_next.egg-info/dependency_links.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)      342 2024-05-21 22:17:30.000000 datalad_next-1.4.1/datalad_next.egg-info/entry_points.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)      167 2024-05-21 22:17:30.000000 datalad_next-1.4.1/datalad_next.egg-info/requires.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)       13 2024-05-21 22:17:30.000000 datalad_next-1.4.1/datalad_next.egg-info/top_level.txt
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.254108 datalad_next-1.4.1/docs/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      658 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/CODEOWNERS
+-rw-rw-r--   0 mih       (1000) mih       (1000)     7496 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/Makefile
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1755 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/README.md
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.254108 datalad_next-1.4.1/docs/policy/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      826 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/policy/release-management.md
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.254108 datalad_next-1.4.1/docs/source/
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.254108 datalad_next-1.4.1/docs/source/_static/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      958 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/source/_static/datalad_logo.png
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.234108 datalad_next-1.4.1/docs/source/_templates/
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.254108 datalad_next-1.4.1/docs/source/_templates/autosummary/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      116 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/source/_templates/autosummary/class.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      436 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/source/_templates/autosummary/module.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      142 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/source/annex-backends.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      179 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/source/annex-specialremotes.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      218 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/source/api.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      306 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/source/cmd.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4843 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/source/conf.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.254108 datalad_next-1.4.1/docs/source/developer_guide/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3431 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/source/developer_guide/constraints.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      497 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/source/developer_guide/contributing.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      314 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/source/developer_guide/index.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      140 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/source/git-remote-helpers.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3476 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/source/index.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      690 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/source/patches.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      744 2024-05-21 22:17:23.000000 datalad_next-1.4.1/docs/source/pyutils.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2117 2024-05-21 22:17:23.000000 datalad_next-1.4.1/pyproject.toml
+-rw-rw-r--   0 mih       (1000) mih       (1000)      554 2024-05-21 22:17:23.000000 datalad_next-1.4.1/readthedocs.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)      128 2024-05-21 22:17:23.000000 datalad_next-1.4.1/requirements-devel.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1419 2024-05-21 22:17:30.254108 datalad_next-1.4.1/setup.cfg
+-rwxrwxr-x   0 mih       (1000) mih       (1000)      364 2024-05-21 22:17:23.000000 datalad_next-1.4.1/setup.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.234108 datalad_next-1.4.1/tools/
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-21 22:17:30.254108 datalad_next-1.4.1/tools/appveyor/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      291 2024-05-21 22:17:23.000000 datalad_next-1.4.1/tools/appveyor/chmod600.bat
+-rwxrwxr-x   0 mih       (1000) mih       (1000)      311 2024-05-21 22:17:23.000000 datalad_next-1.4.1/tools/appveyor/docker-load-httpbin
+-rwxrwxr-x   0 mih       (1000) mih       (1000)      124 2024-05-21 22:17:23.000000 datalad_next-1.4.1/tools/appveyor/enable-ssh-login
+-rw-rw-r--   0 mih       (1000) mih       (1000)      101 2024-05-21 22:17:23.000000 datalad_next-1.4.1/tools/appveyor/env_setup.bat
+-rwxrwxr-x   0 mih       (1000) mih       (1000)      399 2024-05-21 22:17:23.000000 datalad_next-1.4.1/tools/appveyor/install-git-annex
+-rwxrwxr-x   0 mih       (1000) mih       (1000)      331 2024-05-21 22:17:23.000000 datalad_next-1.4.1/tools/appveyor/install-syspkgs
+-rwxrwxr-x   0 mih       (1000) mih       (1000)     1464 2024-05-21 22:17:23.000000 datalad_next-1.4.1/tools/appveyor/setup-sshd
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1054 2024-05-21 22:17:23.000000 datalad_next-1.4.1/tools/appveyor/setup-sshd.bat
+-rwxrwxr-x   0 mih       (1000) mih       (1000)      330 2024-05-21 22:17:23.000000 datalad_next-1.4.1/tools/appveyor/verify-ssh-access
+-rw-rw-r--   0 mih       (1000) mih       (1000)      343 2024-05-21 22:17:23.000000 datalad_next-1.4.1/tools/appveyor/verify-ssh-access.bat
+-rw-rw-r--   0 mih       (1000) mih       (1000)    86677 2024-05-21 22:17:23.000000 datalad_next-1.4.1/versioneer.py
```

### Comparing `datalad_next-1.4.0/.all-contributorsrc` & `datalad_next-1.4.1/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/.appveyor.yml` & `datalad_next-1.4.1/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/.github/PULL_REQUEST_TEMPLATE.md` & `datalad_next-1.4.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/.github/workflows/docbuild.yml` & `datalad_next-1.4.1/.github/workflows/docbuild.yml`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/.github/workflows/mypy.yml` & `datalad_next-1.4.1/.github/workflows/mypy.yml`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/.github/workflows/update-contributors.yml` & `datalad_next-1.4.1/.github/workflows/update-contributors.yml`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/.zenodo.json` & `datalad_next-1.4.1/.zenodo.json`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/CHANGELOG.md` & `datalad_next-1.4.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+## 1.4.1 (2024-05-22)
+
+### 🐛 Bug Fixes
+
+- dependencies: limit test patch import to test runs [905b99bd]
+
+### 📝 Documentation
+
+- add note of Git >= v2.31 requirement for next-status [093575d8]
+- state conventional-commits requirement [a9180fc0]
+
+### 🛡 Tests
+
+- fixture: add missing import (for non-WebDAV fallback) [ddd66799]
+
 # 1.4.0 (2024-05-17)
 
 ## 🐛 Bug Fixes
 
 - RIA over SSH access from Mac clients to Linux server was broken
   due to an inappropriate platform check that assumed that local and
   remote platform are identical.
@@ -336,14 +351,15 @@
 - A new `next-status` command provides a substantially faster
   alternative to the datalad-core `status` command. It is closely
   aligned to `git status` semantics, only reports changes (not repository
   listings), and supports type change detection. Moreover, it exposes
   the "monorepo" recursion mode, and single-directory reporting options
   of `iter_gitstatus()`. It is the first command to use `dataclass`
   instances as result types, rather than the traditional dictionaries.
+  Git v2.31 or later is required.
 
 - `SshUrlOperations` now supports non-standard SSH ports, non-default
   user names, and custom identity file specifications.
   Fixed https://github.com/datalad/datalad-next/issues/571 via
   https://github.com/datalad/datalad-next/pull/570 (by @mih)
 
 - A new `EnsureRemoteName` constraint improves the parameter validation
```

### Comparing `datalad_next-1.4.0/CITATION.cff` & `datalad_next-1.4.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/CONTRIBUTING.md` & `datalad_next-1.4.1/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 `datalad-next` is a staging area for features, hence any code is expected to move and morph. Therefore, tests are essential. A high test-coverage is desirable. Contributors should aim for 95% coverage or better. Tests must be dedicated for the code of a particular contribution. It is not sufficient, if other code happens to also exercise a new feature.
 
 New code should be type-annotated. At minimum, a type annotation of the main API (e.g., function signatures) is needed. A dedicated CI run is testing type annotations.
 
 Docstrings should be complete with information on parameters, return values, and exception behavior. Documentation should be added to and rendered with the sphinx-based documentation.
 
+Commits and commit messages must be [Conventional Commits](https://www.conventionalcommits.org). Their compliance is checked for each pull request.
 
 ### Code organization
 
 In `datalad-next`, all code is organized in shallow sub-packages. Each sub-package is located in a directory within the `datalad_next` package.
 
 Consequently, there are no top-level source files other than a few exceptions for technical reasons (`__init__.py`, `conftest.py`, `_version.py`).
```

### Comparing `datalad_next-1.4.0/LICENSE` & `datalad_next-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/PKG-INFO` & `datalad_next-1.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad_next
-Version: 1.4.0
+Version: 1.4.1
 Summary: What is next in DataLad
 Home-page: https://github.com/datalad/datalad-next
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -119,14 +119,19 @@
 - A `download` command is provided as a front-end for the new modular URL
   operations framework.
 - A `python-requests` compatible authentication handler (`DataladAuth`) that
   interfaces DataLad's credential system.
 - Boosted throughput of DataLad's `runner` component for command execution.
 - Substantially more comprehensive replacement for DataLad's `constraints` system
   for type conversion and parameter validation.
+- Windows and Mac client support for RIA store access.
+- A `next-status` command that is A LOT faster than `status`, and offers
+  a `mono` recursion mode that shows modifications of nested dataset
+  hierarchies relative to the state of the root dataset.
+  Requires Git v2.31 (or later).
 
 ## Summary of additional features for DataLad extension development
 
 - Framework for uniform command parameter validation. Regardless of the used
   API (Python, CLI, or GUI), command parameters are uniformly validated. This
   facilitates a stricter separation of parameter specification (and validation)
   from the actual implementation of a command. The latter can now focus on a
@@ -158,14 +163,19 @@
   - check that no secrets are left behind by a test
   - provide a temporary configuration that is isolated from a user environment
     and from other tests
   - provide a temporary secret store that is isolated from a user environment
     and from other tests
   - provide a temporary credential manager to perform credential deployment
     and manipulation isolated from a user environment and from other tests
+- An `iter_subproc()` helper that enable communication with subprocesses
+  via input/output iterables.
+- A `shell` context manager that enables interaction with (remote) shells,
+  including support for input/output iterables for each shell-command execution
+  within the context.
 
 ## Patching the DataLad core package.
 
 Some of the features described above rely on a modification of the DataLad core
 package itself, rather than coming in the form of additional commands. Loading
 this extension causes a range of patches to be applied to the `datalad` package
 to enable them. A comprehensive description of the current set of patch is
```

### Comparing `datalad_next-1.4.0/README.md` & `datalad_next-1.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -89,14 +89,19 @@
 - A `download` command is provided as a front-end for the new modular URL
   operations framework.
 - A `python-requests` compatible authentication handler (`DataladAuth`) that
   interfaces DataLad's credential system.
 - Boosted throughput of DataLad's `runner` component for command execution.
 - Substantially more comprehensive replacement for DataLad's `constraints` system
   for type conversion and parameter validation.
+- Windows and Mac client support for RIA store access.
+- A `next-status` command that is A LOT faster than `status`, and offers
+  a `mono` recursion mode that shows modifications of nested dataset
+  hierarchies relative to the state of the root dataset.
+  Requires Git v2.31 (or later).
 
 ## Summary of additional features for DataLad extension development
 
 - Framework for uniform command parameter validation. Regardless of the used
   API (Python, CLI, or GUI), command parameters are uniformly validated. This
   facilitates a stricter separation of parameter specification (and validation)
   from the actual implementation of a command. The latter can now focus on a
@@ -128,14 +133,19 @@
   - check that no secrets are left behind by a test
   - provide a temporary configuration that is isolated from a user environment
     and from other tests
   - provide a temporary secret store that is isolated from a user environment
     and from other tests
   - provide a temporary credential manager to perform credential deployment
     and manipulation isolated from a user environment and from other tests
+- An `iter_subproc()` helper that enable communication with subprocesses
+  via input/output iterables.
+- A `shell` context manager that enables interaction with (remote) shells,
+  including support for input/output iterables for each shell-command execution
+  within the context.
 
 ## Patching the DataLad core package.
 
 Some of the features described above rely on a modification of the DataLad core
 package itself, rather than coming in the form of additional commands. Loading
 this extension causes a range of patches to be applied to the `datalad` package
 to enable them. A comprehensive description of the current set of patch is
```

### Comparing `datalad_next-1.4.0/_datalad_buildsupport/__init__.py` & `datalad_next-1.4.1/_datalad_buildsupport/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/_datalad_buildsupport/formatters.py` & `datalad_next-1.4.1/_datalad_buildsupport/formatters.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/_datalad_buildsupport/setup.py` & `datalad_next-1.4.1/_datalad_buildsupport/setup.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/__init__.py` & `datalad_next-1.4.1/datalad_next/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/annexbackends/base.py` & `datalad_next-1.4.1/datalad_next/annexbackends/base.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/annexbackends/tests/test_base.py` & `datalad_next-1.4.1/datalad_next/annexbackends/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/annexbackends/xdlra.py` & `datalad_next-1.4.1/datalad_next/annexbackends/xdlra.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/annexremotes/__init__.py` & `datalad_next-1.4.1/datalad_next/annexremotes/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/annexremotes/archivist.py` & `datalad_next-1.4.1/datalad_next/annexremotes/archivist.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/annexremotes/tests/test_archivist.py` & `datalad_next-1.4.1/datalad_next/annexremotes/tests/test_archivist.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/annexremotes/tests/test_uncurl.py` & `datalad_next-1.4.1/datalad_next/annexremotes/tests/test_uncurl.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/annexremotes/uncurl.py` & `datalad_next-1.4.1/datalad_next/annexremotes/uncurl.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/archive_operations/__init__.py` & `datalad_next-1.4.1/datalad_next/archive_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/archive_operations/base.py` & `datalad_next-1.4.1/datalad_next/archive_operations/base.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/archive_operations/tarfile.py` & `datalad_next-1.4.1/datalad_next/archive_operations/tarfile.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/archive_operations/tests/test_tarfile.py` & `datalad_next-1.4.1/datalad_next/archive_operations/tests/test_tarfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,72 +12,72 @@
 from datalad_next.iter_collections import FileSystemItemType
 from datalad_next.tests.marker import skipif_no_network
 
 from ..tarfile import TarArchiveOperations
 
 
 @dataclass
-class TestArchive:
+class _TestArchive:
     path: Path
     item_count: int
     content: bytes
     target_hash: dict[str, str]
 
 
 @pytest.fixture(scope='session')
 def structured_sample_tar_xz(
     sample_tar_xz
-) -> Generator[TestArchive, None, None]:
-    yield TestArchive(
+) -> Generator[_TestArchive, None, None]:
+    yield _TestArchive(
         path=sample_tar_xz,
         item_count=6,
         content=b'123\n',
         target_hash={
             'SHA1': 'b5dfcec4d1b6166067226fae102f7fbcf6bd1bd4',
             'md5': 'd700214df5487801e8ee23d31e60382a',
         }
     )
 
 
 @skipif_no_network
-def test_tararchive_basics(structured_sample_tar_xz: TestArchive):
+def test_tararchive_basics(structured_sample_tar_xz: _TestArchive):
     spec = structured_sample_tar_xz
     # this is intentionally a hard-coded POSIX relpath
     member_name = 'test-archive/onetwothree.txt'
     with TarArchiveOperations(spec.path) as archive_ops:
         with archive_ops.open(member_name) as member:
             assert member.read() == spec.content
         with archive_ops.open(PurePosixPath(member_name)) as member:
             assert member.read() == spec.content
 
 
 @skipif_no_network
-def test_tararchive_contain(structured_sample_tar_xz: TestArchive):
+def test_tararchive_contain(structured_sample_tar_xz: _TestArchive):
     # this is intentionally a hard-coded POSIX relpath
     member_name = 'test-archive/onetwothree.txt'
     archive_ops = TarArchiveOperations(structured_sample_tar_xz.path)
     # POSIX path str
     assert member_name in archive_ops
     # POSIX path as obj
     assert PurePosixPath(member_name) in archive_ops
     assert 'bogus' not in archive_ops
 
 
 @skipif_no_network
-def test_tararchive_iterator(structured_sample_tar_xz: TestArchive):
+def test_tararchive_iterator(structured_sample_tar_xz: _TestArchive):
     spec = structured_sample_tar_xz
     with TarArchiveOperations(spec.path) as archive_ops:
         items = list(archive_ops)
         assert len(items) == spec.item_count
         for item in items:
             assert item.name in archive_ops
 
 
 @skipif_no_network
-def test_open(structured_sample_tar_xz: TestArchive):
+def test_open(structured_sample_tar_xz: _TestArchive):
     spec = structured_sample_tar_xz
     file_pointer = set()
     with TarArchiveOperations(spec.path) as tf:
         for item in tf:
             if item.type == FileSystemItemType.file:
                 with tf.open(str(PurePosixPath(item.name))) as fp:
                     file_pointer.add(fp)
```

### Comparing `datalad_next-1.4.0/datalad_next/archive_operations/tests/test_zipfile.py` & `datalad_next-1.4.1/datalad_next/archive_operations/tests/test_zipfile.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,88 +11,88 @@
 
 from datalad_next.iter_collections import FileSystemItemType
 
 from ..zipfile import ZipArchiveOperations
 
 
 @dataclass
-class TestArchive:
+class _TestArchive:
     path: Path
     item_count: int
     content: bytes
     target_hash: dict[str, str]
 
 
 @pytest.fixture(scope='session')
-def structured_sample_zip(sample_zip) -> Generator[TestArchive, None, None]:
-    yield TestArchive(
+def structured_sample_zip(sample_zip) -> Generator[_TestArchive, None, None]:
+    yield _TestArchive(
         path=sample_zip,
         item_count=4,
         content=b'zip-123\n',
         target_hash={
             'SHA1': 'b5dfcec4d1b6166067226fae102f7fbcf6bd1bd4',
             'md5': 'd700214df5487801e8ee23d31e60382a',
         }
     )
 
 
-def test_ziparchive_basics(structured_sample_zip: TestArchive):
+def test_ziparchive_basics(structured_sample_zip: _TestArchive):
     spec = structured_sample_zip
     # this is intentionally a hard-coded POSIX relpath
     member_name = 'test-archive/onetwothree.txt'
     with ZipArchiveOperations(spec.path) as archive_ops:
         with archive_ops.open(member_name) as member:
             assert member.read() == spec.content
         with archive_ops.open(PurePosixPath(member_name)) as member:
             assert member.read() == spec.content
 
 
-def test_ziparchive_contain(structured_sample_zip: TestArchive):
+def test_ziparchive_contain(structured_sample_zip: _TestArchive):
     # this is intentionally a hard-coded POSIX relpath
     member_name = 'test-archive/onetwothree.txt'
     with ZipArchiveOperations(structured_sample_zip.path) as archive_ops:
         assert member_name in archive_ops
         assert PurePosixPath(member_name) in archive_ops
         assert 'bogus' not in archive_ops
 
 
-def test_ziparchive_iterator(structured_sample_zip: TestArchive):
+def test_ziparchive_iterator(structured_sample_zip: _TestArchive):
     spec = structured_sample_zip
     with ZipArchiveOperations(spec.path) as archive_ops:
         items = list(archive_ops)
         assert len(items) == spec.item_count
         for item in items:
             assert item.name in archive_ops
 
 
-def test_open(structured_sample_zip: TestArchive):
+def test_open(structured_sample_zip: _TestArchive):
     spec = structured_sample_zip
     file_pointer = set()
     with ZipArchiveOperations(spec.path) as zf:
         for item in zf:
             if item.type != FileSystemItemType.file:
                 continue
             with zf.open(item.name) as fp:
                 file_pointer.add(fp)
                 assert fp.read(len(spec.content)) == spec.content
         for fp in file_pointer:
             assert fp.closed is True
 
 
-def test_open_zipinfo(structured_sample_zip: TestArchive):
+def test_open_zipinfo(structured_sample_zip: _TestArchive):
     spec = structured_sample_zip
     with ZipArchiveOperations(spec.path) as zf:
         # get zipfile-native ZipInfo items
         for item in zf.zipfile.infolist():
             if item.filename.endswith('/'):
                 # crude approach to skippping non-files
                 continue
             with zf.open(item) as fp:
                 assert fp.read(len(spec.content)) == spec.content
 
 
-def test_ziparchive_noncontext(structured_sample_zip: TestArchive):
+def test_ziparchive_noncontext(structured_sample_zip: _TestArchive):
     spec = structured_sample_zip
     zip = ZipArchiveOperations(spec.path)
     assert zip.zipfile.filename == str(spec.path)
     zip.close()
     assert zip._zipfile is None
```

### Comparing `datalad_next-1.4.0/datalad_next/archive_operations/zipfile.py` & `datalad_next-1.4.1/datalad_next/archive_operations/zipfile.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/commands/__init__.py` & `datalad_next-1.4.1/datalad_next/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/commands/create_sibling_webdav.py` & `datalad_next-1.4.1/datalad_next/commands/create_sibling_webdav.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/commands/credentials.py` & `datalad_next-1.4.1/datalad_next/commands/credentials.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/commands/download.py` & `datalad_next-1.4.1/datalad_next/commands/download.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/commands/ls_file_collection.py` & `datalad_next-1.4.1/datalad_next/commands/ls_file_collection.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/commands/results.py` & `datalad_next-1.4.1/datalad_next/commands/results.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/commands/status.py` & `datalad_next-1.4.1/datalad_next/commands/status.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/commands/tests/test_create_sibling_webdav.py` & `datalad_next-1.4.1/datalad_next/commands/tests/test_create_sibling_webdav.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/commands/tests/test_credentials.py` & `datalad_next-1.4.1/datalad_next/commands/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/commands/tests/test_download.py` & `datalad_next-1.4.1/datalad_next/commands/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/commands/tests/test_ls_file_collection.py` & `datalad_next-1.4.1/datalad_next/commands/tests/test_ls_file_collection.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/commands/tests/test_results.py` & `datalad_next-1.4.1/datalad_next/commands/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/commands/tests/test_status.py` & `datalad_next-1.4.1/datalad_next/commands/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/commands/tests/test_tree.py` & `datalad_next-1.4.1/datalad_next/commands/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/commands/tree.py` & `datalad_next-1.4.1/datalad_next/commands/tree.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/config/tests/test_utils.py` & `datalad_next-1.4.1/datalad_next/config/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/config/utils.py` & `datalad_next-1.4.1/datalad_next/config/utils.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/conftest.py` & `datalad_next-1.4.1/datalad_next/conftest.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/constraints/__init__.py` & `datalad_next-1.4.1/datalad_next/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/constraints/base.py` & `datalad_next-1.4.1/datalad_next/constraints/base.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/constraints/basic.py` & `datalad_next-1.4.1/datalad_next/constraints/basic.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/constraints/compound.py` & `datalad_next-1.4.1/datalad_next/constraints/compound.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/constraints/dataset.py` & `datalad_next-1.4.1/datalad_next/constraints/dataset.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/constraints/exceptions.py` & `datalad_next-1.4.1/datalad_next/constraints/exceptions.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/constraints/formats.py` & `datalad_next-1.4.1/datalad_next/constraints/formats.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/constraints/git.py` & `datalad_next-1.4.1/datalad_next/constraints/git.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/constraints/parameter.py` & `datalad_next-1.4.1/datalad_next/constraints/parameter.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/constraints/parameter_legacy.py` & `datalad_next-1.4.1/datalad_next/constraints/parameter_legacy.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/constraints/tests/test_base.py` & `datalad_next-1.4.1/datalad_next/constraints/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/constraints/tests/test_basic.py` & `datalad_next-1.4.1/datalad_next/constraints/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/constraints/tests/test_cmdarg_validation.py` & `datalad_next-1.4.1/datalad_next/constraints/tests/test_cmdarg_validation.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/constraints/tests/test_compound.py` & `datalad_next-1.4.1/datalad_next/constraints/tests/test_compound.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/constraints/tests/test_exceptions.py` & `datalad_next-1.4.1/datalad_next/constraints/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/constraints/tests/test_special_purpose.py` & `datalad_next-1.4.1/datalad_next/constraints/tests/test_special_purpose.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/constraints/tests/test_tutorial.py` & `datalad_next-1.4.1/datalad_next/constraints/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/constraints/utils.py` & `datalad_next-1.4.1/datalad_next/constraints/utils.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/consts/__init__.py` & `datalad_next-1.4.1/datalad_next/consts/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/credman/manager.py` & `datalad_next-1.4.1/datalad_next/credman/manager.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/credman/tests/test_credman.py` & `datalad_next-1.4.1/datalad_next/credman/tests/test_credman.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/datasets/__init__.py` & `datalad_next-1.4.1/datalad_next/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/datasets/annexrepo.py` & `datalad_next-1.4.1/datalad_next/datasets/annexrepo.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/exceptions/__init__.py` & `datalad_next-1.4.1/datalad_next/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/gitremotes/datalad_annex.py` & `datalad_next-1.4.1/datalad_next/gitremotes/datalad_annex.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/gitremotes/tests/test_datalad_annex.py` & `datalad_next-1.4.1/datalad_next/gitremotes/tests/test_datalad_annex.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/__init__.py` & `datalad_next-1.4.1/datalad_next/iter_collections/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/annexworktree.py` & `datalad_next-1.4.1/datalad_next/iter_collections/annexworktree.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/directory.py` & `datalad_next-1.4.1/datalad_next/iter_collections/directory.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/gitdiff.py` & `datalad_next-1.4.1/datalad_next/iter_collections/gitdiff.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         call_git([
             'update-index',
             # must come first, we recurse ourselves
             '--ignore-submodules',
             # we want to continue the refresh when the index need updating
             '-q',
             '--refresh',
-        ])
+        ], cwd=path)
 
     # when do we need to condense subdir reports into a single dir-report
     reported_dirs: set[str] = set()
     _single_dir = (cmd[0] == 'diff-index') and recursive == 'no'
     # diff-tree reports the compared tree when no from is given, we need
     # to skip that output below
     skip_first = (cmd[0] == 'diff-tree') and from_treeish is None
```

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/gitstatus.py` & `datalad_next-1.4.1/datalad_next/iter_collections/gitstatus.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,19 @@
 
     Yields
     ------
     :class:`GitDiffItem`
       The ``name`` and ``prev_name`` attributes of an item are a ``str`` with
       the corresponding (relative) path, as reported by Git
       (in POSIX conventions).
+
+    .. note::
+
+       The implementation requires `git rev-parse --path-format=relative`
+       that was introduced with Git v2.31.
     """
     path = Path(path)
 
     head, corresponding_head = get_worktree_head(path)
     if head is None:
         # no commit at all -> compare to an empty repo.
         head = PRE_INIT_COMMIT_SHA
```

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/gittree.py` & `datalad_next-1.4.1/datalad_next/iter_collections/gittree.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/gitworktree.py` & `datalad_next-1.4.1/datalad_next/iter_collections/gitworktree.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/tarfile.py` & `datalad_next-1.4.1/datalad_next/iter_collections/tarfile.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/tests/test_iterannexworktree.py` & `datalad_next-1.4.1/datalad_next/iter_collections/tests/test_iterannexworktree.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/tests/test_iterdir.py` & `datalad_next-1.4.1/datalad_next/iter_collections/tests/test_iterdir.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itergitdiff.py` & `datalad_next-1.4.1/datalad_next/iter_collections/tests/test_itergitdiff.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itergitstatus.py` & `datalad_next-1.4.1/datalad_next/iter_collections/tests/test_itergitstatus.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itergittree.py` & `datalad_next-1.4.1/datalad_next/iter_collections/tests/test_itergittree.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itergitworktree.py` & `datalad_next-1.4.1/datalad_next/iter_collections/tests/test_itergitworktree.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itertar.py` & `datalad_next-1.4.1/datalad_next/iter_collections/tests/test_itertar.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/tests/test_iterzip.py` & `datalad_next-1.4.1/datalad_next/iter_collections/tests/test_iterzip.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/tests/test_utils.py` & `datalad_next-1.4.1/datalad_next/iter_collections/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/utils.py` & `datalad_next-1.4.1/datalad_next/iter_collections/utils.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iter_collections/zipfile.py` & `datalad_next-1.4.1/datalad_next/iter_collections/zipfile.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iterable_subprocess/.github/workflows/deploy-package-to-pypi.yml` & `datalad_next-1.4.1/datalad_next/iterable_subprocess/.github/workflows/deploy-package-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iterable_subprocess/.github/workflows/test.yml` & `datalad_next-1.4.1/datalad_next/iterable_subprocess/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iterable_subprocess/.gitignore` & `datalad_next-1.4.1/datalad_next/iterable_subprocess/.gitignore`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iterable_subprocess/LICENSE` & `datalad_next-1.4.1/datalad_next/iterable_subprocess/LICENSE`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iterable_subprocess/README.md` & `datalad_next-1.4.1/datalad_next/iterable_subprocess/README.md`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iterable_subprocess/__init__.py` & `datalad_next-1.4.1/datalad_next/iterable_subprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iterable_subprocess/iterable_subprocess.py` & `datalad_next-1.4.1/datalad_next/iterable_subprocess/iterable_subprocess.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iterable_subprocess/pyproject.toml` & `datalad_next-1.4.1/datalad_next/iterable_subprocess/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/iterable_subprocess/test_iterable_subprocess.py` & `datalad_next-1.4.1/datalad_next/iterable_subprocess/test_iterable_subprocess.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/itertools/__init__.py` & `datalad_next-1.4.1/datalad_next/itertools/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/itertools/align_pattern.py` & `datalad_next-1.4.1/datalad_next/itertools/align_pattern.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/itertools/decode_bytes.py` & `datalad_next-1.4.1/datalad_next/itertools/decode_bytes.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/itertools/itemize.py` & `datalad_next-1.4.1/datalad_next/itertools/itemize.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/itertools/load_json.py` & `datalad_next-1.4.1/datalad_next/itertools/load_json.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/itertools/reroute.py` & `datalad_next-1.4.1/datalad_next/itertools/reroute.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/itertools/tests/test_align_pattern.py` & `datalad_next-1.4.1/datalad_next/itertools/tests/test_align_pattern.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/itertools/tests/test_decode_bytes.py` & `datalad_next-1.4.1/datalad_next/itertools/tests/test_decode_bytes.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/itertools/tests/test_itemize.py` & `datalad_next-1.4.1/datalad_next/itertools/tests/test_itemize.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/itertools/tests/test_load_json.py` & `datalad_next-1.4.1/datalad_next/itertools/tests/test_load_json.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/itertools/tests/test_reroute.py` & `datalad_next-1.4.1/datalad_next/itertools/tests/test_reroute.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/__init__.py` & `datalad_next-1.4.1/datalad_next/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/add_method_url2transport_path.py` & `datalad_next-1.4.1/datalad_next/patches/add_method_url2transport_path.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,26 +42,26 @@
         return Path(path_str)
 
 
 def local_io_url2transport_path(
         self,
         url_path: PurePosixPath
 ) -> Path | PurePosixPath:
-    assert url_path.__class__ is PurePosixPath
+    assert isinstance(url_path, PurePosixPath)
     if on_windows:
         return str2windows_path(url_path)
     else:
         return Path(url_path)
 
 
 def http_remote_io_url2transport_path(
         self,
         url_path: PurePosixPath
 ) -> Path | PurePosixPath:
-    assert url_path.__class__ is PurePosixPath
+    assert isinstance(url_path, PurePosixPath)
     return url_path
 
 
 # Add a `url2transport_path`-method to `ora_remote.LocalIO`
 apply_patch(
     'datalad.distributed.ora_remote',
     'LocalIO',
```

### Comparing `datalad_next-1.4.0/datalad_next/patches/annexrepo.py` & `datalad_next-1.4.1/datalad_next/patches/annexrepo.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/cli_configoverrides.py` & `datalad_next-1.4.1/datalad_next/patches/cli_configoverrides.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/commanderror.py` & `datalad_next-1.4.1/datalad_next/patches/commanderror.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/configuration.py` & `datalad_next-1.4.1/datalad_next/patches/configuration.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/create_sibling_ghlike.py` & `datalad_next-1.4.1/datalad_next/patches/create_sibling_ghlike.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/create_sibling_gitlab.py` & `datalad_next-1.4.1/datalad_next/patches/create_sibling_gitlab.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/customremotes_main.py` & `datalad_next-1.4.1/datalad_next/patches/customremotes_main.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/distribution_dataset.py` & `datalad_next-1.4.1/datalad_next/patches/distribution_dataset.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/fix_ria_ora_tests.py` & `datalad_next-1.4.1/datalad_next/patches/fix_ria_ora_tests.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/interface_utils.py` & `datalad_next-1.4.1/datalad_next/patches/interface_utils.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/push_optimize.py` & `datalad_next-1.4.1/datalad_next/patches/push_optimize.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/push_to_export_remote.py` & `datalad_next-1.4.1/datalad_next/patches/push_to_export_remote.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/replace_create_sibling_ria.py` & `datalad_next-1.4.1/datalad_next/patches/replace_create_sibling_ria.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/replace_ora_remote.py` & `datalad_next-1.4.1/datalad_next/patches/replace_ora_remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 
         # SSH "streaming" buffer
         self.buffer_size = DEFAULT_BUFFER_SIZE
 
     # PATCH: add a helper to assert the type of a path.
     @staticmethod
     def _assert_pure_posix_path(path):
-        assert path.__class__ is PurePosixPath
+        assert isinstance(path, PurePosixPath)
 
     # PATCH: add a close function to ensure that all IO-abstraction objects are
     # closed.
     def close(self):
         if self._io:
             self._io.close()
             self._io = None
```

### Comparing `datalad_next-1.4.0/datalad_next/patches/replace_sshremoteio.py` & `datalad_next-1.4.1/datalad_next/patches/replace_sshremoteio.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/ria_utils.py` & `datalad_next-1.4.1/datalad_next/patches/ria_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     io: SSHRemoteIO or LocalIO
     base_path: PurePosixPath
       root path of a store or dataset
     version: str
       target layout version of the store (dataset tree)
     """
     # PATCH: ensure that `base_path` is an instance of `PurePosixPath`.
-    assert base_path.__class__ is PurePosixPath
+    assert isinstance(base_path, PurePosixPath)
 
     # PATCH: convert abstract `ria-layout-version`-path to concrete IO-specific
     # path
     version_file = io.url2transport_path(base_path / 'ria-layout-version')
     if io.exists(version_file):
         existing_version = io.read_file(version_file).split('|')[0].strip()
         if existing_version != version.split('|')[0]:
@@ -133,15 +133,15 @@
     alias: str, optional
       alias for the dataset in the store
     init_obj_tree: bool
       whether or not to create the base directory for an annex objects tree (
       'annex/objects')
     """
     # PATCH: ensure that `base_path` is an instance of `PurePosixPath`.
-    assert base_path.__class__ is PurePosixPath
+    assert isinstance(base_path, PurePosixPath)
 
     # TODO: Note for RF'ing, that this is about setting up a valid target
     #       for the special remote not a replacement for create-sibling-ria.
     #       There's currently no git (bare) repo created.
 
     try:
         # TODO: This is currently store layout version!
```

### Comparing `datalad_next-1.4.0/datalad_next/patches/run.py` & `datalad_next-1.4.1/datalad_next/patches/run.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/siblings.py` & `datalad_next-1.4.1/datalad_next/patches/siblings.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/ssh_exec.py` & `datalad_next-1.4.1/datalad_next/patches/ssh_exec.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/sshconnector.py` & `datalad_next-1.4.1/datalad_next/patches/sshconnector.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/test_keyring.py` & `datalad_next-1.4.1/datalad_next/patches/test_keyring.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/tests/test_add_method_url2transport_path.py` & `datalad_next-1.4.1/datalad_next/patches/tests/test_add_method_url2transport_path.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/tests/test_annex_progress_logging.py` & `datalad_next-1.4.1/datalad_next/patches/tests/test_annex_progress_logging.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/tests/test_cli_configoverrides.py` & `datalad_next-1.4.1/datalad_next/patches/tests/test_cli_configoverrides.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/tests/test_commanderror.py` & `datalad_next-1.4.1/datalad_next/patches/tests/test_commanderror.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/tests/test_configuration.py` & `datalad_next-1.4.1/datalad_next/patches/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/tests/test_create_sibling_ghlike.py` & `datalad_next-1.4.1/datalad_next/patches/tests/test_create_sibling_ghlike.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/tests/test_create_sibling_gitlab.py` & `datalad_next-1.4.1/datalad_next/patches/tests/test_create_sibling_gitlab.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/tests/test_push.py` & `datalad_next-1.4.1/datalad_next/patches/tests/test_push.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/tests/test_push_to_export_remote.py` & `datalad_next-1.4.1/datalad_next/patches/tests/test_push_to_export_remote.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/tests/test_replace_ora_remote.py` & `datalad_next-1.4.1/datalad_next/patches/tests/test_replace_ora_remote.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/tests/test_ria.py` & `datalad_next-1.4.1/datalad_next/patches/tests/test_ria.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/tests/test_run.py` & `datalad_next-1.4.1/datalad_next/patches/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/tests/test_sshremoteio.py` & `datalad_next-1.4.1/datalad_next/patches/tests/test_sshremoteio.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/patches/update.py` & `datalad_next-1.4.1/datalad_next/patches/update.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/repo_utils/annex.py` & `datalad_next-1.4.1/datalad_next/repo_utils/annex.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/repo_utils/tests/test_annex.py` & `datalad_next-1.4.1/datalad_next/repo_utils/tests/test_annex.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/repo_utils/tests/test_head.py` & `datalad_next-1.4.1/datalad_next/repo_utils/tests/test_head.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/repo_utils/worktree.py` & `datalad_next-1.4.1/datalad_next/repo_utils/worktree.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/runners/__init__.py` & `datalad_next-1.4.1/datalad_next/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/runners/git.py` & `datalad_next-1.4.1/datalad_next/runners/git.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/runners/iter_subproc.py` & `datalad_next-1.4.1/datalad_next/runners/iter_subproc.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/runners/protocols.py` & `datalad_next-1.4.1/datalad_next/runners/protocols.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/runners/tests/test_git.py` & `datalad_next-1.4.1/datalad_next/runners/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/runners/tests/test_iter_subproc.py` & `datalad_next-1.4.1/datalad_next/runners/tests/test_iter_subproc.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/shell/__init__.py` & `datalad_next-1.4.1/datalad_next/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/shell/operations/common.py` & `datalad_next-1.4.1/datalad_next/shell/operations/common.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/shell/operations/posix.py` & `datalad_next-1.4.1/datalad_next/shell/operations/posix.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/shell/response_generators.py` & `datalad_next-1.4.1/datalad_next/shell/response_generators.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/shell/shell.py` & `datalad_next-1.4.1/datalad_next/shell/shell.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/shell/tests/test_response_generators.py` & `datalad_next-1.4.1/datalad_next/shell/tests/test_response_generators.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/shell/tests/test_shell.py` & `datalad_next-1.4.1/datalad_next/shell/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/tests/__init__.py` & `datalad_next-1.4.1/datalad_next/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/tests/fixtures.py` & `datalad_next-1.4.1/datalad_next/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/tests/utils.py` & `datalad_next-1.4.1/datalad_next/tests/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from collections import deque
 import logging
 from functools import wraps
 import os
 from os import environ
 from pathlib import Path
+import pytest
 import subprocess
 from typing import Any
 
 from datalad.support.external_versions import external_versions
 # all datalad-core test utils needed for datalad-next
 from datalad.tests.utils_pytest import (
     DEFAULT_BRANCH,
```

### Comparing `datalad_next-1.4.0/datalad_next/types/annexkey.py` & `datalad_next-1.4.1/datalad_next/types/annexkey.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/types/archivist.py` & `datalad_next-1.4.1/datalad_next/types/archivist.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/types/tests/test_annexkey.py` & `datalad_next-1.4.1/datalad_next/types/tests/test_annexkey.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/types/tests/test_archivist.py` & `datalad_next-1.4.1/datalad_next/types/tests/test_archivist.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/url_operations/__init__.py` & `datalad_next-1.4.1/datalad_next/url_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/url_operations/any.py` & `datalad_next-1.4.1/datalad_next/url_operations/any.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/url_operations/base.py` & `datalad_next-1.4.1/datalad_next/url_operations/base.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/url_operations/exceptions.py` & `datalad_next-1.4.1/datalad_next/url_operations/exceptions.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/url_operations/file.py` & `datalad_next-1.4.1/datalad_next/url_operations/file.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/url_operations/http.py` & `datalad_next-1.4.1/datalad_next/url_operations/http.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/url_operations/ssh.py` & `datalad_next-1.4.1/datalad_next/url_operations/ssh.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/url_operations/tests/test_any.py` & `datalad_next-1.4.1/datalad_next/url_operations/tests/test_any.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/url_operations/tests/test_file.py` & `datalad_next-1.4.1/datalad_next/url_operations/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/url_operations/tests/test_http.py` & `datalad_next-1.4.1/datalad_next/url_operations/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/url_operations/tests/test_ssh.py` & `datalad_next-1.4.1/datalad_next/url_operations/tests/test_ssh.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/utils/__init__.py` & `datalad_next-1.4.1/datalad_next/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/utils/deprecate.py` & `datalad_next-1.4.1/datalad_next/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/utils/http_helpers.py` & `datalad_next-1.4.1/datalad_next/utils/http_helpers.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/utils/multihash.py` & `datalad_next-1.4.1/datalad_next/utils/multihash.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/utils/patch.py` & `datalad_next-1.4.1/datalad_next/utils/patch.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/utils/requests_auth.py` & `datalad_next-1.4.1/datalad_next/utils/requests_auth.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/utils/specialremote.py` & `datalad_next-1.4.1/datalad_next/utils/specialremote.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/utils/tests/test_deprecated.py` & `datalad_next-1.4.1/datalad_next/utils/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/utils/tests/test_multihash.py` & `datalad_next-1.4.1/datalad_next/utils/tests/test_multihash.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next/utils/tests/test_parse_www_authenticate.py` & `datalad_next-1.4.1/datalad_next/utils/tests/test_parse_www_authenticate.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/datalad_next.egg-info/PKG-INFO` & `datalad_next-1.4.1/datalad_next.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad-next
-Version: 1.4.0
+Version: 1.4.1
 Summary: What is next in DataLad
 Home-page: https://github.com/datalad/datalad-next
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -119,14 +119,19 @@
 - A `download` command is provided as a front-end for the new modular URL
   operations framework.
 - A `python-requests` compatible authentication handler (`DataladAuth`) that
   interfaces DataLad's credential system.
 - Boosted throughput of DataLad's `runner` component for command execution.
 - Substantially more comprehensive replacement for DataLad's `constraints` system
   for type conversion and parameter validation.
+- Windows and Mac client support for RIA store access.
+- A `next-status` command that is A LOT faster than `status`, and offers
+  a `mono` recursion mode that shows modifications of nested dataset
+  hierarchies relative to the state of the root dataset.
+  Requires Git v2.31 (or later).
 
 ## Summary of additional features for DataLad extension development
 
 - Framework for uniform command parameter validation. Regardless of the used
   API (Python, CLI, or GUI), command parameters are uniformly validated. This
   facilitates a stricter separation of parameter specification (and validation)
   from the actual implementation of a command. The latter can now focus on a
@@ -158,14 +163,19 @@
   - check that no secrets are left behind by a test
   - provide a temporary configuration that is isolated from a user environment
     and from other tests
   - provide a temporary secret store that is isolated from a user environment
     and from other tests
   - provide a temporary credential manager to perform credential deployment
     and manipulation isolated from a user environment and from other tests
+- An `iter_subproc()` helper that enable communication with subprocesses
+  via input/output iterables.
+- A `shell` context manager that enables interaction with (remote) shells,
+  including support for input/output iterables for each shell-command execution
+  within the context.
 
 ## Patching the DataLad core package.
 
 Some of the features described above rely on a modification of the DataLad core
 package itself, rather than coming in the form of additional commands. Loading
 this extension causes a range of patches to be applied to the `datalad` package
 to enable them. A comprehensive description of the current set of patch is
```

### Comparing `datalad_next-1.4.0/datalad_next.egg-info/SOURCES.txt` & `datalad_next-1.4.1/datalad_next.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .all-contributorsrc
 .appveyor.yml
+.changelog.md.j2
 .codeclimate.yml
 .codespell-exclude
 .codespellrc
 .coveragerc
 .gitattributes
 .gitignore
 .noannex
@@ -20,14 +21,15 @@
 readthedocs.yml
 requirements-devel.txt
 setup.cfg
 setup.py
 versioneer.py
 .github/PULL_REQUEST_TEMPLATE.md
 .github/workflows/codespell.yml
+.github/workflows/conventional-commits.yml
 .github/workflows/docbuild.yml
 .github/workflows/mypy.yml
 .github/workflows/update-contributors.yml
 _datalad_buildsupport/__init__.py
 _datalad_buildsupport/formatters.py
 _datalad_buildsupport/setup.py
 changelog.d/README
```

### Comparing `datalad_next-1.4.0/docs/CODEOWNERS` & `datalad_next-1.4.1/docs/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/docs/Makefile` & `datalad_next-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/docs/README.md` & `datalad_next-1.4.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/docs/policy/release-management.md` & `datalad_next-1.4.1/docs/policy/release-management.md`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/docs/source/_static/datalad_logo.png` & `datalad_next-1.4.1/docs/source/_static/datalad_logo.png`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/docs/source/conf.py` & `datalad_next-1.4.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/docs/source/developer_guide/constraints.rst` & `datalad_next-1.4.1/docs/source/developer_guide/constraints.rst`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/docs/source/index.rst` & `datalad_next-1.4.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/docs/source/patches.rst` & `datalad_next-1.4.1/docs/source/patches.rst`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/docs/source/pyutils.rst` & `datalad_next-1.4.1/docs/source/pyutils.rst`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/readthedocs.yml` & `datalad_next-1.4.1/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/setup.cfg` & `datalad_next-1.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/tools/appveyor/setup-sshd` & `datalad_next-1.4.1/tools/appveyor/setup-sshd`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/tools/appveyor/setup-sshd.bat` & `datalad_next-1.4.1/tools/appveyor/setup-sshd.bat`

 * *Files identical despite different names*

### Comparing `datalad_next-1.4.0/versioneer.py` & `datalad_next-1.4.1/versioneer.py`

 * *Files identical despite different names*

