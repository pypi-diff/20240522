# Comparing `tmp/types-setuptools-69.5.0.20240519.tar.gz` & `tmp/types-setuptools-69.5.0.20240522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-setuptools-69.5.0.20240519.tar", last modified: Sun May 19 02:23:46 2024, max compression
+gzip compressed data, was "types-setuptools-69.5.0.20240522.tar", last modified: Wed May 22 02:22:14 2024, max compression
```

## Comparing `types-setuptools-69.5.0.20240519.tar` & `types-setuptools-69.5.0.20240522.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:46.234910 types-setuptools-69.5.0.20240519/
--rw-r--r--   0 runner    (1001) docker     (127)    18085 2024-05-19 02:23:45.000000 types-setuptools-69.5.0.20240519/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 02:23:45.000000 types-setuptools-69.5.0.20240519/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-19 02:23:46.234910 types-setuptools-69.5.0.20240519/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:46.218909 types-setuptools-69.5.0.20240519/distutils-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-19 02:23:45.000000 types-setuptools-69.5.0.20240519/distutils-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/_modified.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/ccompiler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/cmd.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:46.222910 types-setuptools-69.5.0.20240519/distutils-stubs/command/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/command/bdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/command/upload.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:46.222910 types-setuptools-69.5.0.20240519/distutils-stubs/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:45.000000 types-setuptools-69.5.0.20240519/distutils-stubs/compat/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/filelist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/sysconfig.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/distutils-stubs/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:46.222910 types-setuptools-69.5.0.20240519/pkg_resources-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-19 02:23:45.000000 types-setuptools-69.5.0.20240519/pkg_resources-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)    20037 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/pkg_resources-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:46.222910 types-setuptools-69.5.0.20240519/pkg_resources-stubs/_vendored_packaging/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/pkg_resources-stubs/_vendored_packaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/pkg_resources-stubs/_vendored_packaging/markers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/pkg_resources-stubs/_vendored_packaging/requirements.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/pkg_resources-stubs/_vendored_packaging/specifiers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/pkg_resources-stubs/_vendored_packaging/version.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:46.222910 types-setuptools-69.5.0.20240519/pkg_resources-stubs/extern/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/pkg_resources-stubs/extern/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:45.000000 types-setuptools-69.5.0.20240519/pkg_resources-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 02:23:46.234910 types-setuptools-69.5.0.20240519/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-19 02:23:45.000000 types-setuptools-69.5.0.20240519/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:46.226909 types-setuptools-69.5.0.20240519/setuptools-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-19 02:23:45.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:46.226909 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/_modified.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/ccompiler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/cmd.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:46.230910 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/bdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/upload.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:46.230910 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/filelist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/sysconfig.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/build_meta.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:46.234910 types-setuptools-69.5.0.20240519/setuptools-stubs/command/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/alias.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/bdist_egg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/develop.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/dist_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/easy_install.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/editable_wheel.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/install_egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/rotate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/saveopts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/setopt.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/test.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/upload.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/command/upload_docs.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:46.234910 types-setuptools-69.5.0.20240519/setuptools-stubs/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/compat/py310.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/compat/py311.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/compat/py39.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:46.234910 types-setuptools-69.5.0.20240519/setuptools-stubs/config/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/config/expand.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/config/pyprojecttoml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/config/setupcfg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/depends.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/discovery.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/extension.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:46.234910 types-setuptools-69.5.0.20240519/setuptools-stubs/extern/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/extern/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/glob.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/installer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/launch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/logging.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/modified.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/monkey.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/msvc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/namespaces.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/package_index.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:45.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/sandbox.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/unicode_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/warnings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/wheel.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-19 02:23:25.000000 types-setuptools-69.5.0.20240519/setuptools-stubs/windows_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:46.234910 types-setuptools-69.5.0.20240519/types_setuptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-19 02:23:46.000000 types-setuptools-69.5.0.20240519/types_setuptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-19 02:23:46.000000 types-setuptools-69.5.0.20240519/types_setuptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 02:23:46.000000 types-setuptools-69.5.0.20240519/types_setuptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-19 02:23:46.000000 types-setuptools-69.5.0.20240519/types_setuptools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.776876 types-setuptools-69.5.0.20240522/
+-rw-r--r--   0 runner    (1001) docker     (127)    18241 2024-05-22 02:22:12.000000 types-setuptools-69.5.0.20240522/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 02:22:12.000000 types-setuptools-69.5.0.20240522/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-22 02:22:14.776876 types-setuptools-69.5.0.20240522/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.760876 types-setuptools-69.5.0.20240522/distutils-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-22 02:22:12.000000 types-setuptools-69.5.0.20240522/distutils-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/_modified.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/ccompiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/cmd.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.764876 types-setuptools-69.5.0.20240522/distutils-stubs/command/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/bdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/command/upload.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.764876 types-setuptools-69.5.0.20240522/distutils-stubs/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:12.000000 types-setuptools-69.5.0.20240522/distutils-stubs/compat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/filelist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/sysconfig.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/distutils-stubs/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.764876 types-setuptools-69.5.0.20240522/pkg_resources-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-22 02:22:12.000000 types-setuptools-69.5.0.20240522/pkg_resources-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    20179 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/pkg_resources-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.764876 types-setuptools-69.5.0.20240522/pkg_resources-stubs/_vendored_packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/pkg_resources-stubs/_vendored_packaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/pkg_resources-stubs/_vendored_packaging/markers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/pkg_resources-stubs/_vendored_packaging/requirements.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/pkg_resources-stubs/_vendored_packaging/specifiers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/pkg_resources-stubs/_vendored_packaging/version.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.764876 types-setuptools-69.5.0.20240522/pkg_resources-stubs/extern/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/pkg_resources-stubs/extern/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:12.000000 types-setuptools-69.5.0.20240522/pkg_resources-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 02:22:14.776876 types-setuptools-69.5.0.20240522/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-22 02:22:12.000000 types-setuptools-69.5.0.20240522/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.768876 types-setuptools-69.5.0.20240522/setuptools-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-22 02:22:12.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.768876 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/_modified.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/ccompiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/cmd.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.772876 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/bdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/upload.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.772876 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/filelist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/sysconfig.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/build_meta.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.776876 types-setuptools-69.5.0.20240522/setuptools-stubs/command/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/alias.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/bdist_egg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/develop.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/dist_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/easy_install.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/editable_wheel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/install_egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/rotate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/saveopts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/setopt.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/test.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/command/upload_docs.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.776876 types-setuptools-69.5.0.20240522/setuptools-stubs/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/compat/py310.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/compat/py311.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/compat/py39.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.776876 types-setuptools-69.5.0.20240522/setuptools-stubs/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/config/expand.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/config/pyprojecttoml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/config/setupcfg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/depends.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/discovery.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/extension.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.776876 types-setuptools-69.5.0.20240522/setuptools-stubs/extern/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/extern/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/glob.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/installer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/launch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/logging.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/modified.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/monkey.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/msvc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/namespaces.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/package_index.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:12.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/sandbox.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/unicode_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/warnings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/wheel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-22 02:22:00.000000 types-setuptools-69.5.0.20240522/setuptools-stubs/windows_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:14.776876 types-setuptools-69.5.0.20240522/types_setuptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-22 02:22:14.000000 types-setuptools-69.5.0.20240522/types_setuptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-22 02:22:14.000000 types-setuptools-69.5.0.20240522/types_setuptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:22:14.000000 types-setuptools-69.5.0.20240522/types_setuptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 02:22:14.000000 types-setuptools-69.5.0.20240522/types_setuptools.egg-info/top_level.txt
```

### Comparing `types-setuptools-69.5.0.20240519/CHANGELOG.md` & `types-setuptools-69.5.0.20240522/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 69.5.0.20240522 (2024-05-22)
+
+`distutils` & `setuptools`: Relax path related params (#11948)
+
+Co-authored-by: Jelle Zijlstra <jelle.zijlstra@gmail.com>
+
 ## 69.5.0.20240519 (2024-05-19)
 
 Make `distutils.dist.Distribution.get_command_obj` not return `None` by default (#11950)
 
 `distutils` & `setuptools`: Complete `sub_commands` `ClassVar` typing (#11951)
 
 ## 69.5.0.20240518 (2024-05-18)
```

### Comparing `types-setuptools-69.5.0.20240519/PKG-INFO` & `types-setuptools-69.5.0.20240522/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 69.5.0.20240519
+Version: 69.5.0.20240522
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-setuptools` aims to provide accurate annotations
 for `setuptools==69.5.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `5445a4a243f5e41c9b4ab8b4ffa93da0820218bb` and was tested
+This package was generated from typeshed commit `489e8dbf41d3350388331b2303bd4f3d13ecbfff` and was tested
 with mypy 1.10.0, pyright 1.1.363, and
 pytype 2024.4.11.
```

### Comparing `types-setuptools-69.5.0.20240519/pkg_resources-stubs/__init__.pyi` & `types-setuptools-69.5.0.20240522/pkg_resources-stubs/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import types
 import zipimport
-from _typeshed import Incomplete, StrPath, Unused
+from _typeshed import BytesPath, Incomplete, StrOrBytesPath, StrPath, Unused
 from collections.abc import Callable, Generator, Iterable, Iterator, Sequence
 from io import BytesIO
 from itertools import chain
 from pkgutil import get_importer as get_importer
 from re import Pattern
 from typing import IO, Any, ClassVar, Final, Literal, NoReturn, Protocol, TypeVar, overload, type_check_only
 from typing_extensions import Self, TypeAlias
@@ -179,19 +179,19 @@
 iter_entry_points = working_set.iter_entry_points
 add_activation_listener = working_set.subscribe
 run_script = working_set.run_script
 run_main = run_script
 
 class Environment:
     def __init__(
-        self, search_path: Sequence[str] | None = None, platform: str | None = ..., python: str | None = ...
+        self, search_path: Iterable[str] | None = None, platform: str | None = ..., python: str | None = ...
     ) -> None: ...
     def can_add(self, dist: Distribution) -> bool: ...
     def remove(self, dist: Distribution) -> None: ...
-    def scan(self, search_path: Sequence[str] | None = None) -> None: ...
+    def scan(self, search_path: Iterable[str] | None = None) -> None: ...
     def __getitem__(self, project_name: str) -> list[Distribution]: ...
     def add(self, dist: Distribution) -> None: ...
     @overload
     def best_match(
         self, req: Requirement, working_set: WorkingSet, installer: _StrictInstallerType[_D], replace_conflicting: bool = False
     ) -> _D: ...
     @overload
@@ -280,16 +280,16 @@
     def resource_exists(self, package_or_requirement: _PkgReqType, resource_name: str) -> bool: ...
     def resource_isdir(self, package_or_requirement: _PkgReqType, resource_name: str) -> bool: ...
     def resource_filename(self, package_or_requirement: _PkgReqType, resource_name: str) -> str: ...
     def resource_stream(self, package_or_requirement: _PkgReqType, resource_name: str) -> IO[bytes]: ...
     def resource_string(self, package_or_requirement: _PkgReqType, resource_name: str) -> bytes: ...
     def resource_listdir(self, package_or_requirement: _PkgReqType, resource_name: str) -> list[str]: ...
     def extraction_error(self) -> NoReturn: ...
-    def get_cache_path(self, archive_name: str, names: Iterable[str] = ()) -> str: ...
-    def postprocess(self, tempname: str, filename: str) -> None: ...
+    def get_cache_path(self, archive_name: str, names: Iterable[StrPath] = ()) -> str: ...
+    def postprocess(self, tempname: StrOrBytesPath, filename: str) -> None: ...
     def set_extraction_path(self, path: str) -> None: ...
     def cleanup_resources(self, force: bool = False) -> list[str]: ...
 
 __resource_manager: ResourceManager  # Doesn't exist at runtime
 resource_exists = __resource_manager.resource_exists
 resource_isdir = __resource_manager.resource_isdir
 resource_filename = __resource_manager.resource_filename
@@ -417,15 +417,15 @@
     def parsed_version(self) -> packaging_version.Version: ...
     @property
     def version(self) -> str: ...
     def requires(self, extras: Iterable[str] = ()) -> list[Requirement]: ...
     def activate(self, path: list[str] | None = None, replace: bool = False) -> None: ...
     def egg_name(self) -> str: ...  # type: ignore[override]  # supertype's egg_name is a variable, not a method
     @classmethod
-    def from_filename(cls, filename: str, metadata: _MetadataType = None, *, precedence: int = 3) -> Distribution: ...
+    def from_filename(cls, filename: StrOrBytesPath, metadata: _MetadataType = None, *, precedence: int = 3) -> Distribution: ...
     def as_requirement(self) -> Requirement: ...
     def load_entry_point(self, group: str, name: str) -> _ResolvedEntryPoint: ...
     @overload
     def get_entry_map(self, group: None = None) -> dict[str, dict[str, EntryPoint]]: ...
     @overload
     def get_entry_map(self, group: str) -> dict[str, EntryPoint]: ...
     def get_entry_info(self, group: str, name: str) -> EntryPoint | None: ...
@@ -487,11 +487,14 @@
 def get_build_platform() -> str: ...
 
 get_platform = get_build_platform
 
 def get_supported_platform() -> str: ...
 def compatible_platforms(provided: str | None, required: str | None) -> bool: ...
 def get_default_cache() -> str: ...
-def ensure_directory(path: str) -> None: ...
-def normalize_path(filename: str) -> str: ...
+def ensure_directory(path: StrOrBytesPath) -> None: ...
+@overload
+def normalize_path(filename: StrPath) -> str: ...
+@overload
+def normalize_path(filename: BytesPath) -> bytes: ...
 
 class PkgResourcesDeprecationWarning(Warning): ...
```

### Comparing `types-setuptools-69.5.0.20240519/pkg_resources-stubs/_vendored_packaging/markers.pyi` & `types-setuptools-69.5.0.20240522/pkg_resources-stubs/_vendored_packaging/markers.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/pkg_resources-stubs/_vendored_packaging/specifiers.pyi` & `types-setuptools-69.5.0.20240522/pkg_resources-stubs/_vendored_packaging/specifiers.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/pkg_resources-stubs/_vendored_packaging/version.pyi` & `types-setuptools-69.5.0.20240522/pkg_resources-stubs/_vendored_packaging/version.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/pkg_resources-stubs/extern/__init__.pyi` & `types-setuptools-69.5.0.20240522/pkg_resources-stubs/extern/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setup.py` & `types-setuptools-69.5.0.20240522/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-setuptools` aims to provide accurate annotations
 for `setuptools==69.5.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `5445a4a243f5e41c9b4ab8b4ffa93da0820218bb` and was tested
+This package was generated from typeshed commit `489e8dbf41d3350388331b2303bd4f3d13ecbfff` and was tested
 with mypy 1.10.0, pyright 1.1.363, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="69.5.0.20240519",
+      version="69.5.0.20240522",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md",
```

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/__init__.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/ccompiler.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/ccompiler.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-from collections.abc import Callable
-from typing import Any, ClassVar, Literal
+from _typeshed import BytesPath, StrPath
+from collections.abc import Callable, Iterable
+from typing import Any, ClassVar, Literal, TypeVar, overload
 from typing_extensions import TypeAlias
 
 _Macro: TypeAlias = tuple[str] | tuple[str, str | None]
+_StrPathT = TypeVar("_StrPathT", bound=StrPath)
+_BytesPathT = TypeVar("_BytesPathT", bound=BytesPath)
 
 def gen_lib_options(
     compiler: CCompiler, library_dirs: list[str], runtime_library_dirs: list[str], libraries: list[str]
 ) -> list[str]: ...
 def gen_preprocess_options(macros: list[_Macro], include_dirs: list[str]) -> list[str]: ...
 def get_default_compiler(osname: str | None = ..., platform: str | None = ...) -> str: ...
 def new_compiler(
@@ -150,22 +153,31 @@
         source: str,
         output_file: str | None = ...,
         macros: list[_Macro] | None = ...,
         include_dirs: list[str] | None = ...,
         extra_preargs: list[str] | None = ...,
         extra_postargs: list[str] | None = ...,
     ) -> None: ...
-    def executable_filename(self, basename: str, strip_dir: bool | Literal[0, 1] = 0, output_dir: str = ...) -> str: ...
+    @overload
+    def executable_filename(self, basename: str, strip_dir: Literal[0, False] = 0, output_dir: StrPath = ...) -> str: ...
+    @overload
+    def executable_filename(self, basename: StrPath, strip_dir: Literal[1, True], output_dir: StrPath = ...) -> str: ...
     def library_filename(
-        self, libname: str, lib_type: str = "static", strip_dir: bool | Literal[0, 1] = 0, output_dir: str = ""
+        self, libname: str, lib_type: str = "static", strip_dir: bool | Literal[0, 1] = 0, output_dir: StrPath = ""
     ) -> str: ...
     def object_filenames(
-        self, source_filenames: list[str], strip_dir: bool | Literal[0, 1] = 0, output_dir: str = ...
+        self, source_filenames: Iterable[StrPath], strip_dir: bool | Literal[0, 1] = 0, output_dir: StrPath | None = ...
     ) -> list[str]: ...
-    def shared_object_filename(self, basename: str, strip_dir: bool | Literal[0, 1] = 0, output_dir: str = ...) -> str: ...
+    @overload
+    def shared_object_filename(self, basename: str, strip_dir: Literal[0, False] = 0, output_dir: StrPath = ...) -> str: ...
+    @overload
+    def shared_object_filename(self, basename: StrPath, strip_dir: Literal[1, True], output_dir: StrPath = ...) -> str: ...
     def execute(self, func: Callable[..., object], args: tuple[Any, ...], msg: str | None = ..., level: int = ...) -> None: ...
     def spawn(self, cmd: list[str]) -> None: ...
     def mkpath(self, name: str, mode: int = ...) -> None: ...
-    def move_file(self, src: str, dst: str) -> str: ...
+    @overload
+    def move_file(self, src: StrPath, dst: _StrPathT) -> _StrPathT | str: ...
+    @overload
+    def move_file(self, src: BytesPath, dst: _BytesPathT) -> _BytesPathT | bytes: ...
     def announce(self, msg: str, level: int = ...) -> None: ...
     def warn(self, msg: str) -> None: ...
     def debug_print(self, msg: str) -> None: ...
```

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/bdist.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/bdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/bdist_rpm.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/bdist_rpm.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/build.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/build.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/build_clib.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/build_clib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/build_ext.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/build_py.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/install.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/install_lib.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/install_lib.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -13,11 +13,11 @@
     compile: Incomplete
     optimize: Incomplete
     skip_build: Incomplete
     def initialize_options(self) -> None: ...
     def finalize_options(self) -> None: ...
     def run(self) -> None: ...
     def build(self) -> None: ...
-    def install(self): ...
+    def install(self) -> list[str]: ...
     def byte_compile(self, files) -> None: ...
     def get_outputs(self): ...
     def get_inputs(self): ...
```

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/register.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/register.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/sdist.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/command/upload.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/command/upload.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, StrOrBytesPath
 from collections.abc import Iterable, Iterator
 from typing import AnyStr, ClassVar, TypeVar, overload
 
 from ..config import PyPIRCCommand
 
 _T = TypeVar("_T")
 
@@ -14,15 +14,15 @@
     sign: bool
     identity: Incomplete
     def initialize_options(self) -> None: ...
     repository: Incomplete
     realm: Incomplete
     def finalize_options(self) -> None: ...
     def run(self) -> None: ...
-    def upload_file(self, command: str, pyversion: str, filename: str) -> None: ...
+    def upload_file(self, command: str, pyversion: str, filename: StrOrBytesPath) -> None: ...
 
 @overload
 def make_iterable(values: None) -> list[None]: ...
 @overload
 def make_iterable(values: AnyStr) -> Iterator[AnyStr]: ...
 @overload
 def make_iterable(values: Iterable[_T]) -> Iterator[_T]: ...
```

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/dist.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/dist.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from _typeshed import FileDescriptorOrPath, Incomplete, SupportsWrite
+from _typeshed import Incomplete, StrOrBytesPath, StrPath, SupportsWrite
 from collections.abc import Iterable, Mapping
 from re import Pattern
 from typing import IO, Any, ClassVar, Literal, TypeVar, overload
 from typing_extensions import TypeAlias
 
 from .cmd import Command
 
 command_re: Pattern[str]
 
 _OptionsList: TypeAlias = list[tuple[str, str | None, str, int] | tuple[str, str | None, str]]
 _CommandT = TypeVar("_CommandT", bound=Command)
 
 class DistributionMetadata:
-    def __init__(self, path: FileDescriptorOrPath | None = None) -> None: ...
+    def __init__(self, path: StrOrBytesPath | None = None) -> None: ...
     name: str | None
     version: str | None
     author: str | None
     author_email: str | None
     maintainer: str | None
     maintainer_email: str | None
     url: str | None
@@ -27,15 +27,15 @@
     platforms: str | list[str] | None
     classifiers: str | list[str] | None
     download_url: str | None
     provides: list[str] | None
     requires: list[str] | None
     obsoletes: list[str] | None
     def read_pkg_file(self, file: IO[str]) -> None: ...
-    def write_pkg_info(self, base_dir: str) -> None: ...
+    def write_pkg_info(self, base_dir: StrPath) -> None: ...
     def write_pkg_file(self, file: SupportsWrite[str]) -> None: ...
     def get_name(self) -> str: ...
     def get_version(self) -> str: ...
     def get_fullname(self) -> str: ...
     def get_author(self) -> str: ...
     def get_author_email(self) -> str: ...
     def get_maintainer(self) -> str: ...
```

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/errors.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/extension.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/filelist.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/filelist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/sysconfig.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/sysconfig.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/_distutils/util.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/_distutils/util.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/archive_util.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/archive_util.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/build_meta.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/build_meta.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from _typeshed import StrPath
 from collections.abc import Mapping
 from typing import Any
 
 from . import dist
 
 __all__ = [
     "get_requires_for_build_sdist",
@@ -29,19 +30,19 @@
     def run_setup(self, setup_script: str = "setup.py") -> None: ...
     def get_requires_for_build_wheel(self, config_settings: Mapping[str, Any] | None = None) -> list[str]: ...
     def get_requires_for_build_sdist(self, config_settings: Mapping[str, Any] | None = None) -> list[str]: ...
     def prepare_metadata_for_build_wheel(
         self, metadata_directory: str, config_settings: Mapping[str, Any] | None = None
     ) -> str: ...
     def build_wheel(
-        self, wheel_directory: str, config_settings: Mapping[str, Any] | None = None, metadata_directory: str | None = None
+        self, wheel_directory: StrPath, config_settings: Mapping[str, Any] | None = None, metadata_directory: str | None = None
     ) -> str: ...
-    def build_sdist(self, sdist_directory: str, config_settings: Mapping[str, Any] | None = None) -> str: ...
+    def build_sdist(self, sdist_directory: StrPath, config_settings: Mapping[str, Any] | None = None) -> str: ...
     def build_editable(
-        self, wheel_directory: str, config_settings: Mapping[str, Any] | None = None, metadata_directory: str | None = None
+        self, wheel_directory: StrPath, config_settings: Mapping[str, Any] | None = None, metadata_directory: str | None = None
     ) -> str: ...
     def get_requires_for_build_editable(self, config_settings: Mapping[str, Any] | None = None) -> list[str]: ...
     def prepare_metadata_for_build_editable(
         self, metadata_directory: str, config_settings: Mapping[str, Any] | None = None
     ) -> str: ...
 
 class _BuildMetaLegacyBackend(_BuildMetaBackend):
```

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/command/bdist_egg.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/command/bdist_egg.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/command/build_ext.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/command/build_py.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/command/develop.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/command/develop.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/command/easy_install.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/command/easy_install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/command/editable_wheel.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/command/editable_wheel.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/command/egg_info.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/command/egg_info.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/command/install.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/command/install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/command/sdist.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/command/setopt.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/command/setopt.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/command/test.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/command/test.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/command/upload_docs.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/command/upload_docs.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/config/expand.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/config/expand.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _VCo = TypeVar("_VCo", covariant=True)
 
 class StaticModule:
     def __init__(self, name: str, spec: ModuleSpec) -> None: ...
     def __getattr__(self, attr): ...
 
 def glob_relative(patterns: Iterable[str], root_dir: StrPath | None = None) -> list[str]: ...
-def read_files(filepaths: str | bytes | Iterable[StrPath], root_dir: Incomplete | None = None) -> str: ...
+def read_files(filepaths: StrPath | Iterable[StrPath], root_dir: StrPath | None = None) -> str: ...
 def read_attr(attr_desc: str, package_dir: Mapping[str, str] | None = None, root_dir: StrPath | None = None): ...
 def resolve_class(
     qualified_class_name: str, package_dir: Mapping[str, str] | None = None, root_dir: StrPath | None = None
 ) -> Callable[..., Incomplete]: ...
 def cmdclass(
     values: dict[str, str], package_dir: Mapping[str, str] | None = None, root_dir: StrPath | None = None
 ) -> dict[str, Callable[..., Incomplete]]: ...
```

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/config/pyprojecttoml.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/config/pyprojecttoml.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/config/setupcfg.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/config/setupcfg.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/depends.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/depends.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/discovery.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/discovery.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/dist.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/dist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/errors.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/extension.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/extern/__init__.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/extern/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/msvc.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/msvc.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/package_index.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/package_index.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/setuptools-stubs/sandbox.pyi` & `types-setuptools-69.5.0.20240522/setuptools-stubs/sandbox.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240519/types_setuptools.egg-info/PKG-INFO` & `types-setuptools-69.5.0.20240522/types_setuptools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 69.5.0.20240519
+Version: 69.5.0.20240522
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-setuptools` aims to provide accurate annotations
 for `setuptools==69.5.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `5445a4a243f5e41c9b4ab8b4ffa93da0820218bb` and was tested
+This package was generated from typeshed commit `489e8dbf41d3350388331b2303bd4f3d13ecbfff` and was tested
 with mypy 1.10.0, pyright 1.1.363, and
 pytype 2024.4.11.
```

### Comparing `types-setuptools-69.5.0.20240519/types_setuptools.egg-info/SOURCES.txt` & `types-setuptools-69.5.0.20240522/types_setuptools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

