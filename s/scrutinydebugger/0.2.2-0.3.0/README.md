# Comparing `tmp/scrutinydebugger-0.2.2.tar.gz` & `tmp/scrutinydebugger-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrutinydebugger-0.2.2.tar", last modified: Sun May 12 15:58:04 2024, max compression
+gzip compressed data, was "scrutinydebugger-0.3.0.tar", last modified: Wed May 22 03:03:20 2024, max compression
```

## Comparing `scrutinydebugger-0.2.2.tar` & `scrutinydebugger-0.3.0.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.113279 scrutinydebugger-0.2.2/
--rw-rw-r--   0 py        (1000) py        (1000)     1073 2024-03-25 03:09:50.000000 scrutinydebugger-0.2.2/LICENSE
--rw-r--r--   0 py        (1000) py        (1000)      887 2024-05-12 15:58:04.113279 scrutinydebugger-0.2.2/PKG-INFO
--rw-rw-r--   0 py        (1000) py        (1000)      596 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.2/README.md
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.097279 scrutinydebugger-0.2.2/scrutiny/
--rw-rw-r--   0 py        (1000) py        (1000)      188 2024-05-12 15:54:02.000000 scrutinydebugger-0.2.2/scrutiny/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)      453 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/__main__.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.097279 scrutinydebugger-0.2.2/scrutiny/cli/
--rw-rw-r--   0 py        (1000) py        (1000)       39 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.2/scrutiny/cli/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     5089 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.2/scrutiny/cli/cli.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.097279 scrutinydebugger-0.2.2/scrutiny/cli/commands/
--rw-rw-r--   0 py        (1000) py        (1000)     1577 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.2/scrutiny/cli/commands/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     5166 2024-04-15 02:52:23.000000 scrutinydebugger-0.2.2/scrutiny/cli/commands/add_alias.py
--rw-rw-r--   0 py        (1000) py        (1000)     1431 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.2/scrutiny/cli/commands/base_command.py
--rw-rw-r--   0 py        (1000) py        (1000)     2774 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/cli/commands/datalog_info.py
--rw-rw-r--   0 py        (1000) py        (1000)     1481 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.2/scrutiny/cli/commands/delete_datalog.py
--rw-rw-r--   0 py        (1000) py        (1000)     2148 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.2/scrutiny/cli/commands/elf2varmap.py
--rw-rw-r--   0 py        (1000) py        (1000)     1699 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.2/scrutiny/cli/commands/export_datalog.py
--rw-rw-r--   0 py        (1000) py        (1000)     2082 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.2/scrutiny/cli/commands/get_firmware_id.py
--rw-rw-r--   0 py        (1000) py        (1000)     1314 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.2/scrutiny/cli/commands/install_sfd.py
--rw-rw-r--   0 py        (1000) py        (1000)     2024 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/cli/commands/launch_server.py
--rw-rw-r--   0 py        (1000) py        (1000)     5569 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/cli/commands/list_datalog.py
--rw-rw-r--   0 py        (1000) py        (1000)     3746 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/cli/commands/list_sfd.py
--rw-rw-r--   0 py        (1000) py        (1000)     2880 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.2/scrutiny/cli/commands/make_metadata.py
--rw-rw-r--   0 py        (1000) py        (1000)     1641 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.2/scrutiny/cli/commands/make_sfd.py
--rw-rw-r--   0 py        (1000) py        (1000)     3618 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.2/scrutiny/cli/commands/runtest.py
--rw-rw-r--   0 py        (1000) py        (1000)     1970 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.2/scrutiny/cli/commands/tag_firmware_id.py
--rw-rw-r--   0 py        (1000) py        (1000)     1498 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.2/scrutiny/cli/commands/uninstall_sfd.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.101279 scrutinydebugger-0.2.2/scrutiny/core/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.2/scrutiny/core/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     7134 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.2/scrutiny/core/alias.py
--rw-rw-r--   0 py        (1000) py        (1000)     6707 2024-05-08 23:43:40.000000 scrutinydebugger-0.2.2/scrutiny/core/basic_types.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.101279 scrutinydebugger-0.2.2/scrutiny/core/bintools/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.2/scrutiny/core/bintools/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     1924 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/core/bintools/demangler.py
--rw-rw-r--   0 py        (1000) py        (1000)    37593 2024-05-08 23:43:40.000000 scrutinydebugger-0.2.2/scrutiny/core/bintools/elf_dwarf_var_extractor.py
--rw-rw-r--   0 py        (1000) py        (1000)      223 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/core/bintools/elftools_stubs.py
--rw-rw-r--   0 py        (1000) py        (1000)      547 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.2/scrutiny/core/bintools/elftools_stubs.pyi
--rw-rw-r--   0 py        (1000) py        (1000)      755 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/core/bintools/get_var_memrange.py
--rw-rw-r--   0 py        (1000) py        (1000)     5385 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/core/codecs.py
--rw-rw-r--   0 py        (1000) py        (1000)     7670 2024-04-21 14:05:12.000000 scrutinydebugger-0.2.2/scrutiny/core/datalogging.py
--rw-rw-r--   0 py        (1000) py        (1000)    10600 2024-04-21 03:45:36.000000 scrutinydebugger-0.2.2/scrutiny/core/firmware_description.py
--rw-rw-r--   0 py        (1000) py        (1000)      402 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/core/firmware_id.py
--rw-rw-r--   0 py        (1000) py        (1000)     3653 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/core/firmware_parser.py
--rw-rw-r--   0 py        (1000) py        (1000)    14117 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.2/scrutiny/core/memory_content.py
--rw-rw-r--   0 py        (1000) py        (1000)     6939 2024-04-15 02:52:23.000000 scrutinydebugger-0.2.2/scrutiny/core/sfd_storage.py
--rw-rw-r--   0 py        (1000) py        (1000)      787 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/core/typehints.py
--rw-rw-r--   0 py        (1000) py        (1000)     3000 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.2/scrutiny/core/validation.py
--rw-rw-r--   0 py        (1000) py        (1000)    14999 2024-05-08 23:43:40.000000 scrutinydebugger-0.2.2/scrutiny/core/variable.py
--rw-rw-r--   0 py        (1000) py        (1000)    10690 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.2/scrutiny/core/varmap.py
--rw-rw-r--   0 py        (1000) py        (1000)      290 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/exceptions.py
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-27 04:12:19.000000 scrutinydebugger-0.2.2/scrutiny/py.typed
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.101279 scrutinydebugger-0.2.2/scrutiny/sdk/
--rw-rw-r--   0 py        (1000) py        (1000)      350 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.2/scrutiny/sdk/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)    35478 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.2/scrutiny/sdk/_api_parser.py
--rw-rw-r--   0 py        (1000) py        (1000)    73474 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.2/scrutiny/sdk/client.py
--rw-rw-r--   0 py        (1000) py        (1000)    23098 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/sdk/datalogging.py
--rw-rw-r--   0 py        (1000) py        (1000)    13027 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/sdk/definitions.py
--rw-rw-r--   0 py        (1000) py        (1000)     1539 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/sdk/exceptions.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.101279 scrutinydebugger-0.2.2/scrutiny/sdk/listeners/
--rw-rw-r--   0 py        (1000) py        (1000)    11930 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.2/scrutiny/sdk/listeners/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     1365 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.2/scrutiny/sdk/listeners/buffered_reader_listener.py
--rw-rw-r--   0 py        (1000) py        (1000)    10506 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.2/scrutiny/sdk/listeners/csv_file_listener.py
--rw-rw-r--   0 py        (1000) py        (1000)     2127 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.2/scrutiny/sdk/listeners/text_stream_listener.py
--rw-rw-r--   0 py        (1000) py        (1000)     9981 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/sdk/watchable_handle.py
--rw-rw-r--   0 py        (1000) py        (1000)     3707 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/sdk/write_request.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.101279 scrutinydebugger-0.2.2/scrutiny/server/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.2/scrutiny/server/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     8039 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/active_sfd_handler.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.105279 scrutinydebugger-0.2.2/scrutiny/server/api/
--rw-rw-r--   0 py        (1000) py        (1000)    79426 2024-05-12 15:52:59.000000 scrutinydebugger-0.2.2/scrutiny/server/api/API.py
--rw-rw-r--   0 py        (1000) py        (1000)       64 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.2/scrutiny/server/api/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     1203 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/api/abstract_client_handler.py
--rw-rw-r--   0 py        (1000) py        (1000)     5976 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/api/dummy_client_handler.py
--rw-rw-r--   0 py        (1000) py        (1000)    11185 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.2/scrutiny/server/api/typing.py
--rw-rw-r--   0 py        (1000) py        (1000)     2868 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/api/value_streamer.py
--rw-rw-r--   0 py        (1000) py        (1000)     4652 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/api/websocket_client_handler.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.105279 scrutinydebugger-0.2.2/scrutiny/server/datalogging/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.2/scrutiny/server/datalogging/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)    29373 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.2/scrutiny/server/datalogging/datalogging_manager.py
--rw-rw-r--   0 py        (1000) py        (1000)    22438 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/datalogging/datalogging_storage.py
--rw-rw-r--   0 py        (1000) py        (1000)     2294 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/datalogging/datalogging_utilities.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.105279 scrutinydebugger-0.2.2/scrutiny/server/datalogging/definitions/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.2/scrutiny/server/datalogging/definitions/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     2771 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/datalogging/definitions/api.py
--rw-rw-r--   0 py        (1000) py        (1000)    11122 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/datalogging/definitions/device.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.105279 scrutinydebugger-0.2.2/scrutiny/server/datastore/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.2/scrutiny/server/datastore/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)    14837 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/datastore/datastore.py
--rw-rw-r--   0 py        (1000) py        (1000)    17593 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.2/scrutiny/server/datastore/datastore_entry.py
--rw-rw-r--   0 py        (1000) py        (1000)      716 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/datastore/entry_type.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.105279 scrutinydebugger-0.2.2/scrutiny/server/device/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.2/scrutiny/server/device/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)    48107 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.2/scrutiny/server/device/device_handler.py
--rw-rw-r--   0 py        (1000) py        (1000)     5021 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/device/device_info.py
--rw-rw-r--   0 py        (1000) py        (1000)    50160 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/device/emulated_device.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.105279 scrutinydebugger-0.2.2/scrutiny/server/device/links/
--rw-rw-r--   0 py        (1000) py        (1000)       94 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.2/scrutiny/server/device/links/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     1946 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/device/links/abstract_link.py
--rw-rw-r--   0 py        (1000) py        (1000)     5921 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/device/links/dummy_link.py
--rw-rw-r--   0 py        (1000) py        (1000)     7416 2024-05-12 15:52:59.000000 scrutinydebugger-0.2.2/scrutiny/server/device/links/serial_link.py
--rw-rw-r--   0 py        (1000) py        (1000)     5386 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/device/links/udp_link.py
--rw-rw-r--   0 py        (1000) py        (1000)     9056 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/device/request_dispatcher.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.105279 scrutinydebugger-0.2.2/scrutiny/server/device/submodules/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.2/scrutiny/server/device/submodules/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)    37665 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/device/submodules/datalogging_poller.py
--rw-rw-r--   0 py        (1000) py        (1000)     6350 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.2/scrutiny/server/device/submodules/device_searcher.py
--rw-rw-r--   0 py        (1000) py        (1000)     6341 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.2/scrutiny/server/device/submodules/heartbeat_generator.py
--rw-rw-r--   0 py        (1000) py        (1000)    28019 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/device/submodules/info_poller.py
--rw-rw-r--   0 py        (1000) py        (1000)    30897 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.2/scrutiny/server/device/submodules/memory_reader.py
--rw-rw-r--   0 py        (1000) py        (1000)    25434 2024-04-19 01:49:41.000000 scrutinydebugger-0.2.2/scrutiny/server/device/submodules/memory_writer.py
--rw-rw-r--   0 py        (1000) py        (1000)     6047 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/device/submodules/session_initializer.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.109279 scrutinydebugger-0.2.2/scrutiny/server/protocol/
--rw-rw-r--   0 py        (1000) py        (1000)      191 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.2/scrutiny/server/protocol/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)    16181 2024-05-05 03:12:23.000000 scrutinydebugger-0.2.2/scrutiny/server/protocol/comm_handler.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.109279 scrutinydebugger-0.2.2/scrutiny/server/protocol/commands/
--rw-rw-r--   0 py        (1000) py        (1000)      360 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.2/scrutiny/server/protocol/commands/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     1639 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/protocol/commands/base_command.py
--rw-rw-r--   0 py        (1000) py        (1000)     1084 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/protocol/commands/comm_control.py
--rw-rw-r--   0 py        (1000) py        (1000)     1439 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/protocol/commands/datalog_control.py
--rw-rw-r--   0 py        (1000) py        (1000)      517 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/protocol/commands/dummy_command.py
--rw-rw-r--   0 py        (1000) py        (1000)     1738 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/protocol/commands/get_info.py
--rw-rw-r--   0 py        (1000) py        (1000)     1448 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/protocol/commands/memory_control.py
--rw-rw-r--   0 py        (1000) py        (1000)      481 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/protocol/commands/user_command.py
--rw-rw-r--   0 py        (1000) py        (1000)      622 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/protocol/crc32.py
--rw-rw-r--   0 py        (1000) py        (1000)      790 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/protocol/exceptions.py
--rw-rw-r--   0 py        (1000) py        (1000)    61707 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.2/scrutiny/server/protocol/protocol.py
--rw-rw-r--   0 py        (1000) py        (1000)     4218 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/protocol/request.py
--rw-rw-r--   0 py        (1000) py        (1000)     4315 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/protocol/response.py
--rw-rw-r--   0 py        (1000) py        (1000)     6527 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/server/protocol/typing.py
--rw-rw-r--   0 py        (1000) py        (1000)     5269 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.2/scrutiny/server/server.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.109279 scrutinydebugger-0.2.2/scrutiny/tools/
--rw-rw-r--   0 py        (1000) py        (1000)      101 2024-05-12 14:19:24.000000 scrutinydebugger-0.2.2/scrutiny/tools/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     2573 2024-05-08 20:47:25.000000 scrutinydebugger-0.2.2/scrutiny/tools/selectable_queue.py
--rw-rw-r--   0 py        (1000) py        (1000)     4733 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.2/scrutiny/tools/synchronous_websocket_server.py
--rw-rw-r--   0 py        (1000) py        (1000)     5442 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.2/scrutiny/tools/throttler.py
--rw-rw-r--   0 py        (1000) py        (1000)     1287 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.2/scrutiny/tools/timer.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 15:58:04.109279 scrutinydebugger-0.2.2/scrutinydebugger.egg-info/
--rw-r--r--   0 py        (1000) py        (1000)      887 2024-05-12 15:58:04.000000 scrutinydebugger-0.2.2/scrutinydebugger.egg-info/PKG-INFO
--rw-rw-r--   0 py        (1000) py        (1000)     4630 2024-05-12 15:58:04.000000 scrutinydebugger-0.2.2/scrutinydebugger.egg-info/SOURCES.txt
--rw-rw-r--   0 py        (1000) py        (1000)        1 2024-05-12 15:58:04.000000 scrutinydebugger-0.2.2/scrutinydebugger.egg-info/dependency_links.txt
--rw-rw-r--   0 py        (1000) py        (1000)       52 2024-05-12 15:58:04.000000 scrutinydebugger-0.2.2/scrutinydebugger.egg-info/entry_points.txt
--rw-rw-r--   0 py        (1000) py        (1000)      222 2024-05-12 15:58:04.000000 scrutinydebugger-0.2.2/scrutinydebugger.egg-info/requires.txt
--rw-rw-r--   0 py        (1000) py        (1000)        9 2024-05-12 15:58:04.000000 scrutinydebugger-0.2.2/scrutinydebugger.egg-info/top_level.txt
--rw-rw-r--   0 py        (1000) py        (1000)       38 2024-05-12 15:58:04.113279 scrutinydebugger-0.2.2/setup.cfg
--rw-rw-r--   0 py        (1000) py        (1000)     1403 2024-05-12 14:19:24.000000 scrutinydebugger-0.2.2/setup.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.119618 scrutinydebugger-0.3.0/
+-rw-rw-r--   0 py        (1000) py        (1000)     1073 2024-03-25 03:09:50.000000 scrutinydebugger-0.3.0/LICENSE
+-rw-r--r--   0 py        (1000) py        (1000)      887 2024-05-22 03:03:20.119618 scrutinydebugger-0.3.0/PKG-INFO
+-rw-rw-r--   0 py        (1000) py        (1000)      596 2024-04-11 01:05:46.000000 scrutinydebugger-0.3.0/README.md
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.103618 scrutinydebugger-0.3.0/scrutiny/
+-rw-rw-r--   0 py        (1000) py        (1000)      188 2024-05-22 03:02:53.000000 scrutinydebugger-0.3.0/scrutiny/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)      453 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/__main__.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.103618 scrutinydebugger-0.3.0/scrutiny/cli/
+-rw-rw-r--   0 py        (1000) py        (1000)       39 2024-03-25 02:32:28.000000 scrutinydebugger-0.3.0/scrutiny/cli/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5088 2024-05-12 23:51:29.000000 scrutinydebugger-0.3.0/scrutiny/cli/cli.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.107617 scrutinydebugger-0.3.0/scrutiny/cli/commands/
+-rw-rw-r--   0 py        (1000) py        (1000)     1577 2024-03-25 02:32:28.000000 scrutinydebugger-0.3.0/scrutiny/cli/commands/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5166 2024-04-15 02:52:23.000000 scrutinydebugger-0.3.0/scrutiny/cli/commands/add_alias.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1431 2024-04-15 01:53:14.000000 scrutinydebugger-0.3.0/scrutiny/cli/commands/base_command.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2774 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/cli/commands/datalog_info.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1481 2024-04-15 01:53:14.000000 scrutinydebugger-0.3.0/scrutiny/cli/commands/delete_datalog.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2148 2024-04-15 01:53:14.000000 scrutinydebugger-0.3.0/scrutiny/cli/commands/elf2varmap.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1699 2024-04-15 01:53:14.000000 scrutinydebugger-0.3.0/scrutiny/cli/commands/export_datalog.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2082 2024-04-15 01:53:14.000000 scrutinydebugger-0.3.0/scrutiny/cli/commands/get_firmware_id.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1314 2024-04-15 01:53:14.000000 scrutinydebugger-0.3.0/scrutiny/cli/commands/install_sfd.py
+-rw-rw-r--   0 py        (1000) py        (1000)     3437 2024-05-20 14:12:17.000000 scrutinydebugger-0.3.0/scrutiny/cli/commands/launch_server.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5569 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/cli/commands/list_datalog.py
+-rw-rw-r--   0 py        (1000) py        (1000)     3746 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/cli/commands/list_sfd.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2880 2024-04-15 01:53:14.000000 scrutinydebugger-0.3.0/scrutiny/cli/commands/make_metadata.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1641 2024-04-15 01:53:14.000000 scrutinydebugger-0.3.0/scrutiny/cli/commands/make_sfd.py
+-rw-rw-r--   0 py        (1000) py        (1000)     3618 2024-04-15 01:53:14.000000 scrutinydebugger-0.3.0/scrutiny/cli/commands/runtest.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1970 2024-04-15 01:53:14.000000 scrutinydebugger-0.3.0/scrutiny/cli/commands/tag_firmware_id.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1498 2024-04-22 02:42:58.000000 scrutinydebugger-0.3.0/scrutiny/cli/commands/uninstall_sfd.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.107617 scrutinydebugger-0.3.0/scrutiny/core/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.3.0/scrutiny/core/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     7785 2024-05-22 03:02:40.000000 scrutinydebugger-0.3.0/scrutiny/core/alias.py
+-rw-rw-r--   0 py        (1000) py        (1000)     6707 2024-05-08 23:43:40.000000 scrutinydebugger-0.3.0/scrutiny/core/basic_types.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.111617 scrutinydebugger-0.3.0/scrutiny/core/bintools/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.3.0/scrutiny/core/bintools/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1924 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/core/bintools/demangler.py
+-rw-rw-r--   0 py        (1000) py        (1000)    37585 2024-05-22 03:02:40.000000 scrutinydebugger-0.3.0/scrutiny/core/bintools/elf_dwarf_var_extractor.py
+-rw-rw-r--   0 py        (1000) py        (1000)      223 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/core/bintools/elftools_stubs.py
+-rw-rw-r--   0 py        (1000) py        (1000)      547 2024-04-15 01:53:14.000000 scrutinydebugger-0.3.0/scrutiny/core/bintools/elftools_stubs.pyi
+-rw-rw-r--   0 py        (1000) py        (1000)      755 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/core/bintools/get_var_memrange.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5385 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/core/codecs.py
+-rw-rw-r--   0 py        (1000) py        (1000)     7670 2024-04-21 14:05:12.000000 scrutinydebugger-0.3.0/scrutiny/core/datalogging.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2830 2024-05-22 03:02:40.000000 scrutinydebugger-0.3.0/scrutiny/core/embedded_enum.py
+-rw-rw-r--   0 py        (1000) py        (1000)    10600 2024-04-21 03:45:36.000000 scrutinydebugger-0.3.0/scrutiny/core/firmware_description.py
+-rw-rw-r--   0 py        (1000) py        (1000)      402 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/core/firmware_id.py
+-rw-rw-r--   0 py        (1000) py        (1000)     3653 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/core/firmware_parser.py
+-rw-rw-r--   0 py        (1000) py        (1000)    14117 2024-04-22 02:42:58.000000 scrutinydebugger-0.3.0/scrutiny/core/memory_content.py
+-rw-rw-r--   0 py        (1000) py        (1000)     6939 2024-04-15 02:52:23.000000 scrutinydebugger-0.3.0/scrutiny/core/sfd_storage.py
+-rw-rw-r--   0 py        (1000) py        (1000)      334 2024-05-20 19:35:12.000000 scrutinydebugger-0.3.0/scrutiny/core/typehints.py
+-rw-rw-r--   0 py        (1000) py        (1000)     3000 2024-04-11 01:05:46.000000 scrutinydebugger-0.3.0/scrutiny/core/validation.py
+-rw-rw-r--   0 py        (1000) py        (1000)    13338 2024-05-22 03:02:40.000000 scrutinydebugger-0.3.0/scrutiny/core/variable.py
+-rw-rw-r--   0 py        (1000) py        (1000)    10695 2024-05-22 03:02:40.000000 scrutinydebugger-0.3.0/scrutiny/core/varmap.py
+-rw-rw-r--   0 py        (1000) py        (1000)      290 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/exceptions.py
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-27 04:12:19.000000 scrutinydebugger-0.3.0/scrutiny/py.typed
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.111617 scrutinydebugger-0.3.0/scrutiny/sdk/
+-rw-rw-r--   0 py        (1000) py        (1000)      350 2024-03-25 02:32:28.000000 scrutinydebugger-0.3.0/scrutiny/sdk/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)    36938 2024-05-22 03:02:40.000000 scrutinydebugger-0.3.0/scrutiny/sdk/_api_parser.py
+-rw-rw-r--   0 py        (1000) py        (1000)    73445 2024-05-22 03:02:40.000000 scrutinydebugger-0.3.0/scrutiny/sdk/client.py
+-rw-rw-r--   0 py        (1000) py        (1000)    23098 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/sdk/datalogging.py
+-rw-rw-r--   0 py        (1000) py        (1000)    13001 2024-05-20 14:12:17.000000 scrutinydebugger-0.3.0/scrutiny/sdk/definitions.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1650 2024-05-22 03:02:40.000000 scrutinydebugger-0.3.0/scrutiny/sdk/exceptions.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.111617 scrutinydebugger-0.3.0/scrutiny/sdk/listeners/
+-rw-rw-r--   0 py        (1000) py        (1000)    11943 2024-05-12 23:51:29.000000 scrutinydebugger-0.3.0/scrutiny/sdk/listeners/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1365 2024-04-11 01:05:46.000000 scrutinydebugger-0.3.0/scrutiny/sdk/listeners/buffered_reader_listener.py
+-rw-rw-r--   0 py        (1000) py        (1000)    10506 2024-04-11 01:05:46.000000 scrutinydebugger-0.3.0/scrutiny/sdk/listeners/csv_file_listener.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2127 2024-04-11 01:05:46.000000 scrutinydebugger-0.3.0/scrutiny/sdk/listeners/text_stream_listener.py
+-rw-rw-r--   0 py        (1000) py        (1000)    12565 2024-05-22 03:02:40.000000 scrutinydebugger-0.3.0/scrutiny/sdk/watchable_handle.py
+-rw-rw-r--   0 py        (1000) py        (1000)     3707 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/sdk/write_request.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.111617 scrutinydebugger-0.3.0/scrutiny/server/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.3.0/scrutiny/server/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     7890 2024-05-20 19:35:12.000000 scrutinydebugger-0.3.0/scrutiny/server/active_sfd_handler.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.111617 scrutinydebugger-0.3.0/scrutiny/server/api/
+-rw-rw-r--   0 py        (1000) py        (1000)    79349 2024-05-22 03:02:40.000000 scrutinydebugger-0.3.0/scrutiny/server/api/API.py
+-rw-rw-r--   0 py        (1000) py        (1000)       64 2024-03-25 02:32:28.000000 scrutinydebugger-0.3.0/scrutiny/server/api/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1261 2024-05-20 14:12:17.000000 scrutinydebugger-0.3.0/scrutiny/server/api/abstract_client_handler.py
+-rw-rw-r--   0 py        (1000) py        (1000)     6259 2024-05-20 14:12:17.000000 scrutinydebugger-0.3.0/scrutiny/server/api/dummy_client_handler.py
+-rw-rw-r--   0 py        (1000) py        (1000)    11237 2024-05-22 03:02:40.000000 scrutinydebugger-0.3.0/scrutiny/server/api/typing.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2868 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/server/api/value_streamer.py
+-rw-rw-r--   0 py        (1000) py        (1000)     4774 2024-05-20 19:35:12.000000 scrutinydebugger-0.3.0/scrutiny/server/api/websocket_client_handler.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.115617 scrutinydebugger-0.3.0/scrutiny/server/datalogging/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.3.0/scrutiny/server/datalogging/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)    29329 2024-05-20 19:35:12.000000 scrutinydebugger-0.3.0/scrutiny/server/datalogging/datalogging_manager.py
+-rw-rw-r--   0 py        (1000) py        (1000)    22438 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/server/datalogging/datalogging_storage.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2294 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/server/datalogging/datalogging_utilities.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.115617 scrutinydebugger-0.3.0/scrutiny/server/datalogging/definitions/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.3.0/scrutiny/server/datalogging/definitions/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2680 2024-05-20 19:35:12.000000 scrutinydebugger-0.3.0/scrutiny/server/datalogging/definitions/api.py
+-rw-rw-r--   0 py        (1000) py        (1000)    11122 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/server/datalogging/definitions/device.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.115617 scrutinydebugger-0.3.0/scrutiny/server/datastore/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.3.0/scrutiny/server/datastore/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)    14406 2024-05-20 19:35:12.000000 scrutinydebugger-0.3.0/scrutiny/server/datastore/datastore.py
+-rw-rw-r--   0 py        (1000) py        (1000)    17792 2024-05-22 03:02:40.000000 scrutinydebugger-0.3.0/scrutiny/server/datastore/datastore_entry.py
+-rw-rw-r--   0 py        (1000) py        (1000)      716 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/server/datastore/entry_type.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.115617 scrutinydebugger-0.3.0/scrutiny/server/device/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.3.0/scrutiny/server/device/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)    48109 2024-05-20 19:35:12.000000 scrutinydebugger-0.3.0/scrutiny/server/device/device_handler.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5021 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/server/device/device_info.py
+-rw-rw-r--   0 py        (1000) py        (1000)    50049 2024-05-20 14:12:17.000000 scrutinydebugger-0.3.0/scrutiny/server/device/emulated_device.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.115617 scrutinydebugger-0.3.0/scrutiny/server/device/links/
+-rw-rw-r--   0 py        (1000) py        (1000)       94 2024-03-25 02:32:28.000000 scrutinydebugger-0.3.0/scrutiny/server/device/links/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1976 2024-05-20 14:12:17.000000 scrutinydebugger-0.3.0/scrutiny/server/device/links/abstract_link.py
+-rw-rw-r--   0 py        (1000) py        (1000)     3853 2024-05-20 14:12:17.000000 scrutinydebugger-0.3.0/scrutiny/server/device/links/dummy_link.py
+-rw-rw-r--   0 py        (1000) py        (1000)     7395 2024-05-20 14:12:17.000000 scrutinydebugger-0.3.0/scrutiny/server/device/links/serial_link.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5494 2024-05-20 14:12:17.000000 scrutinydebugger-0.3.0/scrutiny/server/device/links/udp_link.py
+-rw-rw-r--   0 py        (1000) py        (1000)     8885 2024-05-20 19:35:12.000000 scrutinydebugger-0.3.0/scrutiny/server/device/request_dispatcher.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.119618 scrutinydebugger-0.3.0/scrutiny/server/device/submodules/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.3.0/scrutiny/server/device/submodules/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)    37471 2024-05-20 19:35:12.000000 scrutinydebugger-0.3.0/scrutiny/server/device/submodules/datalogging_poller.py
+-rw-rw-r--   0 py        (1000) py        (1000)     6282 2024-05-20 19:35:12.000000 scrutinydebugger-0.3.0/scrutiny/server/device/submodules/device_searcher.py
+-rw-rw-r--   0 py        (1000) py        (1000)     6202 2024-05-20 19:35:12.000000 scrutinydebugger-0.3.0/scrutiny/server/device/submodules/heartbeat_generator.py
+-rw-rw-r--   0 py        (1000) py        (1000)    27629 2024-05-20 19:35:12.000000 scrutinydebugger-0.3.0/scrutiny/server/device/submodules/info_poller.py
+-rw-rw-r--   0 py        (1000) py        (1000)    30694 2024-05-20 19:35:12.000000 scrutinydebugger-0.3.0/scrutiny/server/device/submodules/memory_reader.py
+-rw-rw-r--   0 py        (1000) py        (1000)    25277 2024-05-20 19:35:12.000000 scrutinydebugger-0.3.0/scrutiny/server/device/submodules/memory_writer.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5979 2024-05-20 19:35:12.000000 scrutinydebugger-0.3.0/scrutiny/server/device/submodules/session_initializer.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.119618 scrutinydebugger-0.3.0/scrutiny/server/protocol/
+-rw-rw-r--   0 py        (1000) py        (1000)      191 2024-03-25 02:32:28.000000 scrutinydebugger-0.3.0/scrutiny/server/protocol/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)    18574 2024-05-20 14:12:17.000000 scrutinydebugger-0.3.0/scrutiny/server/protocol/comm_handler.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.119618 scrutinydebugger-0.3.0/scrutiny/server/protocol/commands/
+-rw-rw-r--   0 py        (1000) py        (1000)      360 2024-03-25 02:32:28.000000 scrutinydebugger-0.3.0/scrutiny/server/protocol/commands/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1639 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/server/protocol/commands/base_command.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1084 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/server/protocol/commands/comm_control.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1439 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/server/protocol/commands/datalog_control.py
+-rw-rw-r--   0 py        (1000) py        (1000)      517 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/server/protocol/commands/dummy_command.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1738 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/server/protocol/commands/get_info.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1448 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/server/protocol/commands/memory_control.py
+-rw-rw-r--   0 py        (1000) py        (1000)      481 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/server/protocol/commands/user_command.py
+-rw-rw-r--   0 py        (1000) py        (1000)      622 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/server/protocol/crc32.py
+-rw-rw-r--   0 py        (1000) py        (1000)      790 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/server/protocol/exceptions.py
+-rw-rw-r--   0 py        (1000) py        (1000)    61707 2024-04-22 02:42:58.000000 scrutinydebugger-0.3.0/scrutiny/server/protocol/protocol.py
+-rw-rw-r--   0 py        (1000) py        (1000)     4218 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/server/protocol/request.py
+-rw-rw-r--   0 py        (1000) py        (1000)     4315 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/server/protocol/response.py
+-rw-rw-r--   0 py        (1000) py        (1000)     6527 2024-04-08 03:00:50.000000 scrutinydebugger-0.3.0/scrutiny/server/protocol/typing.py
+-rw-rw-r--   0 py        (1000) py        (1000)     6227 2024-05-20 14:12:17.000000 scrutinydebugger-0.3.0/scrutiny/server/server.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.119618 scrutinydebugger-0.3.0/scrutiny/tools/
+-rw-rw-r--   0 py        (1000) py        (1000)      779 2024-05-19 15:35:07.000000 scrutinydebugger-0.3.0/scrutiny/tools/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     4971 2024-05-20 14:12:17.000000 scrutinydebugger-0.3.0/scrutiny/tools/synchronous_websocket_server.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5442 2024-04-22 02:42:58.000000 scrutinydebugger-0.3.0/scrutiny/tools/throttler.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1287 2024-04-22 02:42:58.000000 scrutinydebugger-0.3.0/scrutiny/tools/timer.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-22 03:03:20.119618 scrutinydebugger-0.3.0/scrutinydebugger.egg-info/
+-rw-r--r--   0 py        (1000) py        (1000)      887 2024-05-22 03:03:20.000000 scrutinydebugger-0.3.0/scrutinydebugger.egg-info/PKG-INFO
+-rw-rw-r--   0 py        (1000) py        (1000)     4626 2024-05-22 03:03:20.000000 scrutinydebugger-0.3.0/scrutinydebugger.egg-info/SOURCES.txt
+-rw-rw-r--   0 py        (1000) py        (1000)        1 2024-05-22 03:03:20.000000 scrutinydebugger-0.3.0/scrutinydebugger.egg-info/dependency_links.txt
+-rw-rw-r--   0 py        (1000) py        (1000)       52 2024-05-22 03:03:20.000000 scrutinydebugger-0.3.0/scrutinydebugger.egg-info/entry_points.txt
+-rw-rw-r--   0 py        (1000) py        (1000)      222 2024-05-22 03:03:20.000000 scrutinydebugger-0.3.0/scrutinydebugger.egg-info/requires.txt
+-rw-rw-r--   0 py        (1000) py        (1000)        9 2024-05-22 03:03:20.000000 scrutinydebugger-0.3.0/scrutinydebugger.egg-info/top_level.txt
+-rw-rw-r--   0 py        (1000) py        (1000)       38 2024-05-22 03:03:20.127617 scrutinydebugger-0.3.0/setup.cfg
+-rw-rw-r--   0 py        (1000) py        (1000)     1403 2024-05-20 14:12:17.000000 scrutinydebugger-0.3.0/setup.py
```

### Comparing `scrutinydebugger-0.2.2/LICENSE` & `scrutinydebugger-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/PKG-INFO` & `scrutinydebugger-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: scrutinydebugger
-Version: 0.2.2
+Version: 0.3.0
 Summary: Scrutiny debugger Python framework
 Home-page: https://github.com/scrutinydebugger/scrutiny-python
 Author: Pier-Yves Lessard
 License: MIT
 Requires-Python: >3.8
 License-File: LICENSE
-Requires-Dist: appdirs>=1.4.4
-Requires-Dist: pyelftools>=0.29
-Requires-Dist: websockets>=11.0.3
-Requires-Dist: sortedcontainers>=2.4
-Requires-Dist: pyserial>=3.5
+Requires-Dist: appdirs==1.4.4
+Requires-Dist: pyelftools==0.31
+Requires-Dist: websockets==12.0
+Requires-Dist: sortedcontainers==2.4.0
+Requires-Dist: pyserial==3.5
 Provides-Extra: test
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: sphinx-book-theme==1.1.2; extra == "test"
 Requires-Dist: sphinx==7.2.6; extra == "test"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
```

### Comparing `scrutinydebugger-0.2.2/README.md` & `scrutinydebugger-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/cli/cli.py` & `scrutinydebugger-0.3.0/scrutiny/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                 return 0
 
         cargs, command_cargs = self.parser.parse_known_args(args)
         if cargs.command not in [cls.get_name() for cls in self.command_list]:
             if except_failed:
                 raise Exception('Unknown command %s' % cargs.command)
             self.parser.print_help()
-            return -1
+            return 1
 
         error = None
         try:
             logging_level_str = cargs.loglevel if cargs.loglevel else self.default_log_level
             logging_level = getattr(logging, logging_level_str.upper())
             format_string = ""
             if logging_level == logging.DEBUG:
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/cli/commands/__init__.py` & `scrutinydebugger-0.3.0/scrutiny/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/cli/commands/add_alias.py` & `scrutinydebugger-0.3.0/scrutiny/cli/commands/add_alias.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/cli/commands/base_command.py` & `scrutinydebugger-0.3.0/scrutiny/cli/commands/base_command.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/cli/commands/datalog_info.py` & `scrutinydebugger-0.3.0/scrutiny/cli/commands/datalog_info.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/cli/commands/delete_datalog.py` & `scrutinydebugger-0.3.0/scrutiny/cli/commands/delete_datalog.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/cli/commands/elf2varmap.py` & `scrutinydebugger-0.3.0/scrutiny/cli/commands/elf2varmap.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/cli/commands/export_datalog.py` & `scrutinydebugger-0.3.0/scrutiny/cli/commands/export_datalog.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/cli/commands/get_firmware_id.py` & `scrutinydebugger-0.3.0/scrutiny/cli/commands/get_firmware_id.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/cli/commands/install_sfd.py` & `scrutinydebugger-0.3.0/scrutiny/cli/commands/install_sfd.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/cli/commands/list_datalog.py` & `scrutinydebugger-0.3.0/scrutiny/cli/commands/list_datalog.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/cli/commands/list_sfd.py` & `scrutinydebugger-0.3.0/scrutiny/cli/commands/list_sfd.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/cli/commands/make_metadata.py` & `scrutinydebugger-0.3.0/scrutiny/cli/commands/make_metadata.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/cli/commands/make_sfd.py` & `scrutinydebugger-0.3.0/scrutiny/cli/commands/make_sfd.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/cli/commands/runtest.py` & `scrutinydebugger-0.3.0/scrutiny/cli/commands/runtest.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/cli/commands/tag_firmware_id.py` & `scrutinydebugger-0.3.0/scrutiny/cli/commands/tag_firmware_id.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/cli/commands/uninstall_sfd.py` & `scrutinydebugger-0.3.0/scrutiny/cli/commands/uninstall_sfd.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/core/alias.py` & `scrutinydebugger-0.3.0/scrutiny/core/alias.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #
 #   Copyright (c) 2021 Scrutiny Debugger
 
 import json
 import math
 
 from scrutiny.server.datastore.entry_type import EntryType
+from scrutiny.core.embedded_enum import EmbeddedEnum
 
 from typing import Dict, Optional, Any, Union
 
 
 class Alias:
     """
     Represent an Alias. Read/write to an alias are deferred to another object (either a Variable or a Runtime Published Value)
@@ -32,14 +33,16 @@
     """Optional multiplier to apply on the value. 1 if ``None``"""
     offset: Optional[float]
     """Optional offset to apply on the value. 0 if ``None``"""
     min: Optional[float]
     """Optional max to apply on the value. +inf if ``None``"""
     max: Optional[float]
     """Optional min to apply on the value. -inf if ``None``"""
+    enum:Optional[EmbeddedEnum]
+    """Optional enum to add on top of the value being watched"""
 
     @classmethod
     def from_json(cls, fullpath: str, json_str: str) -> 'Alias':
         d = json.loads(json_str)
         return cls.from_dict(fullpath, d)
 
     @classmethod
@@ -49,20 +52,30 @@
         obj_out = cls(
             fullpath=fullpath,
             target=obj['target'],
             target_type=obj['target_type'] if 'target_type' in obj else None,
             gain=obj['gain'] if 'gain' in obj else None,
             offset=obj['offset'] if 'offset' in obj else None,
             min=obj['min'] if 'min' in obj else None,
-            max=obj['max'] if 'max' in obj else None
+            max=obj['max'] if 'max' in obj else None,
+            enum=EmbeddedEnum.from_def(obj['enum']) if 'enum' in obj else None
         )
         obj_out.validate()
         return obj_out
 
-    def __init__(self, fullpath: str, target: str, target_type: Optional[EntryType] = None, gain: Optional[float] = None, offset: Optional[float] = None, min: Optional[float] = None, max: Optional[float] = None):
+    def __init__(self, 
+            fullpath: str, 
+            target: str, 
+            target_type: Optional[EntryType] = None, 
+            gain: Optional[float] = None, 
+            offset: Optional[float] = None, 
+            min: Optional[float] = None, 
+            max: Optional[float] = None,
+            enum:Optional[EmbeddedEnum] = None
+        ):
         self.fullpath = fullpath
         # Target type can be set later on.
         if target_type is not None:
             target_type = EntryType(target_type)
             if target_type == EntryType.Alias:
                 raise ValueError("Cannot make an alias over another alias.")
             self.target_type = EntryType(target_type)
@@ -70,14 +83,15 @@
             self.target_type = None
         self.target = target
         # Set to None if unset. getter will return the default value.
         self.gain = float(gain) if gain is not None else None
         self.offset = float(offset) if offset is not None else None
         self.min = float(min) if min is not None else None
         self.max = float(max) if max is not None else None
+        self.enum = enum
 
     def validate(self) -> None:
         """Raise an exception if internal values are bad"""
         if not self.fullpath or not isinstance(self.fullpath, str):
             raise ValueError('fullpath is not valid')
 
         if self.target_type is not None:
@@ -100,14 +114,18 @@
 
         if not math.isfinite(self.get_gain()):
             raise ValueError('Gain is not a finite value')
 
         if not math.isfinite(self.get_offset()):
             raise ValueError('Gain is not a finite value')
 
+        if self.enum is not None:
+            if not isinstance(self.enum, EmbeddedEnum):
+                raise ValueError("enum must be a valid EmbeddedEnum")
+
     def to_dict(self) -> Dict[str, Any]:
         """Make a dict containing all the information on the alias and that can be loaded with `from_json` """
         d: Dict[str, Any] = dict(target=self.target, target_type=self.target_type)
 
         # Save some space in alias.json by ommiting defaults value
         if self.gain is not None and self.gain != 1.0:
             d['gain'] = self.gain
@@ -116,14 +134,17 @@
             d['offset'] = self.offset
 
         if self.min is not None and self.min != float('-inf'):
             d['min'] = self.min
 
         if self.max is not None and self.max != float('inf'):
             d['max'] = self.max
+        
+        if self.enum is not None:
+            d['enum'] = self.enum.get_def()
 
         return d
 
     def to_json(self) -> str:
         return json.dumps(self.to_dict())
 
     def get_fullpath(self) -> str:
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/core/basic_types.py` & `scrutinydebugger-0.3.0/scrutiny/core/basic_types.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/core/bintools/demangler.py` & `scrutinydebugger-0.3.0/scrutiny/core/bintools/demangler.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/core/bintools/elf_dwarf_var_extractor.py` & `scrutinydebugger-0.3.0/scrutiny/core/bintools/elf_dwarf_var_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,20 +18,19 @@
 import inspect
 from dataclasses import dataclass
 from inspect import currentframe
 
 from scrutiny.core.varmap import VarMap
 from scrutiny.core.basic_types import *
 from scrutiny.core.variable import *
+from scrutiny.core.embedded_enum import *
 from scrutiny.exceptions import EnvionmentNotSetUpException
 from scrutiny.core.bintools import elftools_stubs
 
-from typing import Optional, List, Dict, Any, Union, cast, Iterable, Callable, Set, Tuple, TYPE_CHECKING, Tuple
-
-
+from typing import Optional, List, Dict, Union, cast, Set, Tuple
 
 def get_linenumber() -> int:
     cf = currentframe()
     if cf is None:
         return -1
     if cf.f_back is None:
         return -1
@@ -55,15 +54,14 @@
     enum_die:Optional[ "elftools_stubs.Die"]
     type_die: "elftools_stubs.Die"
 
 class ElfParsingError(Exception):
     pass
 
 
-
 class CuName:
     """
     Handles a compile unit name. Useful to build a unique name as small as possible.
     """
     _class_internal_id = 0
     PATH_JOIN_CHAR = '_'
 
@@ -139,15 +137,15 @@
         DW_ATE_lo_user = 0x80
         DW_ATE_hi_user = 0xff
 
     varmap: VarMap
     die2typeid_map: Dict["elftools_stubs.Die", str]
     die2vartype_map: Dict["elftools_stubs.Die", EmbeddedDataType]
     cu_name_map: Dict["elftools_stubs.CompileUnit", str]
-    enum_die_map: Dict["elftools_stubs.Die", VariableEnum]
+    enum_die_map: Dict["elftools_stubs.Die", EmbeddedEnum]
     struct_die_map: Dict["elftools_stubs.Die", Struct]
     endianness: Endianness
     cppfilt: Optional[str]
     logger: logging.Logger
 
     def __init__(self, filename: Optional[str] = None, cppfilt: Optional[str] = None) -> None:
         self.varmap = VarMap()    # This is what we want to generate.
@@ -446,15 +444,15 @@
         self.die2typeid_map[die] = self.varmap.get_type_id(name)
         self.die2vartype_map[die] = basetype
 
     def die_process_enum(self, die: "elftools_stubs.Die") -> None:
         self.log_debug_process_die(die)
         name = self.get_name(die)
         if die not in self.enum_die_map:
-            enum = VariableEnum(name)
+            enum = EmbeddedEnum(name)
 
             for child in die.iter_children():
                 if child.tag != 'DW_TAG_enumerator':
                     continue
 
                 name = self.get_name(child)
                 if 'DW_AT_const_value' in child.attributes:
@@ -606,15 +604,15 @@
     def get_member_from_die(self, die: "elftools_stubs.Die", is_in_union:bool=False) -> Optional[Struct.Member]:
         self.log_debug_process_die(die)
         try:
             name = self.get_name(die) 
         except Exception:
             name = ""
         type_desc = self.get_type_of_var(die)
-        enum:Optional[VariableEnum] = None
+        enum:Optional[EmbeddedEnum] = None
         if type_desc.type in (TypeOfVar.Struct, TypeOfVar.Class, TypeOfVar.Union):
             substruct = self.get_composite_type_def(type_desc.type_die)  # recursion
             typename = None
         elif type_desc.type in (TypeOfVar.BaseType, TypeOfVar.EnumOnly):
             if type_desc.enum_die is not None:
                 self.die_process_enum(type_desc.enum_die)
                 enum = self.enum_die_map[type_desc.enum_die]
@@ -725,15 +723,15 @@
             )
 
     def register_variable(self, 
                           name:str, 
                           path_segments:List[str], 
                           location:VariableLocation, 
                           original_type_name:str, 
-                          enum:Optional[VariableEnum] 
+                          enum:Optional[EmbeddedEnum] 
                           ) -> None:
         """Adds a variable to the varmap.
         
             :param name: Name of the variable
             :param path_segments: List of str representing each level of display tree
             :param location: The address of the variable
             :param original_type_name: The name of the underlying type. Must be a name coming from the binary. Will resolve to an EmbeddedDataType
@@ -793,15 +791,15 @@
                     self.die_process_struct_class_union(type_desc.type_die)
                     self.register_struct_var(die, type_desc.type_die, location)
                 # Base type
                 elif type_desc.type in (TypeOfVar.BaseType, TypeOfVar.EnumOnly):
                     path_segments = self.make_varpath(die)
                     name = self.get_name(die)
                     
-                    enum:Optional[VariableEnum] = None
+                    enum:Optional[EmbeddedEnum] = None
                     if type_desc.enum_die is not None:
                         self.die_process_enum(type_desc.enum_die)
                         enum = self.enum_die_map[type_desc.enum_die]
 
                     if type_desc.type == TypeOfVar.BaseType :   # Most common case
                         self.die_process_base_type(type_desc.type_die)    # Just in case it is unknown yet
                         typename = self.get_typename_from_die(type_desc.type_die)
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/core/bintools/elftools_stubs.pyi` & `scrutinydebugger-0.3.0/scrutiny/core/bintools/elftools_stubs.pyi`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/core/bintools/get_var_memrange.py` & `scrutinydebugger-0.3.0/scrutiny/core/bintools/get_var_memrange.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/core/codecs.py` & `scrutinydebugger-0.3.0/scrutiny/core/codecs.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/core/datalogging.py` & `scrutinydebugger-0.3.0/scrutiny/core/datalogging.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/core/firmware_description.py` & `scrutinydebugger-0.3.0/scrutiny/core/firmware_description.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/core/firmware_parser.py` & `scrutinydebugger-0.3.0/scrutiny/core/firmware_parser.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/core/memory_content.py` & `scrutinydebugger-0.3.0/scrutiny/core/memory_content.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/core/sfd_storage.py` & `scrutinydebugger-0.3.0/scrutiny/core/sfd_storage.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/core/validation.py` & `scrutinydebugger-0.3.0/scrutiny/core/validation.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/core/variable.py` & `scrutinydebugger-0.3.0/scrutiny/core/variable.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 #   - License : MIT - See LICENSE file.
 #   - Project :  Scrutiny Debugger (github.com/scrutinydebugger/scrutiny-python)
 #
 #   Copyright (c) 2021 Scrutiny Debugger
 
 __all__ = [
     'VariableLocation',
-    'VariableEnumDef',
-    'VariableEnum',
     'Struct',
     'Variable'
 ]
 
 import struct
 from scrutiny.core.basic_types import Endianness, EmbeddedDataType
+from scrutiny.core.embedded_enum import EmbeddedEnum
 from scrutiny.core.codecs import Codecs, Encodable, UIntCodec
-from typing import Dict, Union, List, Literal, Optional, TypedDict, Any, Tuple
+from typing import Dict, Union, List, Literal, Optional,  Tuple
 from copy import deepcopy
 
 MASK_MAP: Dict[int, int] = {}
 for i in range(64):
     v = 0
     for j in range(i):
         v |= (1 << j)
@@ -86,95 +85,34 @@
     def __str__(self) -> str:
         return str(self.get_address())
 
     def __repr__(self) -> str:
         return '<%s - 0x%08X>' % (self.__class__.__name__, self.get_address())
 
 
-class VariableEnumDef(TypedDict):
-    """
-    Represent the dictionary version of the VariableEnum (for .json import/export).
-    Used only for type hints
-    """
-    name: str
-    values: Dict[str, int]
-
-
-class VariableEnum:
-    """
-    Represents an enumeration in the embedded code.
-    Match a string to an int value
-    """
-    name: str
-    vals: Dict[str, int]
-
-    def __init__(self, name: str):
-        self.name = name
-        self.vals = {}
-
-    def add_value(self, name: str, value: int) -> None:
-        """Add a string/value pair in the enum"""
-        if name in self.vals and self.vals[name] != value:
-            raise Exception('Duplicate entry for enum %s. %s can either be %s or %s' % (self.name, name, self.vals[name], value))
-
-        self.vals[name] = value
-
-    def get_name(self) -> str:
-        """Return the name of the enum"""
-        return self.name
-
-    def get_value(self, name: str) -> int:
-        """Return the value associated with a name"""
-        if name not in self.vals:
-            raise Exception('%s is not a valid name for enum %s' % (name, self.name))
-        return self.vals[name]
-
-    def get_def(self) -> VariableEnumDef:
-        """Export to dict for json serialization mainly"""
-        obj: VariableEnumDef = {
-            'name': self.name,
-            'values': self.vals
-        }
-        return obj
-
-    def has_signed_value(self) -> bool:
-        for v in self.vals.values():
-            if v < 0:
-                return True
-        return False
-
-
-    @classmethod
-    def from_def(cls, enum_def: VariableEnumDef) -> "VariableEnum":
-        """Recreate from a .json dict"""
-        obj = VariableEnum(enum_def['name'])
-        obj.vals = enum_def['values']
-        return obj
-
-
 class Struct:
     class Member:
         name: str
         is_substruct: bool
         original_type_name: Optional[str]
         bitoffset: Optional[int]
         byte_offset: Optional[int]
         bitsize: Optional[int]
         substruct: Optional['Struct']
-        enum:Optional['VariableEnum']
+        enum:Optional[EmbeddedEnum]
         is_unnamed:bool
 
         def __init__(self, name: str,
                      is_substruct: bool = False,
                      original_type_name: Optional[str] = None,
                      byte_offset: Optional[int] = None,
                      bitoffset: Optional[int] = None,
                      bitsize: Optional[int] = None,
                      substruct: Optional['Struct'] = None,
-                     enum:Optional['VariableEnum'] = None,
+                     enum:Optional[EmbeddedEnum] = None,
                      is_unnamed:bool=False
                      ):
 
             if not is_substruct:
                 if original_type_name is None:
                     raise ValueError('A typename must be given for non-struct member')
 
@@ -265,17 +203,26 @@
     vartype: EmbeddedDataType
     path_segments: List[str]
     location: VariableLocation
     endianness: Endianness
     bitsize: Optional[int]
     bitfield: bool
     bitoffset: Optional[int]
-    enum: Optional[VariableEnum]
+    enum: Optional[EmbeddedEnum]
 
-    def __init__(self, name: str, vartype: EmbeddedDataType, path_segments: List[str], location: Union[int, VariableLocation], endianness: Endianness, bitsize: Optional[int] = None, bitoffset: Optional[int] = None, enum: Optional[VariableEnum] = None):
+    def __init__(self, 
+        name: str, 
+        vartype: EmbeddedDataType, 
+        path_segments: List[str], 
+        location: Union[int, VariableLocation], 
+        endianness: Endianness, 
+        bitsize: Optional[int] = None, 
+        bitoffset: Optional[int] = None, 
+        enum: Optional[EmbeddedEnum] = None
+    ) -> None:
 
         self.name = name
         self.vartype = vartype
         self.path_segments = path_segments
         if isinstance(location, VariableLocation):
             self.location = location.copy()
         else:
@@ -369,15 +316,15 @@
         """Get the variable address"""
         return self.location.get_address()
 
     def has_enum(self) -> bool:
         """True if an enum is attached to that variable"""
         return self.enum is not None
 
-    def get_enum(self) -> Optional[VariableEnum]:
+    def get_enum(self) -> Optional[EmbeddedEnum]:
         """Return the enum attached to the variable. None if it does not exists"""
         return self.enum
 
     def get_size(self) -> int:
         """Returns the size of the variable in bytes"""
         size_bit = self.vartype.get_size_bit()
         return int(size_bit / 8)
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/core/varmap.py` & `scrutinydebugger-0.3.0/scrutiny/core/varmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 #
 #   Copyright (c) 2021 Scrutiny Debugger
 
 import json
 import os
 import logging
 
-from scrutiny.core.variable import Variable, VariableEnum, VariableLocation
+from scrutiny.core.variable import Variable, VariableLocation
 from scrutiny.core.basic_types import EmbeddedDataType, Endianness
 from typing import Dict, TypedDict, List, Tuple, Optional, Any, Union, Generator
-from scrutiny.core.variable import VariableEnumDef
+from scrutiny.core.embedded_enum import EmbeddedEnum, EmbeddedEnumDef
 
 
 class TypeEntry(TypedDict):
     name: str
     type: str
 
 
@@ -33,20 +33,20 @@
 
 # TODO : This class requires more work and unit tests
 class VarMap:
     logger: logging.Logger
     endianness: Endianness
     typemap: Dict[str, TypeEntry]
     variables: Dict[str, VariableEntry]
-    enums: Dict[str, VariableEnumDef]
+    enums: Dict[str, EmbeddedEnumDef]
 
     next_type_id: int
     next_enum_id: int
     typename2typeid_map: Dict[str, str]      # name to numeric id as string
-    enums_to_id_map: Dict[VariableEnum, int]
+    enums_to_id_map: Dict[EmbeddedEnum, int]
 
     def __init__(self, file: Optional[Union[str, bytes]] = None):
         self.logger = logging.getLogger(self.__class__.__name__)
         error = None
         if file is not None:
             try:
                 if os.path.isfile(file):
@@ -84,15 +84,15 @@
         self.validate()  # Validate only if loaded. Otherwise, we may be building a new varmap file (from CLI)
         self.init_all()
 
     def init_all(self) -> None:
         self.next_type_id = 0
         self.next_enum_id = 0
         self.typename2typeid_map = {}   # Maps the type id of this VarMap to the original name inside the binary.
-        self.enums_to_id_map = {}       # Maps a VariableEnum object to it's internal id
+        self.enums_to_id_map = {}       # Maps a EmbeddedEnum object to it's internal id
 
         # Build typename2typeid_map
         for typeid_str in self.typemap:
             typeid_int = int(typeid_str)
             if typeid_int > self.next_type_id:
                 self.next_type_id = typeid_int
 
@@ -101,15 +101,15 @@
 
         # Build enums_to_id_map
         for enum_id_str in self.enums:
             enum_id_int = int(enum_id_str)
             if enum_id_int > self.next_enum_id:
                 self.next_enum_id = enum_id_int
 
-            enum = VariableEnum.from_def(self.enums[str(enum_id_int)])
+            enum = EmbeddedEnum.from_def(self.enums[str(enum_id_int)])
             self.enums_to_id_map[enum] = enum_id_int
 
     def set_endianness(self, endianness: Endianness) -> None:
         if endianness not in [Endianness.Little, Endianness.Big]:
             raise ValueError('Invalid endianness %s' % endianness)
         self.endianness = endianness
 
@@ -154,15 +154,15 @@
     def add_variable(self,
                      path_segments: List[str],
                      name: str,
                      location: VariableLocation,
                      original_type_name: str,
                      bitsize: Optional[int] = None,
                      bitoffset: Optional[int] = None,
-                     enum: Optional[VariableEnum] = None
+                     enum: Optional[EmbeddedEnum] = None
                      ) -> None:
         if not self.is_known_type(original_type_name):
             raise ValueError('Cannot add variable of type %s. Type has not been registered yet' % (original_type_name))
 
         fullname = self.make_fullname(path_segments, name)
         if fullname in self.variables:
             self.logger.warning('duplicate entry %s' % fullname)
@@ -268,19 +268,19 @@
         return None
 
     def get_bitoffset(self, vardef: VariableEntry) -> Optional[int]:
         if 'bitoffset' in vardef:
             return vardef['bitoffset']
         return None
 
-    def get_enum(self, vardef: VariableEntry) -> Optional[VariableEnum]:
+    def get_enum(self, vardef: VariableEntry) -> Optional[EmbeddedEnum]:
         if 'enum' in vardef:
             enum_id = str(vardef['enum'])
             if enum_id not in self.enums:
                 raise Exception("Unknown enum ID %s" % enum_id)
             enum_def = self.enums[enum_id]
-            return VariableEnum.from_def(enum_def)
+            return EmbeddedEnum.from_def(enum_def)
         return None
 
     def iterate_vars(self) -> Generator[Tuple[str, Variable], None, None]:
         for fullname in self.variables:
             yield (fullname, self.get_var(fullname))
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/sdk/_api_parser.py` & `scrutinydebugger-0.3.0/scrutiny/sdk/_api_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #
 #   Copyright (c) 2021 Scrutiny Debugger
 
 import scrutiny.sdk
 import scrutiny.sdk.datalogging
 sdk = scrutiny.sdk  # Workaround for vscode linter an submodule on alias
 from scrutiny.core.basic_types import *
+from scrutiny.core.embedded_enum import EmbeddedEnum
 from scrutiny.core.firmware_description import MetadataType as FirmwareMetadataDict
 from scrutiny.server.api.API import API
 from scrutiny.server.api import typing as api_typing
 from dataclasses import dataclass
 from datetime import datetime
 from base64 import b64decode
 import binascii
@@ -23,14 +24,15 @@
 
 
 @dataclass(frozen=True)
 class WatchableConfiguration:
     watchable_type: sdk.WatchableType
     datatype: EmbeddedDataType
     server_id: str
+    enum:Optional[EmbeddedEnum]
 
 
 @dataclass(frozen=True)
 class WatchableUpdate:
     server_id: str
     value: Union[bool, int, float]
 
@@ -218,25 +220,39 @@
     _check_response_dict(cmd, content, 'datatype', str, keyprefix)
 
     if content['datatype'] not in API.APISTR_2_DATATYPE:
         raise sdk.exceptions.BadResponseError(f"Unknown datatype {content['datatype']}")
 
     datatype = EmbeddedDataType(API.APISTR_2_DATATYPE[content['datatype']])
 
+    enum:Optional[EmbeddedEnum] = None
+    if 'enum' in content and content['enum'] is not None:
+        _check_response_dict(cmd, content, 'enum', dict)
+        _check_response_dict(cmd, content, 'enum.name', str)
+        _check_response_dict(cmd, content, 'enum.values', dict)
+        enum = EmbeddedEnum(name=content['enum']['name'])
+        for key, val in content['enum']['values'].items():
+            if not isinstance(key, str): 
+                raise sdk.exceptions.BadResponseError('Invalid enum. Key is not a string')
+            if not isinstance(val, int): 
+                raise sdk.exceptions.BadResponseError('Invalid enum. Value is not an integer')
+            enum.add_value(key, val)
+
     if requested_path != content['display_path']:
         raise sdk.exceptions.BadResponseError(
             f"The display path of the element returned by the server does not matched the requested path. Got {content['display_path']} but expected {requested_path}")
 
     if not isinstance(content['id'], str):
         raise sdk.exceptions.BadResponseError(f"Invalid server id received for watchable {requested_path}")
 
     return WatchableConfiguration(
         watchable_type=watchable_type,
         datatype=datatype,
-        server_id=content['id']
+        server_id=content['id'],
+        enum=enum
     )
 
 
 def parse_subscribe_watchable_response(response: api_typing.S2C.SubscribeWatchable) -> Dict[str, WatchableConfiguration]:
     """Parse a response to get_watchable_list and assume the request was for a single watchable"""
     assert isinstance(response, dict)
     assert 'cmd' in response
@@ -249,14 +265,28 @@
         if not isinstance(k, str):
             raise sdk.exceptions.BadResponseError('Gotten a subscription dict with invalid key')
 
         _check_response_dict(cmd, v, 'datatype', str)
         _check_response_dict(cmd, v, 'type', str)
         _check_response_dict(cmd, v, 'id', str)
 
+        enum:Optional[EmbeddedEnum] = None
+        if 'enum' in v and v['enum'] is not None:
+            _check_response_dict(cmd, v, 'enum', dict)
+            _check_response_dict(cmd, v, 'enum.name', str)
+            _check_response_dict(cmd, v, 'enum.values', dict)
+            enum = EmbeddedEnum(name=v['enum']['name'])
+            for key, val in v['enum']['values'].items():
+                if not isinstance(key, str): 
+                    raise sdk.exceptions.BadResponseError('Invalid enum. Key is not a string')
+                if not isinstance(val, int): 
+                    raise sdk.exceptions.BadResponseError('Invalid enum. Value is not an integer')
+                enum.add_value(key, val)
+                
+
         if v['datatype'] not in API.APISTR_2_DATATYPE:
             raise sdk.exceptions.BadResponseError(f"Unknown datatype {v['datatype']}")
 
         datatype = EmbeddedDataType(API.APISTR_2_DATATYPE[v['datatype']])
         if v['type'] == 'alias':
             watchable_type = sdk.WatchableType.Alias
         elif v['type'] == 'var':
@@ -265,15 +295,16 @@
             watchable_type = sdk.WatchableType.RuntimePublishedValue
         else:
             raise sdk.exceptions.BadResponseError(f"Unsupported watchable type {v['type']}")
 
         outdict[k] = WatchableConfiguration(
             watchable_type=watchable_type,
             datatype=datatype,
-            server_id=v['id']
+            server_id=v['id'],
+            enum=enum
         )
     return outdict
 
 
 def parse_inform_server_status(response: api_typing.S2C.InformServerStatus) -> sdk.ServerInfo:
     """Parse the inform_server_status message"""
 
@@ -406,16 +437,14 @@
     def _link_type(api_val: api_typing.LinkType) -> sdk.DeviceLinkType:
         if api_val == 'none':
             return sdk.DeviceLinkType.NA
         if api_val == 'serial':
             return sdk.DeviceLinkType.Serial
         if api_val == 'dummy':
             return sdk.DeviceLinkType._Dummy
-        if api_val == 'thread_safe_dummy':
-            return sdk.DeviceLinkType._DummyThreadSafe
         if api_val == 'udp':
             return sdk.DeviceLinkType.UDP
         raise sdk.exceptions.BadResponseError('Unsupported device link type "{api_val}"')
 
     link_type = _link_type(response['device_comm_link']['link_type'])
 
     link_config: Optional[sdk.SupportedLinkConfig]
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/sdk/client.py` & `scrutinydebugger-0.3.0/scrutiny/sdk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -936,14 +936,15 @@
                     raise sdk.exceptions.BadResponseError(
                         f'The server did not confirm the subscription for the right watchable. Got {list(response["subscribed"].keys())[0]}, expected {path}')
 
                 watchable._configure(
                     datatype=watchable_defs[path].datatype,
                     watchable_type=watchable_defs[path].watchable_type,
                     server_id=watchable_defs[path].server_id,
+                    enum=watchable_defs[path].enum
                 )
 
         req = self._make_request(API.Command.Client2Api.SUBSCRIBE_WATCHABLE, {
             'watchables': [watchable.display_path]  # Single element
         })
         future = self._send(req, wt_subscribe_callback)
         assert future is not None
@@ -1484,15 +1485,14 @@
         assert link_type is not None
         assert link_config is not None
 
         api_map: Dict["DeviceLinkType", Tuple[str, Type[Union[BaseLinkConfig, None]]]] = {
             DeviceLinkType.Serial: ('serial', sdk.SerialLinkConfig),
             DeviceLinkType.UDP: ('udp', sdk.UDPLinkConfig),
             DeviceLinkType.TCP: ('tcp', sdk.TCPLinkConfig),
-            DeviceLinkType._DummyThreadSafe: ('thread_safe_dummy', type(None)),
             DeviceLinkType._Dummy: ('dummy', type(None))
         }
 
         if link_type not in api_map:
             raise ValueError(f"Unsupported link type : {link_type.name}")
 
         link_type_api_name, config_type = api_map[link_type]
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/sdk/datalogging.py` & `scrutinydebugger-0.3.0/scrutiny/sdk/datalogging.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/sdk/definitions.py` & `scrutinydebugger-0.3.0/scrutiny/sdk/definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,14 @@
     Error = 5
     """The datalogger has encountered a problem and is not operational"""
 
 
 class DeviceLinkType(enum.Enum):
     """(Enum) The type of communication link used between the server and the device"""
 
-    _DummyThreadSafe = -2
     _Dummy = -1
     NA = 0
     UDP = 1
     """UDP/IP socket"""
     TCP = 2
     """TCP/IP Socket"""
     Serial = 3
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/sdk/exceptions.py` & `scrutinydebugger-0.3.0/scrutiny/sdk/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,19 @@
 
 class TimeoutException(ScrutinySDKException):
     """Raised when synchronous operations times out"""
     pass
 
 
 class NameNotFoundError(ScrutinySDKException):
-    """Raised when raised when trying to reference an element by its name and the name is invalid or unknown"""
+    """Raised when trying to reference an element by its name and the name is invalid or unknown"""
+    pass
+
+class BadEnumError(ScrutinySDKException):
+    """Raised when trying access an enum value that does not exists"""
     pass
 
 
 class ApiError(ScrutinySDKException):
     """Base class for all error related to the API"""
     pass
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/sdk/listeners/__init__.py` & `scrutinydebugger-0.3.0/scrutiny/sdk/listeners/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
         self._stop_request_event.clear()
         self._started_event.clear()
         self._setup_error=False
         self._teardown_error=False
         self._receive_error=False
         self._update_count=0
         self._update_queue = queue.Queue(self._queue_max_size)
-        self._thread = threading.Thread(target=self._thread_task)
+        self._thread = threading.Thread(target=self._thread_task, daemon=True)
         self._thread.start()
 
         self._started_event.wait(2)
         if not self._started_event.is_set():
             self.stop()
             raise sdk_exceptions.OperationFailure("Failed to start listener thread")
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/sdk/listeners/buffered_reader_listener.py` & `scrutinydebugger-0.3.0/scrutiny/sdk/listeners/buffered_reader_listener.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/sdk/listeners/csv_file_listener.py` & `scrutinydebugger-0.3.0/scrutiny/sdk/listeners/csv_file_listener.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/sdk/listeners/text_stream_listener.py` & `scrutinydebugger-0.3.0/scrutiny/sdk/listeners/text_stream_listener.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/sdk/watchable_handle.py` & `scrutinydebugger-0.3.0/scrutiny/sdk/watchable_handle.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import threading
 from datetime import datetime
 import time
 
 from scrutiny.sdk.definitions import *
 from scrutiny.core.basic_types import *
+from scrutiny.core.embedded_enum import EmbeddedEnum
 import scrutiny.sdk.exceptions as sdk_exceptions
 from scrutiny.sdk.write_request import WriteRequest
 from scrutiny.core import validation
 from typing import Optional, Union, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from scrutiny.sdk.client import ScrutinyClient
@@ -33,14 +34,15 @@
     _shortname: str         # Name of the last element in the display path
     _lock: threading.Lock   # A lock to access the value
 
     _datatype: EmbeddedDataType     # The datatype represented in the device (uint8, float32, etc)
     _watchable_type: WatchableType  # Tye of watchable : Alias, Variable or RPV
     _server_id: Optional[str]       # The ID assigned by the server
     _status: ValueStatus            # Status of the value. Tells if the value is valid or not and why it is invalid if not
+    _enum: Optional[EmbeddedEnum]   # Enum that applies to this watchable
 
     _value: Optional[ValType]       # Contain the latest value gotten by the client
     _last_value_dt: Optional[datetime]  # Datetime of the last value update by the client
     _last_write_dt: Optional[datetime]  # Datetime of the last completed write on this element
     _update_counter: int    # A counter that gets incremented each time the value is updated
 
     def __init__(self, client: "ScrutinyClient", display_path: str) -> None:
@@ -51,23 +53,28 @@
         self._update_counter = 0
         self._set_invalid(ValueStatus.NeverSet)
 
     def __repr__(self) -> str:
         addr = "0x%0.8x" % id(self)
         return f'<{self.__class__.__name__} "{self._shortname}" [{self._datatype.name}] at {addr}>'
 
-    def _configure(self, watchable_type: WatchableType, datatype: EmbeddedDataType, server_id: str) -> None:
+    def _configure(self, 
+                   watchable_type: WatchableType, 
+                   datatype: EmbeddedDataType, 
+                   server_id: str,
+                   enum:Optional[EmbeddedEnum] = None) -> None:
         with self._lock:
             self._watchable_type = watchable_type
             self._datatype = datatype
             self._server_id = server_id
             self._status = ValueStatus.NeverSet
             self._value = None
             self._last_value_dt = None
             self._update_counter = 0
+            self._enum = enum
 
     def _set_last_write_datetime(self, dt: Optional[datetime] = None) -> None:
         if dt is None:
             dt = datetime.now()
 
         with self._lock:
             self._last_write_dt = dt
@@ -101,21 +108,27 @@
             val_status = self._status
 
         if val is None or val_status != ValueStatus.Valid:
             raise sdk_exceptions.InvalidValueError(f"Value of {self._shortname} is unusable. {val_status._get_error()}")
 
         return val
 
-    def _write(self, val: ValType) -> WriteRequest:
+    def _write(self, val: Union[ValType, str]) -> WriteRequest:
+        if isinstance(val, str):
+            val = self.parse_enum_val(val)  # check for enum is done inside this
         write_request = WriteRequest(self, val)
         self._client._process_write_request(write_request)
         if not self._client._is_batch_write_in_progress():
             write_request.wait_for_completion()
         return write_request
 
+    def _assert_has_enum(self) -> None:
+        if not self.has_enum():
+            raise sdk_exceptions.BadEnumError(f"Watchable {self._shortname} has no enum defined")
+
     def unwatch(self) -> None:
         """Stop watching this item by unsubscribing to the server
 
         :raise NameNotFoundError: If the required path is not presently being watched
         :raise OperationFailure: If the subscription cancellation failed in any way
         """
         self._client.unwatch(self._display_path)
@@ -147,15 +160,15 @@
                 raise sdk_exceptions.InvalidValueError(self._status._get_error())
 
             if entry_counter != self._update_counter:
                 break
 
             time.sleep(sleep_interval)
 
-    def wait_value(self, value: ValType, timeout: float, sleep_interval: float = 0.02) -> None:
+    def wait_value(self, value: Union[ValType, str], timeout: float, sleep_interval: float = 0.02) -> None:
         """ 
         Wait for the watchable to reach a given value. Raises an exception if it does not happen within a timeout value
 
         :param value: The value that this watchable must have to exit the wait state
         :param timeout: Maximum amount of time to wait for the given value
         :param sleep_interval: Value passed to ``time.sleep`` while waiting
 
@@ -164,33 +177,66 @@
         :raise InvalidValueError: If the watchable becomes invalid while waiting
         :raise TimeoutException: If the watchable value never changes for the given value within the given timeout
         """
 
         timeout = validation.assert_float_range(timeout, 'timeout', minval=0)
         sleep_interval = validation.assert_float_range(sleep_interval, 'timeout', minval=0)
 
+        if isinstance(value, str):
+            value = self.parse_enum_val(value)
+
         if value < 0 and not self.datatype.is_signed():
             raise ValueError(f"{self._shortname} is unsigned and will never have a negative value as requested")
 
         t1 = time.monotonic()
         while True:
             if time.monotonic() - t1 > timeout:
-                raise sdk_exceptions.TimeoutException(f'Value of {self._shortname} did set to {value} in {timeout}s')
+                raise sdk_exceptions.TimeoutException(f'Value of {self._shortname} did not set to {value} in {timeout}s')
 
             if self.datatype.is_float():
                 if float(value) == self.value_float:
                     break
             elif self.datatype.is_integer():
                 if int(value) == self.value_int:
                     break
             elif self.datatype == EmbeddedDataType.boolean:
                 if bool(value) == self.value_bool:
                     break
 
             time.sleep(sleep_interval)
+    
+    def has_enum(self) -> bool:
+        """Tells if the watchable has an enum associated with it"""
+        return self._enum is not None
+    
+    def get_enum(self) -> EmbeddedEnum:
+        """ Returns the enum associated with this watchable
+
+        :raises BadEnumError: If the watchable has no enum assigned
+        """
+        self._assert_has_enum()
+        assert self._enum is not None
+        return self._enum.copy()
+    
+    def parse_enum_val(self, val:str) -> int:
+        """Converts an enum value name (string) to the underlying integer value
+
+        :param val: The enumerator name to convert
+
+        :raises BadEnumError: If the watchable has no enum assigned or the given value is not a valid enumerator
+        :raise TypeError: Given parameter not of the expected type
+        """
+        validation.assert_type(val, 'val', str)
+        self._assert_has_enum()
+        assert self._enum is not None
+        if not self._enum.has_value(val):
+            raise sdk_exceptions.BadEnumError(f"Value {val} is not a valid value for enum {self._enum.name}")
+        
+        return self._enum.get_value(val)
+
 
     @property
     def display_path(self) -> str:
         """Contains the watchable full tree path"""
         return self._display_path
 
     @property
@@ -206,15 +252,15 @@
     @property
     def datatype(self) -> EmbeddedDataType:
         """The data type of the device element pointed by this watchable. (sint16, float32, etc.)"""
         return self._datatype
 
     @property
     def value(self) -> ValType:
-        """The last value received for this watchable"""
+        """The last value received for this watchable. Can be written"""
         return self._read()
 
     @value.setter
     def value(self, val: ValType) -> None:
         self._write(val)
 
     @property
@@ -227,14 +273,30 @@
         """The value casted as int"""
         return int(self.value)
 
     @property
     def value_float(self) -> float:
         """The value casted as float"""
         return float(self.value)
+    
+    @property
+    def value_enum(self) -> str:
+        """The value converted to its first enum name (alphabetical order). Returns a string. Can be written with a string"""
+        val_int = self.value_int
+        self._assert_has_enum()
+        assert self._enum is not None
+        for k in sorted(self._enum.vals.keys()):
+            if self._enum.vals[k] == val_int:
+                return k
+        raise sdk_exceptions.InvalidValueError(f"Watchable {self._shortname} has value {val_int} which is not a valid enum value for enum {self._enum.name}")
+
+    @value_enum.setter
+    def value_enum(self, val: str) -> None:
+        # This setter only exists because mypy does not handle getter/setter with different signature. See issue #3004
+        self._write(val)
 
     @property
     def last_update_timestamp(self) -> Optional[datetime]:
         """Time of the last value update. ``None`` if not updated at least once. Not reliable for change detection"""
         return self._last_value_dt
 
     @property
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/sdk/write_request.py` & `scrutinydebugger-0.3.0/scrutiny/sdk/write_request.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/active_sfd_handler.py` & `scrutinydebugger-0.3.0/scrutiny/server/active_sfd_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,18 @@
 from scrutiny.server.datastore.datastore_entry import EntryType
 from scrutiny.server.device.device_handler import DeviceHandler
 from scrutiny.server.datastore.datastore import Datastore
 from scrutiny.server.datastore.datastore_entry import *
 from scrutiny.server.datastore.entry_type import EntryType
 
 from typing import Optional, List, Callable
-from scrutiny.core.typehints import GenericCallback
 
 
-class SFDLoadedCallback(GenericCallback):
-    callback: Callable[[FirmwareDescription], None]
-
-
-class SFDUnloadedCallback(GenericCallback):
-    callback: Callable[[None], None]
-
+SFDLoadedCallback = Callable[[FirmwareDescription], None]
+SFDUnloadedCallback = Callable[[], None]
 
 class ActiveSFDHandler:
     """
     Handle which Scrutiny Firmware Description file (SFD) is loaded. Automatically load one
     when the DeviceHandler connects to a device and the device broadcast a firmware ID associated with 
     an installed SFD.
 
@@ -142,15 +136,15 @@
                     self.datastore.add_entry(entry_alias)
                 except Exception as e:
                     self.logger.warning('Cannot add entry "%s". %s' % (fullname, str(e)))
                     self.logger.debug(traceback.format_exc())
 
             for callback in self.loaded_callbacks:
                 try:
-                    callback.__call__(self.sfd)
+                    callback(self.sfd)
                 except Exception as e:
                     self.logger.critical('Error in SFD Load callback. %s' % str(e))
                     self.logger.debug(traceback.format_exc())
 
         else:
             if verbose:
                 self.logger.warning('No SFD file installed for device with firmware ID %s' % firmware_id)
@@ -167,11 +161,11 @@
         # We only clear the entry types coming from the SFD. (i.e. no RPV)
         self.datastore.clear(EntryType.Alias)
         self.datastore.clear(EntryType.Var)
         if must_call_callback:
             self.logger.debug('Triggering SFD Unload callback')
             for callback in self.unloaded_callbacks:
                 try:
-                    callback.__call__()
+                    callback()
                 except Exception as e:
                     self.logger.critical('Error in SFD Unload callback. %s' % str(e))
                     self.logger.debug(traceback.format_exc())
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/api/API.py` & `scrutinydebugger-0.3.0/scrutiny/server/api/API.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from dataclasses import dataclass
 import functools
 from uuid import uuid4
 from fnmatch import fnmatch
 import itertools
 from base64 import b64encode, b64decode
 import binascii
+import threading
 
 from scrutiny.server.datalogging.datalogging_storage import DataloggingStorage
 from scrutiny.server.datalogging.datalogging_manager import DataloggingManager
 from scrutiny.server.datastore.datastore import Datastore
 from scrutiny.server.datastore.datastore_entry import EntryType, DatastoreEntry, UpdateTargetRequestCallback
 from scrutiny.server.device.device_handler import DeviceHandler, DeviceStateChangedCallback, RawMemoryReadRequestCompletionCallback, \
     RawMemoryReadRequest, RawMemoryWriteRequestCompletionCallback, RawMemoryWriteRequest, UserCommandCallback
@@ -30,39 +31,35 @@
 from scrutiny.core.basic_types import EmbeddedDataType
 from scrutiny.core.firmware_description import FirmwareDescription
 import scrutiny.server.datalogging.definitions.api as api_datalogging
 import scrutiny.server.datalogging.definitions.device as device_datalogging
 from scrutiny.server.device.device_info import ExecLoopType
 from scrutiny.core.basic_types import MemoryRegion
 import scrutiny.core.datalogging as core_datalogging
+from scrutiny.core.typehints import EmptyDict
 
 
 from .websocket_client_handler import WebsocketClientHandler
 from .dummy_client_handler import DummyClientHandler
 from .value_streamer import ValueStreamer
 import scrutiny.server.api.typing as api_typing
 
 from .abstract_client_handler import AbstractClientHandler, ClientHandlerMessage
 from scrutiny.server.device.links.abstract_link import LinkConfig as DeviceLinkConfig
 
-from scrutiny.core.typehints import EmptyDict, GenericCallback
 from typing import List, Dict, Set, Optional, Callable, Any, TypedDict, cast, Generator, Literal, Type
 
 
 class APIConfig(TypedDict, total=False):
     client_interface_type: str
     client_interface_config: Any
 
 
-class UpdateVarCallback(GenericCallback):
-    callback: Callable[[str, DatastoreEntry], None]
-
-
-class TargetUpdateCallback(GenericCallback):
-    callback: Callable[[str, DatastoreEntry], None]
+UpdateVarCallback = Callable[[str, DatastoreEntry], None]
+TargetUpdateCallback = Callable[[str, DatastoreEntry], None]
 
 
 class InvalidRequestException(Exception):
     def __init__(self, req:Any, msg:str) -> None:
         super().__init__(msg)
         self.req = req
 
@@ -276,21 +273,22 @@
 
     def __init__(self,
                  config: APIConfig,
                  datastore: Datastore,
                  device_handler: DeviceHandler,
                  sfd_handler: ActiveSFDHandler,
                  datalogging_manager: DataloggingManager,
-                 enable_debug: bool = False):
+                 enable_debug: bool = False,
+                 rx_event:Optional[threading.Event]=None):
         self.validate_config(config)
 
         if config['client_interface_type'] == 'websocket':
-            self.client_handler = WebsocketClientHandler(config['client_interface_config'])
+            self.client_handler = WebsocketClientHandler(config['client_interface_config'], rx_event=rx_event)
         elif config['client_interface_type'] == 'dummy':
-            self.client_handler = DummyClientHandler(config['client_interface_config'])
+            self.client_handler = DummyClientHandler(config['client_interface_config'], rx_event=rx_event)
         else:
             raise NotImplementedError('Unsupported client interface type. %s', config['client_interface_type'])
 
         self.datastore = datastore
         self.device_handler = device_handler
         self.sfd_handler = sfd_handler
         self.datalogging_manager = datalogging_manager
@@ -303,17 +301,17 @@
         self.enable_debug = enable_debug
 
         if enable_debug:
             import ipdb # type: ignore
             API.Command.Client2Api.DEBUG = 'debug'
             self.ApiRequestCallbacks[API.Command.Client2Api.DEBUG] = 'process_debug'
 
-        self.sfd_handler.register_sfd_loaded_callback(SFDLoadedCallback(self.sfd_loaded_callback))
-        self.sfd_handler.register_sfd_unloaded_callback(SFDUnloadedCallback(self.sfd_unloaded_callback))
-        self.device_handler.register_device_state_change_callback(DeviceStateChangedCallback(self.device_state_changed_callback))
+        self.sfd_handler.register_sfd_loaded_callback(self.sfd_loaded_callback)
+        self.sfd_handler.register_sfd_unloaded_callback(self.sfd_unloaded_callback)
+        self.device_handler.register_device_state_change_callback(self.device_state_changed_callback)
 
     @classmethod
     def get_datatype_name(cls, datatype: EmbeddedDataType) -> str:
         if datatype not in cls.DATATYPE_2_APISTR:
             raise ValueError('Unknown datatype : %s' % (str(datatype)))
 
         return cls.DATATYPE_2_APISTR[datatype]
@@ -422,16 +420,16 @@
 
             if not isinstance(cmd, str):
                 raise InvalidRequestException(req, 'cmd is not a valid string')
 
             # Fetch the right function from a global dict and call it
             # Response are sent in each callback. Not all requests requires a response
             if cmd in self.ApiRequestCallbacks:
-                callback = getattr(self, self.ApiRequestCallbacks[cmd])
-                callback.__call__(conn_id, req)
+                callback = cast(Callable[[str, api_typing.C2SMessage], None], getattr(self, self.ApiRequestCallbacks[cmd]))
+                callback(conn_id, req)
             else:
                 raise InvalidRequestException(req, 'Unsupported command %s' % cmd)
 
         except InvalidRequestException as e:
             # Client sent a bad request. Controlled error
             self.logger.debug('[Conn:%s] Invalid request #%d. %s' % (conn_id, self.req_count, str(e)))
             response = self.make_error_response(req, str(e))
@@ -595,22 +593,25 @@
             try:
                 entry = self.datastore.get_entry_by_display_path(path)  # Will raise an exception if not existent
                 subscribed[path] = {
                     'type': self.ENTRY_TYPE_2_APISTR[entry.get_type()],
                     'datatype': self.DATATYPE_2_APISTR[entry.get_data_type()],
                     'id': entry.get_id()
                 }
+                if entry.has_enum():
+                    subscribed[path]['enum'] = entry.get_enum().get_def()
+
             except KeyError as e:
                 raise InvalidRequestException(req, 'Unknown watchable : %s' % str(path))
 
         for path in req['watchables']:
             self.datastore.start_watching(
                 entry_id=subscribed[path]['id'],
                 watcher=conn_id,    # We use the API connection ID as datastore watcher ID
-                value_change_callback=UpdateVarCallback(self.entry_value_change_callback)
+                value_change_callback=self.entry_value_change_callback
             )
 
         response: api_typing.S2C.SubscribeWatchable = {
             'cmd': self.Command.Api2Client.SUBSCRIBE_WATCHABLE_RESPONSE,
             'reqid': self.get_req_id(req),
             'subscribed': subscribed
         }
@@ -866,15 +867,15 @@
                 raise InvalidRequestException(req, 'Cannot update entry %s without being subscribed to it' % entry.get_id())
 
         if len(set(update['batch_index'] for update in req['updates'])) != len(req['updates']):
             raise InvalidRequestException(req, "Duplicate batch_index in request")
 
         request_token = uuid4().hex
         for update in req['updates']:
-            callback = UpdateTargetRequestCallback(functools.partial(self.entry_target_update_callback, request_token, update['batch_index']))
+            callback = functools.partial(self.entry_target_update_callback, request_token, update['batch_index'])
             self.datastore.update_target_value(update['watchable'], update['value'], callback=callback)
 
         response: api_typing.S2C.WriteValue = {
             'cmd': self.Command.Api2Client.WRITE_WATCHABLE_RESPONSE,
             'reqid': self.get_req_id(req),
             'request_token': request_token,
             'count': len(req['updates'])
@@ -900,15 +901,15 @@
 
         if req['size'] <= 0:
             raise InvalidRequestException(req, '"size" field is not valid')
 
         request_token = uuid4().hex
         callback = functools.partial(self.read_raw_memory_callback, request_token=request_token, conn_id=conn_id)
 
-        self.device_handler.read_memory(req['address'], req['size'], callback=RawMemoryReadRequestCompletionCallback(callback))
+        self.device_handler.read_memory(req['address'], req['size'], callback=callback)
 
         response: api_typing.S2C.ReadMemory = {
             'cmd': self.Command.Api2Client.READ_MEMORY_RESPONSE,
             'reqid': self.get_req_id(req),
             'request_token': request_token
         }
 
@@ -937,15 +938,15 @@
 
         if len(data) <= 0:
             raise InvalidRequestException(req, '"data" field is not valid')
 
         request_token = uuid4().hex
         callback = functools.partial(self.write_raw_memory_callback, request_token=request_token, conn_id=conn_id)
 
-        self.device_handler.write_memory(req['address'], data, callback=RawMemoryWriteRequestCompletionCallback(callback))
+        self.device_handler.write_memory(req['address'], data, callback=callback)
 
         response: api_typing.S2C.WriteMemory = {
             'cmd': self.Command.Api2Client.WRITE_MEMORY_RESPONSE,
             'reqid': self.get_req_id(req),
             'request_token': request_token
         }
 
@@ -1276,15 +1277,15 @@
 
         # We use a partial func to pass the request token and conn id
         request_token = uuid4().hex
         callback = functools.partial(self.datalogging_acquisition_completion_callback, conn_id, request_token)
 
         self.datalogging_manager.request_acquisition(
             request=acq_req,
-            callback=api_datalogging.APIAcquisitionRequestCompletionCallback(callback)
+            callback=callback
         )
 
         response: api_typing.S2C.RequestDataloggingAcquisition = {
             'cmd': API.Command.Api2Client.REQUEST_DATALOGGING_ACQUISITION_RESPONSE,
             'reqid': self.get_req_id(req),
             'request_token': request_token
         }
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/api/abstract_client_handler.py` & `scrutinydebugger-0.3.0/scrutiny/server/api/abstract_client_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 #   - Project :  Scrutiny Debugger (github.com/scrutinydebugger/scrutiny-python)
 #
 #   Copyright (c) 2021 Scrutiny Debugger
 
 from abc import abstractmethod
 from typing import Dict, Optional, Union
 from dataclasses import dataclass
+import threading
 
 import scrutiny.server.api.typing as api_typing
 
 ClientHandlerConfig = Dict[str, str]
 
 
 @dataclass
@@ -20,15 +21,15 @@
     conn_id: str
     obj: Union[api_typing.C2SMessage, api_typing.S2CMessage]
 
 
 class AbstractClientHandler:
 
     @abstractmethod
-    def __init__(self, config: ClientHandlerConfig):
+    def __init__(self, config: ClientHandlerConfig, rx_event:Optional[threading.Event]=None):
         pass
 
     @abstractmethod
     def send(self, msg: ClientHandlerMessage) -> None:
         pass
 
     @abstractmethod
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/api/dummy_client_handler.py` & `scrutinydebugger-0.3.0/scrutiny/server/api/dummy_client_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -88,25 +88,30 @@
     txqueue: "queue.Queue[ClientHandlerMessage]"
     config: Dict[str, str]
     logger: logging.Logger
     stop_requested: bool
     connections: List[DummyConnection]
     connection_map: Dict[str, DummyConnection]
     started: bool
+    rx_event:Optional[threading.Event]
 
-    def __init__(self, config: ClientHandlerConfig) -> None:
+    def __init__(self, 
+                 config: ClientHandlerConfig, 
+                 rx_event:Optional[threading.Event]=None
+                 ) -> None:
         self.rxqueue = queue.Queue()
         self.txqueue = queue.Queue()
         self.config = config
         self.logger = logging.getLogger(self.__class__.__name__)
         self.stop_requested = False
         self.validate_config(config)
         self.connection_map = {}
         self.connections = []
         self.started = False
+        self.rx_event=rx_event
 
     def set_connections(self, connections: List[DummyConnection]) -> None:
         self.connections = connections
         for conn in self.connections:
             self.connection_map[conn.get_id()] = conn
 
     def validate_config(self, config: ClientHandlerConfig) -> None:
@@ -131,14 +136,16 @@
                     while conn.from_client_available():
                         msg = conn.read_from_client()
                         if msg is not None:
                             try:
                                 self.logger.debug('Received from ID %s. "%s"' % (conn.get_id(), msg))
                                 obj = json.loads(msg)
                                 self.rxqueue.put(ClientHandlerMessage(conn_id=conn.get_id(), obj=obj))
+                                if self.rx_event is not None:
+                                    self.rx_event.set()
                             except Exception as e:
                                 self.logger.error('Received invalid msg.  %s' % str(e))
 
                 while not self.txqueue.empty():
                     container = self.txqueue.get()
                     if container is not None:
                         try:
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/api/typing.py` & `scrutinydebugger-0.3.0/scrutiny/server/api/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 #   - License : MIT - See LICENSE file.
 #   - Project :  Scrutiny Debugger (github.com/scrutinydebugger/scrutiny-python)
 #
 #   Copyright (c) 2021 Scrutiny Debugger
 
 from typing import TypedDict, Optional, List, Dict, Union, Literal, Any
 from scrutiny.core.typehints import EmptyDict
-from enum import Enum
 
 import scrutiny.core.firmware_description
+from scrutiny.core.embedded_enum import EmbeddedEnumDef
 import scrutiny.server.device.links.serial_link
 import scrutiny.server.device.links.udp_link
 
 WatchableType = Literal['alias', 'var', 'rpv']
 # Mapping between app type and API type.
 SFDMetadata = scrutiny.core.firmware_description.MetadataType
 SerialLinkConfig = scrutiny.server.device.links.serial_link.SerialConfig
 UdpLinkConfig = scrutiny.server.device.links.udp_link.UdpConfig
 LinkConfig = Union[EmptyDict, UdpLinkConfig, SerialLinkConfig]
-LinkType = Literal['none', 'udp', 'serial', 'dummy', 'thread_safe_dummy']
+LinkType = Literal['none', 'udp', 'serial', 'dummy']
 SupportedFeature = Literal['memory_write', 'datalogging', 'user_command', '_64bits']
 Datatype = Literal[
     'sint8', 'sint16', 'sint32', 'sint64', 'sint128', 'sint256',
     'uint8', 'uint16', 'uint32', 'uint64', 'uint128', 'uint256',
     'float8', 'float16', 'float32', 'float64', 'float128', 'float256',
     'cfloat8', 'cfloat16', 'cfloat32', 'cfloat64', 'cfloat128', 'cfloat256',
     'boolean'
@@ -174,17 +174,18 @@
 
 
 class AxisNameUpdateEntry(TypedDict):
     id: int
     name: str
 
 
-class SubscribedInfo(TypedDict):
+class SubscribedInfo(TypedDict, total=False):
     type: WatchableType
     datatype: Datatype
+    enum: EmbeddedEnumDef
     id: str
 
 
 class C2S:
     "Client To Server"
     class Echo(BaseC2SMessage):
         payload: str
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/api/value_streamer.py` & `scrutinydebugger-0.3.0/scrutiny/server/api/value_streamer.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/api/websocket_client_handler.py` & `scrutinydebugger-0.3.0/scrutiny/server/api/websocket_client_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 #   - Project :  Scrutiny Debugger (github.com/scrutinydebugger/scrutiny-python)
 #
 #   Copyright (c) 2021 Scrutiny Debugger
 
 import uuid
 import logging
 import json
+import threading
 
 from scrutiny.server.api.abstract_client_handler import AbstractClientHandler, ClientHandlerConfig, ClientHandlerMessage
 from scrutiny.tools.synchronous_websocket_server import SynchronousWebsocketServer
 
 from typing import Dict, Any, Optional
-from scrutiny.core.typehints import GenericCallback
 
 # WebsocketType = websockets.server.WebSocketServerProtocol
 WebsocketType = Any  # todo fix this
 
 
 class WebsocketClientHandler(AbstractClientHandler):
     """
@@ -32,22 +32,29 @@
     config: ClientHandlerConfig
     logger: logging.Logger
     id2ws_map: Dict[str, WebsocketType]
     ws2id_map: Dict[WebsocketType, str]
     port: Optional[int]
     force_silent: bool  # For unit testing of timeouts
 
-    def __init__(self, config: ClientHandlerConfig):
+    def __init__(self, 
+                 config: ClientHandlerConfig, 
+                 rx_event:Optional[threading.Event]=None
+                 ) -> None:
         self.config = config
         self.logger = logging.getLogger(self.__class__.__name__)
         self.id2ws_map = dict()
         self.ws2id_map = dict()
         self.force_silent = False
-        self.server = SynchronousWebsocketServer(connect_callback=GenericCallback(
-            self.register), disconnect_callback=GenericCallback(self.unregister))
+        self.server = SynchronousWebsocketServer(
+            connect_callback=self.register, 
+            disconnect_callback=self.unregister,
+            rx_event=rx_event
+            )
+        self.rx_event=rx_event
 
     def register(self, websocket: WebsocketType) -> None:
         # Callback on new websocket connection.  We make a unique ID for each object.
         wsid = self.make_id()
         self.id2ws_map[wsid] = websocket
         self.ws2id_map[websocket] = wsid
         self.logger.info('New client connected (ID=%s). %d clients total' % (wsid, len(self.ws2id_map)))
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/datalogging/datalogging_manager.py` & `scrutinydebugger-0.3.0/scrutiny/server/datalogging/datalogging_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
                         if self.device_handler.is_ready_for_datalogging_acquisition_request():
                             self.active_request = self.acquisition_request_queue.get()
                             # We rely on the device handler to call our callback regardless
                             # of what will happen. Success, failure, error, external reset.
                             self.device_handler.request_datalogging_acquisition(
                                 loop_id=self.active_request.api_request.rate_identifier,
                                 config=self.active_request.device_config,
-                                callback=DeviceAcquisitionRequestCompletionCallback(self.acquisition_complete_callback)
+                                callback=self.acquisition_complete_callback
                             )
                         else:
                             # Cause of not ready:
                             # - not started : Device status will not be CONNECTED_READY, will exit cleanly
                             # - setup not completed : not possible as we waited on this before going here
                             # - error : Condition for that, will go to CLEAR_ERROR
                             # - cancel_requested : We wait until cancel is completed and active_request is set to None by the callback
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/datalogging/datalogging_storage.py` & `scrutinydebugger-0.3.0/scrutiny/server/datalogging/datalogging_storage.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/datalogging/datalogging_utilities.py` & `scrutinydebugger-0.3.0/scrutiny/server/datalogging/datalogging_utilities.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/datalogging/definitions/api.py` & `scrutinydebugger-0.3.0/scrutiny/server/datalogging/definitions/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,14 @@
 
 from scrutiny.core.datalogging import DataloggingAcquisition, AxisDefinition
 from scrutiny.server.device.device_info import ExecLoopType
 from scrutiny.server.datastore.datastore_entry import DatastoreEntry
 import scrutiny.server.datalogging.definitions.device as device_datalogging
 from typing import List, Optional, Callable, Union, Set
 
-from scrutiny.core.typehints import GenericCallback
-
-
 class XAxisType(Enum):
     """Represent a type of X-Axis that a user can select"""
     IdealTime = 0,
     MeasuredTime = 1,
     Signal = 2,
     Indexed = 3
 
@@ -47,17 +44,15 @@
     """Represent a sampling rate that a use can select"""
     name: str
     frequency: Optional[float]
     rate_type: ExecLoopType
     device_identifier: int
 
 
-class APIAcquisitionRequestCompletionCallback(GenericCallback):
-    callback: Callable[[bool, str, Optional[DataloggingAcquisition]], None]
-
+APIAcquisitionRequestCompletionCallback = Callable[[bool, str, Optional[DataloggingAcquisition]], None]
 
 TriggerConditionID = device_datalogging.TriggerConditionID
 
 
 class TriggerConditionOperandType(Enum):
     LITERAL = 0
     WATCHABLE = 1
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/datalogging/definitions/device.py` & `scrutinydebugger-0.3.0/scrutiny/server/datalogging/definitions/device.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/datastore/datastore.py` & `scrutinydebugger-0.3.0/scrutiny/server/datastore/datastore.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,17 @@
 #   Copyright (c) 2021 Scrutiny Debugger
 
 import logging
 import functools
 from scrutiny.server.datastore.datastore_entry import *
 from scrutiny.server.datastore.entry_type import EntryType
 
-from scrutiny.core.typehints import GenericCallback
-
 from typing import Callable, List, Dict, Generator, Set, List, Optional, Union, Any
 
-
-class WatchCallback(GenericCallback):
-    callback: Callable[[str], None]     # str is the owner
-
+WatchCallback = Callable[[str], None]
 
 class Datastore:
     """
     Class at the center of the server. It contains the value of all watched items.
     the device handler writes variable and RPV (Runtime Published Values) into the datastore
     and the user subscribe to value change by setting a callback in the datastore through the API.
 
@@ -130,50 +125,45 @@
 
     def add_unwatch_callback(self, callback: WatchCallback) -> None:
         self.global_unwatch_callbacks.append(callback)
 
     def start_watching(self,
                        entry_id: Union[DatastoreEntry, str],
                        watcher: str,
-                       value_change_callback: Optional[GenericCallback] = None,
-                       target_update_callback: Optional[GenericCallback] = None
+                       value_change_callback: Optional[UserValueChangeCallback] = None,
+                       target_update_callback: Optional[UpdateTargetRequestCallback] = None
                        ) -> None:
         """ 
         Register a new callback on the entry identified by the given entry_id.
         The watcher parameter will be given back when calling the callback.
         We ensure to call the callback for each watcher.
         """
 
-        if value_change_callback is None:   # No callback mainly happens with unit tests
-            value_change_callback = GenericCallback(lambda *args, **kwargs: None)
-
-        if target_update_callback is None:  # No callback mainly happens with unit tests
-            target_update_callback = GenericCallback(lambda *args, **kwargs: None)
-
         entry_id = self.interpret_entry_id(entry_id)
         entry = self.get_entry(entry_id)
 
         if entry_id not in self.watcher_map[entry.get_type()]:
             self.watcher_map[entry.get_type()][entry.get_id()] = set()
         self.watcher_map[entry.get_type()][entry_id].add(watcher)
 
         if not entry.has_value_change_callback(watcher):
-            entry.register_value_change_callback(owner=watcher, callback=value_change_callback)
+            if value_change_callback is not None:
+                entry.register_value_change_callback(owner=watcher, callback=value_change_callback)
 
         # Mainly used to notify device handler that a new variable is to be polled
         for callback in self.global_watch_callbacks:
             callback(entry_id)
 
         if isinstance(entry, DatastoreAliasEntry):
             # Alias are tricky. When we subscribe to them, another hidden subscription to the referenced entry is made here
             alias_value_change_callback = functools.partial(self.alias_value_change_callback, watching_entry=entry)
             self.start_watching(
                 entry_id=entry.resolve(),
                 watcher=self.make_owner_from_alias_entry(entry),
-                value_change_callback=GenericCallback(alias_value_change_callback)
+                value_change_callback=alias_value_change_callback
             )
 
     def is_watching(self, entry: Union[DatastoreEntry, str], watcher: str) -> bool:
         """ Tell if the given watcher is actually watching an entry"""
         entry_id = self.interpret_entry_id(entry)
         entry = self.get_entry(entry_id)
         if entry_id not in self.watcher_map[entry.get_type()]:
@@ -255,15 +245,15 @@
             entry = entry_id
         else:
             entry = self.get_entry(entry_id)
         update_request = UpdateTargetRequest(value, entry=entry, callback=callback)
 
         if isinstance(entry, DatastoreAliasEntry):
             new_value = entry.aliasdef.compute_user_to_device(value)
-            nested_callback = UpdateTargetRequestCallback(functools.partial(self.alias_target_update_callback, update_request))
+            nested_callback = functools.partial(self.alias_target_update_callback, update_request)
             new_request = self.update_target_value(entry.resolve(), new_value, callback=nested_callback)
             if new_request.is_complete():  # Edge case if failed to enqueue request.
                 new_request.complete(success=update_request.is_complete())
             return update_request
         else:
             self.target_update_request_queue.append(update_request)
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/datastore/datastore_entry.py` & `scrutinydebugger-0.3.0/scrutiny/server/datastore/datastore_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,61 +9,60 @@
 __all__ = [
     'EntryType',
     'DatastoreEntry',
     'DatastoreVariableEntry',
     'DatastoreAliasEntry',
     'DatastoreRPVEntry',
     'UpdateTargetRequestCallback',
-    'UpdateTargetRequest'
+    'UpdateTargetRequest',
+    'UserValueChangeCallback'
 ]
 
 import uuid
 import time
 import abc
 import re
 from scrutiny.core.basic_types import RuntimePublishedValue
 import queue
 
 from scrutiny.server.datastore.entry_type import EntryType
 from scrutiny.core.basic_types import EmbeddedDataType, Endianness
-from scrutiny.core.variable import Variable, VariableEnum
+from scrutiny.core.variable import Variable
+from scrutiny.core.embedded_enum import EmbeddedEnum
 from scrutiny.core.codecs import *
 
-from scrutiny.core.typehints import GenericCallback
 from scrutiny.core.alias import Alias
 from typing import Any, Optional, Dict, Callable, Tuple, Union
 
 
-class ValueChangeCallback():
+
+UpdateTargetRequestCallback = Callable[[bool, 'DatastoreEntry', float], None]   # callback(success, entry, timestamp)
+UserValueChangeCallback = Callable[[str, "DatastoreEntry"], None]
+
+class ValueChangeCallbackInstance:
     """
     Callback object that ties a function and a owner ID.
     Is assigned to watched datastore entry so the watcher can be notified.
     """
-    fn: GenericCallback
+    fn: UserValueChangeCallback
     owner: str
     args: Any
 
-    def __init__(self, fn: GenericCallback, owner: str) -> None:
+    def __init__(self, fn: Callable[..., None], owner: str) -> None:
         if not callable(fn):
             raise ValueError('callback must be a callable')
 
         if owner is None:
             raise ValueError('Invalid owner for callback')
 
         self.fn = fn
         self.owner = owner
 
     def __call__(self, *args: Any, **kwargs: Any) -> None:
-        self.fn.__call__(self.owner, *args, **kwargs)
-
-
-class UpdateTargetRequestCallback(GenericCallback):
-    """Callback to call when a target update request completes"""
-    fn: Callable[[bool, 'DatastoreEntry', float], None]
-
+        self.fn(self.owner, *args, **kwargs)
 
 class UpdateTargetRequest:
     """
     Represent a request to write an entry in the target device.
     Once this request is completed and successful, the datastore can be updated.
     """
     value: Any
@@ -155,15 +154,15 @@
 
     @abc.abstractmethod
     def has_enum(self) -> bool:
         """Returns True if the entry has an enum"""
         raise NotImplementedError("Abstract method")
 
     @abc.abstractmethod
-    def get_enum(self) -> VariableEnum:
+    def get_enum(self) -> EmbeddedEnum:
         """Returns the enum attached to the entry. Raise an exception if there is None"""
         raise NotImplementedError("Abstract method")
 
     @abc.abstractmethod
     def encode(self, value: Encodable) -> Tuple[bytes, Optional[bytes]]:
         """Encode the value to a stream of bytes and a data mask. 
         Returns as tuple : (data, mask)"""
@@ -191,22 +190,22 @@
         self.set_value(self.decode(data))
 
     def execute_value_change_callback(self) -> None:
         """Run all the callbacks when the value is updated"""
         for owner in self.value_change_callback:
             self.value_change_callback[owner](self)
 
-    def register_value_change_callback(self, owner: str, callback: GenericCallback) -> None:
+    def register_value_change_callback(self, owner: str, callback: UserValueChangeCallback) -> None:
         """Add a callback to be called when this entry value changes"""
-        thecallback = ValueChangeCallback(fn=callback, owner=owner)
+        thecallback = ValueChangeCallbackInstance(fn=callback, owner=owner)
         if owner in self.value_change_callback:
             raise ValueError('This owner already has a callback registered')
         self.value_change_callback[owner] = thecallback
 
-    def unregister_value_change_callback(self, owner: Any) -> None:
+    def unregister_value_change_callback(self, owner: str) -> None:
         """Remove a callback on value change"""
         if owner in self.value_change_callback:
             del self.value_change_callback[owner]
 
     def has_value_change_callback(self, owner: Optional[str] = None) -> bool:
         """Tells if this entry has at least one callback for the given owner."""
         if owner is None:
@@ -267,15 +266,15 @@
         """Return the variable data size"""
         return self.variable_def.get_type().get_size_byte()
 
     def has_enum(self) -> bool:
         """Returns True if the entry has an enum"""
         return self.variable_def.has_enum()
 
-    def get_enum(self) -> VariableEnum:
+    def get_enum(self) -> EmbeddedEnum:
         """Returns the enum attached to the entry. Raise an exception if there is None"""
         enum = self.variable_def.get_enum()  # Possibly has no enum.
         assert enum is not None             # Should have checked with has_enum() first
         return enum
 
     def is_bitfield(self) -> bool:
         """Returns True if this variable is a bitfield"""
@@ -332,18 +331,22 @@
 
     def get_data_type(self) -> EmbeddedDataType:
         """Return the datastore entry type"""
         return self.refentry.get_data_type()    # Variable datatype
 
     def has_enum(self) -> bool:
         """Returns True if the entry has an enum"""
+        if self.aliasdef.enum is not None:
+            return True
         return self.refentry.has_enum()
 
-    def get_enum(self) -> VariableEnum:
+    def get_enum(self) -> EmbeddedEnum:
         """Returns the enum attached to the entry. Raise an exception if there is None"""
+        if self.aliasdef.enum is not None:
+            return self.aliasdef.enum
         return self.refentry.get_enum()
 
     def encode(self, value: Encodable) -> Tuple[bytes, Optional[bytes]]:
         """Encode the value to a stream of bytes and a data mask. 
         Returns as tuple : (data, mask)"""
         return self.refentry.encode(value)
 
@@ -381,15 +384,14 @@
         val = val or self.aliasdef.gain is not None 
         val = val or self.aliasdef.offset is not None 
         val = val or self.aliasdef.max is not None 
         val = val or self.aliasdef.min is not None
         return val
 
 
-
 class DatastoreRPVEntry(DatastoreEntry):
     """A datastore entry that represents a Runtime Published Value"""
 
     rpv: RuntimePublishedValue
     codec: BaseCodec
 
     def __init__(self, display_path: str, rpv: RuntimePublishedValue):
@@ -405,15 +407,15 @@
         """Return the datastore entry type"""
         return self.rpv.datatype
 
     def has_enum(self) -> bool:
         """Returns True if the entry has an enum"""
         return False
 
-    def get_enum(self) -> VariableEnum:
+    def get_enum(self) -> EmbeddedEnum:
         """Returns the enum attached to the entry. Raise an exception if there is None"""
         raise NotImplementedError('RuntimePublishedValues does not have enums')
 
     def encode(self, value: Encodable) -> Tuple[bytes, Optional[bytes]]:
         """Encode the value to a stream of bytes and a data mask. 
         Returns as tuple : (data, mask)"""
         value = Codecs.make_value_valid(self.get_data_type(), value)
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/datastore/entry_type.py` & `scrutinydebugger-0.3.0/scrutiny/server/datastore/entry_type.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/device/device_handler.py` & `scrutinydebugger-0.3.0/scrutiny/server/device/device_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,50 +23,43 @@
 import logging
 import binascii
 import time
 from enum import Enum, auto
 import traceback
 from uuid import uuid4
 import math
+import threading
 from scrutiny.server.datastore.datastore_entry import DatastoreRPVEntry, EntryType
 import scrutiny.server.datalogging.definitions.device as device_datalogging
 from scrutiny.server.protocol import *
 import scrutiny.server.protocol.typing as protocol_typing
 from scrutiny.server.protocol.comm_handler import CommHandler
 from scrutiny.server.protocol.commands import DummyCommand
-from scrutiny.server.device.request_dispatcher import RequestDispatcher, RequestRecord, SuccessCallback, FailureCallback
+from scrutiny.server.device.request_dispatcher import RequestDispatcher, RequestRecord
 from scrutiny.server.device.submodules.device_searcher import DeviceSearcher
 from scrutiny.server.device.submodules.heartbeat_generator import HeartbeatGenerator
-from scrutiny.server.device.submodules.info_poller import InfoPoller, ProtocolVersionCallback, CommParamCallback
+from scrutiny.server.device.submodules.info_poller import InfoPoller
 from scrutiny.server.device.submodules.session_initializer import SessionInitializer
 from scrutiny.server.device.submodules.memory_reader import MemoryReader, RawMemoryReadRequestCompletionCallback, RawMemoryReadRequest
 from scrutiny.server.device.submodules.memory_writer import MemoryWriter, RawMemoryWriteRequestCompletionCallback, RawMemoryWriteRequest
 from scrutiny.server.device.submodules.datalogging_poller import DataloggingPoller, DeviceAcquisitionRequestCompletionCallback
 from scrutiny.server.device.device_info import DeviceInfo
-from scrutiny.tools import Timer
+from scrutiny.tools import Timer, update_dict_recursive
 from scrutiny.server.datastore.datastore import Datastore
 from scrutiny.server.device.links import AbstractLink, LinkConfig
 from scrutiny.core.firmware_id import PLACEHOLDER as DEFAULT_FIRMWARE_ID
 
 
 from typing import TypedDict, Optional, Callable, Any, Dict, cast, List
-from scrutiny.core.typehints import GenericCallback
 
 DEFAULT_FIRMWARE_ID_ASCII = binascii.hexlify(DEFAULT_FIRMWARE_ID).decode('ascii')
 """Default firmware ID assigned to a binary that uses libscrutiny-embedded without tagging the binary after compilation"""
 
-
-class DisconnectCallback(GenericCallback):
-    callback: Callable[[bool], None]
-
-
-class DeviceStateChangedCallback(GenericCallback):
-    callback: Callable[["DeviceHandler.ConnectionStatus"], None]
-
-
+DisconnectCallback = Callable[[bool], None]
+DeviceStateChangedCallback = Callable[["DeviceHandler.ConnectionStatus"], None]
 # callback(success, subfn, data, error_str) -> None
 UserCommandCallback = Callable[[bool, int, Optional[bytes], Optional[str]], None]
 
 
 class DeviceHandlerConfig(TypedDict, total=False):
     """DeviceHandler configuration in a dict format that can be loaded from a json file"""
 
@@ -92,15 +85,15 @@
     by the device if it broadcast a smaller limit"""
 
     max_bitrate_bps: int
     """Maximum bitrate to use on the device communication channel.
     This value can be overridden if the device requires a smaller value"""
 
     link_type: str
-    """The type of communication link to use to talk with a device. udp, serial, dummy, dummy_threadsafe, etc"""
+    """The type of communication link to use to talk with a device. udp, serial, dummy, etc"""
 
     link_config: LinkConfig
     """The configuration dictionary that will configure the communication link layer. 
     Unique for each type of link (udp, serial, etc)"""
 
 
 class DeviceHandler:
@@ -194,63 +187,71 @@
         DISCONNECTING = auto()
 
     class OperatingMode(Enum):
         """Tells the main function of the device handler. Modes different from Normal are meant for unit tests"""
         Normal = 0
         Test_CheckThrottling = 1
 
-    def __init__(self, config: DeviceHandlerConfig, datastore: Datastore):
+    def __init__(self, 
+                 config: DeviceHandlerConfig, 
+                 datastore: Datastore,
+                 rx_event:Optional[threading.Event] = None
+                 ):
         self.logger = logging.getLogger(self.__class__.__name__)
 
         self.config = copy.copy(self.DEFAULT_PARAMS)
-        self.config.update(config)
+        update_dict_recursive(self.config, config)  # type: ignore
         self.datastore = datastore
         self.dispatcher = RequestDispatcher()
         (major, minor) = self.config['default_protocol_version'].split('.')
         self.protocol = Protocol(int(major), int(minor))
         self.device_searcher = DeviceSearcher(self.protocol, self.dispatcher, priority=self.RequestPriority.Discover)
         self.session_initializer = SessionInitializer(self.protocol, self.dispatcher, priority=self.RequestPriority.Connect)
         self.heartbeat_generator = HeartbeatGenerator(self.protocol, self.dispatcher, priority=self.RequestPriority.Heartbeat)
         self.info_poller = InfoPoller(
             self.protocol,
             self.dispatcher,
             priority=self.RequestPriority.PollInfo,
-            protocol_version_callback=ProtocolVersionCallback(self.get_protocol_version_callback),  # Called when protocol version is polled
-            comm_param_callback=CommParamCallback(self.get_comm_params_callback),            # Called when communication params are polled
+            protocol_version_callback=self.get_protocol_version_callback,  # Called when protocol version is polled
+            comm_param_callback=self.get_comm_params_callback,            # Called when communication params are polled
         )
         self.datalogging_poller = DataloggingPoller(
             self.protocol,
             self.dispatcher,
             self.RequestPriority.Datalogging
         )
 
         self.memory_reader = MemoryReader(self.protocol, self.dispatcher, self.datastore,
                                           request_priority=self.RequestPriority.ReadMemory)
 
         self.memory_writer = MemoryWriter(self.protocol, self.dispatcher, self.datastore,
                                           request_priority=self.RequestPriority.WriteMemory)
 
         self.comm_handler = CommHandler(cast(Dict[str, Any], self.config))
+        if rx_event is not None:
+            self.comm_handler.set_rx_data_event(rx_event)
         self.comm_handler_open_restart_timer = Timer(1.0)
 
         self.heartbeat_generator.set_interval(max(0.5, self.config['heartbeat_timeout'] * 0.75))
         self.comm_broken = False
         self.device_id = None
         self.operating_mode = self.OperatingMode.Normal
         self.wait_clean_state_timestamp = time.monotonic()
         self.active_request_record = None
         self.device_state_changed_callbacks = []
         self.expect_no_timeout = False  # Unit tests will set this to True
+        
 
         if 'link_type' in self.config and 'link_config' in self.config:
             self.configure_comm(self.config['link_type'], self.config['link_config'])
 
         self.reset_comm()
 
     def register_device_state_change_callback(self, callback: DeviceStateChangedCallback) -> None:
+        """Register a callback to be called when the state of the device communication changes"""
         self.device_state_changed_callbacks.append(callback)
 
     def get_device_id(self) -> Optional[str]:
         """Returns the firmware ID of the connected device. None if not connected"""
         return self.device_id
 
     def set_operating_mode(self, mode: "DeviceHandler.OperatingMode") -> None:
@@ -356,16 +357,16 @@
                 subfn = cast(int, subfn.value)
 
             callback(False, subfn, None, "Failed to request the UserCommand with subfunction %s and %d bytes of data" %
                      (subfn, request.data_size()))
 
         self.dispatcher.register_request(
             request=self.protocol.user_command(subfn, data),
-            success_callback=SuccessCallback(success_callback),
-            failure_callback=FailureCallback(failure_callback),
+            success_callback=success_callback,
+            failure_callback=failure_callback,
             priority=self.RequestPriority.UserCommand
         )
 
     def get_comm_params_callback(self, partial_device_info: DeviceInfo) -> None:
         """Callback given to InfoPoller to be called whenever the GetParams command completes."""
         # In the POLLING_INFO stage, there is a point where we will have gotten the communication params.
         # This callback is called right after it so we can adapt.
@@ -571,17 +572,20 @@
         if self.operating_mode == self.OperatingMode.Normal:
             if state_entry:
                 self.memory_reader.start()
                 self.memory_writer.start()
             # Nothing else to do
         elif self.operating_mode == self.OperatingMode.Test_CheckThrottling:    # For unit tests
             if self.dispatcher.peek_next() is None:
-                dummy_request = Request(DummyCommand, subfn=1, payload=b'\x00' * 32, response_payload_size=32);
-                self.dispatcher.register_request(dummy_request, success_callback=SuccessCallback(
-                    lambda *args, **kwargs: None), failure_callback=FailureCallback(self.test_failure_callback))
+                dummy_request = Request(DummyCommand, subfn=1, payload=b'\x00' * 32, response_payload_size=32)
+                self.dispatcher.register_request(
+                    dummy_request, 
+                    success_callback=lambda *args, **kwargs: None, 
+                    failure_callback=self.test_failure_callback
+                    )
 
     def test_failure_callback(self, request: Request, params: Any) -> None:
         """Callback used for unit testing only"""
         if self.operating_mode == self.OperatingMode.Test_CheckThrottling:
             self.logger.error('Dummy Command failed to be achieved. Stopping test')
             self.comm_broken = True
 
@@ -801,16 +805,16 @@
 
             if not self.connected or self.device_session_id is None:
                 next_state = self.FsmState.INIT
             else:
                 if state_entry:
                     self.dispatcher.register_request(
                         request=self.protocol.comm_disconnect(self.device_session_id),
-                        success_callback=SuccessCallback(self.disconnect_complete_success),
-                        failure_callback=FailureCallback(self.disconnect_complete_failure),
+                        success_callback=self.disconnect_complete_success,
+                        failure_callback=self.disconnect_complete_failure,
                         priority=self.RequestPriority.Disconnect
                     )
 
             if self.disconnect_complete:
                 next_state != self.FsmState.DISCONNECTING
 
         else:
@@ -819,25 +823,25 @@
         # ====  FSM END ====
 
         self.last_fsm_state = self.fsm_state
         if next_state != self.fsm_state:
             self.logger.debug('Moving FSM to state %s' % next_state)
         self.fsm_state = next_state
 
-    def disconnect_complete_success(self, request: Request, response_code: ResponseCode, response_data: protocol_typing.ResponseData, params: Any = None) -> None:
+    def disconnect_complete_success(self, request: Request, response:Response, params: Any = None) -> None:
         """Callback called when a disconnect request completes successfully"""
         self.disconnect_complete = True
         if self.disconnect_callback is not None:
-            self.disconnect_callback.__call__(True)
+            self.disconnect_callback(True)
 
     def disconnect_complete_failure(self, request: Request, params: Any = None) -> None:
         """Callback called when a disconnect request fails to complete"""
         self.disconnect_complete = True
         if self.disconnect_callback is not None:
-            self.disconnect_callback.__call__(False)
+            self.disconnect_callback(False)
 
     def process_comm(self) -> None:
         """Process the communication with the device. To be called periodically"""
         done: bool = False
 
         # Try open automatically the communication with device if we can
         if not self.comm_handler.is_open():
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/device/device_info.py` & `scrutinydebugger-0.3.0/scrutiny/server/device/device_info.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/device/emulated_device.py` & `scrutinydebugger-0.3.0/scrutiny/server/device/emulated_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import collections
 from abc import ABC
 from dataclasses import dataclass
 from abc import ABC, abstractmethod
 
 from scrutiny.core.codecs import Encodable
 import scrutiny.server.protocol.commands as cmd
-from scrutiny.server.device.links.dummy_link import DummyLink, ThreadSafeDummyLink
+from scrutiny.server.device.links.dummy_link import DummyLink
 from scrutiny.server.protocol import Protocol, Request, Response, ResponseCode
 import scrutiny.server.protocol.typing as protocol_typing
 from scrutiny.core.memory_content import MemoryContent
 from scrutiny.core.basic_types import RuntimePublishedValue, EmbeddedDataType, MemoryRegion, Endianness
 import scrutiny.server.datalogging.definitions.device as device_datalogging
 from scrutiny.core.codecs import *
 from scrutiny.server.device.device_info import ExecLoop, VariableFreqLoop, FixedFreqLoop
@@ -429,15 +429,15 @@
         # The validity of this depends on the datalogger capacity to stop acquiring at the right moment.
         # if it continues acquiring and the encoder discards data, this value becomes invalid
         return self.encoder.get_entry_counter() - self.entry_counter_at_trigger
 
 
 class EmulatedDevice:
     logger: logging.Logger
-    link: Union[DummyLink, ThreadSafeDummyLink]
+    link: DummyLink
     firmware_id: bytes
     request_history: List[RequestLogRecord]
     request_history_lock: threading.Lock
     protocol: Protocol
     comm_enabled: bool
     connected: bool
     request_shutdown: bool
@@ -467,16 +467,16 @@
     loops: List[ExecLoop]
 
     additional_tasks: List[Callable[[], None]]
     failed_read_request_list: List[Request]
     failed_write_request_list: List[Request]
     ignore_user_command: bool
 
-    def __init__(self, link: Union[DummyLink, ThreadSafeDummyLink]) -> None:
-        if not isinstance(link, DummyLink) and not isinstance(link, ThreadSafeDummyLink):
+    def __init__(self, link:DummyLink) -> None:
+        if not isinstance(link, DummyLink):
             raise ValueError('EmulatedDevice expects a DummyLink object')
         self.logger = logging.getLogger(self.__class__.__name__)
         self.link = link    # Pre opened link.
         self.firmware_id = bytes(range(16))
         self.request_history = []
         self.protocol = Protocol(1, 0)
 
@@ -918,15 +918,15 @@
         else:
             return Response(cmd.UserCommand, subfn=req.subfn, code=ResponseCode.FailureToProceed)
 
     def start(self) -> None:
         self.logger.debug('Starting thread')
         self.request_shutdown = False
         self.thread_started_event.clear()
-        self.thread = threading.Thread(target=self.thread_task)
+        self.thread = threading.Thread(target=self.thread_task, daemon=True)
         self.thread.start()
         self.thread_started_event.wait()
         self.logger.debug('Thread started')
 
     def stop(self) -> None:
         if self.thread is not None:
             self.logger.debug('Stopping thread')
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/device/links/abstract_link.py` & `scrutinydebugger-0.3.0/scrutiny/server/device/links/abstract_link.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     @abstractmethod
     def write(self, data: bytes) -> None:
         """Write data into the communication channels"""
         pass
 
     @abstractmethod
-    def read(self) -> Optional[bytes]:
+    def read(self, timeout:Optional[float]=None) -> Optional[bytes]:
         """Reads data from the communication channel. Returns None if not available"""
         pass
 
     @abstractmethod
     def process(self) -> None:
         """To be called periodically"""
         pass
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/device/links/serial_link.py` & `scrutinydebugger-0.3.0/scrutiny/server/device/links/serial_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,29 +152,28 @@
 
     def operational(self) -> bool:
         """ Tells if this comm channel is in proper state to be functional"""
         if self.port is None:
             return False
         return self.port.isOpen() and self.initialized()
 
-    def read(self) -> Optional[bytes]:
-        """ Reads bytes Non-Blocking from the comm channel. None if no data available"""
-        data: Optional[bytes] = None
-        if self.operational():
-            assert self.port is not None    # For mypy
-            try:
-                n = self.port.in_waiting
-                if n > 0:
-                    data = self.port.read(n)
-            except Exception as e:
-                self.logger.debug("Cannot read data. " + str(e))
-                self.port.close()
-
+    def read(self, timeout:Optional[float] = None) -> Optional[bytes]:
+        """ Reads bytes in a blocking fashion from the comm channel. None if no data available after timeout"""
+        if not self.operational():
+            return None
+        
+        assert self.port is not None    # For mypy
+        self.port.timeout = timeout
+        data:bytes = self.port.read(max(self.port.in_waiting, 1))
+        n = self.port.in_waiting
+        if n > 0:
+            data += self.port.read(n)
         return data
 
+
     def write(self, data: bytes) -> None:
         """ Write data to the comm channel."""
         if self.operational():
             assert self.port is not None    # For mypy
             try:
                 self.port.write(data)
                 self.port.flush()
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/device/links/udp_link.py` & `scrutinydebugger-0.3.0/scrutiny/server/device/links/udp_link.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     def make(cls, config: LinkConfig) -> "UdpLink":
         return cls(config)
 
     def __init__(self, config: LinkConfig):
         self.validate_config(config)
 
         self.config = cast(UdpConfig, {
-            'host': config['host'],
+            'host': str(config['host']),
             'port': int(config['port'])
         })
 
         self.ip_address = socket.gethostbyname(self.config['host'])  # get the IP of the device
 
         self.logger = logging.getLogger(self.__class__.__name__)
         self.sock = None            # the socket
@@ -73,15 +73,14 @@
         """ Creates the UDP socket and listen on all interfaces"""
         try:
             if self.sock is not None:
                 self.sock.close()
 
             self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             self.sock.bind(('0.0.0.0', 0))  # 0.0.0.0 listen on all interface.  Port 0 = takes any available
-            self.sock.setblocking(False)
             (addr, port) = self.sock.getsockname()  # Read our own address and port, will tell the receiving port auto attributed
             self.logger.debug('Socket bound to address=%s and port=%d' % (addr, port))
             self.bound = True
         except Exception as e:
             self.logger.debug(str(e))
             self.bound = False
 
@@ -97,25 +96,28 @@
 
     def operational(self) -> bool:
         """ Tells the upper layer if we are in a working state (to the best of our knowledge)"""
         if self.sock is not None and self.bound == True:    # If bound, we are necessarily initialized
             return True
         return False
 
-    def read(self) -> Optional[bytes]:
-        """ Reads bytes Non-Blocking from the comm channel. None if no data available"""
+    def read(self,  timeout:Optional[float] = None) -> Optional[bytes]:
+        """ Reads bytes in a blocking fashion from the comm channel. None if no data available after timeout"""
         if not self.operational():
             return None
 
         try:
             assert self.sock is not None
             err = None
+            self.sock.settimeout(timeout)
             data, (ip_address, port) = self.sock.recvfrom(self.BUFSIZE)
             if ip_address == self.ip_address and port == self.config['port']:  # Make sure the datagram comes from our target device
                 return data
+        except TimeoutError:
+            pass
         except socket.error as e:
             err = e
             if e.args[0] == errno.EAGAIN or e.args[0] == errno.EWOULDBLOCK:
                 err = None
 
         if err:
             self.logger.debug('Socket error : ' + str(err))
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/device/request_dispatcher.py` & `scrutinydebugger-0.3.0/scrutiny/server/device/request_dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,23 @@
 #
 #   - License : MIT - See LICENSE file.
 #   - Project :  Scrutiny Debugger (github.com/scrutinydebugger/scrutiny-python)
 #
 #   Copyright (c) 2021 Scrutiny Debugger
 
 import bisect
-from scrutiny.server.protocol import Request, Response, ResponseCode
+from scrutiny.server.protocol import Request, Response
 from time import time
 import logging
 
 from typing import List, Optional, Callable, Any
-from scrutiny.core.typehints import GenericCallback
-
 
 # Type for mypy validation only
-class SuccessCallback(GenericCallback):
-    callback: Callable[[Request, ResponseCode, bytes, Any], None]
-
-
-class FailureCallback(GenericCallback):
-    callback: Callable[[Request, Any], None]
-
+SuccessCallback = Callable[[Request, Response, Any], None]
+FailureCallback = Callable[[Request, Any], None]
 
 class RequestQueue:
     """
     Non-thread-safe Queue with priority.
     Replace queue.PriorityQueue simply because I don't like that they compare data and don't want to introduce workarounds or 
     dataclass from Python 3.7 just for not comparing the data when selecting priority.
     We will have all the flexibility we need with our own minimalist custom class
@@ -127,17 +120,17 @@
 
     def complete(self, success: bool = False, response: Optional[Response] = None) -> None:
         """Mark this record as completed (success or failure). Will triggers callback execution"""
         self.completed = True  # Set to true at beginning so that it is still true if an exception raise in the callback
         if success:
             if response is None:
                 raise ValueError('Missing response')
-            self.success_callback.__call__(self.request, response, self.success_params)
+            self.success_callback(self.request, response, self.success_params)
         else:
-            self.failure_callback.__call__(self.request, self.failure_params)
+            self.failure_callback(self.request, self.failure_params)
 
     def is_completed(self) -> bool:
         """Return True if the request has completed (success or failure)"""
         return self.completed
 
 
 class RequestDispatcher:
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/device/submodules/datalogging_poller.py` & `scrutinydebugger-0.3.0/scrutiny/server/device/submodules/datalogging_poller.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 
 import logging
 import traceback
 from enum import Enum, auto
 from dataclasses import dataclass
 
 from scrutiny.server.protocol import *
-from scrutiny.server.device.request_dispatcher import RequestDispatcher, SuccessCallback, FailureCallback
+from scrutiny.server.device.request_dispatcher import RequestDispatcher
 import scrutiny.server.datalogging.definitions.device as device_datalogging
 import scrutiny.server.protocol.typing as protocol_typing
 import scrutiny.server.protocol.commands as cmd
 from scrutiny.tools import Timer
 from scrutiny.server.protocol.crc32 import crc32
 from scrutiny.core.basic_types import RuntimePublishedValue
 from scrutiny.server.datalogging.datalogging_utilities import extract_signal_from_data
 
-from scrutiny.core.typehints import GenericCallback
 from typing import Optional, Any, cast, Callable, List, Dict
 
 
 class FSMState(Enum):
     IDLE = auto()
     GET_SETUP = auto()
     WAIT_FOR_REQUEST = auto()
@@ -35,20 +34,16 @@
     WAIT_FOR_DATA = auto()
     READ_METADATA = auto()
     RETRIEVING_DATA = auto()
     DATA_RETRIEVAL_FINISHED_SUCCESS = auto()
     REQUEST_RESET = auto()
 
 
-class DeviceAcquisitionRequestCompletionCallback(GenericCallback):
-    callback: Callable[[bool, str, Optional[List[List[bytes]]], Optional[device_datalogging.AcquisitionMetadata]], None]
-
-
-class DataloggingReceiveSetupCallback(GenericCallback):
-    callback: Callable[[device_datalogging.DataloggingSetup], None]
+DeviceAcquisitionRequestCompletionCallback = Callable[[bool, str, Optional[List[List[bytes]]], Optional[device_datalogging.AcquisitionMetadata]], None]
+DataloggingReceiveSetupCallback = Callable[[device_datalogging.DataloggingSetup], None]
 
 
 @dataclass
 class AcquisitionRequest:
     loop_id: int
     config: device_datalogging.Configuration
     completion_callback: DeviceAcquisitionRequestCompletionCallback
@@ -570,16 +565,16 @@
         subfn = DatalogSubfn(req.subfn)
         if self.request_pending[subfn]:    # We don't stack request (even if we could)
             raise RuntimeError(
                 "Dispatched a request of subfunction %s before having received the previous response of the same subfunction" % subfn.name)
 
         self.dispatcher.register_request(
             req,
-            SuccessCallback(self.success_callback),
-            FailureCallback(self.failure_callback),
+            self.success_callback,
+            self.failure_callback,
             priority=self.request_priority)
         self.request_pending[subfn] = True
         self.request_failed[subfn] = False
 
     def success_callback(self, request: Request, response: Response, params: Any = None) -> None:
         """Called when a request completes and succeeds"""
         self.logger.debug("Success callback. Request=%s. Response Code=%s, Params=%s" % (request, response.code, params))
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/device/submodules/device_searcher.py` & `scrutinydebugger-0.3.0/scrutiny/server/device/submodules/device_searcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import time
 import logging
 import binascii
 import traceback
 
 from scrutiny.server.protocol import *
 import scrutiny.server.protocol.typing as protocol_typing
-from scrutiny.server.device.request_dispatcher import RequestDispatcher, SuccessCallback, FailureCallback
+from scrutiny.server.device.request_dispatcher import RequestDispatcher
 
 from typing import Optional, Tuple, Any, cast
 
 
 class DeviceSearcher:
     """
     Generates Discover request in loop and inform the upper layers if a device has been found
@@ -104,16 +104,16 @@
             self.found_device = None
 
         if self.pending == False:
             if self.last_request_timestamp is None or (time.monotonic() - self.last_request_timestamp > self.DISCOVER_INTERVAL):
                 self.logger.debug('Registering a Discover request')
                 self.dispatcher.register_request(
                     request=self.protocol.comm_discover(),
-                    success_callback=SuccessCallback(self.success_callback),
-                    failure_callback=FailureCallback(self.failure_callback),
+                    success_callback=self.success_callback,
+                    failure_callback=self.failure_callback,
                     priority=self.priority
                 )
                 self.pending = True
                 self.last_request_timestamp = time.monotonic()
 
     def success_callback(self, request: Request, response: Response, params: Any = None) -> None:
         # Called by the dispatcher when a request is completed and succeeded
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/device/submodules/heartbeat_generator.py` & `scrutinydebugger-0.3.0/scrutiny/server/device/submodules/heartbeat_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 #   Copyright (c) 2021 Scrutiny Debugger
 
 import time
 import logging
 import traceback
 
 from scrutiny.server.protocol import *
-from scrutiny.server.protocol.commands.comm_control import CommControl
 import scrutiny.server.protocol.typing as protocol_typing
-from scrutiny.server.device.request_dispatcher import RequestDispatcher, SuccessCallback, FailureCallback
+from scrutiny.server.device.request_dispatcher import RequestDispatcher
 
 from typing import Any, Optional, cast
 
 
 class HeartbeatGenerator:
     """
     Poll the device with periodic heartbeat message to know if it is still there and alive.
@@ -83,16 +82,16 @@
 
         # If no request is being waited and we have a session ID assigned
         if self.pending == False and self.session_id is not None:
             if self.last_heartbeat_request is None or (time.monotonic() - self.last_heartbeat_request > self.interval):
                 self.logger.debug('Registering a Heartbeat request')
                 self.dispatcher.register_request(
                     request=self.protocol.comm_heartbeat(session_id=self.session_id, challenge=self.challenge),
-                    success_callback=SuccessCallback(self.success_callback),
-                    failure_callback=FailureCallback(self.failure_callback),
+                    success_callback=self.success_callback,
+                    failure_callback=self.failure_callback,
                     priority=self.priority
                 )
                 self.pending = True
                 self.last_heartbeat_request = time.monotonic()
 
     def success_callback(self, request: Request, response: Response, params: Any = None) -> None:
         """ Called by the dispatcher when a request is completed and succeeded"""
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/device/submodules/info_poller.py` & `scrutinydebugger-0.3.0/scrutiny/server/device/submodules/info_poller.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,29 +12,23 @@
 import enum
 import copy
 import traceback
 
 from scrutiny.server.protocol import ResponseCode
 from scrutiny.server.device.device_info import *
 import scrutiny.server.protocol.commands as cmd
-from scrutiny.server.device.request_dispatcher import RequestDispatcher, SuccessCallback, FailureCallback
+from scrutiny.server.device.request_dispatcher import RequestDispatcher
 from scrutiny.server.protocol import *
 import scrutiny.server.protocol.typing as protocol_typing
 
-from scrutiny.core.typehints import GenericCallback
-
 from typing import Optional, Callable, Any, cast
 
 
-class ProtocolVersionCallback(GenericCallback):
-    callback: Callable[[int, int], Any]
-
-
-class CommParamCallback(GenericCallback):
-    callback: Callable[[DeviceInfo], Any]
+ProtocolVersionCallback = Callable[[int, int], Any]
+CommParamCallback = Callable[[DeviceInfo], Any]
 
 
 class InfoPoller:
     """Class that will successfully sends polling request to the device
     to gather all of its internal parameters. Will fill a DeviceInformation structure"""
 
     logger: logging.Logger
@@ -153,69 +147,72 @@
                 next_state = self.FsmState.GetProtocolVersion
 
         # ======= [GetProtocolVersion] =====
         elif self.fsm_state == self.FsmState.GetProtocolVersion:
             # We already know the protocol version from the discover request.  This should maybe be removed...
             if state_entry:
                 self.dispatcher.register_request(request=self.protocol.get_protocol_version(),
-                                                 success_callback=SuccessCallback(self.success_callback), failure_callback=FailureCallback(self.failure_callback), priority=self.priority)
+                                                 success_callback=self.success_callback, failure_callback=self.failure_callback, priority=self.priority)
                 self.request_pending = True
 
             if self.request_failed:
                 next_state = self.FsmState.Error
             if not self.request_pending:    # Request completed
                 try:
+                    assert self.info.protocol_major is not None
+                    assert self.info.protocol_minor is not None
+
                     if self.protocol_version_callback is not None:
-                        self.protocol_version_callback.__call__(self.info.protocol_major, self.info.protocol_minor)
+                        self.protocol_version_callback(self.info.protocol_major, self.info.protocol_minor)
                     next_state = self.FsmState.GetCommParams
                 except Exception as e:
                     self.logger.error('Error while processing protocol version. %s' % str(e))
                     self.logger.debug(traceback.format_exc())
                     next_state = self.FsmState.Error
 
         # ======= [GetCommParams] =====
         elif self.fsm_state == self.FsmState.GetCommParams:
             if state_entry:
                 self.dispatcher.register_request(request=self.protocol.comm_get_params(),
-                                                 success_callback=SuccessCallback(self.success_callback), failure_callback=FailureCallback(self.failure_callback), priority=self.priority)
+                                                 success_callback=self.success_callback, failure_callback=self.failure_callback, priority=self.priority)
                 self.request_pending = True
 
             if self.request_failed:
                 next_state = self.FsmState.Error
 
             if not self.request_pending:
                 try:
                     if self.comm_param_callback is not None:
                         # Some comm params will change the device handling. So let the deviceHandler know right away
-                        self.comm_param_callback.__call__(copy.copy(self.info))
+                        self.comm_param_callback(copy.copy(self.info))
                     next_state = self.FsmState.GetSupportedFeatures
                 except Exception as e:
                     self.logger.error('Error while processing communication params. %s' % str(e))
                     self.logger.debug(traceback.format_exc())
                     next_state = self.FsmState.Error
 
         # ======= [GetSupportedFeatures] =====
         elif self.fsm_state == self.FsmState.GetSupportedFeatures:
             if state_entry:
                 self.dispatcher.register_request(request=self.protocol.get_supported_features(),
-                                                 success_callback=SuccessCallback(self.success_callback), failure_callback=FailureCallback(self.failure_callback), priority=self.priority)
+                                                 success_callback=self.success_callback, failure_callback=self.failure_callback, priority=self.priority)
                 self.request_pending = True
 
             if self.request_failed:
                 next_state = self.FsmState.Error
             if not self.request_pending:
                 next_state = self.FsmState.GetSpecialMemoryRegionCount
 
         # ======= [GetSpecialMemoryRegionCount] =====
         elif self.fsm_state == self.FsmState.GetSpecialMemoryRegionCount:
             if state_entry:
                 self.forbidden_memory_region_count = None
                 self.readonly_memory_region_count = None
                 self.dispatcher.register_request(request=self.protocol.get_special_memory_region_count(),
-                                                 success_callback=SuccessCallback(self.success_callback), failure_callback=FailureCallback(self.failure_callback), priority=self.priority)
+                                                 success_callback=self.success_callback, failure_callback=self.failure_callback, priority=self.priority)
                 self.request_pending = True
 
             if self.request_failed:
                 next_state = self.FsmState.Error
             if not self.request_pending:
                 next_state = self.FsmState.GetForbiddenMemoryRegions
 
@@ -225,15 +222,15 @@
                 next_state = self.FsmState.Error
                 self.logger.error("Internal error - Forbidden memory region count is not set")
             else:
                 if state_entry:
                     self.info.forbidden_memory_regions = []
                     for i in range(self.forbidden_memory_region_count):
                         self.dispatcher.register_request(request=self.protocol.get_special_memory_region_location(cmd.GetInfo.MemoryRangeType.Forbidden, i),
-                                                         success_callback=SuccessCallback(self.success_callback), failure_callback=FailureCallback(self.failure_callback), priority=self.priority)
+                                                         success_callback=self.success_callback, failure_callback=self.failure_callback, priority=self.priority)
 
                 if self.request_failed:
                     next_state = self.FsmState.Error
 
                 assert self.info.forbidden_memory_regions is not None   # for mypy
                 if len(self.info.forbidden_memory_regions) >= self.forbidden_memory_region_count:
                     next_state = self.FsmState.GetReadOnlyMemoryRegions
@@ -244,29 +241,29 @@
                 next_state = self.FsmState.Error
                 self.logger.error("Internal error - Readonly memory region count is not set")
             else:
                 if state_entry:
                     self.info.readonly_memory_regions = []
                     for i in range(self.readonly_memory_region_count):
                         self.dispatcher.register_request(request=self.protocol.get_special_memory_region_location(cmd.GetInfo.MemoryRangeType.ReadOnly, i),
-                                                         success_callback=SuccessCallback(self.success_callback), failure_callback=FailureCallback(self.failure_callback), priority=self.priority)
+                                                         success_callback=self.success_callback, failure_callback=self.failure_callback, priority=self.priority)
 
                 if self.request_failed:
                     next_state = self.FsmState.Error
 
                 assert self.info.readonly_memory_regions is not None
                 if len(self.info.readonly_memory_regions) >= self.readonly_memory_region_count:
                     next_state = self.FsmState.GetRPVCount
 
         # ======= [GetRPVCount] =====
         elif self.fsm_state == self.FsmState.GetRPVCount:
             if state_entry:
                 self.rpv_count = None   # Will be set in success callback
                 self.dispatcher.register_request(request=self.protocol.get_rpv_count(),
-                                                 success_callback=SuccessCallback(self.success_callback), failure_callback=FailureCallback(self.failure_callback), priority=self.priority)
+                                                 success_callback=self.success_callback, failure_callback=self.failure_callback, priority=self.priority)
                 self.request_pending = True
 
             if self.request_failed:
                 next_state = self.FsmState.Error
             if not self.request_pending:
                 next_state = self.FsmState.GetRPVDefinition
 
@@ -293,28 +290,28 @@
                 # Issue a new request until all RPV are read
                 already_read_count = len(self.info.runtime_published_values)
                 if already_read_count < self.rpv_count:
                     count = min(max_rpv_per_request, self.rpv_count - already_read_count)
                     request = self.protocol.get_rpv_definition(start=len(self.info.runtime_published_values), count=count)
                     self.dispatcher.register_request(
                         request=request,
-                        success_callback=SuccessCallback(self.success_callback),
-                        failure_callback=FailureCallback(self.failure_callback),
+                        success_callback=self.success_callback,
+                        failure_callback=self.failure_callback,
                         priority=self.priority
                     )
                     self.request_pending = True
                 else:
                     next_state = self.FsmState.GetLoopCount
 
         # ======= [GetLoopCount] =====
         elif self.fsm_state == self.FsmState.GetLoopCount:
             if state_entry:
                 self.loop_count = None   # Will be set in success callback
                 self.dispatcher.register_request(request=self.protocol.get_loop_count(),
-                                                 success_callback=SuccessCallback(self.success_callback), failure_callback=FailureCallback(self.failure_callback), priority=self.priority)
+                                                 success_callback=self.success_callback, failure_callback=self.failure_callback, priority=self.priority)
                 self.request_pending = True
 
             if self.request_failed:
                 next_state = self.FsmState.Error
             if not self.request_pending:
                 next_state = self.FsmState.GetLoopDefinition
 
@@ -324,15 +321,15 @@
                 next_state = self.FsmState.Error
                 self.logger.error("Internal error - Loop count is not set")
             else:
                 if state_entry:
                     self.info.loops = []
                     for i in range(self.loop_count):
                         self.dispatcher.register_request(request=self.protocol.get_loop_definition(i),
-                                                         success_callback=SuccessCallback(self.success_callback), failure_callback=FailureCallback(self.failure_callback), priority=self.priority)
+                                                         success_callback=self.success_callback, failure_callback=self.failure_callback, priority=self.priority)
 
                 if self.request_failed:
                     next_state = self.FsmState.Error
 
                 assert self.info.loops is not None
                 if len(self.info.loops) >= self.loop_count:
                     next_state = self.FsmState.Done
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/device/submodules/memory_reader.py` & `scrutinydebugger-0.3.0/scrutiny/server/device/submodules/memory_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,23 @@
 import time
 import queue
 from sortedcontainers import SortedSet  # type: ignore
 
 from scrutiny.server.protocol import *
 import scrutiny.server.protocol.commands as cmd
 import scrutiny.server.protocol.typing as protocol_typing
-from scrutiny.server.device.request_dispatcher import RequestDispatcher, SuccessCallback, FailureCallback
-from scrutiny.server.datastore.datastore import Datastore, WatchCallback
+from scrutiny.server.device.request_dispatcher import RequestDispatcher
+from scrutiny.server.datastore.datastore import Datastore
 from scrutiny.server.datastore.datastore_entry import *
 from scrutiny.core.memory_content import MemoryContent, Cluster
 from scrutiny.core.basic_types import MemoryRegion
 
 from typing import cast, Set, List, Any, Optional, Callable, Tuple, Dict
-from scrutiny.core.typehints import GenericCallback
-
-
-class RawMemoryReadRequestCompletionCallback(GenericCallback):
-    callback: Callable[["RawMemoryReadRequest", bool, Optional[bytes], str], None]
 
+RawMemoryReadRequestCompletionCallback = Callable[["RawMemoryReadRequest", bool, Optional[bytes], str], None]
 
 class RawMemoryReadRequest:
     address: int
     size: int
     completed: bool
     success: bool
     completion_callback: Optional[RawMemoryReadRequestCompletionCallback]
@@ -170,16 +166,16 @@
 
     def __init__(self, protocol: Protocol, dispatcher: RequestDispatcher, datastore: Datastore, request_priority: int):
         self.logger = logging.getLogger(self.__class__.__name__)
         self.dispatcher = dispatcher
         self.protocol = protocol
         self.datastore = datastore
         self.request_priority = request_priority
-        self.datastore.add_watch_callback(WatchCallback(self.the_watch_callback))
-        self.datastore.add_unwatch_callback(WatchCallback(self.the_unwatch_callback))
+        self.datastore.add_watch_callback(self.the_watch_callback)
+        self.datastore.add_unwatch_callback(self.the_unwatch_callback)
         self.active_raw_read_request = None
         self.raw_read_request_queue = queue.Queue()
 
         self.reset()
 
     def set_max_request_payload_size(self, max_size: int) -> None:
         """Set the maximum payload size that can be sent in a request. Depends on device internal buffer size"""
@@ -328,16 +324,16 @@
             else:
                 raise Exception('Unknown read type.')
 
     def dispatch(self, request: Request) -> None:
         """Sends a request to the request dispatcher and assign the corrects completion callbacks"""
         self.dispatcher.register_request(
             request=request,
-            success_callback=SuccessCallback(self.success_callback),
-            failure_callback=FailureCallback(self.failure_callback),
+            success_callback=self.success_callback,
+            failure_callback=self.failure_callback,
             priority=self.request_priority
         )
         self.pending_request = request
 
     def make_next_var_entries_request(self) -> Tuple[Optional[Request], List[DatastoreVariableEntry], bool]:
         """
         This method generate a read request by moving in a list of watched variable entries
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/device/submodules/memory_writer.py` & `scrutinydebugger-0.3.0/scrutiny/server/device/submodules/memory_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,28 +10,25 @@
 
 import logging
 from scrutiny.server.datastore.datastore_entry import DatastoreRPVEntry, DatastoreVariableEntry, UpdateTargetRequest
 
 from scrutiny.server.protocol import *
 import scrutiny.server.protocol.commands as cmd
 import scrutiny.server.protocol.typing as protocol_typing
-from scrutiny.server.device.request_dispatcher import RequestDispatcher, SuccessCallback, FailureCallback
+from scrutiny.server.device.request_dispatcher import RequestDispatcher
 from scrutiny.server.datastore.datastore import Datastore
 from scrutiny.server.datastore.datastore_entry import DatastoreEntry
 from scrutiny.core.codecs import Codecs, Encodable
-from scrutiny.core.typehints import GenericCallback
 from scrutiny.core.basic_types import MemoryRegion
 import time
 import queue
 from typing import Any, List, Optional, cast, Callable
 
 
-class RawMemoryWriteRequestCompletionCallback(GenericCallback):
-    callback: Callable[["RawMemoryWriteRequest", bool, str], None]
-
+RawMemoryWriteRequestCompletionCallback = Callable[["RawMemoryWriteRequest", bool, str], None]
 
 class RawMemoryWriteRequest:
     address: int
     data: bytes
     completed: bool
     success: bool
     completion_callback: Optional[RawMemoryWriteRequestCompletionCallback]
@@ -478,12 +475,12 @@
         self.pending_request = None
 
     def dispatch(self, request: Request) -> None:
         """Sends a request to the request dispatcher and assign the corrects completion callbacks"""
         self.logger.debug('Registering a MemoryWrite request. %s' % (request))
         self.dispatcher.register_request(
             request=request,
-            success_callback=SuccessCallback(self.success_callback),
-            failure_callback=FailureCallback(self.failure_callback),
+            success_callback=self.success_callback,
+            failure_callback=self.failure_callback,
             priority=self.request_priority
         )
         self.pending_request = request
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/device/submodules/session_initializer.py` & `scrutinydebugger-0.3.0/scrutiny/server/device/submodules/session_initializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import logging
 from time import time
 import traceback
 
 from scrutiny.server.protocol import *
 import scrutiny.server.protocol.typing as protocol_typing
-from scrutiny.server.device.request_dispatcher import RequestDispatcher, SuccessCallback, FailureCallback
+from scrutiny.server.device.request_dispatcher import RequestDispatcher
 
 from typing import Optional, Any, cast
 
 
 class SessionInitializer:
     """
     Try to establish a connection with a device by sending Connects requests.
@@ -96,16 +96,16 @@
             return
 
         if not self.connection_pending and (self.last_connect_sent is None or time() - self.last_connect_sent > self.RECONNECT_DELAY):
             self.success = False
             self.last_connect_sent = time()
             self.logger.debug('Registering a Connect request')
             self.dispatcher.register_request(request=self.protocol.comm_connect(),
-                                             success_callback=SuccessCallback(self.success_callback),
-                                             failure_callback=FailureCallback(self.failure_callback),
+                                             success_callback=self.success_callback,
+                                             failure_callback=self.failure_callback,
                                              priority=self.priority)
             self.connection_pending = True
 
     def success_callback(self, request: Request, response: Response, params: Any = None) -> None:
         """Callback called by the request dispatcher when a request succeeds to complete"""
         if response.code == ResponseCode.OK:
             try:
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/protocol/comm_handler.py` & `scrutinydebugger-0.3.0/scrutiny/server/protocol/comm_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,26 +6,28 @@
 #        It manages the low level part of the communication protocol with the device
 #
 #   - License : MIT - See LICENSE file.
 #   - Project :  Scrutiny Debugger (github.com/scrutinydebugger/scrutiny-python)
 #
 #   Copyright (c) 2021 Scrutiny Debugger
 
-from queue import Queue
+
 from scrutiny.server.protocol import Request, Response
 from scrutiny.tools import Timer, Throttler
 from copy import copy
 import logging
 import struct
 from binascii import hexlify
 import time
 from scrutiny.server.device.links import AbstractLink, LinkConfig
 import traceback
+import queue
 
 from typing import TypedDict, Optional, Any, Dict, Type, cast
+import threading
 
 
 class CommHandler:
     """
     This class is the bridge between the application and the communication channel with the device.
     It exchange bytes with the device and exchanges request/response with the upper layer.
     The link object abstract the communication channel.
@@ -51,322 +53,378 @@
             self.length_bytes_received = 0
             self.data_buffer = bytes()
 
     DEFAULT_PARAMS: "CommHandler.Params" = {
         'response_timeout': 1
     }
 
-    active_request: Optional[Request]
-    received_response: Optional[Response]
-    link: Optional[AbstractLink]
-    params: "CommHandler.Params"
-    response_timer: Timer
-    rx_data: "CommHandler.RxData"
-    logger: logging.Logger
-    opened: bool
-    throttler: Throttler
-    rx_bitcount: int
-    tx_bitcount: int
-    bitcount_time: float
-    timed_out: bool
-    pending_request: Optional[Request]
-    link_type: str
-    last_open_error: Optional[str]
+    _active_request: Optional[Request]
+    _received_response: Optional[Response]
+    _link: Optional[AbstractLink]
+    _params: "CommHandler.Params"
+    _response_timer: Timer
+    _rx_data: "CommHandler.RxData"
+    _logger: logging.Logger
+    _opened: bool
+    _throttler: Throttler
+    _rx_bitcount: int
+    _tx_bitcount: int
+    _bitcount_time: float
+    _timed_out: bool
+    _pending_request: Optional[Request]
+    _link_type: str
+    _last_open_error: Optional[str]
+    _rx_data_event:Optional[threading.Event]
+    
+    _rx_queue:"queue.Queue[bytes]"
+    _rx_thread:Optional[threading.Thread]
+    _rx_thread_started:threading.Event
+    _rx_thread_stop_requested:threading.Event
 
     def __init__(self, params: Dict[str, Any] = {}) -> None:
-        self.active_request = None      # Contains the request object that has been sent to the device. When None, no request sent and we are standby
-        self.received_response = None   # Indicates that a response has been received.
-        self.link = None                # Abstracted communication channel that implements  initialize, destroy, write, read
+        self._active_request = None      # Contains the request object that has been sent to the device. When None, no request sent and we are standby
+        self._received_response = None   # Indicates that a response has been received.
+        self._link = None                # Abstracted communication channel that implements  initialize, destroy, write, read
         self.params = copy(self.DEFAULT_PARAMS)
         self.params.update(cast(CommHandler.Params, params))
 
-        self.response_timer = Timer(self.params['response_timeout'])    # Timer for response timeout management
-        self.rx_data = self.RxData()    # Contains the response data while we read it.
-        self.logger = logging.getLogger(self.__class__.__name__)
-        self.opened = False     # True when communication channel is active and working.
+        self._response_timer = Timer(self.params['response_timeout'])    # Timer for response timeout management
+        self._rx_data = self.RxData()    # Contains the response data while we read it.
+        self._logger = logging.getLogger(self.__class__.__name__)
+        self._opened = False     # True when communication channel is active and working.
         self.reset_bitrate_monitor()
-        self.throttler = Throttler()
-        self.link_type = "none"
-        self.last_open_error = None
+        self._throttler = Throttler()
+        self._link_type = "none"
+        self._last_open_error = None
+        self._rx_data_event = None
+
+        self._rx_queue = queue.Queue()
+        self._rx_thread_started = threading.Event()
+        self._rx_thread = None
+        self._rx_thread_stop_requested = threading.Event()
+
+    def _rx_thread_task(self) -> None:
+        self._logger.debug("RX thread started")
+        self._rx_thread_started.set()
+        while not self._rx_thread_stop_requested.is_set():
+            if self._link is not None:
+                try:
+                    data = self._link.read(timeout=0.5)
+                    if data is not None and len(data) > 0:
+                        self._rx_queue.put(data)
+                        if self._rx_data_event is not None:
+                            self._rx_data_event.set()
+                except Exception as e:
+                    self._logger.error(str(e))
+            else:
+                time.sleep(0.2)
+        self._logger.debug("RX thread exiting")
+        
+
+    def set_rx_data_event(self, evt:threading.Event) -> None:
+        self._rx_data_event = evt
 
     def enable_throttling(self, bitrate: float) -> None:
         """Enable throttling on communication.
         Overall bitrate (incoming and outgoing data included) will try to be respected.
         This does not take in account the protocol overhead. Just the payload sum.
         """
-        self.throttler.set_bitrate(bitrate)
-        self.throttler.enable()
+        self._throttler.set_bitrate(bitrate)
+        self._throttler.enable()
 
     def disable_throttling(self) -> None:
         """Disable throttling on communication with the device"""
-        self.throttler.set_bitrate(0)
-        self.throttler.disable()
+        self._throttler.set_bitrate(0)
+        self._throttler.disable()
 
     def is_throttling_enabled(self) -> bool:
         """Returns True if throttling is enabled on the device communication"""
-        return self.throttler.is_enabled()
+        return self._throttler.is_enabled()
 
     def get_throttling_bitrate(self) -> Optional[float]:
         """Get the target bitrate for throttling. None if disabled"""
-        return self.throttler.get_bitrate() if self.throttler.is_enabled() else None
+        return self._throttler.get_bitrate() if self._throttler.is_enabled() else None
 
     def reset_bitrate_monitor(self) -> None:
         """Reset data size counters"""
         self.rx_bitcount = 0
         self.tx_bitcount = 0
         self.bitcount_time = time.perf_counter()
 
     def get_link(self) -> Optional[AbstractLink]:
         """Return the Link object used to talk with the device."""
-        return self.link
+        return self._link
 
     def get_link_type(self) -> str:
         """Return the link type as a string. This type is the same used by the server configuration"""
-        return self.link_type
+        return self._link_type
 
     def set_link(self, link_type: str, link_config: LinkConfig) -> None:
         """Set the device Link object from a type and a configuration."""
-        self.logger.debug('Configuring new device link of type %s with config : %s' % (link_type, str(link_config)))
+        self._logger.debug('Configuring new device link of type %s with config : %s' % (link_type, str(link_config)))
 
         self.close()
         if link_type == 'none':
-            self.link = None
-            self.link_type = "none"
+            self._link = None
+            self._link_type = "none"
             return
 
-        self.link_type = link_type
+        self._link_type = link_type
 
-        link_class = self.get_link_class(link_type)
-        self.link = link_class.make(link_config)
-        self.last_open_error = None
+        link_class = self._get_link_class(link_type)
+        self._link = link_class.make(link_config)
+        self._last_open_error = None
 
     def validate_link_config(self, link_type: str, link_config: LinkConfig) -> None:
         """Raises an exception if the given configuration is wrong for the given link type"""
-        link_class = self.get_link_class(link_type)
+        link_class = self._get_link_class(link_type)
         return link_class.validate_config(link_config)
 
-    def get_link_class(self, link_type: str) -> Type[AbstractLink]:
+    def _get_link_class(self, link_type: str) -> Type[AbstractLink]:
         """Link Factory that returns the correct Link class based on a type given as string."""
         link_class: Type[AbstractLink]
 
         if link_type == 'udp':
             from scrutiny.server.device.links.udp_link import UdpLink
             link_class = UdpLink
         elif link_type == 'serial':
             from scrutiny.server.device.links.serial_link import SerialLink
             link_class = SerialLink
         elif link_type == 'dummy':
             from scrutiny.server.device.links.dummy_link import DummyLink
             link_class = DummyLink
-        elif link_type == 'thread_safe_dummy':
-            from scrutiny.server.device.links.dummy_link import ThreadSafeDummyLink
-            link_class = ThreadSafeDummyLink
         else:
             raise ValueError('Unknown link type %s' % link_type)
 
         return link_class
 
+    def _stop_rx_thread(self, timeout:float = 1) -> None:
+        """Stop the internal thread dedicated to reading the device link object"""
+        if self._rx_thread is not None:
+            if self._rx_thread.is_alive():
+                self._rx_thread_stop_requested.set()
+                self._rx_thread.join(timeout)
+                if self._rx_thread.is_alive():
+                    self._logger.error("Failed to stop the RX thread")
+        
+        self._rx_thread = None
+
     def open(self) -> None:
+        self._logger.debug("Opening communication with device")
         """Try to open the communication channel with the device."""
-        if self.link is None:
+        if self._link is None:
             raise Exception('Link must be set before opening')
 
         try:
-            self.link.initialize()
-            self.opened = True
-            self.last_open_error = None
+            self._link.initialize()
+            self._rx_queue = queue.Queue()
+            self._rx_thread = threading.Thread(target=self._rx_thread_task, daemon=True)
+            self._rx_thread_started.clear()
+            self._rx_thread_stop_requested.clear()
+            self._rx_thread.start()
+            if not self._rx_thread_started.wait(timeout=1):
+                self._stop_rx_thread()
+                raise TimeoutError("RX thread did not start")
+            
+            self._opened = True
+            self._last_open_error = None
+            self._logger.debug("Communication with device opened")
         except Exception as e:
             err = str(e)
             full_error = f"Cannot initialize device. {err}"
-            if self.last_open_error != err:
-                self.logger.error(full_error)
-            elif self.logger.isEnabledFor(logging.DEBUG):
-                self.logger.debug(full_error)
-            self.last_open_error = err
-            self.opened = False 
+            if self._last_open_error != err:
+                self._logger.error(full_error)
+            elif self._logger.isEnabledFor(logging.DEBUG):
+                self._logger.debug(full_error)
+            self._last_open_error = err
+            self._opened = False 
 
     def is_open(self) -> bool:
         """Return True if the communication channel is open with the device"""
-        return self.opened
+        return self._opened
 
     def close(self) -> None:
         """Close the communication channel with the device"""
-        if self.link is not None:
-            self.link.destroy()
+        self._logger.debug("Closing communication with device")
+        self._stop_rx_thread()
+
+        if self._link is not None:
+            self._link.destroy()
 
         self.reset()
-        self.opened = False
-        self.last_open_error = None
+        self._last_open_error = None
+        self._opened = False
+        self._logger.debug("Communication with device closed")
 
     def is_operational(self) -> bool:
         """Return True if the communication channel is presently in a healthy state."""
-        if self.link is None:
+        if self._link is None:
             return False
 
-        return self.opened and self.link.operational()
+        return self._opened and self._link.operational()
 
     def process(self) -> None:
         """To be called periodically"""
-        if self.link is None:
+        if self._link is None:
             self.reset()
             return
 
-        if self.link.initialized() and not self.link.operational():
-            self.logger.error('Communication link stopped working. Stopping communication')
+        if self._link.initialized() and not self._link.operational():
+            self._logger.error('Communication link stopped working. Stopping communication')
             # Something broken here. Hardware disconnected maybe?
             self.close()    # Destroy and deinit the link
             return
 
         if self.is_operational():
-            self.link.process()  # Process the link handling
-            self.throttler.process()
-            self.process_rx()   # Treat response reception
-            self.process_tx()   # Handle throttling
+            self._link.process()  # Process the link handling
+            self._throttler.process()
+            self._process_rx()   # Treat response reception
+            self._process_tx()   # Handle throttling
 
-    def process_rx(self) -> None:
+    def _process_rx(self) -> None:
         """Handle data reception"""
-        assert self.link is not None
+        assert self._link is not None
 
         # If we haven't got a response or we know we won't get one. Mark the request as timed out
-        if self.waiting_response() and (self.response_timer.is_timed_out() or not self.link.operational()):
+        if self.waiting_response() and (self._response_timer.is_timed_out() or not self._link.operational()):
             self.reset_rx()
             self.timed_out = True
 
-        data: Optional[bytes] = self.link.read()
-        if data is None or len(data) == 0:
-            return  # No data, exit.
+        if self._rx_queue.empty():
+            return
+        data = self._rx_queue.get()
 
         datasize_bits = len(data) * 8
-        self.throttler.consume_bandwidth(datasize_bits)
+        self._throttler.consume_bandwidth(datasize_bits)
         self.rx_bitcount += datasize_bits
-        self.logger.debug('Received : %s' % (hexlify(data).decode('ascii')))
+        self._logger.debug('Received : %s' % (hexlify(data).decode('ascii')))
 
         if self.response_available() or not self.waiting_response():
-            self.logger.debug('Received unwanted data: ' + hexlify(data).decode('ascii'))
+            self._logger.debug('Received unwanted data: ' + hexlify(data).decode('ascii'))
             return  # Purposely discard data if we are not expecting any
 
-        self.rx_data.data_buffer += data    # Add data to receive buffer
+        self._rx_data.data_buffer += data    # Add data to receive buffer
 
-        if len(self.rx_data.data_buffer) >= 5:  # We have a valid command,subcommand, code and length (16bits)
-            if self.rx_data.length is None:
-                self.rx_data.length, = struct.unpack('>H', self.rx_data.data_buffer[3:5])   # Read the data length
-
-        if self.rx_data.length is not None:  # We already received a valid header
-            expected_bytes_count = self.rx_data.length + 9  # payload + header (5 bytes), CRC (4bytes)
-            if len(self.rx_data.data_buffer) >= expected_bytes_count:
-                self.rx_data.data_buffer = self.rx_data.data_buffer[0:expected_bytes_count]  # Remove extra bytes
+        if len(self._rx_data.data_buffer) >= 5:  # We have a valid command,subcommand, code and length (16bits)
+            if self._rx_data.length is None:
+                self._rx_data.length, = struct.unpack('>H', self._rx_data.data_buffer[3:5])   # Read the data length
+
+        if self._rx_data.length is not None:  # We already received a valid header
+            expected_bytes_count = self._rx_data.length + 9  # payload + header (5 bytes), CRC (4bytes)
+            if len(self._rx_data.data_buffer) >= expected_bytes_count:
+                self._rx_data.data_buffer = self._rx_data.data_buffer[0:expected_bytes_count]  # Remove extra bytes
 
                 # We have enough data, try to decode the response and validate the CRC.
                 try:
-                    self.received_response = Response.from_bytes(self.rx_data.data_buffer)  # CRC validation is done here
+                    self._received_response = Response.from_bytes(self._rx_data.data_buffer)  # CRC validation is done here
 
                     # Decoding did not raised an exception, we have a valid payload!
-                    self.logger.debug("Received Response %s" % self.received_response)
-                    self.rx_data.clear()        # Empty the receive buffer
-                    self.response_timer.stop()  # Timeout timer can be stop
-                    if self.active_request is not None:  # Just to please mypy
+                    self._logger.debug("Received Response %s" % self._received_response)
+                    self._rx_data.clear()        # Empty the receive buffer
+                    self._response_timer.stop()  # Timeout timer can be stop
+                    if self._active_request is not None:  # Just to please mypy
                         # Validate that the response match the request
-                        if self.received_response.command != self.active_request.command:
-                            raise Exception("Unexpected Response command ID : %s Expecting: %s" %
-                                            (str(self.received_response), self.active_request.command))
-                        if self.received_response.subfn != self.active_request.subfn:
-                            raise Exception("Unexpected Response subfunction : %s. Expecting: %s" %
-                                            (str(self.received_response), self.active_request.subfn))
+                        if self._received_response.command != self._active_request.command:
+                            raise RuntimeError("Unexpected Response command ID : %s Expecting: %s" %
+                                            (str(self._received_response), self._active_request.command))
+                        if self._received_response.subfn != self._active_request.subfn:
+                            raise RuntimeError("Unexpected Response subfunction : %s. Expecting: %s" %
+                                            (str(self._received_response), self._active_request.subfn))
                     else:
                         # Should never happen. waiting_response() is checked above
-                        raise Exception('Got a response while having no request in process')
+                        raise RuntimeError('Got a response while having no request in process')
 
                     # Here, everything went fine. The application can now send a new request or read the received response.
                 except Exception as e:
-                    self.logger.error("Received malformed message. " + str(e))
+                    self._logger.error("Received malformed message. " + str(e))
                     self.reset_rx()
 
-    def process_tx(self, newrequest: bool = False) -> None:
+    def _process_tx(self, newrequest: bool = False) -> None:
         """Handle data transmission"""
-        assert self.link is not None
+        assert self._link is not None
 
-        if self.pending_request is not None:
-            approx_delta_bandwidth = (self.pending_request.size() + self.pending_request.get_expected_response_size()) * 8;
-            if self.throttler.allowed(approx_delta_bandwidth):
-                self.active_request = self.pending_request
-                self.pending_request = None
-                data = self.active_request.to_bytes()
-                self.logger.debug("Sending request %s" % self.active_request)
-                self.logger.debug("Sending : %s" % (hexlify(data).decode('ascii')))
+        if self._pending_request is not None:
+            approx_delta_bandwidth = (self._pending_request.size() + self._pending_request.get_expected_response_size()) * 8
+            if self._throttler.allowed(approx_delta_bandwidth):
+                self._active_request = self._pending_request
+                self._pending_request = None
+                data = self._active_request.to_bytes()
+                self._logger.debug("Sending request %s" % self._active_request)
+                self._logger.debug("Sending : %s" % (hexlify(data).decode('ascii')))
                 datasize_bits = len(data) * 8
                 try:
-                    self.link.write(data)
+                    self._link.write(data)
                     err = None
                 except Exception as e:
                     err = e
-                    self.logger.error('Cannot write to communication link. %s' % str(e))
-                    self.logger.debug(traceback.format_exc())
+                    self._logger.error('Cannot write to communication link. %s' % str(e))
+                    self._logger.debug(traceback.format_exc())
 
                 if not err:
                     self.tx_bitcount += datasize_bits
-                    self.throttler.consume_bandwidth(datasize_bits)
-                    self.response_timer.start(self.params['response_timeout'])
-            elif not self.throttler.possible(approx_delta_bandwidth):
-                self.logger.critical("Throttling doesn't allow to send request. Dropping %s" % self.pending_request)
-                self.pending_request = None
+                    self._throttler.consume_bandwidth(datasize_bits)
+                    self._response_timer.start(self.params['response_timeout'])
+            elif not self._throttler.possible(approx_delta_bandwidth):
+                self._logger.critical("Throttling doesn't allow to send request. Dropping %s" % self._pending_request)
+                self._pending_request = None
             else:
                 if newrequest:  # Not sent right away
-                    self.logger.debug('Received request to send. Waiting because of throttling. %s' % self.pending_request)
+                    self._logger.debug('Received request to send. Waiting because of throttling. %s' % self._pending_request)
 
     def response_available(self) -> bool:
         """Return True if a response for the pending request has been received"""
-        return (self.received_response is not None)
+        return (self._received_response is not None)
 
     def has_timed_out(self) -> bool:
         """Return True if the pending request has timed out without response"""
         return self.timed_out
 
     def clear_timeout(self) -> None:
         """Clear the timeout if the pending request did time out. Put back the CommHandler in a ready state for the next request"""
         self.timed_out = False
 
     def get_response(self) -> Response:
         """Return the response received for the active request"""
-        if self.received_response is None:
+        if self._received_response is None:
             raise Exception('No response to read')
 
-        response = self.received_response   # Make a copy of the response to return before clearing everything
+        response = self._received_response   # Make a copy of the response to return before clearing everything
         self.reset_rx()  # Since user read the response, it has been acknowledged. Make sure response_available() return False
 
         return response
 
     def reset_rx(self) -> None:
         """ 
         Make sure we can send a new request.
         Also clear the received response so that response_available() return False
         """
-        self.active_request = None
-        self.pending_request = None
-        self.received_response = None
-        self.response_timer.stop()
-        self.rx_data.clear()
+        self._active_request = None
+        self._pending_request = None
+        self._received_response = None
+        self._response_timer.stop()
+        self._rx_data.clear()
 
     def send_request(self, request: Request) -> None:
         """Sends a request to the device"""
         if self.waiting_response():
             raise Exception('Cannot send new request. Already waiting for a response')
 
-        if self.opened:
-            self.pending_request = request
-            self.received_response = None
+        if self._opened:
+            self._pending_request = request
+            self._received_response = None
             self.timed_out = False
-            self.process_tx(newrequest=True)
+            self._process_tx(newrequest=True)
 
     def waiting_response(self) -> bool:
         """Return True if there is a pending request waiting for a response. 
         Will return False if the pending request does time out"""
         # We are waiting response if a request is active, meaning it has been sent and response has not been acknowledge by the application
-        if not self.opened:
+        if not self._opened:
             return False
-        return (self.active_request is not None or self.pending_request is not None)
+        return (self._active_request is not None or self._pending_request is not None)
 
     def reset(self) -> None:
         """Put back the CommHandler to its startup state"""
         self.reset_rx()
         self.clear_timeout()
 
     def get_average_bitrate(self) -> float:
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/protocol/commands/base_command.py` & `scrutinydebugger-0.3.0/scrutiny/server/protocol/commands/base_command.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/protocol/commands/comm_control.py` & `scrutinydebugger-0.3.0/scrutiny/server/protocol/commands/comm_control.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/protocol/commands/datalog_control.py` & `scrutinydebugger-0.3.0/scrutiny/server/protocol/commands/datalog_control.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/protocol/commands/dummy_command.py` & `scrutinydebugger-0.3.0/scrutiny/server/protocol/commands/dummy_command.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/protocol/commands/get_info.py` & `scrutinydebugger-0.3.0/scrutiny/server/protocol/commands/get_info.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/protocol/commands/memory_control.py` & `scrutinydebugger-0.3.0/scrutiny/server/protocol/commands/memory_control.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/protocol/crc32.py` & `scrutinydebugger-0.3.0/scrutiny/server/protocol/crc32.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/protocol/exceptions.py` & `scrutinydebugger-0.3.0/scrutiny/server/protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/protocol/protocol.py` & `scrutinydebugger-0.3.0/scrutiny/server/protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/protocol/request.py` & `scrutinydebugger-0.3.0/scrutiny/server/protocol/request.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/protocol/response.py` & `scrutinydebugger-0.3.0/scrutiny/server/protocol/response.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/protocol/typing.py` & `scrutinydebugger-0.3.0/scrutiny/server/protocol/typing.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/server/server.py` & `scrutinydebugger-0.3.0/scrutiny/server/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,28 +4,32 @@
 #        Allow the clients to interact with the device
 #
 #   - License : MIT - See LICENSE file.
 #   - Project :  Scrutiny Debugger (github.com/scrutinydebugger/scrutiny-python)
 #
 #   Copyright (c) 2021 Scrutiny Debugger
 
+__all__ = ['ScrutinyServer', 'ServerConfig', 'DEFAULT_CONFIG']
+
 import time
 import os
 import json
 import logging
 import traceback
 from copy import copy
+import threading
 
 from scrutiny.server.api import API, APIConfig
 from scrutiny.server.datastore.datastore import Datastore
 from scrutiny.server.device.device_handler import DeviceHandler, DeviceHandlerConfig
 from scrutiny.server.active_sfd_handler import ActiveSFDHandler
 from scrutiny.server.datalogging.datalogging_manager import DataloggingManager
+from scrutiny.tools import update_dict_recursive
 
-from typing import TypedDict, Optional, Union
+from typing import TypedDict, Optional, Union, Dict, cast, Any
 
 
 class ServerConfig(TypedDict, total=False):
     """The server configuration definition loadable from json"""
     name: str
     autoload_sfd: bool
     debug: bool
@@ -60,45 +64,66 @@
     logger: logging.Logger
     config: ServerConfig
     datastore: Datastore
     api: API
     device_handler: DeviceHandler
     sfd_handler: ActiveSFDHandler
     datalogging_manager: DataloggingManager
+    rx_data_event:threading.Event
 
-    def __init__(self, input_config: Optional[Union[str, ServerConfig]] = None) -> None:
+    def __init__(self, 
+                 input_config: Optional[Union[str, ServerConfig]] = None,
+                 additional_config: Optional[ServerConfig] = None
+                 ) -> None:
         self.logger = logging.getLogger(self.__class__.__name__)
         self.config = copy(DEFAULT_CONFIG)
         if input_config is not None:
             if isinstance(input_config, str) and os.path.isfile(input_config):
                 self.logger.debug('Loading user configuration file: "%s"' % input_config)
                 del self.config['name']  # remove "default config" from name
                 with open(input_config) as f:
                     try:
                         user_cfg = json.loads(f.read())
-                        self.config.update(user_cfg)
+                        update_dict_recursive(cast(Dict[Any, Any],self.config), cast(Dict[Any, Any], user_cfg))
                     except Exception as e:
                         raise Exception("Invalid configuration JSON. %s" % e)
             elif isinstance(input_config, dict):
-                self.config.update(input_config)
+                update_dict_recursive(cast(Dict[Any, Any],self.config), cast(Dict[Any, Any],input_config))
+        
+        if additional_config is not None:
+            update_dict_recursive(cast(Dict[Any, Any], self.config), cast(Dict[Any, Any], additional_config))
 
         self.validate_config()
         self.server_name = '<Unnamed>' if 'name' not in self.config else self.config['name']
 
+        self.rx_data_event = threading.Event()
         self.datastore = Datastore()
-        self.device_handler = DeviceHandler(self.config['device'], self.datastore)
-        self.datalogging_manager = DataloggingManager(self.datastore, self.device_handler)
-        self.sfd_handler = ActiveSFDHandler(device_handler=self.device_handler, datastore=self.datastore, autoload=self.config['autoload_sfd'])
+        self.device_handler = DeviceHandler(
+            config=self.config['device'], 
+            datastore=self.datastore, 
+            rx_event=self.rx_data_event
+        )
+        self.datalogging_manager = DataloggingManager(
+            datastore=self.datastore, 
+            device_handler=self.device_handler
+        )
+        self.sfd_handler = ActiveSFDHandler(
+            device_handler=self.device_handler, 
+            datastore=self.datastore, 
+            autoload=self.config['autoload_sfd']
+        )
         self.api = API(
             self.config['api'],
             datastore=self.datastore,
             device_handler=self.device_handler,
             sfd_handler=self.sfd_handler,
             datalogging_manager=self.datalogging_manager,
-            enable_debug=self.config['debug'])
+            enable_debug=self.config['debug'],
+            rx_event=self.rx_data_event
+        )
 
     def validate_config(self) -> None:
         if self.config['debug']:
             try:
                 import ipdb  # type: ignore
             except ImportError:
                 self.config['debug'] = False
@@ -118,15 +143,17 @@
         """Launch the server code. This function is blocking"""
         self.logger.info('Starting server instance "%s"' % (self.server_name))
 
         try:
             self.init()
             while True:
                 self.process()
-                time.sleep(0.01)
+                self.rx_data_event.wait(0.01)   # sleep until we have some IO or 10ms
+                self.rx_data_event.clear()
+
         except (KeyboardInterrupt, SystemExit):
             self.close_all()
         except Exception as e:
             self.logger.error(str(e))
             self.logger.debug(traceback.format_exc())
             self.close_all()
             raise
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/tools/synchronous_websocket_server.py` & `scrutinydebugger-0.3.0/scrutiny/tools/synchronous_websocket_server.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 import websockets
 import websockets.server
 import websockets.exceptions
 import queue
 import asyncio
 import logging
+import threading
 
 from typing import Any, Optional, Tuple, Callable
-from scrutiny.core.typehints import GenericCallback
 
 WebsocketType = websockets.server.WebSocketServerProtocol
 
 
 ConnectCallback = Callable[[WebsocketType], None]
 DiconnectCallback = Callable[[WebsocketType], None]
 
@@ -30,24 +30,31 @@
     """
     rxqueue: "queue.Queue[Tuple[WebsocketType, Any]]"
     txqueue: "queue.Queue[Tuple[WebsocketType, Any]]"
     loop: asyncio.AbstractEventLoop
     logger: logging.Logger
     connect_callback: Optional[ConnectCallback]
     disconnect_callback: Optional[DiconnectCallback]
+    rx_event:Optional[threading.Event]
    # ws_server: Optional[websockets.server.Serve]
 
-    def __init__(self, connect_callback: Optional[ConnectCallback] = None, disconnect_callback: Optional[DiconnectCallback] = None):
+    def __init__(self, 
+                 connect_callback: Optional[ConnectCallback] = None, 
+                 disconnect_callback: Optional[DiconnectCallback] = None,
+                 rx_event:Optional[threading.Event] = None
+                 ):
         self.rxqueue = queue.Queue()
         self.txqueue = queue.Queue()
         self.loop = asyncio.new_event_loop()
         self.ws_server = None
         self.connect_callback = connect_callback
         self.disconnect_callback = disconnect_callback
         self.logger = logging.getLogger(self.__class__.__name__)
+        self.rx_event = rx_event
+
 
     async def server_routine(self, websocket: WebsocketType, path: str) -> None:
         """ The routine given to the websockets module. Executed for each websocket"""
         if self.connect_callback is not None:
             self.connect_callback(websocket)
 
         try:
@@ -57,14 +64,16 @@
                         s = message
                     elif isinstance(message, bytes):
                         s = message.decode('utf8')
                     else:
                         s = message
                     self.logger.debug("Receiving %s" % s)
                 self.rxqueue.put((websocket, message))   # Possible improvement : Handle queue full scenario.
+                if self.rx_event is not None:
+                    self.rx_event.set()
         except (websockets.exceptions.ConnectionClosedOK, websockets.exceptions.ConnectionClosedError):
             pass
         finally:
             if self.disconnect_callback is not None:
                 self.disconnect_callback(websocket)
 
     def process_tx_queue(self) -> None:
```

### Comparing `scrutinydebugger-0.2.2/scrutiny/tools/throttler.py` & `scrutinydebugger-0.3.0/scrutiny/tools/throttler.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutiny/tools/timer.py` & `scrutinydebugger-0.3.0/scrutiny/tools/timer.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.2/scrutinydebugger.egg-info/PKG-INFO` & `scrutinydebugger-0.3.0/scrutinydebugger.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: scrutinydebugger
-Version: 0.2.2
+Version: 0.3.0
 Summary: Scrutiny debugger Python framework
 Home-page: https://github.com/scrutinydebugger/scrutiny-python
 Author: Pier-Yves Lessard
 License: MIT
 Requires-Python: >3.8
 License-File: LICENSE
-Requires-Dist: appdirs>=1.4.4
-Requires-Dist: pyelftools>=0.29
-Requires-Dist: websockets>=11.0.3
-Requires-Dist: sortedcontainers>=2.4
-Requires-Dist: pyserial>=3.5
+Requires-Dist: appdirs==1.4.4
+Requires-Dist: pyelftools==0.31
+Requires-Dist: websockets==12.0
+Requires-Dist: sortedcontainers==2.4.0
+Requires-Dist: pyserial==3.5
 Provides-Extra: test
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: sphinx-book-theme==1.1.2; extra == "test"
 Requires-Dist: sphinx==7.2.6; extra == "test"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
```

### Comparing `scrutinydebugger-0.2.2/scrutinydebugger.egg-info/SOURCES.txt` & `scrutinydebugger-0.3.0/scrutinydebugger.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 scrutiny/cli/commands/tag_firmware_id.py
 scrutiny/cli/commands/uninstall_sfd.py
 scrutiny/core/__init__.py
 scrutiny/core/alias.py
 scrutiny/core/basic_types.py
 scrutiny/core/codecs.py
 scrutiny/core/datalogging.py
+scrutiny/core/embedded_enum.py
 scrutiny/core/firmware_description.py
 scrutiny/core/firmware_id.py
 scrutiny/core/firmware_parser.py
 scrutiny/core/memory_content.py
 scrutiny/core/sfd_storage.py
 scrutiny/core/typehints.py
 scrutiny/core/validation.py
@@ -108,15 +109,14 @@
 scrutiny/server/protocol/commands/comm_control.py
 scrutiny/server/protocol/commands/datalog_control.py
 scrutiny/server/protocol/commands/dummy_command.py
 scrutiny/server/protocol/commands/get_info.py
 scrutiny/server/protocol/commands/memory_control.py
 scrutiny/server/protocol/commands/user_command.py
 scrutiny/tools/__init__.py
-scrutiny/tools/selectable_queue.py
 scrutiny/tools/synchronous_websocket_server.py
 scrutiny/tools/throttler.py
 scrutiny/tools/timer.py
 scrutinydebugger.egg-info/PKG-INFO
 scrutinydebugger.egg-info/SOURCES.txt
 scrutinydebugger.egg-info/dependency_links.txt
 scrutinydebugger.egg-info/entry_points.txt
```

### Comparing `scrutinydebugger-0.2.2/setup.py` & `scrutinydebugger-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 from setuptools import setup, find_packages
 import scrutiny
 import sys
 import os
 
 dependencies = [
-    'appdirs>=1.4.4',
-    'pyelftools>=0.29',
-    'websockets>=11.0.3',
-    'sortedcontainers>=2.4',
-    'pyserial>=3.5'
+    'appdirs==1.4.4',
+    'pyelftools==0.31',
+    'websockets==12.0',
+    'sortedcontainers==2.4.0',
+    'pyserial==3.5'
 ]
 
 doc_dependencies = []
 if (sys.version_info.major, sys.version_info.minor) >= (3, 9):
     doc_dependencies = [
         'sphinx-book-theme==1.1.2',
         'sphinx==7.2.6'
```

