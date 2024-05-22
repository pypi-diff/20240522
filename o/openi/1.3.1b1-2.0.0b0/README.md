# Comparing `tmp/openi-1.3.1b1.tar.gz` & `tmp/openi-2.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-1.3.1b1.tar", last modified: Mon May 20 06:33:10 2024, max compression
+gzip compressed data, was "openi-2.0.0b0.tar", last modified: Wed May 22 03:01:03 2024, max compression
```

## Comparing `openi-1.3.1b1.tar` & `openi-2.0.0b0.tar`

### file list

```diff
@@ -1,41 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 06:33:10.238489 openi-1.3.1b1/
--rw-rw-rw-   0        0        0     3052 2024-05-20 06:33:10.237490 openi-1.3.1b1/PKG-INFO
--rw-rw-rw-   0        0        0     2368 2023-11-10 01:52:31.000000 openi-1.3.1b1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-20 06:33:10.238489 openi-1.3.1b1/setup.cfg
--rw-rw-rw-   0        0        0     1059 2024-05-20 06:30:34.000000 openi-1.3.1b1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:33:10.187947 openi-1.3.1b1/src/
-drwxrwxrwx   0        0        0        0 2024-05-20 06:33:10.199460 openi-1.3.1b1/src/openi/
--rw-rw-rw-   0        0        0      119 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/__init__.py
--rw-rw-rw-   0        0        0     3109 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/_login.py
--rw-rw-rw-   0        0        0    13681 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/apis.py
--rw-rw-rw-   0        0        0     7871 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:33:10.214489 openi-1.3.1b1/src/openi/dataset/
--rw-rw-rw-   0        0        0       48 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/dataset/__init__.py
--rw-rw-rw-   0        0        0     2763 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/dataset/download.py
--rw-rw-rw-   0        0        0     1902 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/dataset/upload.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:33:10.218488 openi-1.3.1b1/src/openi/model/
--rw-rw-rw-   0        0        0       48 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/model/__init__.py
--rw-rw-rw-   0        0        0     4951 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/model/download.py
--rw-rw-rw-   0        0        0     5329 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/model/upload.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:33:10.227488 openi-1.3.1b1/src/openi/services/
--rw-rw-rw-   0        0        0      182 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/services/__init__.py
--rw-rw-rw-   0        0        0     2262 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/services/dataset_struct.py
--rw-rw-rw-   0        0        0     3552 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/services/file_download.py
--rw-rw-rw-   0        0        0     1416 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/services/file_progress_bar.py
--rw-rw-rw-   0        0        0    10985 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/services/file_upload.py
--rw-rw-rw-   0        0        0     2829 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/services/model_struct.py
--rw-rw-rw-   0        0        0     2602 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/services/repo_struct.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:33:10.232488 openi-1.3.1b1/src/openi/utils/
--rw-rw-rw-   0        0        0       49 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/utils/__init__.py
--rw-rw-rw-   0        0        0     4832 2024-05-20 06:30:28.000000 openi-1.3.1b1/src/openi/utils/constants.py
--rw-rw-rw-   0        0        0     1956 2024-05-20 06:29:16.000000 openi-1.3.1b1/src/openi/utils/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:33:10.236501 openi-1.3.1b1/src/openi.egg-info/
--rw-rw-rw-   0        0        0     3052 2024-05-20 06:33:10.000000 openi-1.3.1b1/src/openi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      827 2024-05-20 06:33:10.000000 openi-1.3.1b1/src/openi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 06:33:10.000000 openi-1.3.1b1/src/openi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-20 06:33:10.000000 openi-1.3.1b1/src/openi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-20 06:33:10.000000 openi-1.3.1b1/src/openi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-20 06:33:10.000000 openi-1.3.1b1/src/openi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-20 06:33:10.234488 openi-1.3.1b1/test/
--rw-rw-rw-   0        0        0     1149 2024-04-29 07:10:45.000000 openi-1.3.1b1/test/test.py
--rw-rw-rw-   0        0        0      124 2024-04-28 08:58:09.000000 openi-1.3.1b1/test/test_openi.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:01:03.710951 openi-2.0.0b0/
+-rw-rw-rw-   0        0        0     2102 2024-05-22 03:01:03.709960 openi-2.0.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1491 2024-05-22 02:56:56.000000 openi-2.0.0b0/README.md
+-rw-rw-rw-   0        0        0       80 2024-05-20 06:59:24.000000 openi-2.0.0b0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 03:01:03.711906 openi-2.0.0b0/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2024-05-22 03:00:51.000000 openi-2.0.0b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:01:03.588225 openi-2.0.0b0/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 03:01:03.678837 openi-2.0.0b0/src/openi/
+-rw-rw-rw-   0        0        0      214 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/__init__.py
+-rw-rw-rw-   0        0        0    10892 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/_dataclass.py
+-rw-rw-rw-   0        0        0     7945 2024-05-22 02:53:31.000000 openi-2.0.0b0/src/openi/_exceptions.py
+-rw-rw-rw-   0        0        0     7070 2024-05-20 09:08:09.000000 openi-2.0.0b0/src/openi/_file.py
+-rw-rw-rw-   0        0        0     4370 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/_login.py
+-rw-rw-rw-   0        0        0     9663 2024-05-22 03:00:39.000000 openi-2.0.0b0/src/openi/_session.py
+-rw-rw-rw-   0        0        0     4120 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/_tqdm.py
+-rw-rw-rw-   0        0        0    36274 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:01:03.691877 openi-2.0.0b0/src/openi/commands/
+-rw-rw-rw-   0        0        0      328 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/commands/__init__.py
+-rw-rw-rw-   0        0        0     6792 2024-05-20 09:40:07.000000 openi-2.0.0b0/src/openi/commands/dataset.py
+-rw-rw-rw-   0        0        0     8386 2024-05-20 09:40:07.000000 openi-2.0.0b0/src/openi/commands/model.py
+-rw-rw-rw-   0        0        0      897 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/commands/openi_cli.py
+-rw-rw-rw-   0        0        0     2512 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/commands/user.py
+-rw-rw-rw-   0        0        0     2111 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/constants.py
+-rw-rw-rw-   0        0        0    10572 2024-05-20 09:44:06.000000 openi-2.0.0b0/src/openi/downloader.py
+-rw-rw-rw-   0        0        0     3780 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/log.py
+-rw-rw-rw-   0        0        0     9514 2024-05-22 02:59:11.000000 openi-2.0.0b0/src/openi/uploader.py
+-rw-rw-rw-   0        0        0     2775 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:01:03.708952 openi-2.0.0b0/src/openi.egg-info/
+-rw-rw-rw-   0        0        0     2102 2024-05-22 03:01:03.000000 openi-2.0.0b0/src/openi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2024-05-22 03:01:03.000000 openi-2.0.0b0/src/openi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 03:01:03.000000 openi-2.0.0b0/src/openi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-22 03:01:03.000000 openi-2.0.0b0/src/openi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2024-05-22 03:01:03.000000 openi-2.0.0b0/src/openi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-22 03:01:03.000000 openi-2.0.0b0/src/openi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 03:01:03.707951 openi-2.0.0b0/test/
+-rw-rw-rw-   0        0        0     1149 2024-04-29 07:10:45.000000 openi-2.0.0b0/test/test.py
+-rw-rw-rw-   0        0        0      124 2024-04-28 08:58:09.000000 openi-2.0.0b0/test/test_openi.py
```

### Comparing `openi-1.3.1b1/setup.py` & `openi-2.0.0b0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="openi",
-    version="1.3.1b1",
+    version="2.0.0.b0",
     description="A package for openi pypi",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi",
     author="chenzh05",
     author_email="chenzh.ds@outlook.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent",
     ],
-    entry_points={"console_scripts": ["openi = openi.cli:main"]},
-    install_requires=["requests", "tqdm"],
-    python_requires=">=3.6",
+    entry_points={
+        "console_scripts": ["openi = openi.commands.openi_cli:main"]
+    },
+    install_requires=["requests", "tqdm", "deprecated"],
+    python_requires=">=3.8",
 )
```

### Comparing `openi-1.3.1b1/src/openi/cli.py` & `openi-2.0.0b0/src/openi/commands/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,260 +1,246 @@
-import argparse
-
-from ._login import login, logout, whoami
-from .dataset import *
-from .model import *
-
-
-# import textwrap
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-        usage=CLI.usage,
-        description=CLI.banner,
-    )
-    parser._action_groups.pop()
-    subparsers = parser.add_subparsers(title="commands", dest="commands")
-    subparsers.required = False
-    # subparsers.choices = Help.openi_choices
-    parse_login(subparsers)
-    parse_logout(subparsers)
-    parse_whoami(subparsers)
-    parse_dataset(subparsers)
-    parse_model(subparsers)
-    args = parser.parse_args()
-    if not hasattr(args, "func"):
-        parser.print_help()
-        exit(1)
-
-    command_args = {}
-    command_args.update(vars(args))
-    del command_args["func"]
-    del command_args["commands"]
-    error = False
-
-    out = args.func(**command_args)
-    if out is not None:
-        print(out, end="")
-    # try:
-    #     out = args.func(**command_args)
-    # except Exception as e:
-    #     print(e)
-    #     out = None
-    #     error = True
-    # except ValueError as e:
-    #     print(e)
-    #     out = None
-    #     error = True
-    # except KeyboardInterrupt:
-    #     print("User cancelled operation")
-    #     out = None
-    # if out is not None:
-    #     print(out, end="")
-
-    # This is so that scripts that pick up on error codes can tell when there was a failure
-    if error:
-        exit(1)
-
-
-def parse_login(subparsers):
-    parse_login = subparsers.add_parser(
-        "login",
-        description=CLI.command_login,
-        usage=CLI.login_usage,
-        help=CLI.command_login,
-    )
-    parse_login.add_argument(
-        "-e",  # '--endpoint',
-        dest="endpoint",
-        default=API.DEFAULT_ENDPOINT,
-        required=False,
-        help=CLI.param_endpoint,
-    )
-    parse_login.add_argument(
-        "-t",  # '--token',
-        dest="token",
-        default=None,
-        required=False,
-        help=CLI.param_token,
-    )
-    parse_login.set_defaults(func=login)
-
-
-def parse_logout(subparsers):
-    parse_logout = subparsers.add_parser(
-        "logout",
-        description=CLI.command_logout,
-        usage="openi logout [-h]",
-        help=CLI.command_logout,
-    )
-    parse_logout.set_defaults(func=logout)
-
-
-def parse_whoami(subparsers):
-    parse_whoami = subparsers.add_parser(
-        "whoami",
-        description=CLI.command_whoami,
-        usage="openi whoami [-h]",
-        help=CLI.command_whoami,
-    )
-    parse_whoami.set_defaults(func=whoami)
-
-
-def parse_dataset(subparsers):
-    parser_dataset = subparsers.add_parser(
-        "dataset",
-        usage=CLI.dataset_usage,
-        help=CLI.command_dataset,
-        aliases=["d"],
-    )
-    parser_dataset._action_groups.pop()
-    subparsers_dataset = parser_dataset.add_subparsers(
-        title="commands", dest="commands"
-    )
-    subparsers_dataset.required = True
-
-    # dataset upload
-    parser_dataset_upload = subparsers_dataset.add_parser(
-        "upload",
-        description=CLI.command_dataset_upload,
-        usage=CLI.dataset_upload_usage,
-        help=CLI.dataset_upload_help,
-        # epilog=CLI.dataset_upload_epilog,
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-    )
-    parser_dataset_upload._action_groups.pop()
-    parser_dataset_upload_args = parser_dataset_upload.add_argument_group(
-        "arguments"
-    )
-    parser_dataset_upload_args.add_argument(
-        "-f", dest="file", required=True, help=CLI.dataset_upload_param_file
-    )
-    parser_dataset_upload_args.add_argument(
-        "-r",
-        dest="repo_id",
-        required=True,
-        help=CLI.dataset_upload_param_repo_id,
-    )
-    # parser_dataset_upload_args.add_argument(
-    #     "-c",
-    #     dest="cluster",
-    #     required=False,
-    #     default="NPU",
-    #     choices=["gpu", "npu"],
-    #     help=CLI.dataset_upload_param_cluster,
-    # )
-    parser_dataset_upload.set_defaults(func=upload_file)
-
-    # dataset download
-    parser_dataset_download = subparsers_dataset.add_parser(
-        "download",
-        description=CLI.command_dataset_download,
-        usage=CLI.dataset_download_usage,
-        help=CLI.dataset_download_help,
-        # epilog = CLI.dataset_download_epilog,
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-    )
-    parser_dataset_download._action_groups.pop()
-    parser_dataset_download_args = parser_dataset_download.add_argument_group(
-        "arguments"
-    )
-    parser_dataset_download_args.add_argument(
-        "-f", dest="file", required=True, help=CLI.dataset_download_param_file
-    )
-    parser_dataset_download_args.add_argument(
-        "-r",
-        dest="repo_id",
-        required=True,
-        help=CLI.dataset_upload_param_repo_id,
-    )
-    parser_dataset_download_args.add_argument(
-        "-c",  # '--cluster',
-        dest="cluster",
-        required=False,
-        default="npu",
-        choices=["gpu", "npu"],
-        help=CLI.dataset_upload_param_cluster,
-    )
-    parser_dataset_download_args.add_argument(
-        "-p",  # '--save_path',
-        dest="save_path",
-        required=False,
-        default=PATH.DATASET_SAVE_PATH,
-        help=CLI.dataset_download_param_save_path,
-    )
-    parser_dataset_download.set_defaults(func=download_file)
-
-
-def parse_model(subparsers):
-    parser_model = subparsers.add_parser(
-        "model", usage=CLI.model_usage, help=CLI.command_model, aliases=["m"]
-    )
-    parser_model._action_groups.pop()
-    subparsers_model = parser_model.add_subparsers(
-        title="commands", dest="commands"
-    )
-    subparsers_model.required = True
-
-    # model upload
-    parser_model_upload = subparsers_model.add_parser(
-        "upload",
-        description=CLI.command_model_upload,
-        usage=CLI.model_upload_usage,
-        help=CLI.model_upload_help,
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-    )
-    parser_model_upload._action_groups.pop()
-    parser_model_upload_args = parser_model_upload.add_argument_group(
-        "arguments"
-    )
-    parser_model_upload_args.add_argument(
-        "-f", dest="folder", required=True, help=CLI.model_upload_param_folder
-    )
-    parser_model_upload_args.add_argument(
-        "-r",
-        dest="repo_id",
-        required=True,
-        help=CLI.model_upload_param_repo_id,
-    )
-    parser_model_upload_args.add_argument(
-        "-m",
-        dest="model_name",
-        required=True,
-        help=CLI.model_upload_param_model_name,
-    )
-    parser_model_upload.set_defaults(func=upload_model)
-
-    # model upload
-    parser_model_download = subparsers_model.add_parser(
-        "download",
-        description=CLI.command_model_download,
-        usage=CLI.model_download_usage,
-        help=CLI.model_download_help,
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-    )
-    parser_model_download._action_groups.pop()
-    parser_model_download_args = parser_model_download.add_argument_group(
-        "arguments"
-    )
-    parser_model_download_args.add_argument(
-        "-r",
-        dest="repo_id",
-        required=True,
-        help=CLI.model_upload_param_repo_id,
-    )
-    parser_model_download_args.add_argument(
-        "-m",
-        dest="model_name",
-        required=True,
-        help=CLI.model_upload_param_model_name,
-    )
-    parser_model_download_args.add_argument(
-        "-p",  # '--save_path',
-        dest="save_path",
-        required=False,
-        default=PATH.MODEL_SAVE_PATH,
-        help=CLI.model_download_param_save_path,
-    )
-    parser_model_download.set_defaults(func=download_model)
+from argparse import (
+    _SubParsersAction, Namespace, SUPPRESS,
+)
+from pathlib import Path
+from typing import Optional
+
+from openi.commands import BaseOpeniCLICommand
+from .._exceptions import LocalPathNotFound
+from ..constants import DEFAULT_SAVE_PATH
+from ..downloader import (
+    download_model, download_model_file,
+)
+from ..log import setup_logger
+from ..uploader import (
+    upload_model, upload_model_file,
+)
+
+logger = setup_logger()
+
+
+class ModelCommands(BaseOpeniCLICommand):
+    @staticmethod
+    def register_subcommand(parser: _SubParsersAction):
+        """
+        model command
+        """
+        parser_model = parser.add_parser(
+            "model",
+            help="{upload,download} 上传/下载启智AI协作平台的模型",
+            description="上传/下载启智AI协作平台的模型",
+            aliases=["m"],
+        )
+        parser_model._action_groups.pop()
+        subparsers_model = parser_model.add_subparsers(
+            title="commands",
+            dest="commands",
+        )
+        subparsers_model.required = True
+
+        # Add subcommand
+        DownloadCommand.register_subcommand(subparsers_model)
+        UploadCommand.register_subcommand(subparsers_model)
+
+
+class BaseModelCommand:
+    def __init__(self, args):
+        self.args = args
+
+
+class DownloadCommand(BaseModelCommand):
+    @staticmethod
+    def register_subcommand(subparsers_model):
+        """
+        download subcommand
+        """
+        download_parser = subparsers_model.add_parser(
+            "download",
+            help="下载模型, openi model download -h 查看更多说明",
+            usage="openi model download REPO_ID MODEL_NAME  [--filename FILENAME] [--save_path PATH] [--force]",
+            description="下载模型或模型文件，需指定仓库路径及模型名称，下载公开模型无需登陆",
+        )
+        download_parser._action_groups.pop()
+
+        """
+        arguments
+        """
+        download_parser_args = download_parser.add_argument_group("arguments")
+        download_parser_args.add_argument(
+            "repo_id",
+            help="所在仓库路径，格式为`拥有者/仓库名`，用户需要拥有此仓库权限",
+        )
+        download_parser_args.add_argument(
+            "model_name",
+            help="网页端模型名称",
+        )
+
+        """
+        optional arguments
+        """
+        download_parser_optional_args = download_parser.add_argument_group(
+            "optional arguments"
+        )
+        download_parser_optional_args.add_argument(
+            "-f",
+            "--filename",
+            dest="filename",
+            metavar="",
+            required=False,
+            help="选填: 指定下载模型中的某个文件，不填写此参数则会下载模型内所有文件",
+        )
+        download_parser_optional_args.add_argument(
+            "-p",
+            "--save_path",
+            dest="save_path",
+            metavar="",
+            default=DEFAULT_SAVE_PATH,
+            required=False,
+            help="选填: 指定本地的保存目录，默认为当前目录；若下载整个模型，则会在当前目录默认创建 `模型名称` 文件夹",
+        )
+        download_parser_optional_args.add_argument(
+            "--force",
+            dest="force",
+            action="store_true",
+            required=False,
+            help="选填: 添加此参数将删除本地的缓存与同名文件，强行重新下载文件",
+        )
+        download_parser_optional_args.add_argument(
+            "-t",
+            "--token",
+            dest="token",
+            required=False,
+            help=SUPPRESS,
+        )
+        download_parser_optional_args.add_argument(
+            "-e",
+            "--endpoint",
+            dest="endpoint",
+            required=False,
+            help=SUPPRESS,
+        )
+        download_parser.set_defaults(func=lambda args: DownloadCommand(args))
+
+    def __init__(self, args: Namespace) -> None:
+        self.repo_id: str = args.repo_id
+        self.model_name: str = args.model_name
+
+        self.filename: Optional[str] = args.filename
+        self.save_path: Optional[str] = args.save_path
+        self.force: bool = args.force
+
+        self.token: Optional[str] = args.token
+        self.endpoint: Optional[str] = args.endpoint
+
+    def run(self):
+        if self.filename is not None:
+            download_model_file(
+                file=self.filename,
+                repo_id=self.repo_id,
+                model_name=self.model_name,
+                save_path=self.save_path,
+                force=self.force,
+                token=self.token,
+                endpoint=self.endpoint,
+            )
+        else:
+            download_model(
+                repo_id=self.repo_id,
+                model_name=self.model_name,
+                save_path=self.save_path,
+                force=self.force,
+                token=self.token,
+                endpoint=self.endpoint,
+            )
+
+
+class UploadCommand(BaseModelCommand):
+    @staticmethod
+    def register_subcommand(subparsers_model):
+        """
+        upload subcommand
+        """
+        upload_parser = subparsers_model.add_parser(
+            "upload",
+            help="上传模型, openi model upload -h 查看更多说明",
+            usage="openi model upload FILE_PATH REPO_ID MODEL_NAME  [--upload_name FILENAME]",
+            description="上传本地模型或模型文件，需指定本地路径、仓库路径及模型名称",
+        )
+        upload_parser._action_groups.pop()
+
+        """
+        arguments
+        """
+        upload_parser_args = upload_parser.add_argument_group("arguments")
+        upload_parser_args.add_argument(
+            "file_path",
+            help="本地路径，可传入`本地文件`或`本地文件夹`路径；上传`文件夹`时将包含所有文件与子目录文件",
+        )
+        upload_parser_args.add_argument(
+            "repo_id",
+            help="所在仓库路径，格式为`拥有者/仓库名`，用户需要拥有此仓库权限",
+        )
+        upload_parser_args.add_argument(
+            "model_name",
+            help="网页端模型名称",
+        )
+
+        """
+        optional arguments
+        """
+        upload_parser_optional_args = upload_parser.add_argument_group(
+            "optional arguments"
+        )
+        upload_parser_optional_args.add_argument(
+            "-n",
+            "--upload_name",
+            dest="upload_name",
+            metavar="",
+            required=False,
+            help="选填: 自定义上传文件名，当上传`文件夹`时，本参数失效",
+        )
+        upload_parser_optional_args.add_argument(
+            "-t",
+            "--token",
+            dest="token",
+            required=False,
+            help=SUPPRESS,
+        )
+        upload_parser_optional_args.add_argument(
+            "-e",
+            "--endpoint",
+            dest="endpoint",
+            required=False,
+            help=SUPPRESS,
+        )
+        upload_parser.set_defaults(func=lambda args: UploadCommand(args))
+
+    def __init__(self, args: Namespace) -> None:
+        self.repo_id: str = args.repo_id
+        self.model_name: str = args.model_name
+        self.file_path: Path = Path(args.file_path).absolute()
+
+        self.upload_name: Optional[str] = args.upload_name
+        self.token: Optional[str] = args.token
+        self.endpoint: Optional[str] = args.endpoint
+
+    def run(self):
+        if not self.file_path.exists():
+            raise LocalPathNotFound(self.file_path)
+
+        if self.file_path.is_dir():
+            upload_model(
+                folder=self.file_path,
+                repo_id=self.repo_id,
+                model_name=self.model_name,
+                token=self.token,
+                endpoint=self.endpoint,
+            )
+        else:
+            upload_model_file(
+                file=self.file_path,
+                repo_id=self.repo_id,
+                model_name=self.model_name,
+                upload_name=self.upload_name,
+                token=self.token,
+                endpoint=self.endpoint,
+            )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openi-1.3.1b1/src/openi/utils/logger.py` & `openi-2.0.0b0/src/openi/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,108 @@
-import logging
-import os
 import json
 import time
 from datetime import datetime
+from typing import Callable, Union
 
-from .constants import *
+from .log import setup_logger
 
+logger = setup_logger()
 
-def setup_logger():
-    LOG_FORMAT = "%(asctime)s [%(levelname)s] %(funcName)s(): %(message)s"  # %(filename)s %(funcName)s():
-    DATE_FORMAT = "%Y/%m/%d %H:%M:%S"
-    LOG_SUFFIX = time.strftime("%Y%m%d")
-    LOG_FILE = os.path.join(PATH.LOG_PATH, f"{LOG_SUFFIX}.log")
-    logging.addLevelName(25, "HTTP")
-    logging.addLevelName(26, "RESPONSE")
 
-    logging.basicConfig(
-        filename=LOG_FILE,
-        level=logging.INFO,
-        format=LOG_FORMAT,
-        datefmt=DATE_FORMAT,
-    )
-    logger = logging.getLogger(__name__)
-
-    def http(self, message, *args, **kws):
-        if self.isEnabledFor(25):
-            self._log(25, message, args, **kws)
-
-    def response(self, message, *args, **kws):
-        if self.isEnabledFor(26):
-            self._log(26, message, args, **kws)
-
-    logging.Logger.http = http
-    logging.Logger.response = response
-
-    return logger
-
-
-def get_time():
-    return datetime.now().strftime("%H:%M:%S")
-
-
-def algnprint(input_dict):
-    max_key_length = max(len(key) for key in input_dict.keys()) + 1
+def caltime(func: Callable) -> Callable:
+    """
+    Decorator to calculate the time of a function.
+
+    Args:
+        func (function): function to be decorated
+
+    Returns:
+        function: wrapper function
+    """
+
+    def wrapper(*args, **kwargs):
+        start_time = time.time()
+        result = func(*args, **kwargs)
+        end_time = time.time()
+        elapsed_time = end_time - start_time
+        print(f"{func.__name__} took {elapsed_time:.4f} seconds to run.")
+        return result
+
+    return wrapper
+
+
+def parse_time(timestamp: Union[str, int]) -> datetime:
+    """
+    Parse timestamp to python datetime
+
+    Args:
+        timestamp (Union[str, int]):
+            unix timestamp data, either in plaintext or integer
+
+    Returns:
+        datetime: python datetime object without timezone information
+    """
+    if isinstance(timestamp, int):
+        return datetime.fromtimestamp(timestamp, tz=datetime.timezone.utc).replace(
+            tzinfo=None
+        )
+    elif isinstance(timestamp, str):
+        return datetime.fromisoformat(timestamp).replace(tzinfo=None)
+    else:
+        raise ValueError("Invalid timestamp format")
+
+
+def jprint(input_dict: dict, indent: int = 4):
+    """Print a dict in json format
+
+    Args:
+        input_dict (dict): dict to print
+        indent (int, optional): indent level. Defaults to 4.
+
+    Example:
+        >>> jprint({"a": 1, "bb": 2, "ccc": 3})
+        {
+            "a": 1,
+            "bb": 2,
+            "ccc": 3
+        }
+    """
+    print(json.dumps(input_dict, indent=4, ensure_ascii=False))
+
+
+def aprint(input_dict: dict, colon=False):
+    """
+    print a dict in aligned format
+
+    :param input_dict: dict to be printed
+    :param colon: aligned colon or not
+    :return: None
+
+    e.g.
+    >>> aprint({"a": 1, "bb": 2, "ccc": 3})
+    a:   1
+    bb:  2
+    ccc: 3
+    """
+    max_key_length = max(len(key) for key in input_dict.keys())
     for key, value in input_dict.items():
-        key += ":"
-        formatted_key = f"{key:{max_key_length}}"
-        print(f"{formatted_key} {value}")
-
-
-def jprint(dict):
-    print(json.dumps(dict, indent=4, ensure_ascii=False))
-
-
-def jlog(dict):
-    return json.dumps(dict, indent=4, ensure_ascii=False)
-
+        if not colon:
+            key += ":"
+            formatted_key = f"{key:{max_key_length + 1}}"
+            print(f"{formatted_key} {value}")
+        else:
+            formatted_key = f"{key:{max_key_length}}"
+            print(f"{formatted_key}: {value}")
 
-def jsave(dict, dir=None):
-    with open(dir, "w+") as f:
-        json.dump(dict, f, indent=4, ensure_ascii=False)
-    print(f"jsave to {dir}")
 
+def convert_bytes(byte):
+    """
+    Convert bytes to human-readable units (bytes, KB, MB, GB, TB).
+    """
+    units = ["bytes", "KB", "MB", "GB", "TB"]
+    index = 0
+
+    while byte >= 1024 and index < len(units) - 1:
+        byte /= 1024.0
+        index += 1
 
-def lprint(list, with_index=True):
-    max_index_width = len(str(len(list) - 1))
-    for index, item in enumerate(list):
-        if with_index:
-            index_str = str(index).rjust(max_index_width)
-            print(f"{index_str} {item}")
-        else:
-            print(item)
+    return f"{byte:.2f} {units[index]}"
```

### Comparing `openi-1.3.1b1/src/openi.egg-info/SOURCES.txt` & `openi-2.0.0b0/src/openi.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 README.md
+pyproject.toml
 setup.py
 src/openi/__init__.py
+src/openi/_dataclass.py
+src/openi/_exceptions.py
+src/openi/_file.py
 src/openi/_login.py
-src/openi/apis.py
-src/openi/cli.py
+src/openi/_session.py
+src/openi/_tqdm.py
+src/openi/api.py
+src/openi/constants.py
+src/openi/downloader.py
+src/openi/log.py
+src/openi/uploader.py
+src/openi/utils.py
 src/openi.egg-info/PKG-INFO
 src/openi.egg-info/SOURCES.txt
 src/openi.egg-info/dependency_links.txt
 src/openi.egg-info/entry_points.txt
 src/openi.egg-info/requires.txt
 src/openi.egg-info/top_level.txt
-src/openi/dataset/__init__.py
-src/openi/dataset/download.py
-src/openi/dataset/upload.py
-src/openi/model/__init__.py
-src/openi/model/download.py
-src/openi/model/upload.py
-src/openi/services/__init__.py
-src/openi/services/dataset_struct.py
-src/openi/services/file_download.py
-src/openi/services/file_progress_bar.py
-src/openi/services/file_upload.py
-src/openi/services/model_struct.py
-src/openi/services/repo_struct.py
-src/openi/utils/__init__.py
-src/openi/utils/constants.py
-src/openi/utils/logger.py
+src/openi/commands/__init__.py
+src/openi/commands/dataset.py
+src/openi/commands/model.py
+src/openi/commands/openi_cli.py
+src/openi/commands/user.py
 test/test.py
 test/test_openi.py
```

### Comparing `openi-1.3.1b1/test/test.py` & `openi-2.0.0b0/test/test.py`

 * *Files identical despite different names*

