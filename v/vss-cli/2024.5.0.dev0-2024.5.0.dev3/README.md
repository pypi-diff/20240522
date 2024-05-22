# Comparing `tmp/vss-cli-2024.5.0.dev0.tar.gz` & `tmp/vss-cli-2024.5.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vss-cli-2024.5.0.dev0.tar", last modified: Tue May 21 00:53:26 2024, max compression
+gzip compressed data, was "vss-cli-2024.5.0.dev3.tar", last modified: Wed May 22 17:36:39 2024, max compression
```

## Comparing `vss-cli-2024.5.0.dev0.tar` & `vss-cli-2024.5.0.dev3.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 00:53:26.077841 vss-cli-2024.5.0.dev0/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13872 2024-05-21 00:53:26.077841 vss-cli-2024.5.0.dev0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10991 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/README.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1257 2024-05-21 00:53:26.077841 vss-cli-2024.5.0.dev0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3827 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 00:53:26.057841 vss-cli-2024.5.0.dev0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     5569 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/tests/test_vss_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 00:53:26.061841 vss-cli-2024.5.0.dev0/vss_cli/
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19671 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/autocompletion.py
--rw-rw-rw-   0 root         (0) root         (0)     7453 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    64867 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/config.py
--rw-rw-rw-   0 root         (0) root         (0)    15369 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 00:53:26.065841 vss-cli-2024.5.0.dev0/vss_cli/data/
--rw-rw-rw-   0 root         (0) root         (0)     4500 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/data/clib.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4288 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/data/clone.yaml
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/data/config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2892 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/data/image.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2926 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/data/shell.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4198 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/data/template.yaml
--rw-rw-rw-   0 root         (0) root         (0)    25848 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/data_types.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/hcio.py
--rw-rw-rw-   0 root         (0) root         (0)    12512 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 00:53:26.069841 vss-cli-2024.5.0.dev0/vss_cli/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 00:53:21.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15976 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/account.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/completion.py
--rw-rw-rw-   0 root         (0) root         (0)      908 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 00:53:26.073841 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8906 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/callbacks.py
--rw-rw-rw-   0 root         (0) root         (0)     4015 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/contentlib.py
--rw-rw-rw-   0 root         (0) root         (0)     2813 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/domain.py
--rw-rw-rw-   0 root         (0) root         (0)     3133 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/floppy.py
--rw-rw-rw-   0 root         (0) root         (0)     8680 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/helper.py
--rw-rw-rw-   0 root         (0) root         (0)     3287 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/image.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     3046 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/iso.py
--rw-rw-rw-   0 root         (0) root         (0)     3477 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/net.py
--rw-rw-rw-   0 root         (0) root         (0)     1665 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/os.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/rel_args.py
--rw-rw-rw-   0 root         (0) root         (0)     9604 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/rel_opts.py
--rw-rw-rw-   0 root         (0) root         (0)     3790 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/template.py
--rw-rw-rw-   0 root         (0) root         (0)   149779 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/vm.py
--rw-rw-rw-   0 root         (0) root         (0)     1907 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/vmdks.py
--rw-rw-rw-   0 root         (0) root         (0)    10871 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/configure.py
--rw-rw-rw-   0 root         (0) root         (0)     3481 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/key.py
--rw-rw-rw-   0 root         (0) root         (0)     3010 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/message.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     4310 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/ovf.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/plugins.py
--rw-rw-rw-   0 root         (0) root         (0)     1362 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/raw.py
--rw-rw-rw-   0 root         (0) root         (0)      608 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 00:53:26.073841 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5330 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/change.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/export.py
--rw-rw-rw-   0 root         (0) root         (0)     2372 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     2362 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/image.py
--rw-rw-rw-   0 root         (0) root         (0)     2345 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     2860 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/new.py
--rw-rw-rw-   0 root         (0) root         (0)     2366 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/restore.py
--rw-rw-rw-   0 root         (0) root         (0)     3924 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/retirement.py
--rw-rw-rw-   0 root         (0) root         (0)     3307 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/snapshot.py
--rw-rw-rw-   0 root         (0) root         (0)     2246 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/vmdk.py
--rw-rw-rw-   0 root         (0) root         (0)     1614 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/service.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/shell.py
--rw-rw-rw-   0 root         (0) root         (0)     2325 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/status.py
--rw-rw-rw-   0 root         (0) root         (0)     6761 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/stor.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/token.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/upgrade.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/rel_opts.py
--rw-rw-rw-   0 root         (0) root         (0)     2864 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/sstatus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 00:53:26.073841 vss-cli-2024.5.0.dev0/vss_cli/utils/
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    75203 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/utils/emoji.py
--rw-rw-rw-   0 root         (0) root         (0)     2929 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/utils/threading.py
--rw-rw-rw-   0 root         (0) root         (0)     4734 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/vss.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/vssconst.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 00:53:26.065841 vss-cli-2024.5.0.dev0/vss_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13872 2024-05-21 00:53:26.000000 vss-cli-2024.5.0.dev0/vss_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2453 2024-05-21 00:53:26.000000 vss-cli-2024.5.0.dev0/vss_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 00:53:26.000000 vss-cli-2024.5.0.dev0/vss_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-21 00:53:26.000000 vss-cli-2024.5.0.dev0/vss_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 00:53:26.000000 vss-cli-2024.5.0.dev0/vss_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      683 2024-05-21 00:53:26.000000 vss-cli-2024.5.0.dev0/vss_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-21 00:53:26.000000 vss-cli-2024.5.0.dev0/vss_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 17:36:39.114873 vss-cli-2024.5.0.dev3/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13867 2024-05-22 17:36:39.114873 vss-cli-2024.5.0.dev3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10991 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1257 2024-05-22 17:36:39.114873 vss-cli-2024.5.0.dev3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3827 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 17:36:39.082873 vss-cli-2024.5.0.dev3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5569 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/tests/test_vss_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 17:36:39.090873 vss-cli-2024.5.0.dev3/vss_cli/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19671 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/autocompletion.py
+-rw-rw-rw-   0 root         (0) root         (0)     7453 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    64867 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15406 2024-05-22 17:35:59.000000 vss-cli-2024.5.0.dev3/vss_cli/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 17:36:39.098873 vss-cli-2024.5.0.dev3/vss_cli/data/
+-rw-rw-rw-   0 root         (0) root         (0)     4500 2024-05-22 17:35:59.000000 vss-cli-2024.5.0.dev3/vss_cli/data/clib.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4288 2024-05-22 17:35:59.000000 vss-cli-2024.5.0.dev3/vss_cli/data/clone.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/data/config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2892 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/data/image.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2926 2024-05-22 17:35:59.000000 vss-cli-2024.5.0.dev3/vss_cli/data/shell.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2024-05-22 17:35:59.000000 vss-cli-2024.5.0.dev3/vss_cli/data/template.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    25848 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/data_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/hcio.py
+-rw-rw-rw-   0 root         (0) root         (0)    12512 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 17:36:39.102873 vss-cli-2024.5.0.dev3/vss_cli/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 17:36:34.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15976 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/account.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/completion.py
+-rw-rw-rw-   0 root         (0) root         (0)      908 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 17:36:39.106873 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8906 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/callbacks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4015 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/contentlib.py
+-rw-rw-rw-   0 root         (0) root         (0)     2813 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3133 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/floppy.py
+-rw-rw-rw-   0 root         (0) root         (0)     8680 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     3287 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/iso.py
+-rw-rw-rw-   0 root         (0) root         (0)     3477 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/net.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/os.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/rel_args.py
+-rw-rw-rw-   0 root         (0) root         (0)     9604 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/rel_opts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3790 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/template.py
+-rw-rw-rw-   0 root         (0) root         (0)   149779 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/vm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1907 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/vmdks.py
+-rw-rw-rw-   0 root         (0) root         (0)    10871 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/configure.py
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/key.py
+-rw-rw-rw-   0 root         (0) root         (0)     3010 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4310 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/ovf.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)     1362 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/raw.py
+-rw-rw-rw-   0 root         (0) root         (0)      608 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 17:36:39.106873 vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5330 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/change.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/export.py
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2362 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2860 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/new.py
+-rw-rw-rw-   0 root         (0) root         (0)     2366 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/restore.py
+-rw-rw-rw-   0 root         (0) root         (0)     3924 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/retirement.py
+-rw-rw-rw-   0 root         (0) root         (0)     3307 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/snapshot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2246 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/vmdk.py
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)     2325 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/status.py
+-rw-rw-rw-   0 root         (0) root         (0)     6761 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/stor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/token.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/plugins/upgrade.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/rel_opts.py
+-rw-rw-rw-   0 root         (0) root         (0)     2864 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/sstatus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 17:36:39.106873 vss-cli-2024.5.0.dev3/vss_cli/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    75203 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/utils/emoji.py
+-rw-rw-rw-   0 root         (0) root         (0)     2929 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/utils/threading.py
+-rw-rw-rw-   0 root         (0) root         (0)     4734 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/vss.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/vssconst.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev3/vss_cli/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 17:36:39.090873 vss-cli-2024.5.0.dev3/vss_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13867 2024-05-22 17:36:39.000000 vss-cli-2024.5.0.dev3/vss_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2453 2024-05-22 17:36:39.000000 vss-cli-2024.5.0.dev3/vss_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 17:36:39.000000 vss-cli-2024.5.0.dev3/vss_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-22 17:36:39.000000 vss-cli-2024.5.0.dev3/vss_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 17:36:39.000000 vss-cli-2024.5.0.dev3/vss_cli.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      679 2024-05-22 17:36:39.000000 vss-cli-2024.5.0.dev3/vss_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-22 17:36:39.000000 vss-cli-2024.5.0.dev3/vss_cli.egg-info/top_level.txt
```

### Comparing `vss-cli-2024.5.0.dev0/LICENSE` & `vss-cli-2024.5.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/PKG-INFO` & `vss-cli-2024.5.0.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vss-cli
-Version: 2024.5.0.dev0
+Version: 2024.5.0.dev3
 Summary: ITS Private Cloud Command Line Interface
 Home-page: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
-Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2024.5.0-dev0.zip
+Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2024.5.0-dev3.zip
 Author: University of Toronto
 Author-email: vss-apps@eis.utoronto.ca
 Maintainer-email: vss-py@eis.utoronto.ca
 License: MIT
 Project-URL: Bug Reports, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/issues
 Project-URL: Documentation, https://eis.utoronto.ca/~vss/vss-cli/
 Project-URL: Source, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Systems Administration
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyvss==2023.12.0
+Requires-Dist: pyvss==2024.5.0
 Requires-Dist: click==8.1.7
 Requires-Dist: click-log==0.4.0
 Requires-Dist: click-plugins==1.1.1
 Requires-Dist: click-repl==0.2.0
 Requires-Dist: click-threading==0.5.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: jsonpath-ng<2,>=1.5.1
@@ -48,30 +48,30 @@
 Requires-Dist: setuptools==68.2.2
 Provides-Extra: test
 Requires-Dist: flake8==6.0.0; extra == "test"
 Requires-Dist: nose==1.3.7; extra == "test"
 Requires-Dist: coverage==6.5.0; extra == "test"
 Requires-Dist: pytz==2022.6; extra == "test"
 Requires-Dist: wheel==0.38.4; extra == "test"
-Requires-Dist: minio==7.1.17; extra == "test"
+Requires-Dist: minio==7.2.7; extra == "test"
 Provides-Extra: dev
 Requires-Dist: flake8==6.0.0; extra == "dev"
 Requires-Dist: nose==1.3.7; extra == "dev"
 Requires-Dist: coverage==6.5.0; extra == "dev"
 Requires-Dist: pytz==2022.6; extra == "dev"
 Requires-Dist: wheel==0.38.4; extra == "dev"
-Requires-Dist: minio==7.1.17; extra == "dev"
-Requires-Dist: minio==7.1.17; extra == "dev"
+Requires-Dist: minio==7.2.7; extra == "dev"
+Requires-Dist: minio==7.2.7; extra == "dev"
 Requires-Dist: sphinx-rtd-theme==1.3.0; extra == "dev"
 Requires-Dist: Sphinx==7.2.2; extra == "dev"
 Requires-Dist: bump2version==1.0.1; extra == "dev"
 Requires-Dist: sphinxcontrib-jquery==4.1; extra == "dev"
-Requires-Dist: sphinxcontrib-confluencebuilder==2.2.0; extra == "dev"
+Requires-Dist: sphinxcontrib-confluencebuilder==2.5.2; extra == "dev"
 Provides-Extra: stor
-Requires-Dist: minio==7.1.17; extra == "stor"
+Requires-Dist: minio==7.2.7; extra == "stor"
 
 # ITS Private Cloud Command Line Interface ``vss-cli``
 
 [![PyPI][pypi-img]](https://pypi.python.org/pypi/vss-cli)
 [![PyPI version][pyver-img]](https://pypi.python.org/pypi/vss-cli)
```

### Comparing `vss-cli-2024.5.0.dev0/README.md` & `vss-cli-2024.5.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/setup.cfg` & `vss-cli-2024.5.0.dev3/setup.cfg`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/setup.py` & `vss-cli-2024.5.0.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/tests/test_vss_cli.py` & `vss-cli-2024.5.0.dev3/tests/test_vss_cli.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/autocompletion.py` & `vss-cli-2024.5.0.dev3/vss_cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/cli.py` & `vss-cli-2024.5.0.dev3/vss_cli/cli.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/config.py` & `vss-cli-2024.5.0.dev3/vss_cli/config.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/const.py` & `vss-cli-2024.5.0.dev3/vss_cli/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Constants used by VSS CLI (vss-cli)."""
 import os
 
 import pkg_resources
 
 PACKAGE_NAME = "vss_cli"
 
-__version__ = "2024.5.0-dev0"
+__version__ = "2024.5.0-dev3"
 
 
 DEFAULT_TIMEOUT = 30
 DEFAULT_ENDPOINT = "https://cloud-api.eis.utoronto.ca"
 DEFAULT_ENDPOINT_NAME = "cloud-api"
 DEFAULT_S3_SERVER = "https://vskey-stor.eis.utoronto.ca"
 _LEGACY_CONFIG = ("~", ".vss-cli", "config.json")
@@ -470,15 +470,15 @@
 COLUMNS_VM_VBS = [('vbs_enabled',), ('firmware',), ('tpm', 'tpm[*].label')]
 COLUMNS_VM_HW = [
     ("value",),
     ("status",),
     ("upgrade_policy", "upgrade_policy.upgrade_policy"),
 ]
 COLUMNS_VM_CONSOLIDATION = [("require_disk_consolidation",)]
-COLUMNS_VM_CONTROLLERS = [('scsi.count',)]
+COLUMNS_VM_CONTROLLERS = [('scsi.count',), ('usb.count',), ('usb-xhci.count',)]
 COLUMNS_EXTRA_CONFIG = [("options", "[*]")]
 COLUMNS_VSS_OPTIONS = [("options", "[*]")]
 COLUMNS_GROUP = [
     ("name",),
     ("description",),
     ("users_count",),
     ("ldap.last_sync",),
```

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/data/clib.yaml` & `vss-cli-2024.5.0.dev3/vss_cli/data/clib.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from CLib 2024.5.0-dev0             #
+#     VSS-CLI Spec from CLib 2024.5.0-dev3             #
 ####################################################
 built: clib               # Required: Do not remove.
 machine:
   item: ubuntu-22.04      # Required: Source content library id OVF.
   cpu: 1                  # Optional: CPU count (Default: 1).
   memory: 1               # Optional: Memory in GB (Default: 1GB).
   name: &name Vm-Name     # Required: Target virtual machine name.
```

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/data/clone.yaml` & `vss-cli-2024.5.0.dev3/vss_cli/data/clone.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from Clone 2024.5.0-dev0             #
+#     VSS-CLI Spec from Clone 2024.5.0-dev3             #
 ####################################################
 built: clone              # Required: Do not remove.
 machine:
   source: SourceVM        # Required: Can be a vm name or a vm id.
   name: &name Vm-Name     # Required: Target virtual machine name
   disks:                  # Optional: Disks (Default: source vm disk layout)
     - capacity_gb: 40     # Optional: Disk capacity in GB (Default: source vm disk capacity)
```

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/data/config.yaml` & `vss-cli-2024.5.0.dev3/vss_cli/data/config.yaml`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/data/image.yaml` & `vss-cli-2024.5.0.dev3/vss_cli/data/image.yaml`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/data/shell.yaml` & `vss-cli-2024.5.0.dev3/vss_cli/data/shell.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec shell VM 2024.5.0-dev0             #
+#     VSS-CLI Spec shell VM 2024.5.0-dev3             #
 ####################################################
 built: os_install         # Required: Do not remove.
 machine:
   name: Vm-Name            # Required: Target virtual machine name.
   os: ubuntu64Guest              # Required: Guest Operating System name or Id.
   cpu: 1                   # Optional: CPU count (Default: 1).
   memory: 1                # Optional: Memory in GB (Default: 1GB).
```

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/data/template.yaml` & `vss-cli-2024.5.0.dev3/vss_cli/data/template.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from Template 2024.5.0-dev0        #
+#     VSS-CLI Spec from Template 2024.5.0-dev3        #
 ####################################################
 built: template           # Required: Do not remove.
 machine:
   source: NixSource                # Required: Can be a vm name or a vm id.
   name: &name Vm-Name     # Required: Target virtual machine name
   folder: MyFolder       # Optional: Folder name, path or ID (Default: source vm folder)
   disks:                  # Optional: Disks (Default: source vm disk layout)
```

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/data_types.py` & `vss-cli-2024.5.0.dev3/vss_cli/data_types.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/hcio.py` & `vss-cli-2024.5.0.dev3/vss_cli/hcio.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/helper.py` & `vss-cli-2024.5.0.dev3/vss_cli/helper.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/account.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/account.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/completion.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/completion.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/compute.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/callbacks.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/callbacks.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/contentlib.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/contentlib.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/domain.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/domain.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/floppy.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/floppy.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/folder.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/folder.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/helper.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/helper.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/image.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/image.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/inventory.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/inventory.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/iso.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/iso.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/net.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/net.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/os.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/os.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/rel_args.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/rel_args.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/rel_opts.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/rel_opts.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/template.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/template.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/vm.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/vm.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/vmdks.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/compute_plugins/vmdks.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/configure.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/configure.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/key.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/key.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/message.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/message.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/misc.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/misc.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/ovf.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/ovf.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/plugins.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/raw.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/raw.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/request.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/request.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/change.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/change.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/export.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/export.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/folder.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/folder.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/image.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/image.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/inventory.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/inventory.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/new.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/new.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/restore.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/restore.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/retirement.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/retirement.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/snapshot.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/snapshot.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/vmdk.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/request_plugins/vmdk.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/service.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/service.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/shell.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/shell.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/status.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/status.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/stor.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/stor.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/token.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/token.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/plugins/upgrade.py` & `vss-cli-2024.5.0.dev3/vss_cli/plugins/upgrade.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/rel_opts.py` & `vss-cli-2024.5.0.dev3/vss_cli/rel_opts.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/sstatus.py` & `vss-cli-2024.5.0.dev3/vss_cli/sstatus.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/utils/emoji.py` & `vss-cli-2024.5.0.dev3/vss_cli/utils/emoji.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/utils/threading.py` & `vss-cli-2024.5.0.dev3/vss_cli/utils/threading.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/validators.py` & `vss-cli-2024.5.0.dev3/vss_cli/validators.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/vss.py` & `vss-cli-2024.5.0.dev3/vss_cli/vss.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli/yaml.py` & `vss-cli-2024.5.0.dev3/vss_cli/yaml.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli.egg-info/PKG-INFO` & `vss-cli-2024.5.0.dev3/vss_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vss-cli
-Version: 2024.5.0.dev0
+Version: 2024.5.0.dev3
 Summary: ITS Private Cloud Command Line Interface
 Home-page: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
-Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2024.5.0-dev0.zip
+Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2024.5.0-dev3.zip
 Author: University of Toronto
 Author-email: vss-apps@eis.utoronto.ca
 Maintainer-email: vss-py@eis.utoronto.ca
 License: MIT
 Project-URL: Bug Reports, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/issues
 Project-URL: Documentation, https://eis.utoronto.ca/~vss/vss-cli/
 Project-URL: Source, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Systems Administration
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyvss==2023.12.0
+Requires-Dist: pyvss==2024.5.0
 Requires-Dist: click==8.1.7
 Requires-Dist: click-log==0.4.0
 Requires-Dist: click-plugins==1.1.1
 Requires-Dist: click-repl==0.2.0
 Requires-Dist: click-threading==0.5.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: jsonpath-ng<2,>=1.5.1
@@ -48,30 +48,30 @@
 Requires-Dist: setuptools==68.2.2
 Provides-Extra: test
 Requires-Dist: flake8==6.0.0; extra == "test"
 Requires-Dist: nose==1.3.7; extra == "test"
 Requires-Dist: coverage==6.5.0; extra == "test"
 Requires-Dist: pytz==2022.6; extra == "test"
 Requires-Dist: wheel==0.38.4; extra == "test"
-Requires-Dist: minio==7.1.17; extra == "test"
+Requires-Dist: minio==7.2.7; extra == "test"
 Provides-Extra: dev
 Requires-Dist: flake8==6.0.0; extra == "dev"
 Requires-Dist: nose==1.3.7; extra == "dev"
 Requires-Dist: coverage==6.5.0; extra == "dev"
 Requires-Dist: pytz==2022.6; extra == "dev"
 Requires-Dist: wheel==0.38.4; extra == "dev"
-Requires-Dist: minio==7.1.17; extra == "dev"
-Requires-Dist: minio==7.1.17; extra == "dev"
+Requires-Dist: minio==7.2.7; extra == "dev"
+Requires-Dist: minio==7.2.7; extra == "dev"
 Requires-Dist: sphinx-rtd-theme==1.3.0; extra == "dev"
 Requires-Dist: Sphinx==7.2.2; extra == "dev"
 Requires-Dist: bump2version==1.0.1; extra == "dev"
 Requires-Dist: sphinxcontrib-jquery==4.1; extra == "dev"
-Requires-Dist: sphinxcontrib-confluencebuilder==2.2.0; extra == "dev"
+Requires-Dist: sphinxcontrib-confluencebuilder==2.5.2; extra == "dev"
 Provides-Extra: stor
-Requires-Dist: minio==7.1.17; extra == "stor"
+Requires-Dist: minio==7.2.7; extra == "stor"
 
 # ITS Private Cloud Command Line Interface ``vss-cli``
 
 [![PyPI][pypi-img]](https://pypi.python.org/pypi/vss-cli)
 [![PyPI version][pyver-img]](https://pypi.python.org/pypi/vss-cli)
```

### Comparing `vss-cli-2024.5.0.dev0/vss_cli.egg-info/SOURCES.txt` & `vss-cli-2024.5.0.dev3/vss_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev0/vss_cli.egg-info/requires.txt` & `vss-cli-2024.5.0.dev3/vss_cli.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pyvss==2023.12.0
+pyvss==2024.5.0
 click==8.1.7
 click-log==0.4.0
 click-plugins==1.1.1
 click-repl==0.2.0
 click-threading==0.5.0
 tabulate==0.9.0
 jsonpath-ng<2,>=1.5.1
@@ -21,24 +21,24 @@
 
 [dev]
 flake8==6.0.0
 nose==1.3.7
 coverage==6.5.0
 pytz==2022.6
 wheel==0.38.4
-minio==7.1.17
+minio==7.2.7
 sphinx-rtd-theme==1.3.0
 Sphinx==7.2.2
 bump2version==1.0.1
 sphinxcontrib-jquery==4.1
-sphinxcontrib-confluencebuilder==2.2.0
+sphinxcontrib-confluencebuilder==2.5.2
 
 [stor]
-minio==7.1.17
+minio==7.2.7
 
 [test]
 flake8==6.0.0
 nose==1.3.7
 coverage==6.5.0
 pytz==2022.6
 wheel==0.38.4
-minio==7.1.17
+minio==7.2.7
```

