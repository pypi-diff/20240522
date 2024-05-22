# Comparing `tmp/mdaviz-0.0.2rc3.tar.gz` & `tmp/mdaviz-0.0.2rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdaviz-0.0.2rc3.tar", last modified: Wed May 22 16:39:12 2024, max compression
+gzip compressed data, was "mdaviz-0.0.2rc4.tar", last modified: Wed May 22 16:41:16 2024, max compression
```

## Comparing `mdaviz-0.0.2rc3.tar` & `mdaviz-0.0.2rc4.tar`

### file list

```diff
@@ -1,275 +1,275 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.595033 mdaviz-0.0.2rc3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.555033 mdaviz-0.0.2rc3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.555033 mdaviz-0.0.2rc3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-22 16:39:12.595033 mdaviz-0.0.2rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.555033 mdaviz-0.0.2rc3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.555033 mdaviz-0.0.2rc3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.559033 mdaviz-0.0.2rc3/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/api/aboutdialog.rst
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/api/app.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/api/chartview.rst
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/api/data_table_model.rst
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/api/data_table_view.rst
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/api/empty_table_model.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/api/licensedialog.rst
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/api/mda_file_viz.rst
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/api/mda_folder.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/api/mda_folder_table_model.rst
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/api/mda_folder_table_view.rst
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/api/opendialog.rst
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/api/select_fields_table_model.rst
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/api/select_fields_table_view.rst
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/api/user_settings.rst
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/docs/source/user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/env.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.563033 mdaviz-0.0.2rc3/mdaviz/
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/aboutdialog.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    26847 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/chartview.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.555033 mdaviz-0.0.2rc3/mdaviz/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.563033 mdaviz-0.0.2rc3/mdaviz/data/test_folder1/
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0001.mda
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0002.mda
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0003.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0006.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0007.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0008.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0009.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0010.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0011.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0012.mda
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.567033 mdaviz-0.0.2rc3/mdaviz/data/test_folder1/no_mda_folder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1/no_mda_folder/non_mda.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.567033 mdaviz-0.0.2rc3/mdaviz/data/test_folder1/test_folder1_2/
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1/test_folder1_2/mda_0023.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1/test_folder1_2/mda_0024.mda
--rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1/test_folder1_2/mda_0025.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1/test_folder1_2/mda_0026.mda
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.567033 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0001.mda
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0002.mda
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0003.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0006.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0007.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0008.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0009.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0010.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0011.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0012.mda
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.567033 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0001.mda
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0002.mda
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0003.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0006.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0007.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0008.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0009.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0010.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0011.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0012.mda
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.571033 mdaviz-0.0.2rc3/mdaviz/data/test_folder2/
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0019.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0020.mda
--rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0021.mda
--rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0022.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0023.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0024.mda
--rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0025.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0026.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0027.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0028.mda
--rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0029.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0030.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0031.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0032.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0033.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0034.mda
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.579033 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0001.mda
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0002.mda
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0003.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0004.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0005.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0006.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0007.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0008.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0009.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0010.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0011.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0012.mda
--rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0013.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0014.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0015.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0016.mda
--rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0017.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0018.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0019.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0020.mda
--rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0021.mda
--rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0022.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0023.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0024.mda
--rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0025.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0026.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0027.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0028.mda
--rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0029.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0030.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0031.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0032.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0033.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0034.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0035.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0036.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0037.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0038.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0039.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0040.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0041.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0042.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0043.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0044.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0045.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0046.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0047.mda
--rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0048.mda
--rw-r--r--   0 runner    (1001) docker     (127)    16452 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0049.mda
--rw-r--r--   0 runner    (1001) docker     (127)    16424 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0050.mda
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.579033 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/
--rw-r--r--   0 runner    (1001) docker     (127)    44984 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/mda_0051.mda
--rw-r--r--   0 runner    (1001) docker     (127)    45012 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/mda_0061.mda
--rw-r--r--   0 runner    (1001) docker     (127)    44984 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/mda_0062.mda
--rw-r--r--   0 runner    (1001) docker     (127)    45012 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/mda_0063.mda
--rw-r--r--   0 runner    (1001) docker     (127)    44988 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/mda_0064.mda
--rw-r--r--   0 runner    (1001) docker     (127)    45016 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/mda_0065.mda
--rw-r--r--   0 runner    (1001) docker     (127)    44988 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/mda_0066.mda
--rw-r--r--   0 runner    (1001) docker     (127)    44960 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/mda_0067.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13128 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/mda_0068.mda
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.583033 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/
--rw-r--r--   0 runner    (1001) docker     (127)    45012 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0052.mda
--rw-r--r--   0 runner    (1001) docker     (127)    44956 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0053.mda
--rw-r--r--   0 runner    (1001) docker     (127)    18900 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0059.mda
--rw-r--r--   0 runner    (1001) docker     (127)    45012 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0060.mda
--rw-r--r--   0 runner    (1001) docker     (127)    37176 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0069.mda
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.583033 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/
--rw-r--r--   0 runner    (1001) docker     (127)    44984 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/mda_0054.mda
--rw-r--r--   0 runner    (1001) docker     (127)    44960 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/mda_0055.mda
--rw-r--r--   0 runner    (1001) docker     (127)    45016 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/mda_0056.mda
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.583033 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/
--rw-r--r--   0 runner    (1001) docker     (127)    45016 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/mda_0057.mda
--rw-r--r--   0 runner    (1001) docker     (127)    45016 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/mda_0058.mda
--rw-r--r--   0 runner    (1001) docker     (127)    33004 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/mda_0070.mda
--rw-r--r--   0 runner    (1001) docker     (127)    37204 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/mda_0071.mda
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.583033 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/
--rw-r--r--   0 runner    (1001) docker     (127)    33004 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/mda_0072.mda
--rw-r--r--   0 runner    (1001) docker     (127)    37208 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/mda_0073.mda
--rw-r--r--   0 runner    (1001) docker     (127)    33008 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/mda_0074.mda
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.583033 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/subfolder6/
--rw-r--r--   0 runner    (1001) docker     (127)    37208 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/subfolder6/mda_0075.mda
--rw-r--r--   0 runner    (1001) docker     (127)    33008 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/subfolder6/mda_0076.mda
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.587033 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/
--rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0001.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0002.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0003.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0004.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0005.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0006.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0007.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0008.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0009.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0010.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0011.mda
--rw-r--r--   0 runner    (1001) docker     (127)    12076 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0012.mda
--rw-r--r--   0 runner    (1001) docker     (127)    12120 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0013.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0014.mda
--rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0015.mda
--rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0016.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0017.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0018.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0019.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0020.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0021.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0022.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0023.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0024.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0025.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0026.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0027.mda
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0028.mda
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/data_table_view.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/empty_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/licensedialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (127)    26132 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/mda_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    15063 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/mda_file_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/mda_file_table_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/mda_file_viz.py
--rw-r--r--   0 runner    (1001) docker     (127)    33824 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/mda_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/mda_folder_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/mda_folder_table_view.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/opendialog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.591033 mdaviz-0.0.2rc3/mdaviz/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/aboutdialog.ui
--rw-r--r--   0 runner    (1001) docker     (127)    30269 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/apply.png
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/back.png
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/delete.png
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/first.png
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/first.png.png
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/first.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/last.png
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/last.svg
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/licensedialog.ui
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/mainwindow.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/mda_file.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/mda_file_table_view.ui
--rw-r--r--   0 runner    (1001) docker     (127)    40456 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/mda_file_viz.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/mda_folder.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/mda_folder_table_view.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/next.png
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/open.png
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/open.svg
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)    15535 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/refresh.png
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/select_fields_table_view.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/set.png
--rw-r--r--   0 runner    (1001) docker     (127)    37332 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/resources/viz.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.591033 mdaviz-0.0.2rc3/mdaviz/synApps_mdalib/
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/synApps_mdalib/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/synApps_mdalib/METADATA
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/synApps_mdalib/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/synApps_mdalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/synApps_mdalib/f_xdrlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    56696 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/synApps_mdalib/mda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.595033 mdaviz-0.0.2rc3/mdaviz/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/tests/test_aboutdialog.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/user_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11794 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/mdaviz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:39:12.595033 mdaviz-0.0.2rc3/mdaviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-22 16:39:12.000000 mdaviz-0.0.2rc3/mdaviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-05-22 16:39:12.000000 mdaviz-0.0.2rc3/mdaviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:39:12.000000 mdaviz-0.0.2rc3/mdaviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 16:39:12.000000 mdaviz-0.0.2rc3/mdaviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 16:39:12.000000 mdaviz-0.0.2rc3/mdaviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 16:39:12.000000 mdaviz-0.0.2rc3/mdaviz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-22 16:39:08.000000 mdaviz-0.0.2rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:39:12.595033 mdaviz-0.0.2rc3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.794065 mdaviz-0.0.2rc4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.750065 mdaviz-0.0.2rc4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.750065 mdaviz-0.0.2rc4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-22 16:41:16.794065 mdaviz-0.0.2rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.750065 mdaviz-0.0.2rc4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.754065 mdaviz-0.0.2rc4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.754065 mdaviz-0.0.2rc4/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/api/aboutdialog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/api/app.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/api/chartview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/api/data_table_model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/api/data_table_view.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/api/empty_table_model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/api/licensedialog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/api/mda_file_viz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/api/mda_folder.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/api/mda_folder_table_model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/api/mda_folder_table_view.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/api/opendialog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/api/select_fields_table_model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/api/select_fields_table_view.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/api/user_settings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/docs/source/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/env.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.758066 mdaviz-0.0.2rc4/mdaviz/
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/aboutdialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26847 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/chartview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.750065 mdaviz-0.0.2rc4/mdaviz/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.762066 mdaviz-0.0.2rc4/mdaviz/data/test_folder1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0001.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0002.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0003.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0006.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0007.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0008.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0009.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0010.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0011.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0012.mda
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.766065 mdaviz-0.0.2rc4/mdaviz/data/test_folder1/no_mda_folder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1/no_mda_folder/non_mda.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.766065 mdaviz-0.0.2rc4/mdaviz/data/test_folder1/test_folder1_2/
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1/test_folder1_2/mda_0023.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1/test_folder1_2/mda_0024.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1/test_folder1_2/mda_0025.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1/test_folder1_2/mda_0026.mda
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.762066 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0001.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0002.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0003.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0006.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0007.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0008.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0009.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0010.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0011.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0012.mda
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.766065 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0001.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0002.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0003.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0006.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0007.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0008.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0009.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0010.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0011.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0012.mda
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.770065 mdaviz-0.0.2rc4/mdaviz/data/test_folder2/
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0019.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0020.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0021.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0022.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0023.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0024.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0025.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0026.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0027.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0028.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0029.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0030.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0031.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0032.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0033.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0034.mda
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.778065 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0001.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0002.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0003.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0004.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0005.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0006.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0007.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0008.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0009.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0010.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0011.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0012.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0013.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0014.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0015.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0016.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0017.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0018.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0019.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0020.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0021.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0022.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0023.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0024.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0025.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0026.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0027.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0028.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0029.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0030.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0031.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0032.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0033.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0034.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0035.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0036.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0037.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0038.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0039.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0040.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0041.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0042.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0043.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0044.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0045.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0046.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0047.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0048.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    16452 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0049.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    16424 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0050.mda
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.778065 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/
+-rw-r--r--   0 runner    (1001) docker     (127)    44984 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/mda_0051.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    45012 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/mda_0061.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    44984 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/mda_0062.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    45012 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/mda_0063.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    44988 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/mda_0064.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    45016 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/mda_0065.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    44988 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/mda_0066.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    44960 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/mda_0067.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13128 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/mda_0068.mda
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.782065 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/
+-rw-r--r--   0 runner    (1001) docker     (127)    45012 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0052.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    44956 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0053.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    18900 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0059.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    45012 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0060.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    37176 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0069.mda
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.782065 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/
+-rw-r--r--   0 runner    (1001) docker     (127)    44984 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/mda_0054.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    44960 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/mda_0055.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    45016 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/mda_0056.mda
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.782065 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/
+-rw-r--r--   0 runner    (1001) docker     (127)    45016 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/mda_0057.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    45016 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/mda_0058.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    33004 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/mda_0070.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    37204 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/mda_0071.mda
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.782065 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/
+-rw-r--r--   0 runner    (1001) docker     (127)    33004 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/mda_0072.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    37208 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/mda_0073.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    33008 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/mda_0074.mda
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.782065 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/subfolder6/
+-rw-r--r--   0 runner    (1001) docker     (127)    37208 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/subfolder6/mda_0075.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    33008 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/subfolder6/mda_0076.mda
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.790065 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0001.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0002.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0003.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0004.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0005.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0006.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0007.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0008.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0009.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0010.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0011.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    12076 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0012.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    12120 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0013.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0014.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0015.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0016.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0017.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0018.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0019.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0020.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0021.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0022.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0023.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0024.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0025.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0026.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0027.mda
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0028.mda
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/data_table_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/empty_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/licensedialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/mainwindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26132 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/mda_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15063 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/mda_file_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/mda_file_table_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/mda_file_viz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33824 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/mda_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/mda_folder_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/mda_folder_table_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/opendialog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.794065 mdaviz-0.0.2rc4/mdaviz/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/aboutdialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    30269 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/apply.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/back.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/delete.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/first.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/first.png.png
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/first.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/last.png
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/last.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/licensedialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/mainwindow.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/mda_file.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/mda_file_table_view.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    40456 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/mda_file_viz.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/mda_folder.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/mda_folder_table_view.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/next.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/open.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15535 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/refresh.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/select_fields_table_view.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/set.png
+-rw-r--r--   0 runner    (1001) docker     (127)    37332 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/resources/viz.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.794065 mdaviz-0.0.2rc4/mdaviz/synApps_mdalib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/synApps_mdalib/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/synApps_mdalib/METADATA
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/synApps_mdalib/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/synApps_mdalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/synApps_mdalib/f_xdrlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56696 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/synApps_mdalib/mda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.794065 mdaviz-0.0.2rc4/mdaviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/tests/test_aboutdialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/user_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11794 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/mdaviz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:41:16.794065 mdaviz-0.0.2rc4/mdaviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-22 16:41:16.000000 mdaviz-0.0.2rc4/mdaviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-05-22 16:41:16.000000 mdaviz-0.0.2rc4/mdaviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:41:16.000000 mdaviz-0.0.2rc4/mdaviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 16:41:16.000000 mdaviz-0.0.2rc4/mdaviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 16:41:16.000000 mdaviz-0.0.2rc4/mdaviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 16:41:16.000000 mdaviz-0.0.2rc4/mdaviz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-22 16:41:12.000000 mdaviz-0.0.2rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:41:16.794065 mdaviz-0.0.2rc4/setup.cfg
```

### Comparing `mdaviz-0.0.2rc3/.github/workflows/code.yml` & `mdaviz-0.0.2rc4/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/.github/workflows/docs.yml` & `mdaviz-0.0.2rc4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/.github/workflows/pypi.yml` & `mdaviz-0.0.2rc4/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/.gitignore` & `mdaviz-0.0.2rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/PKG-INFO` & `mdaviz-0.0.2rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdaviz
-Version: 0.0.2rc3
+Version: 0.0.2rc4
 Summary: Python Qt5 application to visualize MDA data.
 Author-email: Fanny Rodolakis <rodolakis@anl.gov>, Pete Jemian <prjemian@gmail.com>
 Maintainer-email: Fanny Rodolakis <rodolakis@anl.gov>, Pete Jemian <prjemian@gmail.com>
 License: Copyright (c) 2017-2023, UChicago Argonne, LLC
         
         All Rights Reserved
         
@@ -52,15 +52,15 @@
         represents that its use would not infringe privately owned rights.
         
         ****************************************************************************
         
 Project-URL: Homepage, https://github.com/BCDA-APS/mdaviz
 Project-URL: Bug Tracker, https://github.com/BCDA-APS/mdaviz/issues
 Keywords: bluesky,databroker,tiled,catalog
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Freely Distributable
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `mdaviz-0.0.2rc3/README.md` & `mdaviz-0.0.2rc4/README.md`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/docs/Makefile` & `mdaviz-0.0.2rc4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/docs/make.bat` & `mdaviz-0.0.2rc4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/docs/source/conf.py` & `mdaviz-0.0.2rc4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/docs/source/index.rst` & `mdaviz-0.0.2rc4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/docs/source/install.rst` & `mdaviz-0.0.2rc4/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/env.yml` & `mdaviz-0.0.2rc4/env.yml`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/LICENSE` & `mdaviz-0.0.2rc4/mdaviz/LICENSE`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/__init__.py` & `mdaviz-0.0.2rc4/mdaviz/__init__.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/aboutdialog.py` & `mdaviz-0.0.2rc4/mdaviz/aboutdialog.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/app.py` & `mdaviz-0.0.2rc4/mdaviz/app.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/chartview.py` & `mdaviz-0.0.2rc4/mdaviz/chartview.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0001.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0001.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0002.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0002.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0003.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0003.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0006.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0006.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0007.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0007.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0008.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0008.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0009.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0009.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0010.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0010.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0011.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0011.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1/mda_0012.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1/mda_0012.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1/test_folder1_2/mda_0023.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1/test_folder1_2/mda_0023.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1/test_folder1_2/mda_0024.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1/test_folder1_2/mda_0024.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1/test_folder1_2/mda_0025.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1/test_folder1_2/mda_0025.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1/test_folder1_2/mda_0026.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1/test_folder1_2/mda_0026.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0001.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0001.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0002.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0002.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0003.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0003.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0006.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0006.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0007.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0007.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0008.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0008.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0009.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0009.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0010.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0010.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0011.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0011.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy/mda_0012.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy/mda_0012.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0001.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0001.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0002.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0002.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0003.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0003.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0006.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0006.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0007.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0007.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0008.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0008.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0009.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0009.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0010.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0010.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0011.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0011.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder1 copy 2/mda_0012.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder1 copy 2/mda_0012.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0019.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0019.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0020.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0020.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0021.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0021.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0022.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0022.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0023.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0023.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0024.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0024.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0025.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0025.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0026.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0026.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0027.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0027.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0028.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0028.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0029.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0029.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0030.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0030.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0031.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0031.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0032.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0032.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0033.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0033.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder2/mda_0034.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder2/mda_0034.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0001.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0001.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0002.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0002.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0003.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0003.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0004.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0004.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0005.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0005.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0006.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0006.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0007.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0007.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0008.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0008.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0009.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0009.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0010.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0010.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0011.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0011.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0012.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0012.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0013.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0013.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0014.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0014.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0015.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0015.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0016.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0016.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0017.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0017.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0018.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0018.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0019.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0019.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0020.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0020.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0021.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0021.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0022.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0022.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0023.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0023.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0024.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0024.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0025.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0025.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0026.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0026.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0027.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0027.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0028.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0028.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0029.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0029.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0030.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0030.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0031.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0031.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0032.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0032.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0033.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0033.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0034.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0034.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0035.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0035.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0036.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0036.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0037.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0037.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0038.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0038.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0039.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0039.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0040.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0040.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0041.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0041.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0042.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0042.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0043.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0043.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0044.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0044.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0045.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0045.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0046.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0046.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0047.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0047.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0048.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0048.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0049.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0049.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/mda_0050.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/mda_0050.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/mda_0051.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/mda_0051.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/mda_0061.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/mda_0061.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/mda_0062.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/mda_0062.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/mda_0063.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/mda_0063.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/mda_0064.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/mda_0064.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/mda_0065.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/mda_0065.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/mda_0066.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/mda_0066.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/mda_0067.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/mda_0067.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/mda_0068.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/mda_0068.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0052.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0052.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0053.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0053.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0059.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0059.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0060.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0060.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0069.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/mda_0069.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/mda_0054.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/mda_0054.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/mda_0055.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/mda_0055.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/mda_0056.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/mda_0056.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/mda_0057.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/mda_0057.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/mda_0058.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/mda_0058.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/mda_0070.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/mda_0070.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/mda_0071.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/mda_0071.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/mda_0072.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/mda_0072.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/mda_0073.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/mda_0073.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/mda_0074.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/mda_0074.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/subfolder6/mda_0075.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/subfolder6/mda_0075.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/subfolder6/mda_0076.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_folder3/subfolder1/subfolder2/subfolder3/subfolder4/subfolder5/subfolder6/mda_0076.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0001.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0001.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0002.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0002.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0003.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0003.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0004.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0004.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0005.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0005.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0006.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0006.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0007.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0007.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0008.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0008.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0009.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0009.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0010.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0010.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0011.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0011.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0012.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0012.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0013.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0013.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0014.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0014.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0015.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0015.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0016.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0016.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0017.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0017.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0018.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0018.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0019.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0019.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0020.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0020.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0021.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0021.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0022.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0022.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0023.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0023.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0024.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0024.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0025.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0025.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0026.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0026.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0027.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0027.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data/test_no_positioner/ARPES_0028.mda` & `mdaviz-0.0.2rc4/mdaviz/data/test_no_positioner/ARPES_0028.mda`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data_table_model.py` & `mdaviz-0.0.2rc4/mdaviz/data_table_model.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/data_table_view.py` & `mdaviz-0.0.2rc4/mdaviz/data_table_view.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/empty_table_model.py` & `mdaviz-0.0.2rc4/mdaviz/empty_table_model.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/licensedialog.py` & `mdaviz-0.0.2rc4/mdaviz/licensedialog.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/mainwindow.py` & `mdaviz-0.0.2rc4/mdaviz/mainwindow.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/mda_file.py` & `mdaviz-0.0.2rc4/mdaviz/mda_file.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/mda_file_table_model.py` & `mdaviz-0.0.2rc4/mdaviz/mda_file_table_model.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/mda_file_table_view.py` & `mdaviz-0.0.2rc4/mdaviz/mda_file_table_view.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/mda_file_viz.py` & `mdaviz-0.0.2rc4/mdaviz/mda_file_viz.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/mda_folder.py` & `mdaviz-0.0.2rc4/mdaviz/mda_folder.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/mda_folder_table_model.py` & `mdaviz-0.0.2rc4/mdaviz/mda_folder_table_model.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/mda_folder_table_view.py` & `mdaviz-0.0.2rc4/mdaviz/mda_folder_table_view.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/opendialog.py` & `mdaviz-0.0.2rc4/mdaviz/opendialog.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/aboutdialog.ui` & `mdaviz-0.0.2rc4/mdaviz/resources/aboutdialog.ui`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/apply.png` & `mdaviz-0.0.2rc4/mdaviz/resources/apply.png`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/back.png` & `mdaviz-0.0.2rc4/mdaviz/resources/back.png`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/delete.png` & `mdaviz-0.0.2rc4/mdaviz/resources/delete.png`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/first.png` & `mdaviz-0.0.2rc4/mdaviz/resources/first.png`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/first.png.png` & `mdaviz-0.0.2rc4/mdaviz/resources/first.png.png`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/first.svg` & `mdaviz-0.0.2rc4/mdaviz/resources/first.svg`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/last.png` & `mdaviz-0.0.2rc4/mdaviz/resources/last.png`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/last.svg` & `mdaviz-0.0.2rc4/mdaviz/resources/last.svg`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/licensedialog.ui` & `mdaviz-0.0.2rc4/mdaviz/resources/licensedialog.ui`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/mainwindow.ui` & `mdaviz-0.0.2rc4/mdaviz/resources/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/mda_file.ui` & `mdaviz-0.0.2rc4/mdaviz/resources/mda_file.ui`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/mda_file_table_view.ui` & `mdaviz-0.0.2rc4/mdaviz/resources/mda_file_table_view.ui`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/mda_file_viz.ui` & `mdaviz-0.0.2rc4/mdaviz/resources/mda_file_viz.ui`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/mda_folder.ui` & `mdaviz-0.0.2rc4/mdaviz/resources/mda_folder.ui`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/mda_folder_table_view.ui` & `mdaviz-0.0.2rc4/mdaviz/resources/mda_folder_table_view.ui`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/next.png` & `mdaviz-0.0.2rc4/mdaviz/resources/next.png`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/open.png` & `mdaviz-0.0.2rc4/mdaviz/resources/open.png`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/open.svg` & `mdaviz-0.0.2rc4/mdaviz/resources/open.svg`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/plus.png` & `mdaviz-0.0.2rc4/mdaviz/resources/plus.png`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/refresh.png` & `mdaviz-0.0.2rc4/mdaviz/resources/refresh.png`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/select_fields_table_view.ui` & `mdaviz-0.0.2rc4/mdaviz/resources/select_fields_table_view.ui`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/set.png` & `mdaviz-0.0.2rc4/mdaviz/resources/set.png`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/resources/viz.png` & `mdaviz-0.0.2rc4/mdaviz/resources/viz.png`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/synApps_mdalib/LICENSE` & `mdaviz-0.0.2rc4/mdaviz/synApps_mdalib/LICENSE`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/synApps_mdalib/f_xdrlib.py` & `mdaviz-0.0.2rc4/mdaviz/synApps_mdalib/f_xdrlib.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/synApps_mdalib/mda.py` & `mdaviz-0.0.2rc4/mdaviz/synApps_mdalib/mda.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/tests/test_app.py` & `mdaviz-0.0.2rc4/mdaviz/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/user_settings.py` & `mdaviz-0.0.2rc4/mdaviz/user_settings.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz/utils.py` & `mdaviz-0.0.2rc4/mdaviz/utils.py`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/mdaviz.egg-info/PKG-INFO` & `mdaviz-0.0.2rc4/mdaviz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdaviz
-Version: 0.0.2rc3
+Version: 0.0.2rc4
 Summary: Python Qt5 application to visualize MDA data.
 Author-email: Fanny Rodolakis <rodolakis@anl.gov>, Pete Jemian <prjemian@gmail.com>
 Maintainer-email: Fanny Rodolakis <rodolakis@anl.gov>, Pete Jemian <prjemian@gmail.com>
 License: Copyright (c) 2017-2023, UChicago Argonne, LLC
         
         All Rights Reserved
         
@@ -52,15 +52,15 @@
         represents that its use would not infringe privately owned rights.
         
         ****************************************************************************
         
 Project-URL: Homepage, https://github.com/BCDA-APS/mdaviz
 Project-URL: Bug Tracker, https://github.com/BCDA-APS/mdaviz/issues
 Keywords: bluesky,databroker,tiled,catalog
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Freely Distributable
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `mdaviz-0.0.2rc3/mdaviz.egg-info/SOURCES.txt` & `mdaviz-0.0.2rc4/mdaviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mdaviz-0.0.2rc3/pyproject.toml` & `mdaviz-0.0.2rc4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["bluesky", "databroker", "tiled", "catalog"]
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/?highlight=license
 license = {file = "mdaviz/LICENSE"}
 # https://pypi.org/classifiers/
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "License :: Freely Distributable",
     "License :: Public Domain",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
```

