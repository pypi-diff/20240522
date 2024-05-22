# Comparing `tmp/hgitaly-1.5.0.tar.gz` & `tmp/hgitaly-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgitaly-1.5.0.tar", last modified: Sat May 18 14:06:03 2024, max compression
+gzip compressed data, was "hgitaly-1.6.0.tar", last modified: Wed May 22 11:16:33 2024, max compression
```

## Comparing `hgitaly-1.5.0.tar` & `hgitaly-1.6.0.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.646772 hgitaly-1.5.0/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18092 2024-05-01 16:09:12.000000 hgitaly-1.5.0/LICENSE
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       33 2024-05-01 16:09:12.000000 hgitaly-1.5.0/MANIFEST.in
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15668 2024-05-18 14:06:03.646772 hgitaly-1.5.0/PKG-INFO
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15287 2024-05-01 16:09:12.000000 hgitaly-1.5.0/README.md
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.625772 hgitaly-1.5.0/hgext3rd/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      157 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgext3rd/__init__.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.625772 hgitaly-1.5.0/hgext3rd/hgitaly/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4418 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgext3rd/hgitaly/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1551 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgext3rd/hgitaly/revset.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.626772 hgitaly-1.5.0/hgext3rd/hgitaly/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgext3rd/hgitaly/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2021 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgext3rd/hgitaly/tests/test_revset.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5392 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgext3rd/hgitaly/tests/test_serve.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.630772 hgitaly-1.5.0/hgitaly/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        6 2024-05-18 14:05:28.000000 hgitaly-1.5.0/hgitaly/VERSION
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      361 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    13506 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      744 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/changelog.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    13280 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4985 2024-05-17 13:05:58.000000 hgitaly-1.5.0/hgitaly/errors.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2749 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/feature.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5607 2024-05-17 13:05:58.000000 hgitaly-1.5.0/hgitaly/file_content.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      701 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/file_context.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4495 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/git.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7133 2024-05-18 12:05:55.000000 hgitaly-1.5.0/hgitaly/gitlab_ref.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.631772 hgitaly-1.5.0/hgitaly/license_detector/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4650 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/license_detector/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)   270608 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/license_detector/spdx-licenses.json
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.631772 hgitaly-1.5.0/hgitaly/linguist/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6420 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/linguist/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)   122122 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/linguist/languages.json
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1183 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/logging.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10350 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/manifest.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9596 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/message.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1506 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/oid.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      953 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/pagination.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1010 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/path.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3252 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/peer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      711 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/procutil.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8872 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7891 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/revision.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5689 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/revset.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.632772 hgitaly-1.5.0/hgitaly/server/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      417 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/server/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1683 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/server/address.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6288 2024-05-17 13:05:58.000000 hgitaly-1.5.0/hgitaly/server/mono.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7216 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/server/prefork.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.632772 hgitaly-1.5.0/hgitaly/server/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/server/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1256 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/server/tests/test_address.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3272 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/server/tests/test_mono.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6502 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/server/tests/test_prefork.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3704 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/server/tests/test_worker.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3748 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/server/worker.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.634772 hgitaly-1.5.0/hgitaly/service/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1787 2024-05-17 13:05:58.000000 hgitaly-1.5.0/hgitaly/service/analysis.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5013 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/blob.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    46662 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/commit.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    25147 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2217 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/interceptors.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1954 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/mercurial_changeset.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    16868 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/mercurial_operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7480 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/mercurial_repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9852 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    23474 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    35623 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      769 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/server.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.635772 hgitaly-1.5.0/hgitaly/service/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7380 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/fixture.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3972 2024-05-17 13:05:58.000000 hgitaly-1.5.0/hgitaly/service/tests/test_analysis.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4628 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_blob.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    52689 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_commit.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2020 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_default_branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    26417 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2973 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_mercurial_changeset.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    22959 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_mercurial_operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18968 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_mercurial_repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10594 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    22409 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    49404 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_repository_service.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      721 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/service/tests/test_server.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17084 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/servicer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1331 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/ssh.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5895 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stream.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.641772 hgitaly-1.5.0/hgitaly/stub/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2812 2024-05-17 13:05:58.000000 hgitaly-1.5.0/hgitaly/stub/analysis_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3419 2024-05-17 13:05:58.000000 hgitaly-1.5.0/hgitaly/stub/analysis_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9342 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/blob_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    12934 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/blob_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32146 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/commit_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    39150 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/commit_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    16478 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/diff_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15634 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/diff_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6477 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/errors_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/errors_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2922 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/lint_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/lint_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4218 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/mercurial_changeset_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2901 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/mercurial_changeset_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7531 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/mercurial_operations_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7995 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/mercurial_operations_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    11048 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/mercurial_repository_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17065 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/mercurial_repository_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29658 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/operations_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32883 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/operations_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    20829 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/ref_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29202 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/ref_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    47292 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/repository_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    79550 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/repository_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5080 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/server_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7231 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/server_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5996 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/shared_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/stub/shared_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1653 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tag.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.642772 hgitaly-1.5.0/hgitaly/testing/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      317 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/testing/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1278 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/testing/bundle.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2828 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/testing/context.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      901 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/testing/grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1147 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/testing/ssh.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3920 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/testing/sshd.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.642772 hgitaly-1.5.0/hgitaly/testing/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/testing/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1191 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/testing/tests/test_sshd.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.644772 hgitaly-1.5.0/hgitaly/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4609 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/common.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9403 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3605 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3778 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_errors.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2406 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_feature.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1439 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_file_context.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4932 2024-05-18 12:11:23.000000 hgitaly-1.5.0/hgitaly/tests/test_gitlab_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1495 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_license_detector.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1547 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_linguist.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5582 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_manifest.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3374 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_messages.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1114 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_oid.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1669 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_peer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      582 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6392 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_revision.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      679 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_revset.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10160 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_servicer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1951 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_stream.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1315 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_tag.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    24221 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/tests/test_workdir.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2017 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/util.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    14533 2024-05-01 16:09:12.000000 hgitaly-1.5.0/hgitaly/workdir.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.630772 hgitaly-1.5.0/hgitaly.egg-info/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15668 2024-05-18 14:06:03.000000 hgitaly-1.5.0/hgitaly.egg-info/PKG-INFO
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4680 2024-05-18 14:06:03.000000 hgitaly-1.5.0/hgitaly.egg-info/SOURCES.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        1 2024-05-18 14:06:03.000000 hgitaly-1.5.0/hgitaly.egg-info/dependency_links.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      151 2024-05-18 14:06:03.000000 hgitaly-1.5.0/hgitaly.egg-info/requires.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       35 2024-05-18 14:06:03.000000 hgitaly-1.5.0/hgitaly.egg-info/top_level.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      151 2024-05-01 16:09:12.000000 hgitaly-1.5.0/install-requirements.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       38 2024-05-18 14:06:03.646772 hgitaly-1.5.0/setup.cfg
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      968 2024-05-01 16:09:12.000000 hgitaly-1.5.0/setup.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-18 14:06:03.645772 hgitaly-1.5.0/tests_with_gitaly/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2437 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    24577 2024-05-18 11:58:42.000000 hgitaly-1.5.0/tests_with_gitaly/comparison.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3545 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/conftest.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2455 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/gitaly.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1775 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/hgitaly_rhgitaly_comparison.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2509 2024-05-18 13:40:58.000000 hgitaly-1.5.0/tests_with_gitaly/rhgitaly.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    25320 2024-05-17 13:05:58.000000 hgitaly-1.5.0/tests_with_gitaly/test_blob_tree.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    34125 2024-05-18 13:51:59.000000 hgitaly-1.5.0/tests_with_gitaly/test_commit.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3284 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/test_comparison.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29596 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/test_diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1371 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/test_gitaly_server.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    11653 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/test_operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17745 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/test_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32317 2024-05-17 18:28:22.000000 hgitaly-1.5.0/tests_with_gitaly/test_repository_service.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      941 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/test_rhgitaly_server.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      820 2024-05-01 16:09:12.000000 hgitaly-1.5.0/tests_with_gitaly/test_server.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.834704 hgitaly-1.6.0/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18092 2022-09-23 11:31:54.000000 hgitaly-1.6.0/LICENSE
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       33 2022-09-23 11:31:54.000000 hgitaly-1.6.0/MANIFEST.in
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15668 2024-05-22 11:16:33.833704 hgitaly-1.6.0/PKG-INFO
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15287 2024-03-07 11:59:14.000000 hgitaly-1.6.0/README.md
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.771703 hgitaly-1.6.0/hgext3rd/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      157 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgext3rd/__init__.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.772703 hgitaly-1.6.0/hgext3rd/hgitaly/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4418 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgext3rd/hgitaly/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1551 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgext3rd/hgitaly/revset.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.772703 hgitaly-1.6.0/hgext3rd/hgitaly/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgext3rd/hgitaly/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2021 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgext3rd/hgitaly/tests/test_revset.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5392 2023-02-11 11:25:44.000000 hgitaly-1.6.0/hgext3rd/hgitaly/tests/test_serve.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.785703 hgitaly-1.6.0/hgitaly/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        6 2024-05-22 11:16:03.000000 hgitaly-1.6.0/hgitaly/VERSION
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      361 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    13506 2023-07-30 07:54:28.000000 hgitaly-1.6.0/hgitaly/branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      744 2023-11-18 14:23:07.000000 hgitaly-1.6.0/hgitaly/changelog.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    13280 2024-03-25 19:47:19.000000 hgitaly-1.6.0/hgitaly/diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4985 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/errors.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2749 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgitaly/feature.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5607 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/file_content.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      701 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/file_context.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4495 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgitaly/git.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7133 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/gitlab_ref.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.787703 hgitaly-1.6.0/hgitaly/license_detector/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4650 2023-12-12 12:58:20.000000 hgitaly-1.6.0/hgitaly/license_detector/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)   270608 2023-12-12 12:58:20.000000 hgitaly-1.6.0/hgitaly/license_detector/spdx-licenses.json
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.790703 hgitaly-1.6.0/hgitaly/linguist/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6420 2023-09-25 08:12:33.000000 hgitaly-1.6.0/hgitaly/linguist/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)   122122 2023-09-25 08:12:33.000000 hgitaly-1.6.0/hgitaly/linguist/languages.json
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1183 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgitaly/logging.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10350 2023-09-25 08:37:11.000000 hgitaly-1.6.0/hgitaly/manifest.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9596 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgitaly/message.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1506 2024-03-25 19:47:19.000000 hgitaly-1.6.0/hgitaly/oid.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      953 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/pagination.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1010 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/path.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3252 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/peer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      711 2023-05-03 12:26:53.000000 hgitaly-1.6.0/hgitaly/procutil.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7973 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7891 2024-01-05 19:34:28.000000 hgitaly-1.6.0/hgitaly/revision.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5689 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgitaly/revset.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.793703 hgitaly-1.6.0/hgitaly/server/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      417 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/server/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1683 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/server/address.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6288 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/server/mono.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7216 2023-05-03 12:26:53.000000 hgitaly-1.6.0/hgitaly/server/prefork.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.795704 hgitaly-1.6.0/hgitaly/server/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/server/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1256 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/server/tests/test_address.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3272 2023-05-03 12:26:53.000000 hgitaly-1.6.0/hgitaly/server/tests/test_mono.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6502 2023-02-11 11:25:44.000000 hgitaly-1.6.0/hgitaly/server/tests/test_prefork.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3704 2023-02-11 11:25:44.000000 hgitaly-1.6.0/hgitaly/server/tests/test_worker.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3748 2023-02-11 11:25:44.000000 hgitaly-1.6.0/hgitaly/server/worker.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.799703 hgitaly-1.6.0/hgitaly/service/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/service/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1787 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/service/analysis.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5013 2023-09-25 08:12:33.000000 hgitaly-1.6.0/hgitaly/service/blob.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    47634 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/service/commit.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    25147 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgitaly/service/diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2217 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgitaly/service/interceptors.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1954 2022-10-27 17:19:53.000000 hgitaly-1.6.0/hgitaly/service/mercurial_changeset.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    16868 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/service/mercurial_operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7480 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgitaly/service/mercurial_repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9852 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/service/operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    23474 2024-03-25 19:49:12.000000 hgitaly-1.6.0/hgitaly/service/ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    33242 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/service/repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      769 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgitaly/service/server.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.806704 hgitaly-1.6.0/hgitaly/service/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/service/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7380 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/service/tests/fixture.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3972 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/service/tests/test_analysis.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4628 2023-09-25 08:12:33.000000 hgitaly-1.6.0/hgitaly/service/tests/test_blob.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    53225 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/service/tests/test_commit.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2020 2023-12-12 12:58:20.000000 hgitaly-1.6.0/hgitaly/service/tests/test_default_branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    26417 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgitaly/service/tests/test_diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2973 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/service/tests/test_mercurial_changeset.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    22959 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/service/tests/test_mercurial_operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18968 2024-01-07 12:13:06.000000 hgitaly-1.6.0/hgitaly/service/tests/test_mercurial_repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10594 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/service/tests/test_operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    22409 2024-03-25 19:49:12.000000 hgitaly-1.6.0/hgitaly/service/tests/test_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    45598 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/service/tests/test_repository_service.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      721 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/service/tests/test_server.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17084 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/servicer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1331 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/ssh.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5895 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgitaly/stream.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.819704 hgitaly-1.6.0/hgitaly/stub/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/stub/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2812 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/stub/analysis_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3419 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/stub/analysis_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9342 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/stub/blob_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    12934 2024-01-05 19:34:28.000000 hgitaly-1.6.0/hgitaly/stub/blob_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32146 2024-03-25 19:47:19.000000 hgitaly-1.6.0/hgitaly/stub/commit_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    39150 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/commit_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18818 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/stub/diff_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17269 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/stub/diff_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6477 2024-03-25 19:47:19.000000 hgitaly-1.6.0/hgitaly/stub/errors_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2022-10-27 17:19:53.000000 hgitaly-1.6.0/hgitaly/stub/errors_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2922 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/lint_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/stub/lint_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4218 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/mercurial_changeset_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2901 2022-10-27 17:19:53.000000 hgitaly-1.6.0/hgitaly/stub/mercurial_changeset_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7531 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/mercurial_operations_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7995 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/mercurial_operations_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    11048 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/mercurial_repository_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17065 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/mercurial_repository_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29692 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/stub/operations_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32883 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/operations_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    20829 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgitaly/stub/ref_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29202 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgitaly/stub/ref_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    45594 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/stub/repository_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    76171 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/stub/repository_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5080 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/server_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7231 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/server_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5996 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/shared_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/stub/shared_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1653 2023-07-30 07:54:28.000000 hgitaly-1.6.0/hgitaly/tag.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.821704 hgitaly-1.6.0/hgitaly/testing/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      317 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/testing/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1278 2023-02-11 11:25:44.000000 hgitaly-1.6.0/hgitaly/testing/bundle.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2828 2024-01-05 19:34:28.000000 hgitaly-1.6.0/hgitaly/testing/context.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      901 2023-05-03 12:26:53.000000 hgitaly-1.6.0/hgitaly/testing/grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1147 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/testing/ssh.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3920 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/testing/sshd.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.821704 hgitaly-1.6.0/hgitaly/testing/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/testing/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1191 2024-01-07 12:13:06.000000 hgitaly-1.6.0/hgitaly/testing/tests/test_sshd.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.827704 hgitaly-1.6.0/hgitaly/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4609 2024-01-05 19:34:28.000000 hgitaly-1.6.0/hgitaly/tests/common.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9403 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/tests/test_branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3605 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgitaly/tests/test_diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3778 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/tests/test_errors.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2406 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgitaly/tests/test_feature.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1439 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/tests/test_file_context.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4932 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/tests/test_gitlab_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1495 2023-12-12 12:58:20.000000 hgitaly-1.6.0/hgitaly/tests/test_license_detector.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1547 2023-12-12 12:58:20.000000 hgitaly-1.6.0/hgitaly/tests/test_linguist.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5582 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/tests/test_manifest.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3374 2023-02-11 11:25:44.000000 hgitaly-1.6.0/hgitaly/tests/test_messages.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1114 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/tests/test_oid.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1669 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/tests/test_peer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      582 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgitaly/tests/test_repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6392 2023-03-23 14:16:22.000000 hgitaly-1.6.0/hgitaly/tests/test_revision.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      679 2023-02-11 11:25:44.000000 hgitaly-1.6.0/hgitaly/tests/test_revset.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10160 2024-01-05 19:34:28.000000 hgitaly-1.6.0/hgitaly/tests/test_servicer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1951 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgitaly/tests/test_stream.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1315 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/tests/test_tag.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    24221 2024-01-05 19:34:28.000000 hgitaly-1.6.0/hgitaly/tests/test_workdir.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2017 2023-09-25 08:12:33.000000 hgitaly-1.6.0/hgitaly/util.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    14533 2024-01-05 19:34:28.000000 hgitaly-1.6.0/hgitaly/workdir.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.786703 hgitaly-1.6.0/hgitaly.egg-info/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15668 2024-05-22 11:16:33.000000 hgitaly-1.6.0/hgitaly.egg-info/PKG-INFO
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4680 2024-05-22 11:16:33.000000 hgitaly-1.6.0/hgitaly.egg-info/SOURCES.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        1 2024-05-22 11:16:33.000000 hgitaly-1.6.0/hgitaly.egg-info/dependency_links.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      151 2024-05-22 11:16:33.000000 hgitaly-1.6.0/hgitaly.egg-info/requires.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       35 2024-05-22 11:16:33.000000 hgitaly-1.6.0/hgitaly.egg-info/top_level.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      151 2024-02-09 22:39:22.000000 hgitaly-1.6.0/install-requirements.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       38 2024-05-22 11:16:33.834704 hgitaly-1.6.0/setup.cfg
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      968 2023-12-12 12:58:20.000000 hgitaly-1.6.0/setup.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.833704 hgitaly-1.6.0/tests_with_gitaly/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2437 2023-07-05 15:04:47.000000 hgitaly-1.6.0/tests_with_gitaly/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    24858 2024-05-22 11:15:45.000000 hgitaly-1.6.0/tests_with_gitaly/comparison.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3545 2023-05-03 12:26:53.000000 hgitaly-1.6.0/tests_with_gitaly/conftest.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2455 2023-07-05 15:04:47.000000 hgitaly-1.6.0/tests_with_gitaly/gitaly.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1775 2023-05-03 12:26:53.000000 hgitaly-1.6.0/tests_with_gitaly/hgitaly_rhgitaly_comparison.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2509 2024-03-10 13:55:24.000000 hgitaly-1.6.0/tests_with_gitaly/rhgitaly.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    25541 2024-05-22 11:15:45.000000 hgitaly-1.6.0/tests_with_gitaly/test_blob_tree.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    34125 2024-05-20 13:45:11.000000 hgitaly-1.6.0/tests_with_gitaly/test_commit.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3284 2023-07-05 15:04:47.000000 hgitaly-1.6.0/tests_with_gitaly/test_comparison.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29596 2024-03-25 19:47:19.000000 hgitaly-1.6.0/tests_with_gitaly/test_diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1371 2022-10-27 17:19:53.000000 hgitaly-1.6.0/tests_with_gitaly/test_gitaly_server.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    11653 2024-02-09 22:39:22.000000 hgitaly-1.6.0/tests_with_gitaly/test_operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17745 2024-03-25 19:49:12.000000 hgitaly-1.6.0/tests_with_gitaly/test_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29926 2024-05-22 11:15:45.000000 hgitaly-1.6.0/tests_with_gitaly/test_repository_service.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      941 2023-05-03 12:26:53.000000 hgitaly-1.6.0/tests_with_gitaly/test_rhgitaly_server.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      820 2023-05-03 12:26:53.000000 hgitaly-1.6.0/tests_with_gitaly/test_server.py
```

### Comparing `hgitaly-1.5.0/LICENSE` & `hgitaly-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/PKG-INFO` & `hgitaly-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgitaly
-Version: 1.5.0
+Version: 1.6.0
 Summary: Server-side implementation of Gitaly protocol for Mercurial
 Home-page: https://foss.heptapod.net/heptapod/hgitaly
 Author: Georges Racinet
 Author-email: georges.racinet@octobus.net
 License: GPLv2+
 Keywords: hg mercurial heptapod gitlab
 Requires-Python: >=3.8
```

### Comparing `hgitaly-1.5.0/README.md` & `hgitaly-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgext3rd/hgitaly/__init__.py` & `hgitaly-1.6.0/hgext3rd/hgitaly/__init__.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgext3rd/hgitaly/revset.py` & `hgitaly-1.6.0/hgext3rd/hgitaly/revset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgext3rd/hgitaly/tests/test_revset.py` & `hgitaly-1.6.0/hgext3rd/hgitaly/tests/test_revset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgext3rd/hgitaly/tests/test_serve.py` & `hgitaly-1.6.0/hgext3rd/hgitaly/tests/test_serve.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/branch.py` & `hgitaly-1.6.0/hgitaly/branch.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/changelog.py` & `hgitaly-1.6.0/hgitaly/changelog.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/diff.py` & `hgitaly-1.6.0/hgitaly/diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/errors.py` & `hgitaly-1.6.0/hgitaly/errors.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/feature.py` & `hgitaly-1.6.0/hgitaly/feature.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/file_content.py` & `hgitaly-1.6.0/hgitaly/file_content.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/file_context.py` & `hgitaly-1.6.0/hgitaly/file_context.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/git.py` & `hgitaly-1.6.0/hgitaly/git.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/gitlab_ref.py` & `hgitaly-1.6.0/hgitaly/gitlab_ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/license_detector/__init__.py` & `hgitaly-1.6.0/hgitaly/license_detector/__init__.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/license_detector/spdx-licenses.json` & `hgitaly-1.6.0/hgitaly/license_detector/spdx-licenses.json`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/linguist/__init__.py` & `hgitaly-1.6.0/hgitaly/linguist/__init__.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/linguist/languages.json` & `hgitaly-1.6.0/hgitaly/linguist/languages.json`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/logging.py` & `hgitaly-1.6.0/hgitaly/logging.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/manifest.py` & `hgitaly-1.6.0/hgitaly/manifest.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/message.py` & `hgitaly-1.6.0/hgitaly/message.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/oid.py` & `hgitaly-1.6.0/hgitaly/oid.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/pagination.py` & `hgitaly-1.6.0/hgitaly/pagination.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/path.py` & `hgitaly-1.6.0/hgitaly/path.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/peer.py` & `hgitaly-1.6.0/hgitaly/peer.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/procutil.py` & `hgitaly-1.6.0/hgitaly/procutil.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/repository.py` & `hgitaly-1.6.0/hgitaly/repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,42 +35,14 @@
     b'without-topic': AutoPublish.WITHOUT_TOPIC,
     b'nothing': AutoPublish.NOTHING,
     b'all': AutoPublish.ALL,
 }
 AUTO_PUBLISH_REVERSE_MAPPING = {v: k for k, v in AUTO_PUBLISH_MAPPING.items()}
 
 
-def set_gitlab_project_full_path(repo, full_path: bytes):
-    """Store information about the full path of GitLab Project.
-
-    In GitLab terminology, ``full_path`` is the URI path, while ``path``
-    its the last segment of ``full_path``.
-
-    In Git repositories, this is stored in config. We could as well use
-    the repo-local hgrcs, but it is simpler to use a dedicated file, and
-    it makes sense to consider it not part of ``store`` (``svfs``), same
-    as ``hgrc``.
-    """
-    with repo.wlock():
-        repo.vfs.write(GITLAB_PROJECT_FULL_PATH_FILENAME, full_path)
-
-
-def get_gitlab_project_full_path(repo):
-    """Get the full path of GitLab Project.
-
-    See also :func:`set_gitlab_project_full_path`.
-
-    :return: the full path, or ``None`` if not set.
-    """
-    try:
-        return repo.vfs.read(GITLAB_PROJECT_FULL_PATH_FILENAME)
-    except FileNotFoundError:
-        return None
-
-
 def unbundle(repo, bundle_path: str, rails_sync=False):
     """Call unbundle with proper options and conversions.
 
     :param bool rails_sync: if ``True``, let the synchronization with the
        Rails app proceed (conversion to Git if needed, pre/post-receive hooks,
        etc.)
     """
```

### Comparing `hgitaly-1.5.0/hgitaly/revision.py` & `hgitaly-1.6.0/hgitaly/revision.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/revset.py` & `hgitaly-1.6.0/hgitaly/revset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/server/address.py` & `hgitaly-1.6.0/hgitaly/server/address.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/server/mono.py` & `hgitaly-1.6.0/hgitaly/server/mono.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/server/prefork.py` & `hgitaly-1.6.0/hgitaly/server/prefork.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/server/tests/test_address.py` & `hgitaly-1.6.0/hgitaly/server/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/server/tests/test_mono.py` & `hgitaly-1.6.0/hgitaly/server/tests/test_mono.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/server/tests/test_prefork.py` & `hgitaly-1.6.0/hgitaly/server/tests/test_prefork.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/server/tests/test_worker.py` & `hgitaly-1.6.0/hgitaly/server/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/server/worker.py` & `hgitaly-1.6.0/hgitaly/server/worker.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/analysis.py` & `hgitaly-1.6.0/hgitaly/service/analysis.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/blob.py` & `hgitaly-1.6.0/hgitaly/service/blob.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/commit.py` & `hgitaly-1.6.0/hgitaly/service/commit.py`

 * *Files 1% similar despite different names*

```diff
@@ -431,14 +431,39 @@
             # the risk.
             # Also would be neat to avoid consuming the iterator into
             # a least, but is it worth the added complexity if it can't
             # be done in the TREES_FIRST case?
             # What if GitLab introduces a sort direction anyway ?
             entries = sorted(entries)  # sorts lexicographically by path
 
+        if not entries:
+            # there is no such thing as an empty directory in Mercurial
+            try:
+                changeset.filectx(path)
+            except error.ManifestLookupError:
+                if request.recursive:
+                    err_code = StatusCode.NOT_FOUND
+                else:
+                    err_code = StatusCode.INVALID_ARGUMENT
+                structured_abort(
+                    context,
+                    err_code,
+                    "invalid revision or path",
+                    GetTreeEntriesError(resolve_tree=ResolveRevisionError(
+                        revision=request.revision))
+                )
+            else:
+                structured_abort(
+                    context,
+                    StatusCode.INVALID_ARGUMENT,
+                    "path not treeish",
+                    GetTreeEntriesError(resolve_tree=ResolveRevisionError(
+                        revision=request.revision))
+                )
+
         def entry_oid(path, is_dir):
             return (tree_oid if is_dir else blob_oid)(repo, sha, path)
 
         page_token = request.pagination_params.page_token
         if page_token:
             for offset, (path, is_dir, _) in enumerate(entries):
                 if entry_oid(path, is_dir) == page_token:
```

### Comparing `hgitaly-1.5.0/hgitaly/service/diff.py` & `hgitaly-1.6.0/hgitaly/service/diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/interceptors.py` & `hgitaly-1.6.0/hgitaly/service/interceptors.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/mercurial_changeset.py` & `hgitaly-1.6.0/hgitaly/service/mercurial_changeset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/mercurial_operations.py` & `hgitaly-1.6.0/hgitaly/service/mercurial_operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/mercurial_repository.py` & `hgitaly-1.6.0/hgitaly/service/mercurial_repository.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/operations.py` & `hgitaly-1.6.0/hgitaly/service/operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/ref.py` & `hgitaly-1.6.0/hgitaly/service/ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/repository.py` & `hgitaly-1.6.0/hgitaly/service/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 # SPDX-License-Identifier: GPL-2.0-or-later
 import gc
 from grpc import StatusCode
 from io import BytesIO
 import itertools
 import logging
 import os
-from pathlib import Path
 from collections import deque
 import re
 import shutil
 import tempfile
 import time
 
 from mercurial import (
@@ -57,17 +56,15 @@
 from ..license_detector import detect_license
 from ..logging import LoggerAdapter
 from ..path import (
     InvalidPath,
     validate_relative_path,
 )
 from ..repository import (
-    get_gitlab_project_full_path,
     repo_size,
-    set_gitlab_project_full_path,
     unbundle,
 )
 from ..revision import (
     ALL_CHANGESETS,
     CHANGESET_HASH_BYTES_REGEXP,
     ZERO_SHA,
     RevisionNotFound,
@@ -100,44 +97,38 @@
     CreateRepositoryFromBundleResponse,
     FetchBundleRequest,
     FetchBundleResponse,
     FindLicenseRequest,
     FindLicenseResponse,
     FindMergeBaseRequest,
     FindMergeBaseResponse,
-    FullPathRequest,
-    FullPathResponse,
     GetRawChangesRequest,
     GetRawChangesResponse,
     GetCustomHooksRequest,
     GetCustomHooksResponse,
     RepositoryExistsRequest,
     RepositoryExistsResponse,
     GetArchiveRequest,
     GetArchiveResponse,
     HasLocalBranchesRequest,
     HasLocalBranchesResponse,
     ObjectFormatRequest,
     ObjectFormatResponse,
-    RemoveAllRequest,
-    RemoveAllResponse,
     RemoveRepositoryRequest,
     RemoveRepositoryResponse,
     RepositorySizeRequest,
     RepositorySizeResponse,
     RestoreCustomHooksRequest,
     RestoreCustomHooksResponse,
     SearchFilesByContentRequest,
     SearchFilesByContentResponse,
     SearchFilesByNameRequest,
     SearchFilesByNameResponse,
     SetCustomHooksRequest,
     SetCustomHooksResponse,
-    SetFullPathRequest,
-    SetFullPathResponse,
     WriteRefRequest,
     WriteRefResponse,
     ApplyGitattributesRequest,
     ApplyGitattributesResponse,
 )
 from ..stub.repository_pb2_grpc import RepositoryServiceServicer
 from ..stub.shared_pb2 import (
@@ -615,36 +606,14 @@
         # at this point, the repo officially does not exist any more, the
         # roster file does not matter, cleanup workdirs if any.
         remove_all_workdirs_bare(self.repo_workdirs_root(request.repository,
                                                          context))
         shutil.rmtree(trash_path)
         return RemoveRepositoryResponse()
 
-    def SetFullPath(self, request: SetFullPathRequest,
-                    context) -> SetFullPathResponse:
-        repo = self.load_repo(request.repository, context)
-
-        if not request.path:
-            context.abort(StatusCode.INVALID_ARGUMENT, "no path provided")
-
-        set_gitlab_project_full_path(repo, request.path.encode('utf-8'))
-        return SetFullPathResponse()
-
-    def FullPath(self, request: FullPathRequest,
-                 context) -> FullPathResponse:
-        repo = self.load_repo(request.repository, context)
-
-        path = get_gitlab_project_full_path(repo)
-        if not path:  # None or (not probable) empty string
-            # Gitaly simply returns the `git config` stderr output for now.
-            # Pretty ridiculous to mimick it, we can hope not much to
-            # depend on it.
-            context.abort(StatusCode.INTERNAL, "Full path not set")
-        return FullPathResponse(path=path)
-
     def CreateBundle(self, request: CreateBundleRequest,
                      context) -> CreateBundleResponse:
         repo = self.load_repo(request.repository, context).unfiltered()
         yield from self.gen_bundle_responses(CreateBundleResponse, repo,
                                              all=True)
 
     def gen_bundle_responses(self, response_class, repo, **bundle_opts):
@@ -788,45 +757,14 @@
             license_short_name=detected['spdx_id'],
             license_name=detected.get('full_name'),
             license_path=detected.get('file'),
             license_url=detected.get('url'),
             license_nickname=detected.get('nickname'),
         )
 
-    def RemoveAll(self, request: RemoveAllRequest,
-                  context) -> RemoveAllResponse:
-        """Remove everything in the given storage.
-
-        This is exactly what Gitaly v15.9 does, hence including all temporary
-        files etc.
-        """
-        storage = request.storage_name
-        root_dir = self.storages.get(storage)
-        if root_dir is None:
-            context.abort(
-                StatusCode.INVALID_ARGUMENT,
-                'remove all: storage not found: "%s"' % storage
-            )
-
-        root_dir = Path(os.fsdecode(root_dir)).resolve()
-        # it would obviously be simpler to use shutil.rmtree() on root_dir
-        # and recreate the storage afterwards *but*
-        # - permission not guaranteed on the root dir
-        # - risky on error recovery
-        try:
-            for sub in root_dir.iterdir():
-                if sub.is_dir() and not sub.is_symlink():
-                    shutil.rmtree(sub)
-                else:
-                    # also works with broken symlinks (even loops)
-                    sub.unlink()
-        except Exception as exc:
-            context.abort(StatusCode.INTERNAL, "remove all: %s" % exc)
-        return RemoveAllResponse()
-
 
 def render_git_grep_matches(buf, ref, path, enum_lines):
     """Render a slice of lines as git grep does.
 
     :param enum_lines: iterable of pairs `(line_no, line)`
     """
     for lineno, line in enum_lines:
```

### Comparing `hgitaly-1.5.0/hgitaly/service/server.py` & `hgitaly-1.6.0/hgitaly/service/server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/tests/fixture.py` & `hgitaly-1.6.0/hgitaly/service/tests/fixture.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/tests/test_analysis.py` & `hgitaly-1.6.0/hgitaly/service/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/tests/test_blob.py` & `hgitaly-1.6.0/hgitaly/service/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/tests/test_commit.py` & `hgitaly-1.6.0/hgitaly/service/tests/test_commit.py`

 * *Files 0% similar despite different names*

```diff
@@ -996,14 +996,26 @@
 
     with pytest.raises(grpc.RpcError) as exc_info:
         get_tree_entries(b'', revision=sha1)
     assert exc_info.value.code() == grpc.StatusCode.INVALID_ARGUMENT
     assert 'empty path' in exc_info.value.details()
 
     with pytest.raises(grpc.RpcError) as exc_info:
+        get_tree_entries(b'sub/bar', revision=sha1)
+    assert exc_info.value.code() == grpc.StatusCode.INVALID_ARGUMENT
+
+    with pytest.raises(grpc.RpcError) as exc_info:
+        get_tree_entries(b'no-such-dir', revision=sha1)
+    assert exc_info.value.code() == grpc.StatusCode.INVALID_ARGUMENT
+
+    with pytest.raises(grpc.RpcError) as exc_info:
+        get_tree_entries(b'no-such-dir', revision=sha1, recursive=True)
+    assert exc_info.value.code() == grpc.StatusCode.NOT_FOUND
+
+    with pytest.raises(grpc.RpcError) as exc_info:
         get_tree_entries(b'.', revision=b'unknown')
     assert exc_info.value.code() == grpc.StatusCode.INVALID_ARGUMENT
     assert 'invalid revision' in exc_info.value.details()
 
     assert get_tree_entries(b'sub', revision=sha1) == ([ba2_default,
                                                         bar_default], '')
```

### Comparing `hgitaly-1.5.0/hgitaly/service/tests/test_default_branch.py` & `hgitaly-1.6.0/hgitaly/service/tests/test_default_branch.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/tests/test_diff.py` & `hgitaly-1.6.0/hgitaly/service/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/tests/test_mercurial_changeset.py` & `hgitaly-1.6.0/hgitaly/service/tests/test_mercurial_changeset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/tests/test_mercurial_operations.py` & `hgitaly-1.6.0/hgitaly/service/tests/test_mercurial_operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/tests/test_mercurial_repository.py` & `hgitaly-1.6.0/hgitaly/service/tests/test_mercurial_repository.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/tests/test_operations.py` & `hgitaly-1.6.0/hgitaly/service/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/tests/test_ref.py` & `hgitaly-1.6.0/hgitaly/service/tests/test_ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/service/tests/test_repository_service.py` & `hgitaly-1.6.0/hgitaly/service/tests/test_repository_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,14 @@
     create_keep_around,
     iter_keep_arounds,
 )
 
 from mercurial_testhelpers import RepoWrapper
 
 from hgitaly.license_detector import license_content
-from hgitaly.repository import (
-    GITLAB_PROJECT_FULL_PATH_FILENAME,
-)
 from hgitaly.revision import ZERO_SHA
 from hgitaly.stream import WRITE_BUFFER_SIZE
 from hgitaly.testing import TEST_DATA_DIR
 from hgitaly.testing.bundle import list_bundle_contents
 from hgitaly.workdir import (
     ROSTER_FILE_NAME as WDS_ROSTER_FILE_NAME,
     working_directory,
@@ -54,28 +51,25 @@
     CreateRepositoryFromBundleRequest,
     CreateRepositoryRequest,
     CreateBundleFromRefListRequest,
     FetchBundleRequest,
     FindLicenseRequest,
     FindLicenseResponse,
     FindMergeBaseRequest,
-    FullPathRequest,
     GetArchiveRequest,
     GetCustomHooksRequest,
     HasLocalBranchesRequest,
     ObjectFormatRequest,
-    RemoveAllRequest,
     RemoveRepositoryRequest,
     RepositoryExistsRequest,
     RepositorySizeRequest,
     RestoreCustomHooksRequest,
     SearchFilesByNameRequest,
     SearchFilesByContentRequest,
     SearchFilesByContentResponse,
-    SetFullPathRequest,
     SetCustomHooksRequest,
     WriteRefRequest,
 )
 from hgitaly.stub.repository_pb2_grpc import RepositoryServiceStub
 from hgitaly.stub.shared_pb2 import (
     ObjectFormat,
 )
@@ -227,27 +221,14 @@
     def remove_repository(self, grpc_repo=None):
         if grpc_repo is None:
             grpc_repo = self.grpc_repo
 
         return self.stub.RemoveRepository(RemoveRepositoryRequest(
             repository=grpc_repo))
 
-    def set_full_path(self, path, grpc_repo=None):
-        if grpc_repo is None:
-            grpc_repo = self.grpc_repo
-
-        return self.stub.SetFullPath(SetFullPathRequest(repository=grpc_repo,
-                                                        path=path))
-
-    def full_path(self, grpc_repo=None):
-        if grpc_repo is None:
-            grpc_repo = self.grpc_repo
-
-        return self.stub.FullPath(FullPathRequest(repository=grpc_repo)).path
-
     def object_format(self, **kw):
         grpc_repo = kw.pop('grpc_repo', self.grpc_repo)
         return self.stub.ObjectFormat(ObjectFormatRequest(repository=grpc_repo,
                                                           **kw))
 
     def create_bundle(self, save_path):
         with open(save_path, 'wb') as fobj:
@@ -293,17 +274,14 @@
                 yield CreateBundleFromRefListRequest(**req_args)
 
         with open(bundle_path, 'wb') as fobj:
             for chunk in self.stub.CreateBundleFromRefList(
                     get_request_iter(ref_patterns)):
                 fobj.write(chunk.data)
 
-    def remove_all(self, storage_name):
-        return self.stub.RemoveAll(RemoveAllRequest(storage_name=storage_name))
-
     def assert_compare_repos(self, target_repo_path):
         """Compare the fixture repo with another one.
         """
         wrapper = self.repo_wrapper
         orig = wrapper.repo.unfiltered()
         target = self.make_repo_wrapper(target_repo_path).repo.unfiltered()
         for rev_str in ('draft()', 'public()', 'obsolete()'):
@@ -928,71 +906,14 @@
     # missing repo argument
     fixture.grpc_repo = None
     with pytest.raises(grpc.RpcError) as exc_info:
         fixture.remove_repository(grpc_repo=None)
     assert exc_info.value.code() == INVALID_ARGUMENT
 
 
-def test_set_full_path(fixture_with_repo):
-    fixture = fixture_with_repo
-    wrapper = fixture.repo_wrapper
-    grpc_repo = fixture.grpc_repo
-
-    def assert_full_path(expected):
-        assert (wrapper.path / '.hg'
-                / GITLAB_PROJECT_FULL_PATH_FILENAME.decode('ascii')
-                ).read_text(encoding='utf-8') == expected
-        assert fixture.full_path() == expected
-
-    def call_then_assert(full_path):
-        fixture.set_full_path(full_path)
-        assert_full_path(full_path)
-
-    def call_then_assert_error(full_path, error_code, grpc_repo=grpc_repo):
-        with pytest.raises(grpc.RpcError) as exc_info:
-            fixture.set_full_path(full_path, grpc_repo=grpc_repo)
-        assert exc_info.value.code() == error_code
-
-    call_then_assert('group/proj')
-    call_then_assert('accent-lovers/projé')
-    call_then_assert('group/subgroup/proj')
-
-    call_then_assert_error('', INVALID_ARGUMENT)
-    call_then_assert_error('some/path', NOT_FOUND,
-                           grpc_repo=Repository(
-                               storage_name=grpc_repo.storage_name,
-                               relative_path='no/such/repo'))
-    call_then_assert_error('some/path', INVALID_ARGUMENT,
-                           grpc_repo=Repository(
-                               relative_path=grpc_repo.relative_path,
-                               storage_name='unknown'))
-
-
-def test_full_path_errors(fixture_with_repo):
-    fixture = fixture_with_repo
-    grpc_repo = fixture.grpc_repo
-
-    def call_then_assert_error(error_code, grpc_repo=None):
-        with pytest.raises(grpc.RpcError) as exc_info:
-            fixture.full_path(grpc_repo=grpc_repo)
-        assert exc_info.value.code() == error_code
-
-    # existing repo, but full path not set
-    call_then_assert_error(INTERNAL)
-
-    call_then_assert_error(NOT_FOUND,
-                           grpc_repo=Repository(
-                               storage_name=grpc_repo.storage_name,
-                               relative_path='no/such/repo'))
-    call_then_assert_error(INVALID_ARGUMENT,
-                           grpc_repo=Repository(
-                               relative_path=grpc_repo.relative_path,
-                               storage_name='unknown'))
-
-
 def test_fetch_bundle(fixture_with_repo, tmpdir):
     fixture = fixture_with_repo
     wrapper = fixture.repo_wrapper
 
     target_repo_path, target_repo_msg = fixture.additional_repo('target_repo')
 
     # first call will create the repo
@@ -1300,33 +1221,11 @@
     nested.commit_file("bar", content="in nested")
     (wrapper.path / '.hgsub').write_bytes(b"nested = nested\n")
     wrapper.command(b'add', subrepos=True)
     wrapper.command(b'commit', subrepos=True, message=b"invalid")
     assert find_license() == FindLicenseResponse()
 
 
-def test_remove_all(fixture_with_repo):
-    fixture = fixture_with_repo
-    storage_path = fixture.storage_path('default')
-    (storage_path / 'foo').write_bytes(b'something')
-    (storage_path / 'bar').symlink_to('foo')
-    (storage_path / 'broken').symlink_to('missing')
-    fixture.remove_all(storage_name='default')
-
-    assert list(storage_path.iterdir()) == []
-
-    with pytest.raises(grpc.RpcError) as exc_info:
-        fixture.remove_all(storage_name='unknown')
-    assert exc_info.value.code() == INVALID_ARGUMENT
-
-    storage_path.rmdir()  # create error condition by removing the root dir
-    with pytest.raises(grpc.RpcError) as exc_info:
-        fixture.remove_all(storage_name='default')
-    exc = exc_info.value
-    assert exc.code() == INTERNAL
-    assert "No such file or directory: '%s'" % storage_path in exc.details()
-
-
 def test_object_format(fixture_with_repo):
     fixture = fixture_with_repo
     assert (fixture.object_format().format
             == ObjectFormat.OBJECT_FORMAT_UNSPECIFIED)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hgitaly-1.5.0/hgitaly/service/tests/test_server.py` & `hgitaly-1.6.0/hgitaly/service/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/servicer.py` & `hgitaly-1.6.0/hgitaly/servicer.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/ssh.py` & `hgitaly-1.6.0/hgitaly/ssh.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stream.py` & `hgitaly-1.6.0/hgitaly/stream.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/analysis_pb2.py` & `hgitaly-1.6.0/hgitaly/stub/analysis_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/analysis_pb2_grpc.py` & `hgitaly-1.6.0/hgitaly/stub/analysis_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/blob_pb2.py` & `hgitaly-1.6.0/hgitaly/stub/blob_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/blob_pb2_grpc.py` & `hgitaly-1.6.0/hgitaly/stub/blob_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/commit_pb2.py` & `hgitaly-1.6.0/hgitaly/stub/commit_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/commit_pb2_grpc.py` & `hgitaly-1.6.0/hgitaly/stub/commit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/diff_pb2.py` & `hgitaly-1.6.0/hgitaly/stub/diff_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import lint_pb2 as lint__pb2
 from . import shared_pb2 as shared__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\ndiff.proto\x12\x06gitaly\x1a\nlint.proto\x1a\x0cshared.proto\"\xd8\x06\n\x11\x43ommitDiffRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\x12\r\n\x05paths\x18\x05 \x03(\x0c\x12\x16\n\x0e\x63ollapse_diffs\x18\x06 \x01(\x08\x12\x16\n\x0e\x65nforce_limits\x18\x07 \x01(\x08\x12\x11\n\tmax_files\x18\x08 \x01(\x05\x12\x11\n\tmax_lines\x18\t \x01(\x05\x12\x11\n\tmax_bytes\x18\n \x01(\x05\x12\x17\n\x0fmax_patch_bytes\x18\x0e \x01(\x05\x12\x16\n\x0esafe_max_files\x18\x0b \x01(\x05\x12\x16\n\x0esafe_max_lines\x18\x0c \x01(\x05\x12\x16\n\x0esafe_max_bytes\x18\r \x01(\x05\x12\x35\n\tdiff_mode\x18\x0f \x01(\x0e\x32\".gitaly.CommitDiffRequest.DiffMode\x12h\n\"max_patch_bytes_for_file_extension\x18\x10 \x03(\x0b\x32<.gitaly.CommitDiffRequest.MaxPatchBytesForFileExtensionEntry\x12G\n\x12whitespace_changes\x18\x11 \x01(\x0e\x32+.gitaly.CommitDiffRequest.WhitespaceChanges\x12\x19\n\x11\x63ollect_all_paths\x18\x12 \x01(\x08\x1a\x44\n\"MaxPatchBytesForFileExtensionEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"%\n\x08\x44iffMode\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x0c\n\x08WORDDIFF\x10\x01\"y\n\x11WhitespaceChanges\x12\"\n\x1eWHITESPACE_CHANGES_UNSPECIFIED\x10\x00\x12\x1d\n\x19WHITESPACE_CHANGES_IGNORE\x10\x01\x12!\n\x1dWHITESPACE_CHANGES_IGNORE_ALL\x10\x02J\x04\x08\x04\x10\x05R\x18ignore_whitespace_change\"\xff\x01\n\x12\x43ommitDiffResponse\x12\x11\n\tfrom_path\x18\x01 \x01(\x0c\x12\x0f\n\x07to_path\x18\x02 \x01(\x0c\x12\x0f\n\x07\x66rom_id\x18\x03 \x01(\t\x12\r\n\x05to_id\x18\x04 \x01(\t\x12\x10\n\x08old_mode\x18\x05 \x01(\x05\x12\x10\n\x08new_mode\x18\x06 \x01(\x05\x12\x0e\n\x06\x62inary\x18\x07 \x01(\x08\x12\x16\n\x0eraw_patch_data\x18\t \x01(\x0c\x12\x14\n\x0c\x65nd_of_patch\x18\n \x01(\x08\x12\x17\n\x0foverflow_marker\x18\x0b \x01(\x08\x12\x11\n\tcollapsed\x18\x0c \x01(\x08\x12\x11\n\ttoo_large\x18\r \x01(\x08J\x04\x08\x08\x10\t\"\x82\x01\n\x12\x43ommitDeltaRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\x12\r\n\x05paths\x18\x04 \x03(\x0c\"u\n\x0b\x43ommitDelta\x12\x11\n\tfrom_path\x18\x01 \x01(\x0c\x12\x0f\n\x07to_path\x18\x02 \x01(\x0c\x12\x0f\n\x07\x66rom_id\x18\x03 \x01(\t\x12\r\n\x05to_id\x18\x04 \x01(\t\x12\x10\n\x08old_mode\x18\x05 \x01(\x05\x12\x10\n\x08new_mode\x18\x06 \x01(\x05\":\n\x13\x43ommitDeltaResponse\x12#\n\x06\x64\x65ltas\x18\x01 \x03(\x0b\x32\x13.gitaly.CommitDelta\"o\n\x0eRawDiffRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\"\x1f\n\x0fRawDiffResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"p\n\x0fRawPatchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\" \n\x10RawPatchResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"q\n\x10\x44iffStatsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\"Q\n\tDiffStats\x12\x0c\n\x04path\x18\x01 \x01(\x0c\x12\x11\n\tadditions\x18\x02 \x01(\x05\x12\x11\n\tdeletions\x18\x03 \x01(\x05\x12\x10\n\x08old_path\x18\x04 \x01(\x0c\"5\n\x11\x44iffStatsResponse\x12 \n\x05stats\x18\x01 \x03(\x0b\x32\x11.gitaly.DiffStats\"\xc4\x05\n\x17\x46indChangedPathsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x13\n\x07\x63ommits\x18\x02 \x03(\tB\x02\x18\x01\x12\x39\n\x08requests\x18\x03 \x03(\x0b\x32\'.gitaly.FindChangedPathsRequest.Request\x12S\n\x16merge_commit_diff_mode\x18\x04 \x01(\x0e\x32\x33.gitaly.FindChangedPathsRequest.MergeCommitDiffMode\x1a\xc2\x02\n\x07Request\x12K\n\x0ctree_request\x18\x01 \x01(\x0b\x32\x33.gitaly.FindChangedPathsRequest.Request.TreeRequestH\x00\x12O\n\x0e\x63ommit_request\x18\x02 \x01(\x0b\x32\x35.gitaly.FindChangedPathsRequest.Request.CommitRequestH\x00\x1a\x46\n\x0bTreeRequest\x12\x1a\n\x12left_tree_revision\x18\x01 \x01(\t\x12\x1b\n\x13right_tree_revision\x18\x02 \x01(\t\x1aI\n\rCommitRequest\x12\x17\n\x0f\x63ommit_revision\x18\x01 \x01(\t\x12\x1f\n\x17parent_commit_revisions\x18\x02 \x03(\tB\x06\n\x04type\"\x90\x01\n\x13MergeCommitDiffMode\x12&\n\"MERGE_COMMIT_DIFF_MODE_UNSPECIFIED\x10\x00\x12)\n%MERGE_COMMIT_DIFF_MODE_INCLUDE_MERGES\x10\x01\x12&\n\"MERGE_COMMIT_DIFF_MODE_ALL_PARENTS\x10\x02\"?\n\x18\x46indChangedPathsResponse\x12#\n\x05paths\x18\x01 \x03(\x0b\x32\x14.gitaly.ChangedPaths\"\xe4\x01\n\x0c\x43hangedPaths\x12\x0c\n\x04path\x18\x01 \x01(\x0c\x12+\n\x06status\x18\x02 \x01(\x0e\x32\x1b.gitaly.ChangedPaths.Status\x12\x10\n\x08old_mode\x18\x03 \x01(\x05\x12\x10\n\x08new_mode\x18\x04 \x01(\x05\x12\x13\n\x0bold_blob_id\x18\x05 \x01(\t\x12\x13\n\x0bnew_blob_id\x18\x06 \x01(\t\"K\n\x06Status\x12\t\n\x05\x41\x44\x44\x45\x44\x10\x00\x12\x0c\n\x08MODIFIED\x10\x01\x12\x0b\n\x07\x44\x45LETED\x10\x02\x12\x0f\n\x0bTYPE_CHANGE\x10\x03\x12\n\n\x06\x43OPIED\x10\x04\"m\n\x11GetPatchIDRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x14\n\x0cold_revision\x18\x02 \x01(\x0c\x12\x14\n\x0cnew_revision\x18\x03 \x01(\x0c\"&\n\x12GetPatchIDResponse\x12\x10\n\x08patch_id\x18\x01 \x01(\t\"+\n\tRangePair\x12\x0e\n\x06range1\x18\x01 \x01(\t\x12\x0e\n\x06range2\x18\x02 \x01(\t\"+\n\rRevisionRange\x12\x0c\n\x04rev1\x18\x01 \x01(\t\x12\x0c\n\x04rev2\x18\x02 \x01(\t\"=\n\x11\x42\x61seWithRevisions\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\x12\x0c\n\x04rev1\x18\x02 \x01(\t\x12\x0c\n\x04rev2\x18\x03 \x01(\t\"\xe5\x01\n\x13RawRangeDiffRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\'\n\nrange_pair\x18\x02 \x01(\x0b\x32\x11.gitaly.RangePairH\x00\x12/\n\x0erevision_range\x18\x03 \x01(\x0b\x32\x15.gitaly.RevisionRangeH\x00\x12\x38\n\x13\x62\x61se_with_revisions\x18\x04 \x01(\x0b\x32\x19.gitaly.BaseWithRevisionsH\x00\x42\x0c\n\nrange_spec\"$\n\x14RawRangeDiffResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"\xe2\x01\n\x10RangeDiffRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\'\n\nrange_pair\x18\x02 \x01(\x0b\x32\x11.gitaly.RangePairH\x00\x12/\n\x0erevision_range\x18\x03 \x01(\x0b\x32\x15.gitaly.RevisionRangeH\x00\x12\x38\n\x13\x62\x61se_with_revisions\x18\x04 \x01(\x0b\x32\x19.gitaly.BaseWithRevisionsH\x00\x42\x0c\n\nrange_spec\"\xc4\x02\n\x11RangeDiffResponse\x12\x16\n\x0e\x66rom_commit_id\x18\x01 \x01(\t\x12\x14\n\x0cto_commit_id\x18\x02 \x01(\t\x12\x38\n\ncomparison\x18\x03 \x01(\x0e\x32$.gitaly.RangeDiffResponse.Comparator\x12\x1c\n\x14\x63ommit_message_title\x18\x07 \x01(\t\x12\x12\n\npatch_data\x18\x08 \x01(\x0c\x12\x14\n\x0c\x65nd_of_patch\x18\t \x01(\x08\"\x7f\n\nComparator\x12 \n\x1c\x43OMPARATOR_EQUAL_UNSPECIFIED\x10\x00\x12\x1b\n\x17\x43OMPARATOR_GREATER_THAN\x10\x01\x12\x18\n\x14\x43OMPARATOR_LESS_THAN\x10\x02\x12\x18\n\x14\x43OMPARATOR_NOT_EQUAL\x10\x03\x32\xd8\x05\n\x0b\x44iffService\x12M\n\nCommitDiff\x12\x19.gitaly.CommitDiffRequest\x1a\x1a.gitaly.CommitDiffResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12P\n\x0b\x43ommitDelta\x12\x1a.gitaly.CommitDeltaRequest\x1a\x1b.gitaly.CommitDeltaResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\x44\n\x07RawDiff\x12\x16.gitaly.RawDiffRequest\x1a\x17.gitaly.RawDiffResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12G\n\x08RawPatch\x12\x17.gitaly.RawPatchRequest\x1a\x18.gitaly.RawPatchResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12J\n\tDiffStats\x12\x18.gitaly.DiffStatsRequest\x1a\x19.gitaly.DiffStatsResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12_\n\x10\x46indChangedPaths\x12\x1f.gitaly.FindChangedPathsRequest\x1a .gitaly.FindChangedPathsResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12K\n\nGetPatchID\x12\x19.gitaly.GetPatchIDRequest\x1a\x1a.gitaly.GetPatchIDResponse\"\x06\xfa\x97(\x02\x08\x02\x12S\n\x0cRawRangeDiff\x12\x1b.gitaly.RawRangeDiffRequest\x1a\x1c.gitaly.RawRangeDiffResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12J\n\tRangeDiff\x12\x18.gitaly.RangeDiffRequest\x1a\x19.gitaly.RangeDiffResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x42\x34Z2gitlab.com/gitlab-org/gitaly/v16/proto/go/gitalypbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\ndiff.proto\x12\x06gitaly\x1a\nlint.proto\x1a\x0cshared.proto\"\xd8\x06\n\x11\x43ommitDiffRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\x12\r\n\x05paths\x18\x05 \x03(\x0c\x12\x16\n\x0e\x63ollapse_diffs\x18\x06 \x01(\x08\x12\x16\n\x0e\x65nforce_limits\x18\x07 \x01(\x08\x12\x11\n\tmax_files\x18\x08 \x01(\x05\x12\x11\n\tmax_lines\x18\t \x01(\x05\x12\x11\n\tmax_bytes\x18\n \x01(\x05\x12\x17\n\x0fmax_patch_bytes\x18\x0e \x01(\x05\x12\x16\n\x0esafe_max_files\x18\x0b \x01(\x05\x12\x16\n\x0esafe_max_lines\x18\x0c \x01(\x05\x12\x16\n\x0esafe_max_bytes\x18\r \x01(\x05\x12\x35\n\tdiff_mode\x18\x0f \x01(\x0e\x32\".gitaly.CommitDiffRequest.DiffMode\x12h\n\"max_patch_bytes_for_file_extension\x18\x10 \x03(\x0b\x32<.gitaly.CommitDiffRequest.MaxPatchBytesForFileExtensionEntry\x12G\n\x12whitespace_changes\x18\x11 \x01(\x0e\x32+.gitaly.CommitDiffRequest.WhitespaceChanges\x12\x19\n\x11\x63ollect_all_paths\x18\x12 \x01(\x08\x1a\x44\n\"MaxPatchBytesForFileExtensionEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"%\n\x08\x44iffMode\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x0c\n\x08WORDDIFF\x10\x01\"y\n\x11WhitespaceChanges\x12\"\n\x1eWHITESPACE_CHANGES_UNSPECIFIED\x10\x00\x12\x1d\n\x19WHITESPACE_CHANGES_IGNORE\x10\x01\x12!\n\x1dWHITESPACE_CHANGES_IGNORE_ALL\x10\x02J\x04\x08\x04\x10\x05R\x18ignore_whitespace_change\"\xff\x01\n\x12\x43ommitDiffResponse\x12\x11\n\tfrom_path\x18\x01 \x01(\x0c\x12\x0f\n\x07to_path\x18\x02 \x01(\x0c\x12\x0f\n\x07\x66rom_id\x18\x03 \x01(\t\x12\r\n\x05to_id\x18\x04 \x01(\t\x12\x10\n\x08old_mode\x18\x05 \x01(\x05\x12\x10\n\x08new_mode\x18\x06 \x01(\x05\x12\x0e\n\x06\x62inary\x18\x07 \x01(\x08\x12\x16\n\x0eraw_patch_data\x18\t \x01(\x0c\x12\x14\n\x0c\x65nd_of_patch\x18\n \x01(\x08\x12\x17\n\x0foverflow_marker\x18\x0b \x01(\x08\x12\x11\n\tcollapsed\x18\x0c \x01(\x08\x12\x11\n\ttoo_large\x18\r \x01(\x08J\x04\x08\x08\x10\t\"\x82\x01\n\x12\x43ommitDeltaRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\x12\r\n\x05paths\x18\x04 \x03(\x0c\"u\n\x0b\x43ommitDelta\x12\x11\n\tfrom_path\x18\x01 \x01(\x0c\x12\x0f\n\x07to_path\x18\x02 \x01(\x0c\x12\x0f\n\x07\x66rom_id\x18\x03 \x01(\t\x12\r\n\x05to_id\x18\x04 \x01(\t\x12\x10\n\x08old_mode\x18\x05 \x01(\x05\x12\x10\n\x08new_mode\x18\x06 \x01(\x05\":\n\x13\x43ommitDeltaResponse\x12#\n\x06\x64\x65ltas\x18\x01 \x03(\x0b\x32\x13.gitaly.CommitDelta\"o\n\x0eRawDiffRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\"\x1f\n\x0fRawDiffResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"p\n\x0fRawPatchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\" \n\x10RawPatchResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"q\n\x10\x44iffStatsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0eleft_commit_id\x18\x02 \x01(\t\x12\x17\n\x0fright_commit_id\x18\x03 \x01(\t\"Q\n\tDiffStats\x12\x0c\n\x04path\x18\x01 \x01(\x0c\x12\x11\n\tadditions\x18\x02 \x01(\x05\x12\x11\n\tdeletions\x18\x03 \x01(\x05\x12\x10\n\x08old_path\x18\x04 \x01(\x0c\"5\n\x11\x44iffStatsResponse\x12 \n\x05stats\x18\x01 \x03(\x0b\x32\x11.gitaly.DiffStats\"\xda\x05\n\x17\x46indChangedPathsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x13\n\x07\x63ommits\x18\x02 \x03(\tB\x02\x18\x01\x12\x39\n\x08requests\x18\x03 \x03(\x0b\x32\'.gitaly.FindChangedPathsRequest.Request\x12S\n\x16merge_commit_diff_mode\x18\x04 \x01(\x0e\x32\x33.gitaly.FindChangedPathsRequest.MergeCommitDiffMode\x12\x14\n\x0c\x66ind_renames\x18\x05 \x01(\x08\x1a\xc2\x02\n\x07Request\x12K\n\x0ctree_request\x18\x01 \x01(\x0b\x32\x33.gitaly.FindChangedPathsRequest.Request.TreeRequestH\x00\x12O\n\x0e\x63ommit_request\x18\x02 \x01(\x0b\x32\x35.gitaly.FindChangedPathsRequest.Request.CommitRequestH\x00\x1a\x46\n\x0bTreeRequest\x12\x1a\n\x12left_tree_revision\x18\x01 \x01(\t\x12\x1b\n\x13right_tree_revision\x18\x02 \x01(\t\x1aI\n\rCommitRequest\x12\x17\n\x0f\x63ommit_revision\x18\x01 \x01(\t\x12\x1f\n\x17parent_commit_revisions\x18\x02 \x03(\tB\x06\n\x04type\"\x90\x01\n\x13MergeCommitDiffMode\x12&\n\"MERGE_COMMIT_DIFF_MODE_UNSPECIFIED\x10\x00\x12)\n%MERGE_COMMIT_DIFF_MODE_INCLUDE_MERGES\x10\x01\x12&\n\"MERGE_COMMIT_DIFF_MODE_ALL_PARENTS\x10\x02\"?\n\x18\x46indChangedPathsResponse\x12#\n\x05paths\x18\x01 \x03(\x0b\x32\x14.gitaly.ChangedPaths\"\xf1\x01\n\x0c\x43hangedPaths\x12\x0c\n\x04path\x18\x01 \x01(\x0c\x12+\n\x06status\x18\x02 \x01(\x0e\x32\x1b.gitaly.ChangedPaths.Status\x12\x10\n\x08old_mode\x18\x03 \x01(\x05\x12\x10\n\x08new_mode\x18\x04 \x01(\x05\x12\x13\n\x0bold_blob_id\x18\x05 \x01(\t\x12\x13\n\x0bnew_blob_id\x18\x06 \x01(\t\"X\n\x06Status\x12\t\n\x05\x41\x44\x44\x45\x44\x10\x00\x12\x0c\n\x08MODIFIED\x10\x01\x12\x0b\n\x07\x44\x45LETED\x10\x02\x12\x0f\n\x0bTYPE_CHANGE\x10\x03\x12\n\n\x06\x43OPIED\x10\x04\x12\x0b\n\x07RENAMED\x10\x05\"m\n\x11GetPatchIDRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x14\n\x0cold_revision\x18\x02 \x01(\x0c\x12\x14\n\x0cnew_revision\x18\x03 \x01(\x0c\"&\n\x12GetPatchIDResponse\x12\x10\n\x08patch_id\x18\x01 \x01(\t\"+\n\tRangePair\x12\x0e\n\x06range1\x18\x01 \x01(\t\x12\x0e\n\x06range2\x18\x02 \x01(\t\"+\n\rRevisionRange\x12\x0c\n\x04rev1\x18\x01 \x01(\t\x12\x0c\n\x04rev2\x18\x02 \x01(\t\"=\n\x11\x42\x61seWithRevisions\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\x12\x0c\n\x04rev1\x18\x02 \x01(\t\x12\x0c\n\x04rev2\x18\x03 \x01(\t\"\xe5\x01\n\x13RawRangeDiffRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\'\n\nrange_pair\x18\x02 \x01(\x0b\x32\x11.gitaly.RangePairH\x00\x12/\n\x0erevision_range\x18\x03 \x01(\x0b\x32\x15.gitaly.RevisionRangeH\x00\x12\x38\n\x13\x62\x61se_with_revisions\x18\x04 \x01(\x0b\x32\x19.gitaly.BaseWithRevisionsH\x00\x42\x0c\n\nrange_spec\"$\n\x14RawRangeDiffResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"\xe2\x01\n\x10RangeDiffRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\'\n\nrange_pair\x18\x02 \x01(\x0b\x32\x11.gitaly.RangePairH\x00\x12/\n\x0erevision_range\x18\x03 \x01(\x0b\x32\x15.gitaly.RevisionRangeH\x00\x12\x38\n\x13\x62\x61se_with_revisions\x18\x04 \x01(\x0b\x32\x19.gitaly.BaseWithRevisionsH\x00\x42\x0c\n\nrange_spec\"\xc4\x02\n\x11RangeDiffResponse\x12\x16\n\x0e\x66rom_commit_id\x18\x01 \x01(\t\x12\x14\n\x0cto_commit_id\x18\x02 \x01(\t\x12\x38\n\ncomparison\x18\x03 \x01(\x0e\x32$.gitaly.RangeDiffResponse.Comparator\x12\x1c\n\x14\x63ommit_message_title\x18\x07 \x01(\t\x12\x12\n\npatch_data\x18\x08 \x01(\x0c\x12\x14\n\x0c\x65nd_of_patch\x18\t \x01(\x08\"\x7f\n\nComparator\x12 \n\x1c\x43OMPARATOR_EQUAL_UNSPECIFIED\x10\x00\x12\x1b\n\x17\x43OMPARATOR_GREATER_THAN\x10\x01\x12\x18\n\x14\x43OMPARATOR_LESS_THAN\x10\x02\x12\x18\n\x14\x43OMPARATOR_NOT_EQUAL\x10\x03\"\xdc\x03\n\x10\x44iffBlobsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x35\n\nblob_pairs\x18\x02 \x03(\x0b\x32!.gitaly.DiffBlobsRequest.BlobPair\x12\x34\n\tdiff_mode\x18\x03 \x01(\x0e\x32!.gitaly.DiffBlobsRequest.DiffMode\x12\x46\n\x12whitespace_changes\x18\x04 \x01(\x0e\x32*.gitaly.DiffBlobsRequest.WhitespaceChanges\x1a/\n\x08\x42lobPair\x12\x10\n\x08left_oid\x18\x01 \x01(\t\x12\x11\n\tright_oid\x18\x02 \x01(\t\"9\n\x08\x44iffMode\x12\x19\n\x15\x44IFF_MODE_UNSPECIFIED\x10\x00\x12\x12\n\x0e\x44IFF_MODE_WORD\x10\x01\"y\n\x11WhitespaceChanges\x12\"\n\x1eWHITESPACE_CHANGES_UNSPECIFIED\x10\x00\x12\x1d\n\x19WHITESPACE_CHANGES_IGNORE\x10\x01\x12!\n\x1dWHITESPACE_CHANGES_IGNORE_ALL\x10\x02\"\xcb\x01\n\x11\x44iffBlobsResponse\x12\x14\n\x0cleft_blob_id\x18\x01 \x01(\t\x12\x15\n\rright_blob_id\x18\x02 \x01(\t\x12\r\n\x05patch\x18\x03 \x01(\x0c\x12\x30\n\x06status\x18\x04 \x01(\x0e\x32 .gitaly.DiffBlobsResponse.Status\x12\x0e\n\x06\x62inary\x18\x05 \x01(\x08\"8\n\x06Status\x12\x15\n\x11STATUS_INCOMPLETE\x10\x00\x12\x17\n\x13STATUS_END_OF_PATCH\x10\x01\x32\xa4\x06\n\x0b\x44iffService\x12M\n\nCommitDiff\x12\x19.gitaly.CommitDiffRequest\x1a\x1a.gitaly.CommitDiffResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12P\n\x0b\x43ommitDelta\x12\x1a.gitaly.CommitDeltaRequest\x1a\x1b.gitaly.CommitDeltaResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\x44\n\x07RawDiff\x12\x16.gitaly.RawDiffRequest\x1a\x17.gitaly.RawDiffResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12G\n\x08RawPatch\x12\x17.gitaly.RawPatchRequest\x1a\x18.gitaly.RawPatchResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12J\n\tDiffStats\x12\x18.gitaly.DiffStatsRequest\x1a\x19.gitaly.DiffStatsResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12_\n\x10\x46indChangedPaths\x12\x1f.gitaly.FindChangedPathsRequest\x1a .gitaly.FindChangedPathsResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12K\n\nGetPatchID\x12\x19.gitaly.GetPatchIDRequest\x1a\x1a.gitaly.GetPatchIDResponse\"\x06\xfa\x97(\x02\x08\x02\x12S\n\x0cRawRangeDiff\x12\x1b.gitaly.RawRangeDiffRequest\x1a\x1c.gitaly.RawRangeDiffResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12J\n\tRangeDiff\x12\x18.gitaly.RangeDiffRequest\x1a\x19.gitaly.RangeDiffResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12J\n\tDiffBlobs\x12\x18.gitaly.DiffBlobsRequest\x1a\x19.gitaly.DiffBlobsResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x42\x34Z2gitlab.com/gitlab-org/gitaly/v16/proto/go/gitalypbb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'diff_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -42,14 +42,16 @@
   _FINDCHANGEDPATHSREQUEST.fields_by_name['commits']._serialized_options = b'\030\001'
   _GETPATCHIDREQUEST.fields_by_name['repository']._options = None
   _GETPATCHIDREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
   _RAWRANGEDIFFREQUEST.fields_by_name['repository']._options = None
   _RAWRANGEDIFFREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
   _RANGEDIFFREQUEST.fields_by_name['repository']._options = None
   _RANGEDIFFREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
+  _DIFFBLOBSREQUEST.fields_by_name['repository']._options = None
+  _DIFFBLOBSREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
   _DIFFSERVICE.methods_by_name['CommitDiff']._options = None
   _DIFFSERVICE.methods_by_name['CommitDiff']._serialized_options = b'\372\227(\002\010\002'
   _DIFFSERVICE.methods_by_name['CommitDelta']._options = None
   _DIFFSERVICE.methods_by_name['CommitDelta']._serialized_options = b'\372\227(\002\010\002'
   _DIFFSERVICE.methods_by_name['RawDiff']._options = None
   _DIFFSERVICE.methods_by_name['RawDiff']._serialized_options = b'\372\227(\002\010\002'
   _DIFFSERVICE.methods_by_name['RawPatch']._options = None
@@ -60,14 +62,16 @@
   _DIFFSERVICE.methods_by_name['FindChangedPaths']._serialized_options = b'\372\227(\002\010\002'
   _DIFFSERVICE.methods_by_name['GetPatchID']._options = None
   _DIFFSERVICE.methods_by_name['GetPatchID']._serialized_options = b'\372\227(\002\010\002'
   _DIFFSERVICE.methods_by_name['RawRangeDiff']._options = None
   _DIFFSERVICE.methods_by_name['RawRangeDiff']._serialized_options = b'\372\227(\002\010\002'
   _DIFFSERVICE.methods_by_name['RangeDiff']._options = None
   _DIFFSERVICE.methods_by_name['RangeDiff']._serialized_options = b'\372\227(\002\010\002'
+  _DIFFSERVICE.methods_by_name['DiffBlobs']._options = None
+  _DIFFSERVICE.methods_by_name['DiffBlobs']._serialized_options = b'\372\227(\002\010\002'
   _globals['_COMMITDIFFREQUEST']._serialized_start=49
   _globals['_COMMITDIFFREQUEST']._serialized_end=905
   _globals['_COMMITDIFFREQUEST_MAXPATCHBYTESFORFILEEXTENSIONENTRY']._serialized_start=643
   _globals['_COMMITDIFFREQUEST_MAXPATCHBYTESFORFILEEXTENSIONENTRY']._serialized_end=711
   _globals['_COMMITDIFFREQUEST_DIFFMODE']._serialized_start=713
   _globals['_COMMITDIFFREQUEST_DIFFMODE']._serialized_end=750
   _globals['_COMMITDIFFREQUEST_WHITESPACECHANGES']._serialized_start=752
@@ -91,45 +95,57 @@
   _globals['_DIFFSTATSREQUEST']._serialized_start=1771
   _globals['_DIFFSTATSREQUEST']._serialized_end=1884
   _globals['_DIFFSTATS']._serialized_start=1886
   _globals['_DIFFSTATS']._serialized_end=1967
   _globals['_DIFFSTATSRESPONSE']._serialized_start=1969
   _globals['_DIFFSTATSRESPONSE']._serialized_end=2022
   _globals['_FINDCHANGEDPATHSREQUEST']._serialized_start=2025
-  _globals['_FINDCHANGEDPATHSREQUEST']._serialized_end=2733
-  _globals['_FINDCHANGEDPATHSREQUEST_REQUEST']._serialized_start=2264
-  _globals['_FINDCHANGEDPATHSREQUEST_REQUEST']._serialized_end=2586
-  _globals['_FINDCHANGEDPATHSREQUEST_REQUEST_TREEREQUEST']._serialized_start=2433
-  _globals['_FINDCHANGEDPATHSREQUEST_REQUEST_TREEREQUEST']._serialized_end=2503
-  _globals['_FINDCHANGEDPATHSREQUEST_REQUEST_COMMITREQUEST']._serialized_start=2505
-  _globals['_FINDCHANGEDPATHSREQUEST_REQUEST_COMMITREQUEST']._serialized_end=2578
-  _globals['_FINDCHANGEDPATHSREQUEST_MERGECOMMITDIFFMODE']._serialized_start=2589
-  _globals['_FINDCHANGEDPATHSREQUEST_MERGECOMMITDIFFMODE']._serialized_end=2733
-  _globals['_FINDCHANGEDPATHSRESPONSE']._serialized_start=2735
-  _globals['_FINDCHANGEDPATHSRESPONSE']._serialized_end=2798
-  _globals['_CHANGEDPATHS']._serialized_start=2801
-  _globals['_CHANGEDPATHS']._serialized_end=3029
-  _globals['_CHANGEDPATHS_STATUS']._serialized_start=2954
-  _globals['_CHANGEDPATHS_STATUS']._serialized_end=3029
-  _globals['_GETPATCHIDREQUEST']._serialized_start=3031
-  _globals['_GETPATCHIDREQUEST']._serialized_end=3140
-  _globals['_GETPATCHIDRESPONSE']._serialized_start=3142
-  _globals['_GETPATCHIDRESPONSE']._serialized_end=3180
-  _globals['_RANGEPAIR']._serialized_start=3182
-  _globals['_RANGEPAIR']._serialized_end=3225
-  _globals['_REVISIONRANGE']._serialized_start=3227
-  _globals['_REVISIONRANGE']._serialized_end=3270
-  _globals['_BASEWITHREVISIONS']._serialized_start=3272
-  _globals['_BASEWITHREVISIONS']._serialized_end=3333
-  _globals['_RAWRANGEDIFFREQUEST']._serialized_start=3336
-  _globals['_RAWRANGEDIFFREQUEST']._serialized_end=3565
-  _globals['_RAWRANGEDIFFRESPONSE']._serialized_start=3567
-  _globals['_RAWRANGEDIFFRESPONSE']._serialized_end=3603
-  _globals['_RANGEDIFFREQUEST']._serialized_start=3606
-  _globals['_RANGEDIFFREQUEST']._serialized_end=3832
-  _globals['_RANGEDIFFRESPONSE']._serialized_start=3835
-  _globals['_RANGEDIFFRESPONSE']._serialized_end=4159
-  _globals['_RANGEDIFFRESPONSE_COMPARATOR']._serialized_start=4032
-  _globals['_RANGEDIFFRESPONSE_COMPARATOR']._serialized_end=4159
-  _globals['_DIFFSERVICE']._serialized_start=4162
-  _globals['_DIFFSERVICE']._serialized_end=4890
+  _globals['_FINDCHANGEDPATHSREQUEST']._serialized_end=2755
+  _globals['_FINDCHANGEDPATHSREQUEST_REQUEST']._serialized_start=2286
+  _globals['_FINDCHANGEDPATHSREQUEST_REQUEST']._serialized_end=2608
+  _globals['_FINDCHANGEDPATHSREQUEST_REQUEST_TREEREQUEST']._serialized_start=2455
+  _globals['_FINDCHANGEDPATHSREQUEST_REQUEST_TREEREQUEST']._serialized_end=2525
+  _globals['_FINDCHANGEDPATHSREQUEST_REQUEST_COMMITREQUEST']._serialized_start=2527
+  _globals['_FINDCHANGEDPATHSREQUEST_REQUEST_COMMITREQUEST']._serialized_end=2600
+  _globals['_FINDCHANGEDPATHSREQUEST_MERGECOMMITDIFFMODE']._serialized_start=2611
+  _globals['_FINDCHANGEDPATHSREQUEST_MERGECOMMITDIFFMODE']._serialized_end=2755
+  _globals['_FINDCHANGEDPATHSRESPONSE']._serialized_start=2757
+  _globals['_FINDCHANGEDPATHSRESPONSE']._serialized_end=2820
+  _globals['_CHANGEDPATHS']._serialized_start=2823
+  _globals['_CHANGEDPATHS']._serialized_end=3064
+  _globals['_CHANGEDPATHS_STATUS']._serialized_start=2976
+  _globals['_CHANGEDPATHS_STATUS']._serialized_end=3064
+  _globals['_GETPATCHIDREQUEST']._serialized_start=3066
+  _globals['_GETPATCHIDREQUEST']._serialized_end=3175
+  _globals['_GETPATCHIDRESPONSE']._serialized_start=3177
+  _globals['_GETPATCHIDRESPONSE']._serialized_end=3215
+  _globals['_RANGEPAIR']._serialized_start=3217
+  _globals['_RANGEPAIR']._serialized_end=3260
+  _globals['_REVISIONRANGE']._serialized_start=3262
+  _globals['_REVISIONRANGE']._serialized_end=3305
+  _globals['_BASEWITHREVISIONS']._serialized_start=3307
+  _globals['_BASEWITHREVISIONS']._serialized_end=3368
+  _globals['_RAWRANGEDIFFREQUEST']._serialized_start=3371
+  _globals['_RAWRANGEDIFFREQUEST']._serialized_end=3600
+  _globals['_RAWRANGEDIFFRESPONSE']._serialized_start=3602
+  _globals['_RAWRANGEDIFFRESPONSE']._serialized_end=3638
+  _globals['_RANGEDIFFREQUEST']._serialized_start=3641
+  _globals['_RANGEDIFFREQUEST']._serialized_end=3867
+  _globals['_RANGEDIFFRESPONSE']._serialized_start=3870
+  _globals['_RANGEDIFFRESPONSE']._serialized_end=4194
+  _globals['_RANGEDIFFRESPONSE_COMPARATOR']._serialized_start=4067
+  _globals['_RANGEDIFFRESPONSE_COMPARATOR']._serialized_end=4194
+  _globals['_DIFFBLOBSREQUEST']._serialized_start=4197
+  _globals['_DIFFBLOBSREQUEST']._serialized_end=4673
+  _globals['_DIFFBLOBSREQUEST_BLOBPAIR']._serialized_start=4444
+  _globals['_DIFFBLOBSREQUEST_BLOBPAIR']._serialized_end=4491
+  _globals['_DIFFBLOBSREQUEST_DIFFMODE']._serialized_start=4493
+  _globals['_DIFFBLOBSREQUEST_DIFFMODE']._serialized_end=4550
+  _globals['_DIFFBLOBSREQUEST_WHITESPACECHANGES']._serialized_start=752
+  _globals['_DIFFBLOBSREQUEST_WHITESPACECHANGES']._serialized_end=873
+  _globals['_DIFFBLOBSRESPONSE']._serialized_start=4676
+  _globals['_DIFFBLOBSRESPONSE']._serialized_end=4879
+  _globals['_DIFFBLOBSRESPONSE_STATUS']._serialized_start=4823
+  _globals['_DIFFBLOBSRESPONSE_STATUS']._serialized_end=4879
+  _globals['_DIFFSERVICE']._serialized_start=4882
+  _globals['_DIFFSERVICE']._serialized_end=5686
 # @@protoc_insertion_point(module_scope)
```

### Comparing `hgitaly-1.5.0/hgitaly/stub/diff_pb2_grpc.py` & `hgitaly-1.6.0/hgitaly/stub/diff_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,19 @@
                 response_deserializer=diff__pb2.RawRangeDiffResponse.FromString,
                 )
         self.RangeDiff = channel.unary_stream(
                 '/gitaly.DiffService/RangeDiff',
                 request_serializer=diff__pb2.RangeDiffRequest.SerializeToString,
                 response_deserializer=diff__pb2.RangeDiffResponse.FromString,
                 )
+        self.DiffBlobs = channel.unary_stream(
+                '/gitaly.DiffService/DiffBlobs',
+                request_serializer=diff__pb2.DiffBlobsRequest.SerializeToString,
+                response_deserializer=diff__pb2.DiffBlobsResponse.FromString,
+                )
 
 
 class DiffServiceServicer(object):
     """DiffService is a service which provides RPCs to inspect differences
     introduced between a set of commits.
     """
 
@@ -138,14 +143,22 @@
     def RangeDiff(self, request, context):
         """RangeDiff outputs the parsed commit pairs from range diff for a given range specification.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def DiffBlobs(self, request, context):
+        """DiffBlobs computes diffs between pairs of blobs. A batch of blob pairs is sent to the server.
+        The resulting patches are then chucked across response messages and streamed to the client.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_DiffServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'CommitDiff': grpc.unary_stream_rpc_method_handler(
                     servicer.CommitDiff,
                     request_deserializer=diff__pb2.CommitDiffRequest.FromString,
                     response_serializer=diff__pb2.CommitDiffResponse.SerializeToString,
@@ -186,14 +199,19 @@
                     response_serializer=diff__pb2.RawRangeDiffResponse.SerializeToString,
             ),
             'RangeDiff': grpc.unary_stream_rpc_method_handler(
                     servicer.RangeDiff,
                     request_deserializer=diff__pb2.RangeDiffRequest.FromString,
                     response_serializer=diff__pb2.RangeDiffResponse.SerializeToString,
             ),
+            'DiffBlobs': grpc.unary_stream_rpc_method_handler(
+                    servicer.DiffBlobs,
+                    request_deserializer=diff__pb2.DiffBlobsRequest.FromString,
+                    response_serializer=diff__pb2.DiffBlobsResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'gitaly.DiffService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -350,7 +368,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_stream(request, target, '/gitaly.DiffService/RangeDiff',
             diff__pb2.RangeDiffRequest.SerializeToString,
             diff__pb2.RangeDiffResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def DiffBlobs(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/gitaly.DiffService/DiffBlobs',
+            diff__pb2.DiffBlobsRequest.SerializeToString,
+            diff__pb2.DiffBlobsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `hgitaly-1.5.0/hgitaly/stub/errors_pb2.py` & `hgitaly-1.6.0/hgitaly/stub/errors_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/lint_pb2.py` & `hgitaly-1.6.0/hgitaly/stub/lint_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/mercurial_changeset_pb2.py` & `hgitaly-1.6.0/hgitaly/stub/mercurial_changeset_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/mercurial_changeset_pb2_grpc.py` & `hgitaly-1.6.0/hgitaly/stub/mercurial_changeset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/mercurial_operations_pb2.py` & `hgitaly-1.6.0/hgitaly/stub/mercurial_operations_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/mercurial_operations_pb2_grpc.py` & `hgitaly-1.6.0/hgitaly/stub/mercurial_operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/mercurial_repository_pb2.py` & `hgitaly-1.6.0/hgitaly/stub/mercurial_repository_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/mercurial_repository_pb2_grpc.py` & `hgitaly-1.6.0/hgitaly/stub/mercurial_repository_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/operations_pb2.py` & `hgitaly-1.6.0/hgitaly/stub/operations_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from . import errors_pb2 as errors__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from . import lint_pb2 as lint__pb2
 from . import shared_pb2 as shared__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10operations.proto\x12\x06gitaly\x1a\x0c\x65rrors.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\nlint.proto\x1a\x0cshared.proto\"\x8d\x01\n\x17UserCreateBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x13\n\x0b\x62ranch_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x13\n\x0bstart_point\x18\x04 \x01(\x0c\"S\n\x18UserCreateBranchResponse\x12\x1e\n\x06\x62ranch\x18\x01 \x01(\x0b\x32\x0e.gitaly.BranchJ\x04\x08\x02\x10\x03R\x11pre_receive_error\"P\n\x15UserCreateBranchError\x12.\n\x0b\x63ustom_hook\x18\x01 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x42\x07\n\x05\x65rror\"\x98\x01\n\x17UserUpdateBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x13\n\x0b\x62ranch_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x0e\n\x06newrev\x18\x04 \x01(\x0c\x12\x0e\n\x06oldrev\x18\x05 \x01(\x0c\"5\n\x18UserUpdateBranchResponse\x12\x19\n\x11pre_receive_error\x18\x01 \x01(\t\"\x92\x01\n\x17UserDeleteBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x13\n\x0b\x62ranch_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x18\n\x10\x65xpected_old_oid\x18\x04 \x01(\t\"3\n\x18UserDeleteBranchResponseJ\x04\x08\x01\x10\x02R\x11pre_receive_error\"\xbc\x01\n\x15UserDeleteBranchError\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x01 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x12\x38\n\x10reference_update\x18\x02 \x01(\x0b\x32\x1c.gitaly.ReferenceUpdateErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x42\x07\n\x05\x65rror\"\x8c\x01\n\x14UserDeleteTagRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08tag_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x18\n\x10\x65xpected_old_oid\x18\x04 \x01(\t\"2\n\x15UserDeleteTagResponse\x12\x19\n\x11pre_receive_error\x18\x01 \x01(\t\"\xcb\x01\n\x14UserCreateTagRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08tag_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x17\n\x0ftarget_revision\x18\x04 \x01(\x0c\x12\x0f\n\x07message\x18\x05 \x01(\x0c\x12-\n\ttimestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"X\n\x15UserCreateTagResponse\x12\x18\n\x03tag\x18\x01 \x01(\x0b\x32\x0b.gitaly.TagJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04R\x06\x65xistsR\x11pre_receive_error\"\xf3\x01\n\x12UserCreateTagError\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x01 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x12\x38\n\x10reference_update\x18\x02 \x01(\x0b\x32\x1c.gitaly.ReferenceUpdateErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x12\x38\n\x10reference_exists\x18\x04 \x01(\x0b\x32\x1c.gitaly.ReferenceExistsErrorH\x00\x42\x07\n\x05\x65rror\"\xee\x01\n\x16UserMergeBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x11\n\tcommit_id\x18\x03 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\x0c\x12\x0f\n\x07message\x18\x05 \x01(\x0c\x12-\n\ttimestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\x08 \x01(\t\x12\r\n\x05\x61pply\x18\x06 \x01(\x08\"\x81\x01\n\x17UserMergeBranchResponse\x12\x11\n\tcommit_id\x18\x01 \x01(\t\x12\x34\n\rbranch_update\x18\x03 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdateJ\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05R\x11pre_receive_error\"\xf1\x01\n\x14UserMergeBranchError\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x01 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x12\x38\n\x10reference_update\x18\x02 \x01(\x0b\x32\x1c.gitaly.ReferenceUpdateErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x12\x34\n\x0emerge_conflict\x18\x04 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x42\x07\n\x05\x65rror\"\xae\x02\n\x15UserMergeToRefRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x12\n\nsource_sha\x18\x03 \x01(\t\x12\x12\n\x06\x62ranch\x18\x04 \x01(\x0c\x42\x02\x18\x01\x12\x12\n\ntarget_ref\x18\x05 \x01(\x0c\x12\x0f\n\x07message\x18\x06 \x01(\x0c\x12\x18\n\x10\x66irst_parent_ref\x18\x07 \x01(\x0c\x12\x1b\n\x0f\x61llow_conflicts\x18\x08 \x01(\x08\x42\x02\x18\x01\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\n \x01(\t\"D\n\x16UserMergeToRefResponse\x12\x11\n\tcommit_id\x18\x01 \x01(\tJ\x04\x08\x02\x10\x03R\x11pre_receive_error\"\xed\x01\n\x16UserRebaseToRefRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x12\n\nsource_sha\x18\x03 \x01(\t\x12\x12\n\ntarget_ref\x18\x05 \x01(\x0c\x12\x18\n\x10\x66irst_parent_ref\x18\x07 \x01(\x0c\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\n \x01(\t\",\n\x17UserRebaseToRefResponse\x12\x11\n\tcommit_id\x18\x01 \x01(\t\"X\n\x15OperationBranchUpdate\x12\x11\n\tcommit_id\x18\x01 \x01(\t\x12\x14\n\x0crepo_created\x18\x02 \x01(\x08\x12\x16\n\x0e\x62ranch_created\x18\x03 \x01(\x08\"\x9c\x01\n\x13UserFFBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x11\n\tcommit_id\x18\x03 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\x0c\x12\x18\n\x10\x65xpected_old_oid\x18\x05 \x01(\t\"g\n\x14UserFFBranchResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\x12\x19\n\x11pre_receive_error\x18\x02 \x01(\t\"\x86\x03\n\x15UserCherryPickRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12!\n\x06\x63ommit\x18\x03 \x01(\x0b\x32\x11.gitaly.GitCommit\x12\x13\n\x0b\x62ranch_name\x18\x04 \x01(\x0c\x12\x0f\n\x07message\x18\x05 \x01(\x0c\x12\x19\n\x11start_branch_name\x18\x06 \x01(\x0c\x12,\n\x10start_repository\x18\x07 \x01(\x0b\x32\x12.gitaly.Repository\x12\x0f\n\x07\x64ry_run\x18\x08 \x01(\x08\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\n \x01(\t\x12\x1a\n\x12\x63ommit_author_name\x18\x0b \x01(\x0c\x12\x1b\n\x13\x63ommit_author_email\x18\x0c \x01(\x0c\"\xb2\x01\n\x16UserCherryPickResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdateJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06R\x11\x63reate_tree_errorR\x0c\x63ommit_errorR\x11pre_receive_errorR\x16\x63reate_tree_error_code\"\x8f\x02\n\x13UserCherryPickError\x12:\n\x14\x63herry_pick_conflict\x18\x01 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x12:\n\x16target_branch_diverged\x18\x02 \x01(\x0b\x32\x18.gitaly.NotAncestorErrorH\x00\x12\x45\n\x17\x63hanges_already_applied\x18\x03 \x01(\x0b\x32\".gitaly.ChangesAlreadyAppliedErrorH\x00\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x04 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x42\x07\n\x05\x65rror\"\xc9\x02\n\x11UserRevertRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12!\n\x06\x63ommit\x18\x03 \x01(\x0b\x32\x11.gitaly.GitCommit\x12\x13\n\x0b\x62ranch_name\x18\x04 \x01(\x0c\x12\x0f\n\x07message\x18\x05 \x01(\x0c\x12\x19\n\x11start_branch_name\x18\x06 \x01(\x0c\x12,\n\x10start_repository\x18\x07 \x01(\x0b\x32\x12.gitaly.Repository\x12\x0f\n\x07\x64ry_run\x18\x08 \x01(\x08\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\n \x01(\t\"\x98\x02\n\x12UserRevertResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\x12\x19\n\x11\x63reate_tree_error\x18\x02 \x01(\t\x12\x14\n\x0c\x63ommit_error\x18\x03 \x01(\t\x12\x19\n\x11pre_receive_error\x18\x04 \x01(\t\x12J\n\x16\x63reate_tree_error_code\x18\x05 \x01(\x0e\x32*.gitaly.UserRevertResponse.CreateTreeError\"4\n\x0f\x43reateTreeError\x12\x08\n\x04NONE\x10\x00\x12\t\n\x05\x45MPTY\x10\x01\x12\x0c\n\x08\x43ONFLICT\x10\x02\"\xf9\x01\n\x0fUserRevertError\x12\x34\n\x0emerge_conflict\x18\x01 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x12\x45\n\x17\x63hanges_already_applied\x18\x02 \x01(\x0b\x32\".gitaly.ChangesAlreadyAppliedErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x12\x30\n\x0cnot_ancestor\x18\x04 \x01(\x0b\x32\x18.gitaly.NotAncestorErrorH\x00\x42\x07\n\x05\x65rror\"\xa7\x02\n\x1bUserCommitFilesActionHeader\x12>\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32..gitaly.UserCommitFilesActionHeader.ActionType\x12\x11\n\tfile_path\x18\x02 \x01(\x0c\x12\x15\n\rprevious_path\x18\x03 \x01(\x0c\x12\x16\n\x0e\x62\x61se64_content\x18\x04 \x01(\x08\x12\x18\n\x10\x65xecute_filemode\x18\x05 \x01(\x08\x12\x15\n\rinfer_content\x18\x06 \x01(\x08\"U\n\nActionType\x12\n\n\x06\x43REATE\x10\x00\x12\x0e\n\nCREATE_DIR\x10\x01\x12\n\n\x06UPDATE\x10\x02\x12\x08\n\x04MOVE\x10\x03\x12\n\n\x06\x44\x45LETE\x10\x04\x12\t\n\x05\x43HMOD\x10\x05\"\x85\x01\n\x15UserCommitFilesAction\x12\x35\n\x06header\x18\x01 \x01(\x0b\x32#.gitaly.UserCommitFilesActionHeaderH\x00\x12\x11\n\x07\x63ontent\x18\x02 \x01(\x0cH\x00\x42\"\n user_commit_files_action_payload\"\x82\x03\n\x1cUserCommitFilesRequestHeader\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x13\n\x0b\x62ranch_name\x18\x03 \x01(\x0c\x12\x16\n\x0e\x63ommit_message\x18\x04 \x01(\x0c\x12\x1a\n\x12\x63ommit_author_name\x18\x05 \x01(\x0c\x12\x1b\n\x13\x63ommit_author_email\x18\x06 \x01(\x0c\x12\x19\n\x11start_branch_name\x18\x07 \x01(\x0c\x12,\n\x10start_repository\x18\x08 \x01(\x0b\x32\x12.gitaly.Repository\x12\r\n\x05\x66orce\x18\t \x01(\x08\x12\x11\n\tstart_sha\x18\n \x01(\t\x12-\n\ttimestamp\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\x0c \x01(\t\"\xa6\x01\n\x16UserCommitFilesRequest\x12\x36\n\x06header\x18\x01 \x01(\x0b\x32$.gitaly.UserCommitFilesRequestHeaderH\x00\x12/\n\x06\x61\x63tion\x18\x02 \x01(\x0b\x32\x1d.gitaly.UserCommitFilesActionH\x00\x42#\n!user_commit_files_request_payload\"\x7f\n\x17UserCommitFilesResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\x12\x13\n\x0bindex_error\x18\x02 \x01(\t\x12\x19\n\x11pre_receive_error\x18\x03 \x01(\t\"\xad\x01\n\x14UserCommitFilesError\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x01 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x12*\n\x0cindex_update\x18\x02 \x01(\x0b\x32\x12.gitaly.IndexErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x42\x07\n\x05\x65rror\"\xb8\x03\n\x1cUserRebaseConfirmableRequest\x12=\n\x06header\x18\x01 \x01(\x0b\x32+.gitaly.UserRebaseConfirmableRequest.HeaderH\x00\x12\x0f\n\x05\x61pply\x18\x02 \x01(\x08H\x00\x1a\x9c\x02\n\x06Header\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x15\n\trebase_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\x0c\x12\x12\n\nbranch_sha\x18\x05 \x01(\t\x12-\n\x11remote_repository\x18\x06 \x01(\x0b\x32\x12.gitaly.Repository\x12\x15\n\rremote_branch\x18\x07 \x01(\x0c\x12\x18\n\x10git_push_options\x18\x08 \x03(\t\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampB)\n\'user_rebase_confirmable_request_payload\"\xa5\x01\n\x1dUserRebaseConfirmableResponse\x12\x14\n\nrebase_sha\x18\x01 \x01(\tH\x00\x12\x18\n\x0erebase_applied\x18\x02 \x01(\x08H\x00\x42*\n(user_rebase_confirmable_response_payloadJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05R\x11pre_receive_errorR\tgit_error\"\xfd\x01\n\x11UserSquashRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x11\n\tstart_sha\x18\x05 \x01(\t\x12\x0f\n\x07\x65nd_sha\x18\x06 \x01(\t\x12\x1c\n\x06\x61uthor\x18\x07 \x01(\x0b\x32\x0c.gitaly.User\x12\x16\n\x0e\x63ommit_message\x18\x08 \x01(\x0c\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05R\tsquash_id\"R\n\x12UserSquashResponse\x12\x12\n\nsquash_sha\x18\x01 \x01(\tJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04R\x11pre_receive_errorR\tgit_error\"\x8e\x01\n\x1aUserRebaseConfirmableError\x12\x35\n\x0frebase_conflict\x18\x01 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x02 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x42\x07\n\x05\x65rror\"\x8b\x01\n\x0fUserSquashError\x12\x38\n\x10resolve_revision\x18\x01 \x01(\x0b\x32\x1c.gitaly.ResolveRevisionErrorH\x00\x12\x35\n\x0frebase_conflict\x18\x02 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x42\x07\n\x05\x65rror\"\xbb\x02\n\x15UserApplyPatchRequest\x12\x36\n\x06header\x18\x01 \x01(\x0b\x32$.gitaly.UserApplyPatchRequest.HeaderH\x00\x12\x11\n\x07patches\x18\x02 \x01(\x0cH\x00\x1a\xb2\x01\n\x06Header\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x15\n\rtarget_branch\x18\x03 \x01(\x0c\x12-\n\ttimestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\x05 \x01(\tB\"\n user_apply_patch_request_payload\"N\n\x16UserApplyPatchResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\"\xfe\x01\n\x1aUserUpdateSubmoduleRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x12\n\ncommit_sha\x18\x03 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\x0c\x12\x11\n\tsubmodule\x18\x05 \x01(\x0c\x12\x16\n\x0e\x63ommit_message\x18\x06 \x01(\x0c\x12-\n\ttimestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\x08 \x01(\t\"\x9d\x01\n\x1bUserUpdateSubmoduleResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\x12\x19\n\x11pre_receive_error\x18\x02 \x01(\t\x12\x14\n\x0c\x63ommit_error\x18\x04 \x01(\tJ\x04\x08\x03\x10\x04R\x11\x63reate_tree_error2\xc9\x0b\n\x10OperationService\x12]\n\x10UserCreateBranch\x12\x1f.gitaly.UserCreateBranchRequest\x1a .gitaly.UserCreateBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12]\n\x10UserUpdateBranch\x12\x1f.gitaly.UserUpdateBranchRequest\x1a .gitaly.UserUpdateBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12]\n\x10UserDeleteBranch\x12\x1f.gitaly.UserDeleteBranchRequest\x1a .gitaly.UserDeleteBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12T\n\rUserCreateTag\x12\x1c.gitaly.UserCreateTagRequest\x1a\x1d.gitaly.UserCreateTagResponse\"\x06\xfa\x97(\x02\x08\x01\x12T\n\rUserDeleteTag\x12\x1c.gitaly.UserDeleteTagRequest\x1a\x1d.gitaly.UserDeleteTagResponse\"\x06\xfa\x97(\x02\x08\x01\x12W\n\x0eUserMergeToRef\x12\x1d.gitaly.UserMergeToRefRequest\x1a\x1e.gitaly.UserMergeToRefResponse\"\x06\xfa\x97(\x02\x08\x01\x12Z\n\x0fUserRebaseToRef\x12\x1e.gitaly.UserRebaseToRefRequest\x1a\x1f.gitaly.UserRebaseToRefResponse\"\x06\xfa\x97(\x02\x08\x01\x12^\n\x0fUserMergeBranch\x12\x1e.gitaly.UserMergeBranchRequest\x1a\x1f.gitaly.UserMergeBranchResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x30\x01\x12Q\n\x0cUserFFBranch\x12\x1b.gitaly.UserFFBranchRequest\x1a\x1c.gitaly.UserFFBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12W\n\x0eUserCherryPick\x12\x1d.gitaly.UserCherryPickRequest\x1a\x1e.gitaly.UserCherryPickResponse\"\x06\xfa\x97(\x02\x08\x01\x12\\\n\x0fUserCommitFiles\x12\x1e.gitaly.UserCommitFilesRequest\x1a\x1f.gitaly.UserCommitFilesResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x12p\n\x15UserRebaseConfirmable\x12$.gitaly.UserRebaseConfirmableRequest\x1a%.gitaly.UserRebaseConfirmableResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x30\x01\x12K\n\nUserRevert\x12\x19.gitaly.UserRevertRequest\x1a\x1a.gitaly.UserRevertResponse\"\x06\xfa\x97(\x02\x08\x01\x12K\n\nUserSquash\x12\x19.gitaly.UserSquashRequest\x1a\x1a.gitaly.UserSquashResponse\"\x06\xfa\x97(\x02\x08\x01\x12Y\n\x0eUserApplyPatch\x12\x1d.gitaly.UserApplyPatchRequest\x1a\x1e.gitaly.UserApplyPatchResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x12\x66\n\x13UserUpdateSubmodule\x12\".gitaly.UserUpdateSubmoduleRequest\x1a#.gitaly.UserUpdateSubmoduleResponse\"\x06\xfa\x97(\x02\x08\x01\x42\x34Z2gitlab.com/gitlab-org/gitaly/v16/proto/go/gitalypbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10operations.proto\x12\x06gitaly\x1a\x0c\x65rrors.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\nlint.proto\x1a\x0cshared.proto\"\x8d\x01\n\x17UserCreateBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x13\n\x0b\x62ranch_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x13\n\x0bstart_point\x18\x04 \x01(\x0c\"S\n\x18UserCreateBranchResponse\x12\x1e\n\x06\x62ranch\x18\x01 \x01(\x0b\x32\x0e.gitaly.BranchJ\x04\x08\x02\x10\x03R\x11pre_receive_error\"P\n\x15UserCreateBranchError\x12.\n\x0b\x63ustom_hook\x18\x01 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x42\x07\n\x05\x65rror\"\x98\x01\n\x17UserUpdateBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x13\n\x0b\x62ranch_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x0e\n\x06newrev\x18\x04 \x01(\x0c\x12\x0e\n\x06oldrev\x18\x05 \x01(\x0c\"5\n\x18UserUpdateBranchResponse\x12\x19\n\x11pre_receive_error\x18\x01 \x01(\t\"\x92\x01\n\x17UserDeleteBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x13\n\x0b\x62ranch_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x18\n\x10\x65xpected_old_oid\x18\x04 \x01(\t\"3\n\x18UserDeleteBranchResponseJ\x04\x08\x01\x10\x02R\x11pre_receive_error\"\xbc\x01\n\x15UserDeleteBranchError\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x01 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x12\x38\n\x10reference_update\x18\x02 \x01(\x0b\x32\x1c.gitaly.ReferenceUpdateErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x42\x07\n\x05\x65rror\"\x8c\x01\n\x14UserDeleteTagRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08tag_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x18\n\x10\x65xpected_old_oid\x18\x04 \x01(\t\"2\n\x15UserDeleteTagResponse\x12\x19\n\x11pre_receive_error\x18\x01 \x01(\t\"\xcb\x01\n\x14UserCreateTagRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08tag_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x17\n\x0ftarget_revision\x18\x04 \x01(\x0c\x12\x0f\n\x07message\x18\x05 \x01(\x0c\x12-\n\ttimestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"X\n\x15UserCreateTagResponse\x12\x18\n\x03tag\x18\x01 \x01(\x0b\x32\x0b.gitaly.TagJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04R\x06\x65xistsR\x11pre_receive_error\"\xf3\x01\n\x12UserCreateTagError\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x01 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x12\x38\n\x10reference_update\x18\x02 \x01(\x0b\x32\x1c.gitaly.ReferenceUpdateErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x12\x38\n\x10reference_exists\x18\x04 \x01(\x0b\x32\x1c.gitaly.ReferenceExistsErrorH\x00\x42\x07\n\x05\x65rror\"\xee\x01\n\x16UserMergeBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x11\n\tcommit_id\x18\x03 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\x0c\x12\x0f\n\x07message\x18\x05 \x01(\x0c\x12-\n\ttimestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\x08 \x01(\t\x12\r\n\x05\x61pply\x18\x06 \x01(\x08\"\x81\x01\n\x17UserMergeBranchResponse\x12\x11\n\tcommit_id\x18\x01 \x01(\t\x12\x34\n\rbranch_update\x18\x03 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdateJ\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05R\x11pre_receive_error\"\xf1\x01\n\x14UserMergeBranchError\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x01 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x12\x38\n\x10reference_update\x18\x02 \x01(\x0b\x32\x1c.gitaly.ReferenceUpdateErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x12\x34\n\x0emerge_conflict\x18\x04 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x42\x07\n\x05\x65rror\"\xae\x02\n\x15UserMergeToRefRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x12\n\nsource_sha\x18\x03 \x01(\t\x12\x12\n\x06\x62ranch\x18\x04 \x01(\x0c\x42\x02\x18\x01\x12\x12\n\ntarget_ref\x18\x05 \x01(\x0c\x12\x0f\n\x07message\x18\x06 \x01(\x0c\x12\x18\n\x10\x66irst_parent_ref\x18\x07 \x01(\x0c\x12\x1b\n\x0f\x61llow_conflicts\x18\x08 \x01(\x08\x42\x02\x18\x01\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\n \x01(\t\"D\n\x16UserMergeToRefResponse\x12\x11\n\tcommit_id\x18\x01 \x01(\tJ\x04\x08\x02\x10\x03R\x11pre_receive_error\"\xed\x01\n\x16UserRebaseToRefRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x12\n\nsource_sha\x18\x03 \x01(\t\x12\x12\n\ntarget_ref\x18\x05 \x01(\x0c\x12\x18\n\x10\x66irst_parent_ref\x18\x07 \x01(\x0c\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\n \x01(\t\",\n\x17UserRebaseToRefResponse\x12\x11\n\tcommit_id\x18\x01 \x01(\t\"X\n\x15OperationBranchUpdate\x12\x11\n\tcommit_id\x18\x01 \x01(\t\x12\x14\n\x0crepo_created\x18\x02 \x01(\x08\x12\x16\n\x0e\x62ranch_created\x18\x03 \x01(\x08\"\x9c\x01\n\x13UserFFBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x11\n\tcommit_id\x18\x03 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\x0c\x12\x18\n\x10\x65xpected_old_oid\x18\x05 \x01(\t\"g\n\x14UserFFBranchResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\x12\x19\n\x11pre_receive_error\x18\x02 \x01(\t\"\x86\x03\n\x15UserCherryPickRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12!\n\x06\x63ommit\x18\x03 \x01(\x0b\x32\x11.gitaly.GitCommit\x12\x13\n\x0b\x62ranch_name\x18\x04 \x01(\x0c\x12\x0f\n\x07message\x18\x05 \x01(\x0c\x12\x19\n\x11start_branch_name\x18\x06 \x01(\x0c\x12,\n\x10start_repository\x18\x07 \x01(\x0b\x32\x12.gitaly.Repository\x12\x0f\n\x07\x64ry_run\x18\x08 \x01(\x08\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\n \x01(\t\x12\x1a\n\x12\x63ommit_author_name\x18\x0b \x01(\x0c\x12\x1b\n\x13\x63ommit_author_email\x18\x0c \x01(\x0c\"\xb2\x01\n\x16UserCherryPickResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdateJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06R\x11\x63reate_tree_errorR\x0c\x63ommit_errorR\x11pre_receive_errorR\x16\x63reate_tree_error_code\"\x8f\x02\n\x13UserCherryPickError\x12:\n\x14\x63herry_pick_conflict\x18\x01 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x12:\n\x16target_branch_diverged\x18\x02 \x01(\x0b\x32\x18.gitaly.NotAncestorErrorH\x00\x12\x45\n\x17\x63hanges_already_applied\x18\x03 \x01(\x0b\x32\".gitaly.ChangesAlreadyAppliedErrorH\x00\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x04 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x42\x07\n\x05\x65rror\"\xc9\x02\n\x11UserRevertRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12!\n\x06\x63ommit\x18\x03 \x01(\x0b\x32\x11.gitaly.GitCommit\x12\x13\n\x0b\x62ranch_name\x18\x04 \x01(\x0c\x12\x0f\n\x07message\x18\x05 \x01(\x0c\x12\x19\n\x11start_branch_name\x18\x06 \x01(\x0c\x12,\n\x10start_repository\x18\x07 \x01(\x0b\x32\x12.gitaly.Repository\x12\x0f\n\x07\x64ry_run\x18\x08 \x01(\x08\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\n \x01(\t\"\x98\x02\n\x12UserRevertResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\x12\x19\n\x11\x63reate_tree_error\x18\x02 \x01(\t\x12\x14\n\x0c\x63ommit_error\x18\x03 \x01(\t\x12\x19\n\x11pre_receive_error\x18\x04 \x01(\t\x12J\n\x16\x63reate_tree_error_code\x18\x05 \x01(\x0e\x32*.gitaly.UserRevertResponse.CreateTreeError\"4\n\x0f\x43reateTreeError\x12\x08\n\x04NONE\x10\x00\x12\t\n\x05\x45MPTY\x10\x01\x12\x0c\n\x08\x43ONFLICT\x10\x02\"\xf9\x01\n\x0fUserRevertError\x12\x34\n\x0emerge_conflict\x18\x01 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x12\x45\n\x17\x63hanges_already_applied\x18\x02 \x01(\x0b\x32\".gitaly.ChangesAlreadyAppliedErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x12\x30\n\x0cnot_ancestor\x18\x04 \x01(\x0b\x32\x18.gitaly.NotAncestorErrorH\x00\x42\x07\n\x05\x65rror\"\xa7\x02\n\x1bUserCommitFilesActionHeader\x12>\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32..gitaly.UserCommitFilesActionHeader.ActionType\x12\x11\n\tfile_path\x18\x02 \x01(\x0c\x12\x15\n\rprevious_path\x18\x03 \x01(\x0c\x12\x16\n\x0e\x62\x61se64_content\x18\x04 \x01(\x08\x12\x18\n\x10\x65xecute_filemode\x18\x05 \x01(\x08\x12\x15\n\rinfer_content\x18\x06 \x01(\x08\"U\n\nActionType\x12\n\n\x06\x43REATE\x10\x00\x12\x0e\n\nCREATE_DIR\x10\x01\x12\n\n\x06UPDATE\x10\x02\x12\x08\n\x04MOVE\x10\x03\x12\n\n\x06\x44\x45LETE\x10\x04\x12\t\n\x05\x43HMOD\x10\x05\"\x85\x01\n\x15UserCommitFilesAction\x12\x35\n\x06header\x18\x01 \x01(\x0b\x32#.gitaly.UserCommitFilesActionHeaderH\x00\x12\x11\n\x07\x63ontent\x18\x02 \x01(\x0cH\x00\x42\"\n user_commit_files_action_payload\"\x90\x03\n\x1cUserCommitFilesRequestHeader\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x13\n\x0b\x62ranch_name\x18\x03 \x01(\x0c\x12\x16\n\x0e\x63ommit_message\x18\x04 \x01(\x0c\x12\x1a\n\x12\x63ommit_author_name\x18\x05 \x01(\x0c\x12\x1b\n\x13\x63ommit_author_email\x18\x06 \x01(\x0c\x12\x19\n\x11start_branch_name\x18\x07 \x01(\x0c\x12,\n\x10start_repository\x18\x08 \x01(\x0b\x32\x12.gitaly.Repository\x12\r\n\x05\x66orce\x18\t \x01(\x08\x12\x11\n\tstart_sha\x18\n \x01(\t\x12-\n\ttimestamp\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\x0c \x01(\t\x12\x0c\n\x04sign\x18\r \x01(\x08\"\xa6\x01\n\x16UserCommitFilesRequest\x12\x36\n\x06header\x18\x01 \x01(\x0b\x32$.gitaly.UserCommitFilesRequestHeaderH\x00\x12/\n\x06\x61\x63tion\x18\x02 \x01(\x0b\x32\x1d.gitaly.UserCommitFilesActionH\x00\x42#\n!user_commit_files_request_payload\"\x7f\n\x17UserCommitFilesResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\x12\x13\n\x0bindex_error\x18\x02 \x01(\t\x12\x19\n\x11pre_receive_error\x18\x03 \x01(\t\"\xad\x01\n\x14UserCommitFilesError\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x01 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x12*\n\x0cindex_update\x18\x02 \x01(\x0b\x32\x12.gitaly.IndexErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x42\x07\n\x05\x65rror\"\xb8\x03\n\x1cUserRebaseConfirmableRequest\x12=\n\x06header\x18\x01 \x01(\x0b\x32+.gitaly.UserRebaseConfirmableRequest.HeaderH\x00\x12\x0f\n\x05\x61pply\x18\x02 \x01(\x08H\x00\x1a\x9c\x02\n\x06Header\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x15\n\trebase_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\x0c\x12\x12\n\nbranch_sha\x18\x05 \x01(\t\x12-\n\x11remote_repository\x18\x06 \x01(\x0b\x32\x12.gitaly.Repository\x12\x15\n\rremote_branch\x18\x07 \x01(\x0c\x12\x18\n\x10git_push_options\x18\x08 \x03(\t\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampB)\n\'user_rebase_confirmable_request_payload\"\xa5\x01\n\x1dUserRebaseConfirmableResponse\x12\x14\n\nrebase_sha\x18\x01 \x01(\tH\x00\x12\x18\n\x0erebase_applied\x18\x02 \x01(\x08H\x00\x42*\n(user_rebase_confirmable_response_payloadJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05R\x11pre_receive_errorR\tgit_error\"\xfd\x01\n\x11UserSquashRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x11\n\tstart_sha\x18\x05 \x01(\t\x12\x0f\n\x07\x65nd_sha\x18\x06 \x01(\t\x12\x1c\n\x06\x61uthor\x18\x07 \x01(\x0b\x32\x0c.gitaly.User\x12\x16\n\x0e\x63ommit_message\x18\x08 \x01(\x0c\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05R\tsquash_id\"R\n\x12UserSquashResponse\x12\x12\n\nsquash_sha\x18\x01 \x01(\tJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04R\x11pre_receive_errorR\tgit_error\"\x8e\x01\n\x1aUserRebaseConfirmableError\x12\x35\n\x0frebase_conflict\x18\x01 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x02 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x42\x07\n\x05\x65rror\"\x8b\x01\n\x0fUserSquashError\x12\x38\n\x10resolve_revision\x18\x01 \x01(\x0b\x32\x1c.gitaly.ResolveRevisionErrorH\x00\x12\x35\n\x0frebase_conflict\x18\x02 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x42\x07\n\x05\x65rror\"\xbb\x02\n\x15UserApplyPatchRequest\x12\x36\n\x06header\x18\x01 \x01(\x0b\x32$.gitaly.UserApplyPatchRequest.HeaderH\x00\x12\x11\n\x07patches\x18\x02 \x01(\x0cH\x00\x1a\xb2\x01\n\x06Header\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x15\n\rtarget_branch\x18\x03 \x01(\x0c\x12-\n\ttimestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\x05 \x01(\tB\"\n user_apply_patch_request_payload\"N\n\x16UserApplyPatchResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\"\xfe\x01\n\x1aUserUpdateSubmoduleRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x12\n\ncommit_sha\x18\x03 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\x0c\x12\x11\n\tsubmodule\x18\x05 \x01(\x0c\x12\x16\n\x0e\x63ommit_message\x18\x06 \x01(\x0c\x12-\n\ttimestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\x08 \x01(\t\"\x9d\x01\n\x1bUserUpdateSubmoduleResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\x12\x19\n\x11pre_receive_error\x18\x02 \x01(\t\x12\x14\n\x0c\x63ommit_error\x18\x04 \x01(\tJ\x04\x08\x03\x10\x04R\x11\x63reate_tree_error2\xc9\x0b\n\x10OperationService\x12]\n\x10UserCreateBranch\x12\x1f.gitaly.UserCreateBranchRequest\x1a .gitaly.UserCreateBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12]\n\x10UserUpdateBranch\x12\x1f.gitaly.UserUpdateBranchRequest\x1a .gitaly.UserUpdateBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12]\n\x10UserDeleteBranch\x12\x1f.gitaly.UserDeleteBranchRequest\x1a .gitaly.UserDeleteBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12T\n\rUserCreateTag\x12\x1c.gitaly.UserCreateTagRequest\x1a\x1d.gitaly.UserCreateTagResponse\"\x06\xfa\x97(\x02\x08\x01\x12T\n\rUserDeleteTag\x12\x1c.gitaly.UserDeleteTagRequest\x1a\x1d.gitaly.UserDeleteTagResponse\"\x06\xfa\x97(\x02\x08\x01\x12W\n\x0eUserMergeToRef\x12\x1d.gitaly.UserMergeToRefRequest\x1a\x1e.gitaly.UserMergeToRefResponse\"\x06\xfa\x97(\x02\x08\x01\x12Z\n\x0fUserRebaseToRef\x12\x1e.gitaly.UserRebaseToRefRequest\x1a\x1f.gitaly.UserRebaseToRefResponse\"\x06\xfa\x97(\x02\x08\x01\x12^\n\x0fUserMergeBranch\x12\x1e.gitaly.UserMergeBranchRequest\x1a\x1f.gitaly.UserMergeBranchResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x30\x01\x12Q\n\x0cUserFFBranch\x12\x1b.gitaly.UserFFBranchRequest\x1a\x1c.gitaly.UserFFBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12W\n\x0eUserCherryPick\x12\x1d.gitaly.UserCherryPickRequest\x1a\x1e.gitaly.UserCherryPickResponse\"\x06\xfa\x97(\x02\x08\x01\x12\\\n\x0fUserCommitFiles\x12\x1e.gitaly.UserCommitFilesRequest\x1a\x1f.gitaly.UserCommitFilesResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x12p\n\x15UserRebaseConfirmable\x12$.gitaly.UserRebaseConfirmableRequest\x1a%.gitaly.UserRebaseConfirmableResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x30\x01\x12K\n\nUserRevert\x12\x19.gitaly.UserRevertRequest\x1a\x1a.gitaly.UserRevertResponse\"\x06\xfa\x97(\x02\x08\x01\x12K\n\nUserSquash\x12\x19.gitaly.UserSquashRequest\x1a\x1a.gitaly.UserSquashResponse\"\x06\xfa\x97(\x02\x08\x01\x12Y\n\x0eUserApplyPatch\x12\x1d.gitaly.UserApplyPatchRequest\x1a\x1e.gitaly.UserApplyPatchResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x12\x66\n\x13UserUpdateSubmodule\x12\".gitaly.UserUpdateSubmoduleRequest\x1a#.gitaly.UserUpdateSubmoduleResponse\"\x06\xfa\x97(\x02\x08\x01\x42\x34Z2gitlab.com/gitlab-org/gitaly/v16/proto/go/gitalypbb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'operations_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -159,41 +159,41 @@
   _globals['_USERCOMMITFILESACTIONHEADER']._serialized_start=5100
   _globals['_USERCOMMITFILESACTIONHEADER']._serialized_end=5395
   _globals['_USERCOMMITFILESACTIONHEADER_ACTIONTYPE']._serialized_start=5310
   _globals['_USERCOMMITFILESACTIONHEADER_ACTIONTYPE']._serialized_end=5395
   _globals['_USERCOMMITFILESACTION']._serialized_start=5398
   _globals['_USERCOMMITFILESACTION']._serialized_end=5531
   _globals['_USERCOMMITFILESREQUESTHEADER']._serialized_start=5534
-  _globals['_USERCOMMITFILESREQUESTHEADER']._serialized_end=5920
-  _globals['_USERCOMMITFILESREQUEST']._serialized_start=5923
-  _globals['_USERCOMMITFILESREQUEST']._serialized_end=6089
-  _globals['_USERCOMMITFILESRESPONSE']._serialized_start=6091
-  _globals['_USERCOMMITFILESRESPONSE']._serialized_end=6218
-  _globals['_USERCOMMITFILESERROR']._serialized_start=6221
-  _globals['_USERCOMMITFILESERROR']._serialized_end=6394
-  _globals['_USERREBASECONFIRMABLEREQUEST']._serialized_start=6397
-  _globals['_USERREBASECONFIRMABLEREQUEST']._serialized_end=6837
-  _globals['_USERREBASECONFIRMABLEREQUEST_HEADER']._serialized_start=6510
-  _globals['_USERREBASECONFIRMABLEREQUEST_HEADER']._serialized_end=6794
-  _globals['_USERREBASECONFIRMABLERESPONSE']._serialized_start=6840
-  _globals['_USERREBASECONFIRMABLERESPONSE']._serialized_end=7005
-  _globals['_USERSQUASHREQUEST']._serialized_start=7008
-  _globals['_USERSQUASHREQUEST']._serialized_end=7261
-  _globals['_USERSQUASHRESPONSE']._serialized_start=7263
-  _globals['_USERSQUASHRESPONSE']._serialized_end=7345
-  _globals['_USERREBASECONFIRMABLEERROR']._serialized_start=7348
-  _globals['_USERREBASECONFIRMABLEERROR']._serialized_end=7490
-  _globals['_USERSQUASHERROR']._serialized_start=7493
-  _globals['_USERSQUASHERROR']._serialized_end=7632
-  _globals['_USERAPPLYPATCHREQUEST']._serialized_start=7635
-  _globals['_USERAPPLYPATCHREQUEST']._serialized_end=7950
-  _globals['_USERAPPLYPATCHREQUEST_HEADER']._serialized_start=7736
-  _globals['_USERAPPLYPATCHREQUEST_HEADER']._serialized_end=7914
-  _globals['_USERAPPLYPATCHRESPONSE']._serialized_start=7952
-  _globals['_USERAPPLYPATCHRESPONSE']._serialized_end=8030
-  _globals['_USERUPDATESUBMODULEREQUEST']._serialized_start=8033
-  _globals['_USERUPDATESUBMODULEREQUEST']._serialized_end=8287
-  _globals['_USERUPDATESUBMODULERESPONSE']._serialized_start=8290
-  _globals['_USERUPDATESUBMODULERESPONSE']._serialized_end=8447
-  _globals['_OPERATIONSERVICE']._serialized_start=8450
-  _globals['_OPERATIONSERVICE']._serialized_end=9931
+  _globals['_USERCOMMITFILESREQUESTHEADER']._serialized_end=5934
+  _globals['_USERCOMMITFILESREQUEST']._serialized_start=5937
+  _globals['_USERCOMMITFILESREQUEST']._serialized_end=6103
+  _globals['_USERCOMMITFILESRESPONSE']._serialized_start=6105
+  _globals['_USERCOMMITFILESRESPONSE']._serialized_end=6232
+  _globals['_USERCOMMITFILESERROR']._serialized_start=6235
+  _globals['_USERCOMMITFILESERROR']._serialized_end=6408
+  _globals['_USERREBASECONFIRMABLEREQUEST']._serialized_start=6411
+  _globals['_USERREBASECONFIRMABLEREQUEST']._serialized_end=6851
+  _globals['_USERREBASECONFIRMABLEREQUEST_HEADER']._serialized_start=6524
+  _globals['_USERREBASECONFIRMABLEREQUEST_HEADER']._serialized_end=6808
+  _globals['_USERREBASECONFIRMABLERESPONSE']._serialized_start=6854
+  _globals['_USERREBASECONFIRMABLERESPONSE']._serialized_end=7019
+  _globals['_USERSQUASHREQUEST']._serialized_start=7022
+  _globals['_USERSQUASHREQUEST']._serialized_end=7275
+  _globals['_USERSQUASHRESPONSE']._serialized_start=7277
+  _globals['_USERSQUASHRESPONSE']._serialized_end=7359
+  _globals['_USERREBASECONFIRMABLEERROR']._serialized_start=7362
+  _globals['_USERREBASECONFIRMABLEERROR']._serialized_end=7504
+  _globals['_USERSQUASHERROR']._serialized_start=7507
+  _globals['_USERSQUASHERROR']._serialized_end=7646
+  _globals['_USERAPPLYPATCHREQUEST']._serialized_start=7649
+  _globals['_USERAPPLYPATCHREQUEST']._serialized_end=7964
+  _globals['_USERAPPLYPATCHREQUEST_HEADER']._serialized_start=7750
+  _globals['_USERAPPLYPATCHREQUEST_HEADER']._serialized_end=7928
+  _globals['_USERAPPLYPATCHRESPONSE']._serialized_start=7966
+  _globals['_USERAPPLYPATCHRESPONSE']._serialized_end=8044
+  _globals['_USERUPDATESUBMODULEREQUEST']._serialized_start=8047
+  _globals['_USERUPDATESUBMODULEREQUEST']._serialized_end=8301
+  _globals['_USERUPDATESUBMODULERESPONSE']._serialized_start=8304
+  _globals['_USERUPDATESUBMODULERESPONSE']._serialized_end=8461
+  _globals['_OPERATIONSERVICE']._serialized_start=8464
+  _globals['_OPERATIONSERVICE']._serialized_end=9945
 # @@protoc_insertion_point(module_scope)
```

### Comparing `hgitaly-1.5.0/hgitaly/stub/operations_pb2_grpc.py` & `hgitaly-1.6.0/hgitaly/stub/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/ref_pb2.py` & `hgitaly-1.6.0/hgitaly/stub/ref_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/ref_pb2_grpc.py` & `hgitaly-1.6.0/hgitaly/stub/ref_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/repository_pb2.py` & `hgitaly-1.6.0/hgitaly/stub/repository_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import lint_pb2 as lint__pb2
 from . import shared_pb2 as shared__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10repository.proto\x12\x06gitaly\x1a\nlint.proto\x1a\x0cshared.proto\"G\n\x17RepositoryExistsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"*\n\x18RepositoryExistsResponse\x12\x0e\n\x06\x65xists\x18\x01 \x01(\x08\"E\n\x15RepositorySizeRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"&\n\x16RepositorySizeResponse\x12\x0c\n\x04size\x18\x01 \x01(\x03\"E\n\x15RepositoryInfoRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\xbb\x02\n\x16RepositoryInfoResponse\x12\x0c\n\x04size\x18\x01 \x01(\x04\x12\x41\n\nreferences\x18\x02 \x01(\x0b\x32-.gitaly.RepositoryInfoResponse.ReferencesInfo\x12;\n\x07objects\x18\x03 \x01(\x0b\x32*.gitaly.RepositoryInfoResponse.ObjectsInfo\x1a:\n\x0eReferencesInfo\x12\x13\n\x0bloose_count\x18\x01 \x01(\x04\x12\x13\n\x0bpacked_size\x18\x02 \x01(\x04\x1aW\n\x0bObjectsInfo\x12\x0c\n\x04size\x18\x01 \x01(\x04\x12\x13\n\x0brecent_size\x18\x02 \x01(\x04\x12\x12\n\nstale_size\x18\x03 \x01(\x04\x12\x11\n\tkeep_size\x18\x04 \x01(\x04\"U\n\x12ObjectsSizeRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\trevisions\x18\x02 \x03(\x0c\"#\n\x13ObjectsSizeResponse\x12\x0c\n\x04size\x18\x01 \x01(\x04\"C\n\x13ObjectFormatRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"<\n\x14ObjectFormatResponse\x12$\n\x06\x66ormat\x18\x01 \x01(\x0e\x32\x14.gitaly.ObjectFormat\"[\n\x19\x41pplyGitattributesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\"\x1c\n\x1a\x41pplyGitattributesResponse\"e\n\x12\x46\x65tchBundleRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x13\n\x0bupdate_head\x18\x03 \x01(\x08\"\x15\n\x13\x46\x65tchBundleResponse\"\x82\x02\n\x12\x46\x65tchRemoteRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\r\n\x05\x66orce\x18\x03 \x01(\x08\x12\x0f\n\x07no_tags\x18\x04 \x01(\x08\x12\x0f\n\x07timeout\x18\x05 \x01(\x05\x12\x0f\n\x07ssh_key\x18\x06 \x01(\t\x12\x13\n\x0bknown_hosts\x18\x07 \x01(\t\x12\x10\n\x08no_prune\x18\t \x01(\x08\x12%\n\rremote_params\x18\n \x01(\x0b\x32\x0e.gitaly.Remote\x12\x1a\n\x12\x63heck_tags_changed\x18\x0b \x01(\x08J\x04\x08\x08\x10\tJ\x04\x08\x02\x10\x03R\x06remote\"+\n\x13\x46\x65tchRemoteResponse\x12\x14\n\x0ctags_changed\x18\x01 \x01(\x08\"\x8c\x01\n\x17\x43reateRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0e\x64\x65\x66\x61ult_branch\x18\x02 \x01(\x0c\x12+\n\robject_format\x18\x03 \x01(\x0e\x32\x14.gitaly.ObjectFormat\"\x1a\n\x18\x43reateRepositoryResponse\"\x99\x02\n\x11GetArchiveRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\tcommit_id\x18\x02 \x01(\t\x12\x0e\n\x06prefix\x18\x03 \x01(\t\x12\x30\n\x06\x66ormat\x18\x04 \x01(\x0e\x32 .gitaly.GetArchiveRequest.Format\x12\x0c\n\x04path\x18\x05 \x01(\x0c\x12\x0f\n\x07\x65xclude\x18\x06 \x03(\x0c\x12\x12\n\nelide_path\x18\x07 \x01(\x08\x12\x19\n\x11include_lfs_blobs\x18\x08 \x01(\x08\"3\n\x06\x46ormat\x12\x07\n\x03ZIP\x10\x00\x12\x07\n\x03TAR\x10\x01\x12\n\n\x06TAR_GZ\x10\x02\x12\x0b\n\x07TAR_BZ2\x10\x03\"\"\n\x12GetArchiveResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"G\n\x17HasLocalBranchesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\")\n\x18HasLocalBranchesResponse\x12\r\n\x05value\x18\x01 \x01(\x08\"\xa2\x01\n\x18\x46\x65tchSourceBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12-\n\x11source_repository\x18\x02 \x01(\x0b\x32\x12.gitaly.Repository\x12\x15\n\rsource_branch\x18\x03 \x01(\x0c\x12\x12\n\ntarget_ref\x18\x04 \x01(\x0c\"+\n\x19\x46\x65tchSourceBranchResponse\x12\x0e\n\x06result\x18\x01 \x01(\x08\";\n\x0b\x46sckRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x1d\n\x0c\x46sckResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\x0c\"\x87\x01\n\x0fWriteRefRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0b\n\x03ref\x18\x02 \x01(\x0c\x12\x10\n\x08revision\x18\x03 \x01(\x0c\x12\x14\n\x0cold_revision\x18\x04 \x01(\x0cJ\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07R\x05\x66orce\"\x18\n\x10WriteRefResponseJ\x04\x08\x01\x10\x02\"W\n\x14\x46indMergeBaseRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\trevisions\x18\x02 \x03(\x0c\"%\n\x15\x46indMergeBaseResponse\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\"\x82\x01\n\x11\x43reateForkRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12-\n\x11source_repository\x18\x02 \x01(\x0b\x32\x12.gitaly.Repository\x12\x10\n\x08revision\x18\x03 \x01(\x0c\"\x14\n\x12\x43reateForkResponse\"\xb9\x01\n\x1e\x43reateRepositoryFromURLRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0b\n\x03url\x18\x02 \x01(\t\x12!\n\x19http_authorization_header\x18\x04 \x01(\t\x12\x0e\n\x06mirror\x18\x05 \x01(\x08\x12\x18\n\x10resolved_address\x18\x06 \x01(\tJ\x04\x08\x03\x10\x04R\thttp_host\"!\n\x1f\x43reateRepositoryFromURLResponse\"C\n\x13\x43reateBundleRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"$\n\x14\x43reateBundleResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"`\n\x1e\x43reateBundleFromRefListRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08patterns\x18\x02 \x03(\x0c\"/\n\x1f\x43reateBundleFromRefListResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"@\n\x10GetConfigRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"!\n\x11GetConfigResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"W\n\x19RestoreCustomHooksRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"S\n\x15SetCustomHooksRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"\x1c\n\x1aRestoreCustomHooksResponse\"\x18\n\x16SetCustomHooksResponse\"H\n\x18\x42\x61\x63kupCustomHooksRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"E\n\x15GetCustomHooksRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\")\n\x19\x42\x61\x63kupCustomHooksResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"&\n\x16GetCustomHooksResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"_\n!CreateRepositoryFromBundleRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"$\n\"CreateRepositoryFromBundleResponse\"B\n\x12\x46indLicenseRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x8c\x01\n\x13\x46indLicenseResponse\x12\x1a\n\x12license_short_name\x18\x01 \x01(\t\x12\x14\n\x0clicense_name\x18\x02 \x01(\t\x12\x13\n\x0blicense_url\x18\x03 \x01(\t\x12\x14\n\x0clicense_path\x18\x04 \x01(\t\x12\x18\n\x10license_nickname\x18\x05 \x01(\t\"H\n\x18GetInfoAttributesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"/\n\x19GetInfoAttributesResponse\x12\x12\n\nattributes\x18\x01 \x01(\x0c\"H\n\x18\x43\x61lculateChecksumRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"-\n\x19\x43\x61lculateChecksumResponse\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\t\"B\n\x12GetSnapshotRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"#\n\x13GetSnapshotResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"\xa3\x01\n#CreateRepositoryFromSnapshotRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08http_url\x18\x02 \x01(\t\x12\x11\n\thttp_auth\x18\x03 \x01(\t\x12\x18\n\x10resolved_address\x18\x05 \x01(\tJ\x04\x08\x04\x10\x05R\thttp_host\"&\n$CreateRepositoryFromSnapshotResponse\"p\n\x14GetRawChangesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x15\n\rfrom_revision\x18\x02 \x01(\t\x12\x13\n\x0bto_revision\x18\x03 \x01(\t\"\xbc\x03\n\x15GetRawChangesResponse\x12<\n\x0braw_changes\x18\x01 \x03(\x0b\x32\'.gitaly.GetRawChangesResponse.RawChange\x1a\xe4\x02\n\tRawChange\x12\x0f\n\x07\x62lob_id\x18\x01 \x01(\t\x12\x0c\n\x04size\x18\x02 \x01(\x03\x12\x44\n\toperation\x18\x05 \x01(\x0e\x32\x31.gitaly.GetRawChangesResponse.RawChange.Operation\x12\x10\n\x08old_mode\x18\x07 \x01(\x05\x12\x10\n\x08new_mode\x18\x08 \x01(\x05\x12\x16\n\x0enew_path_bytes\x18\t \x01(\x0c\x12\x16\n\x0eold_path_bytes\x18\n \x01(\x0c\"i\n\tOperation\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05\x41\x44\x44\x45\x44\x10\x01\x12\n\n\x06\x43OPIED\x10\x02\x12\x0b\n\x07\x44\x45LETED\x10\x03\x12\x0c\n\x08MODIFIED\x10\x04\x12\x0b\n\x07RENAMED\x10\x05\x12\x10\n\x0cTYPE_CHANGED\x10\x06J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x06\x10\x07R\x08new_pathR\x08old_pathR\rraw_operation\"\x93\x01\n\x18SearchFilesByNameRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\r\n\x05query\x18\x02 \x01(\t\x12\x0b\n\x03ref\x18\x03 \x01(\x0c\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\t\x12\r\n\x05limit\x18\x05 \x01(\r\x12\x0e\n\x06offset\x18\x06 \x01(\r\"*\n\x19SearchFilesByNameResponse\x12\r\n\x05\x66iles\x18\x01 \x03(\x0c\"\x7f\n\x1bSearchFilesByContentRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\r\n\x05query\x18\x02 \x01(\t\x12\x0b\n\x03ref\x18\x03 \x01(\x0cJ\x04\x08\x04\x10\x05R\x10\x63hunked_response\"W\n\x1cSearchFilesByContentResponse\x12\x12\n\nmatch_data\x18\x02 \x01(\x0c\x12\x14\n\x0c\x65nd_of_match\x18\x03 \x01(\x08J\x04\x08\x01\x10\x02R\x07matches\"\x87\x01\n\x06Remote\x12\x0b\n\x03url\x18\x01 \x01(\t\x12!\n\x19http_authorization_header\x18\x03 \x01(\t\x12\x16\n\x0emirror_refmaps\x18\x04 \x03(\t\x12\x18\n\x10resolved_address\x18\x06 \x01(\tJ\x04\x08\x02\x10\x03J\x04\x08\x05\x10\x06R\x04nameR\thttp_host\"M\n\x1dGetObjectDirectorySizeRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\".\n\x1eGetObjectDirectorySizeResponse\x12\x0c\n\x04size\x18\x01 \x01(\x03\"G\n\x17RemoveRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x1a\n\x18RemoveRepositoryResponse\"\xa9\x01\n\x1aReplicateRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\"\n\x06source\x18\x02 \x01(\x0b\x32\x12.gitaly.Repository\x12\x39\n1replicate_object_deduplication_network_membership\x18\x03 \x01(\x08\"\x1d\n\x1bReplicateRepositoryResponse\"\xdb\x01\n\x19OptimizeRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12<\n\x08strategy\x18\x02 \x01(\x0e\x32*.gitaly.OptimizeRepositoryRequest.Strategy\"R\n\x08Strategy\x12\x18\n\x14STRATEGY_UNSPECIFIED\x10\x00\x12\x18\n\x14STRATEGY_HEURISTICAL\x10\x01\x12\x12\n\x0eSTRATEGY_EAGER\x10\x02\"\x1c\n\x1aOptimizeRepositoryResponse\"N\n\x1ePruneUnreachableObjectsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"!\n\x1fPruneUnreachableObjectsResponse\"P\n\x12SetFullPathRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x15\n\x13SetFullPathResponse\"?\n\x0f\x46ullPathRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\" \n\x10\x46ullPathResponse\x12\x0c\n\x04path\x18\x01 \x01(\t\".\n\x10RemoveAllRequest\x12\x1a\n\x0cstorage_name\x18\x01 \x01(\tB\x04\x88\xc6,\x01\"\x13\n\x11RemoveAllResponse\"\x9e\x01\n\x17\x42\x61\x63kupRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12-\n\x11vanity_repository\x18\x02 \x01(\x0b\x32\x12.gitaly.Repository\x12\x11\n\tbackup_id\x18\x03 \x01(\t\x12\x13\n\x0bincremental\x18\x04 \x01(\x08\"*\n\x18\x42\x61\x63kupRepositoryResponse\x1a\x0e\n\x0cSkippedError\"\xa1\x01\n\x18RestoreRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12-\n\x11vanity_repository\x18\x02 \x01(\x0b\x32\x12.gitaly.Repository\x12\x11\n\tbackup_id\x18\x03 \x01(\t\x12\x15\n\ralways_create\x18\x04 \x01(\x08\"+\n\x19RestoreRepositoryResponse\x1a\x0e\n\x0cSkippedError\"}\n\x18GetFileAttributesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12\x12\n\nattributes\x18\x03 \x03(\t\x12\r\n\x05paths\x18\x04 \x03(\t\"\xa6\x01\n\x19GetFileAttributesResponse\x12H\n\x0f\x61ttribute_infos\x18\x01 \x03(\x0b\x32/.gitaly.GetFileAttributesResponse.AttributeInfo\x1a?\n\rAttributeInfo\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\tattribute\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t2\xb2 \n\x11RepositoryService\x12]\n\x10RepositoryExists\x12\x1f.gitaly.RepositoryExistsRequest\x1a .gitaly.RepositoryExistsResponse\"\x06\xfa\x97(\x02\x08\x02\x12W\n\x0eRepositorySize\x12\x1d.gitaly.RepositorySizeRequest\x1a\x1e.gitaly.RepositorySizeResponse\"\x06\xfa\x97(\x02\x08\x02\x12W\n\x0eRepositoryInfo\x12\x1d.gitaly.RepositoryInfoRequest\x1a\x1e.gitaly.RepositoryInfoResponse\"\x06\xfa\x97(\x02\x08\x02\x12P\n\x0bObjectsSize\x12\x1a.gitaly.ObjectsSizeRequest\x1a\x1b.gitaly.ObjectsSizeResponse\"\x06\xfa\x97(\x02\x08\x02(\x01\x12Q\n\x0cObjectFormat\x12\x1b.gitaly.ObjectFormatRequest\x1a\x1c.gitaly.ObjectFormatResponse\"\x06\xfa\x97(\x02\x08\x02\x12\x66\n\x12\x41pplyGitattributes\x12!.gitaly.ApplyGitattributesRequest\x1a\".gitaly.ApplyGitattributesResponse\"\t\x88\x02\x01\xfa\x97(\x02\x08\x01\x12N\n\x0b\x46\x65tchRemote\x12\x1a.gitaly.FetchRemoteRequest\x1a\x1b.gitaly.FetchRemoteResponse\"\x06\xfa\x97(\x02\x08\x01\x12]\n\x10\x43reateRepository\x12\x1f.gitaly.CreateRepositoryRequest\x1a .gitaly.CreateRepositoryResponse\"\x06\xfa\x97(\x02\x08\x01\x12M\n\nGetArchive\x12\x19.gitaly.GetArchiveRequest\x1a\x1a.gitaly.GetArchiveResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12]\n\x10HasLocalBranches\x12\x1f.gitaly.HasLocalBranchesRequest\x1a .gitaly.HasLocalBranchesResponse\"\x06\xfa\x97(\x02\x08\x02\x12`\n\x11\x46\x65tchSourceBranch\x12 .gitaly.FetchSourceBranchRequest\x1a!.gitaly.FetchSourceBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12\x39\n\x04\x46sck\x12\x13.gitaly.FsckRequest\x1a\x14.gitaly.FsckResponse\"\x06\xfa\x97(\x02\x08\x02\x12\x45\n\x08WriteRef\x12\x17.gitaly.WriteRefRequest\x1a\x18.gitaly.WriteRefResponse\"\x06\xfa\x97(\x02\x08\x01\x12T\n\rFindMergeBase\x12\x1c.gitaly.FindMergeBaseRequest\x1a\x1d.gitaly.FindMergeBaseResponse\"\x06\xfa\x97(\x02\x08\x02\x12K\n\nCreateFork\x12\x19.gitaly.CreateForkRequest\x1a\x1a.gitaly.CreateForkResponse\"\x06\xfa\x97(\x02\x08\x01\x12r\n\x17\x43reateRepositoryFromURL\x12&.gitaly.CreateRepositoryFromURLRequest\x1a\'.gitaly.CreateRepositoryFromURLResponse\"\x06\xfa\x97(\x02\x08\x01\x12S\n\x0c\x43reateBundle\x12\x1b.gitaly.CreateBundleRequest\x1a\x1c.gitaly.CreateBundleResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12v\n\x17\x43reateBundleFromRefList\x12&.gitaly.CreateBundleFromRefListRequest\x1a\'.gitaly.CreateBundleFromRefListResponse\"\x06\xfa\x97(\x02\x08\x02(\x01\x30\x01\x12P\n\x0b\x46\x65tchBundle\x12\x1a.gitaly.FetchBundleRequest\x1a\x1b.gitaly.FetchBundleResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x12}\n\x1a\x43reateRepositoryFromBundle\x12).gitaly.CreateRepositoryFromBundleRequest\x1a*.gitaly.CreateRepositoryFromBundleResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x12J\n\tGetConfig\x12\x18.gitaly.GetConfigRequest\x1a\x19.gitaly.GetConfigResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12N\n\x0b\x46indLicense\x12\x1a.gitaly.FindLicenseRequest\x1a\x1b.gitaly.FindLicenseResponse\"\x06\xfa\x97(\x02\x08\x02\x12\x65\n\x11GetInfoAttributes\x12 .gitaly.GetInfoAttributesRequest\x1a!.gitaly.GetInfoAttributesResponse\"\t\x88\x02\x01\xfa\x97(\x02\x08\x02\x30\x01\x12`\n\x11\x43\x61lculateChecksum\x12 .gitaly.CalculateChecksumRequest\x1a!.gitaly.CalculateChecksumResponse\"\x06\xfa\x97(\x02\x08\x02\x12P\n\x0bGetSnapshot\x12\x1a.gitaly.GetSnapshotRequest\x1a\x1b.gitaly.GetSnapshotResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\x81\x01\n\x1c\x43reateRepositoryFromSnapshot\x12+.gitaly.CreateRepositoryFromSnapshotRequest\x1a,.gitaly.CreateRepositoryFromSnapshotResponse\"\x06\xfa\x97(\x02\x08\x01\x12V\n\rGetRawChanges\x12\x1c.gitaly.GetRawChangesRequest\x1a\x1d.gitaly.GetRawChangesResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12k\n\x14SearchFilesByContent\x12#.gitaly.SearchFilesByContentRequest\x1a$.gitaly.SearchFilesByContentResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\x62\n\x11SearchFilesByName\x12 .gitaly.SearchFilesByNameRequest\x1a!.gitaly.SearchFilesByNameResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12h\n\x12RestoreCustomHooks\x12!.gitaly.RestoreCustomHooksRequest\x1a\".gitaly.RestoreCustomHooksResponse\"\t\x88\x02\x01\xfa\x97(\x02\x08\x01(\x01\x12Y\n\x0eSetCustomHooks\x12\x1d.gitaly.SetCustomHooksRequest\x1a\x1e.gitaly.SetCustomHooksResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x12\x65\n\x11\x42\x61\x63kupCustomHooks\x12 .gitaly.BackupCustomHooksRequest\x1a!.gitaly.BackupCustomHooksResponse\"\t\x88\x02\x01\xfa\x97(\x02\x08\x02\x30\x01\x12Y\n\x0eGetCustomHooks\x12\x1d.gitaly.GetCustomHooksRequest\x1a\x1e.gitaly.GetCustomHooksResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12o\n\x16GetObjectDirectorySize\x12%.gitaly.GetObjectDirectorySizeRequest\x1a&.gitaly.GetObjectDirectorySizeResponse\"\x06\xfa\x97(\x02\x08\x02\x12]\n\x10RemoveRepository\x12\x1f.gitaly.RemoveRepositoryRequest\x1a .gitaly.RemoveRepositoryResponse\"\x06\xfa\x97(\x02\x08\x01\x12\x66\n\x13ReplicateRepository\x12\".gitaly.ReplicateRepositoryRequest\x1a#.gitaly.ReplicateRepositoryResponse\"\x06\xfa\x97(\x02\x08\x01\x12\x63\n\x12OptimizeRepository\x12!.gitaly.OptimizeRepositoryRequest\x1a\".gitaly.OptimizeRepositoryResponse\"\x06\xfa\x97(\x02\x08\x03\x12r\n\x17PruneUnreachableObjects\x12&.gitaly.PruneUnreachableObjectsRequest\x1a\'.gitaly.PruneUnreachableObjectsResponse\"\x06\xfa\x97(\x02\x08\x03\x12Q\n\x0bSetFullPath\x12\x1a.gitaly.SetFullPathRequest\x1a\x1b.gitaly.SetFullPathResponse\"\t\x88\x02\x01\xfa\x97(\x02\x08\x01\x12H\n\x08\x46ullPath\x12\x17.gitaly.FullPathRequest\x1a\x18.gitaly.FullPathResponse\"\t\x88\x02\x01\xfa\x97(\x02\x08\x02\x12M\n\tRemoveAll\x12\x18.gitaly.RemoveAllRequest\x1a\x19.gitaly.RemoveAllResponse\"\x0b\x88\x02\x01\xfa\x97(\x04\x08\x01\x10\x02\x12]\n\x10\x42\x61\x63kupRepository\x12\x1f.gitaly.BackupRepositoryRequest\x1a .gitaly.BackupRepositoryResponse\"\x06\xfa\x97(\x02\x08\x02\x12`\n\x11RestoreRepository\x12 .gitaly.RestoreRepositoryRequest\x1a!.gitaly.RestoreRepositoryResponse\"\x06\xfa\x97(\x02\x08\x01\x12`\n\x11GetFileAttributes\x12 .gitaly.GetFileAttributesRequest\x1a!.gitaly.GetFileAttributesResponse\"\x06\xfa\x97(\x02\x08\x02\x42\x34Z2gitlab.com/gitlab-org/gitaly/v16/proto/go/gitalypbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10repository.proto\x12\x06gitaly\x1a\nlint.proto\x1a\x0cshared.proto\"G\n\x17RepositoryExistsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"*\n\x18RepositoryExistsResponse\x12\x0e\n\x06\x65xists\x18\x01 \x01(\x08\"E\n\x15RepositorySizeRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"&\n\x16RepositorySizeResponse\x12\x0c\n\x04size\x18\x01 \x01(\x03\"E\n\x15RepositoryInfoRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\xbb\x02\n\x16RepositoryInfoResponse\x12\x0c\n\x04size\x18\x01 \x01(\x04\x12\x41\n\nreferences\x18\x02 \x01(\x0b\x32-.gitaly.RepositoryInfoResponse.ReferencesInfo\x12;\n\x07objects\x18\x03 \x01(\x0b\x32*.gitaly.RepositoryInfoResponse.ObjectsInfo\x1a:\n\x0eReferencesInfo\x12\x13\n\x0bloose_count\x18\x01 \x01(\x04\x12\x13\n\x0bpacked_size\x18\x02 \x01(\x04\x1aW\n\x0bObjectsInfo\x12\x0c\n\x04size\x18\x01 \x01(\x04\x12\x13\n\x0brecent_size\x18\x02 \x01(\x04\x12\x12\n\nstale_size\x18\x03 \x01(\x04\x12\x11\n\tkeep_size\x18\x04 \x01(\x04\"U\n\x12ObjectsSizeRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\trevisions\x18\x02 \x03(\x0c\"#\n\x13ObjectsSizeResponse\x12\x0c\n\x04size\x18\x01 \x01(\x04\"C\n\x13ObjectFormatRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"<\n\x14ObjectFormatResponse\x12$\n\x06\x66ormat\x18\x01 \x01(\x0e\x32\x14.gitaly.ObjectFormat\"[\n\x19\x41pplyGitattributesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\"\x1c\n\x1a\x41pplyGitattributesResponse\"e\n\x12\x46\x65tchBundleRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x13\n\x0bupdate_head\x18\x03 \x01(\x08\"\x15\n\x13\x46\x65tchBundleResponse\"\x82\x02\n\x12\x46\x65tchRemoteRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\r\n\x05\x66orce\x18\x03 \x01(\x08\x12\x0f\n\x07no_tags\x18\x04 \x01(\x08\x12\x0f\n\x07timeout\x18\x05 \x01(\x05\x12\x0f\n\x07ssh_key\x18\x06 \x01(\t\x12\x13\n\x0bknown_hosts\x18\x07 \x01(\t\x12\x10\n\x08no_prune\x18\t \x01(\x08\x12%\n\rremote_params\x18\n \x01(\x0b\x32\x0e.gitaly.Remote\x12\x1a\n\x12\x63heck_tags_changed\x18\x0b \x01(\x08J\x04\x08\x08\x10\tJ\x04\x08\x02\x10\x03R\x06remote\"+\n\x13\x46\x65tchRemoteResponse\x12\x14\n\x0ctags_changed\x18\x01 \x01(\x08\"\x8c\x01\n\x17\x43reateRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0e\x64\x65\x66\x61ult_branch\x18\x02 \x01(\x0c\x12+\n\robject_format\x18\x03 \x01(\x0e\x32\x14.gitaly.ObjectFormat\"\x1a\n\x18\x43reateRepositoryResponse\"\x99\x02\n\x11GetArchiveRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\tcommit_id\x18\x02 \x01(\t\x12\x0e\n\x06prefix\x18\x03 \x01(\t\x12\x30\n\x06\x66ormat\x18\x04 \x01(\x0e\x32 .gitaly.GetArchiveRequest.Format\x12\x0c\n\x04path\x18\x05 \x01(\x0c\x12\x0f\n\x07\x65xclude\x18\x06 \x03(\x0c\x12\x12\n\nelide_path\x18\x07 \x01(\x08\x12\x19\n\x11include_lfs_blobs\x18\x08 \x01(\x08\"3\n\x06\x46ormat\x12\x07\n\x03ZIP\x10\x00\x12\x07\n\x03TAR\x10\x01\x12\n\n\x06TAR_GZ\x10\x02\x12\x0b\n\x07TAR_BZ2\x10\x03\"\"\n\x12GetArchiveResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"G\n\x17HasLocalBranchesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\")\n\x18HasLocalBranchesResponse\x12\r\n\x05value\x18\x01 \x01(\x08\"\xa2\x01\n\x18\x46\x65tchSourceBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12-\n\x11source_repository\x18\x02 \x01(\x0b\x32\x12.gitaly.Repository\x12\x15\n\rsource_branch\x18\x03 \x01(\x0c\x12\x12\n\ntarget_ref\x18\x04 \x01(\x0c\"+\n\x19\x46\x65tchSourceBranchResponse\x12\x0e\n\x06result\x18\x01 \x01(\x08\";\n\x0b\x46sckRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x1d\n\x0c\x46sckResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\x0c\"\x87\x01\n\x0fWriteRefRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0b\n\x03ref\x18\x02 \x01(\x0c\x12\x10\n\x08revision\x18\x03 \x01(\x0c\x12\x14\n\x0cold_revision\x18\x04 \x01(\x0cJ\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07R\x05\x66orce\"\x18\n\x10WriteRefResponseJ\x04\x08\x01\x10\x02\"W\n\x14\x46indMergeBaseRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\trevisions\x18\x02 \x03(\x0c\"%\n\x15\x46indMergeBaseResponse\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\"\x82\x01\n\x11\x43reateForkRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12-\n\x11source_repository\x18\x02 \x01(\x0b\x32\x12.gitaly.Repository\x12\x10\n\x08revision\x18\x03 \x01(\x0c\"\x14\n\x12\x43reateForkResponse\"\xb9\x01\n\x1e\x43reateRepositoryFromURLRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0b\n\x03url\x18\x02 \x01(\t\x12!\n\x19http_authorization_header\x18\x04 \x01(\t\x12\x0e\n\x06mirror\x18\x05 \x01(\x08\x12\x18\n\x10resolved_address\x18\x06 \x01(\tJ\x04\x08\x03\x10\x04R\thttp_host\"!\n\x1f\x43reateRepositoryFromURLResponse\"C\n\x13\x43reateBundleRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"$\n\x14\x43reateBundleResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"`\n\x1e\x43reateBundleFromRefListRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08patterns\x18\x02 \x03(\x0c\"/\n\x1f\x43reateBundleFromRefListResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"H\n\x18GenerateBundleURIRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x1b\n\x19GenerateBundleURIResponse\"@\n\x10GetConfigRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"!\n\x11GetConfigResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"W\n\x19RestoreCustomHooksRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"S\n\x15SetCustomHooksRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"\x1c\n\x1aRestoreCustomHooksResponse\"\x18\n\x16SetCustomHooksResponse\"H\n\x18\x42\x61\x63kupCustomHooksRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"E\n\x15GetCustomHooksRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\")\n\x19\x42\x61\x63kupCustomHooksResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"&\n\x16GetCustomHooksResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"_\n!CreateRepositoryFromBundleRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"$\n\"CreateRepositoryFromBundleResponse\"B\n\x12\x46indLicenseRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x8c\x01\n\x13\x46indLicenseResponse\x12\x1a\n\x12license_short_name\x18\x01 \x01(\t\x12\x14\n\x0clicense_name\x18\x02 \x01(\t\x12\x13\n\x0blicense_url\x18\x03 \x01(\t\x12\x14\n\x0clicense_path\x18\x04 \x01(\t\x12\x18\n\x10license_nickname\x18\x05 \x01(\t\"H\n\x18GetInfoAttributesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"/\n\x19GetInfoAttributesResponse\x12\x12\n\nattributes\x18\x01 \x01(\x0c\"H\n\x18\x43\x61lculateChecksumRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"-\n\x19\x43\x61lculateChecksumResponse\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\t\"B\n\x12GetSnapshotRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"#\n\x13GetSnapshotResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"\xa3\x01\n#CreateRepositoryFromSnapshotRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08http_url\x18\x02 \x01(\t\x12\x11\n\thttp_auth\x18\x03 \x01(\t\x12\x18\n\x10resolved_address\x18\x05 \x01(\tJ\x04\x08\x04\x10\x05R\thttp_host\"&\n$CreateRepositoryFromSnapshotResponse\"p\n\x14GetRawChangesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x15\n\rfrom_revision\x18\x02 \x01(\t\x12\x13\n\x0bto_revision\x18\x03 \x01(\t\"\xbc\x03\n\x15GetRawChangesResponse\x12<\n\x0braw_changes\x18\x01 \x03(\x0b\x32\'.gitaly.GetRawChangesResponse.RawChange\x1a\xe4\x02\n\tRawChange\x12\x0f\n\x07\x62lob_id\x18\x01 \x01(\t\x12\x0c\n\x04size\x18\x02 \x01(\x03\x12\x44\n\toperation\x18\x05 \x01(\x0e\x32\x31.gitaly.GetRawChangesResponse.RawChange.Operation\x12\x10\n\x08old_mode\x18\x07 \x01(\x05\x12\x10\n\x08new_mode\x18\x08 \x01(\x05\x12\x16\n\x0enew_path_bytes\x18\t \x01(\x0c\x12\x16\n\x0eold_path_bytes\x18\n \x01(\x0c\"i\n\tOperation\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05\x41\x44\x44\x45\x44\x10\x01\x12\n\n\x06\x43OPIED\x10\x02\x12\x0b\n\x07\x44\x45LETED\x10\x03\x12\x0c\n\x08MODIFIED\x10\x04\x12\x0b\n\x07RENAMED\x10\x05\x12\x10\n\x0cTYPE_CHANGED\x10\x06J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x06\x10\x07R\x08new_pathR\x08old_pathR\rraw_operation\"\x93\x01\n\x18SearchFilesByNameRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\r\n\x05query\x18\x02 \x01(\t\x12\x0b\n\x03ref\x18\x03 \x01(\x0c\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\t\x12\r\n\x05limit\x18\x05 \x01(\r\x12\x0e\n\x06offset\x18\x06 \x01(\r\"*\n\x19SearchFilesByNameResponse\x12\r\n\x05\x66iles\x18\x01 \x03(\x0c\"\x7f\n\x1bSearchFilesByContentRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\r\n\x05query\x18\x02 \x01(\t\x12\x0b\n\x03ref\x18\x03 \x01(\x0cJ\x04\x08\x04\x10\x05R\x10\x63hunked_response\"W\n\x1cSearchFilesByContentResponse\x12\x12\n\nmatch_data\x18\x02 \x01(\x0c\x12\x14\n\x0c\x65nd_of_match\x18\x03 \x01(\x08J\x04\x08\x01\x10\x02R\x07matches\"\x87\x01\n\x06Remote\x12\x0b\n\x03url\x18\x01 \x01(\t\x12!\n\x19http_authorization_header\x18\x03 \x01(\t\x12\x16\n\x0emirror_refmaps\x18\x04 \x03(\t\x12\x18\n\x10resolved_address\x18\x06 \x01(\tJ\x04\x08\x02\x10\x03J\x04\x08\x05\x10\x06R\x04nameR\thttp_host\"M\n\x1dGetObjectDirectorySizeRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\".\n\x1eGetObjectDirectorySizeResponse\x12\x0c\n\x04size\x18\x01 \x01(\x03\"G\n\x17RemoveRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x1a\n\x18RemoveRepositoryResponse\"n\n\x1aReplicateRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\"\n\x06source\x18\x02 \x01(\x0b\x32\x12.gitaly.Repository\"\x1d\n\x1bReplicateRepositoryResponse\"\xdb\x01\n\x19OptimizeRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12<\n\x08strategy\x18\x02 \x01(\x0e\x32*.gitaly.OptimizeRepositoryRequest.Strategy\"R\n\x08Strategy\x12\x18\n\x14STRATEGY_UNSPECIFIED\x10\x00\x12\x18\n\x14STRATEGY_HEURISTICAL\x10\x01\x12\x12\n\x0eSTRATEGY_EAGER\x10\x02\"\x1c\n\x1aOptimizeRepositoryResponse\"N\n\x1ePruneUnreachableObjectsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"!\n\x1fPruneUnreachableObjectsResponse\"\x9e\x01\n\x17\x42\x61\x63kupRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12-\n\x11vanity_repository\x18\x02 \x01(\x0b\x32\x12.gitaly.Repository\x12\x11\n\tbackup_id\x18\x03 \x01(\t\x12\x13\n\x0bincremental\x18\x04 \x01(\x08\"*\n\x18\x42\x61\x63kupRepositoryResponse\x1a\x0e\n\x0cSkippedError\"\xa1\x01\n\x18RestoreRepositoryRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12-\n\x11vanity_repository\x18\x02 \x01(\x0b\x32\x12.gitaly.Repository\x12\x11\n\tbackup_id\x18\x03 \x01(\t\x12\x15\n\ralways_create\x18\x04 \x01(\x08\"+\n\x19RestoreRepositoryResponse\x1a\x0e\n\x0cSkippedError\"}\n\x18GetFileAttributesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08revision\x18\x02 \x01(\x0c\x12\x12\n\nattributes\x18\x03 \x03(\t\x12\r\n\x05paths\x18\x04 \x03(\t\"\xa6\x01\n\x19GetFileAttributesResponse\x12H\n\x0f\x61ttribute_infos\x18\x01 \x03(\x0b\x32/.gitaly.GetFileAttributesResponse.AttributeInfo\x1a?\n\rAttributeInfo\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\tattribute\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t2\xa8\x1f\n\x11RepositoryService\x12]\n\x10RepositoryExists\x12\x1f.gitaly.RepositoryExistsRequest\x1a .gitaly.RepositoryExistsResponse\"\x06\xfa\x97(\x02\x08\x02\x12W\n\x0eRepositorySize\x12\x1d.gitaly.RepositorySizeRequest\x1a\x1e.gitaly.RepositorySizeResponse\"\x06\xfa\x97(\x02\x08\x02\x12W\n\x0eRepositoryInfo\x12\x1d.gitaly.RepositoryInfoRequest\x1a\x1e.gitaly.RepositoryInfoResponse\"\x06\xfa\x97(\x02\x08\x02\x12P\n\x0bObjectsSize\x12\x1a.gitaly.ObjectsSizeRequest\x1a\x1b.gitaly.ObjectsSizeResponse\"\x06\xfa\x97(\x02\x08\x02(\x01\x12Q\n\x0cObjectFormat\x12\x1b.gitaly.ObjectFormatRequest\x1a\x1c.gitaly.ObjectFormatResponse\"\x06\xfa\x97(\x02\x08\x02\x12\x66\n\x12\x41pplyGitattributes\x12!.gitaly.ApplyGitattributesRequest\x1a\".gitaly.ApplyGitattributesResponse\"\t\x88\x02\x01\xfa\x97(\x02\x08\x01\x12N\n\x0b\x46\x65tchRemote\x12\x1a.gitaly.FetchRemoteRequest\x1a\x1b.gitaly.FetchRemoteResponse\"\x06\xfa\x97(\x02\x08\x01\x12]\n\x10\x43reateRepository\x12\x1f.gitaly.CreateRepositoryRequest\x1a .gitaly.CreateRepositoryResponse\"\x06\xfa\x97(\x02\x08\x01\x12M\n\nGetArchive\x12\x19.gitaly.GetArchiveRequest\x1a\x1a.gitaly.GetArchiveResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12]\n\x10HasLocalBranches\x12\x1f.gitaly.HasLocalBranchesRequest\x1a .gitaly.HasLocalBranchesResponse\"\x06\xfa\x97(\x02\x08\x02\x12`\n\x11\x46\x65tchSourceBranch\x12 .gitaly.FetchSourceBranchRequest\x1a!.gitaly.FetchSourceBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12\x39\n\x04\x46sck\x12\x13.gitaly.FsckRequest\x1a\x14.gitaly.FsckResponse\"\x06\xfa\x97(\x02\x08\x02\x12\x45\n\x08WriteRef\x12\x17.gitaly.WriteRefRequest\x1a\x18.gitaly.WriteRefResponse\"\x06\xfa\x97(\x02\x08\x01\x12T\n\rFindMergeBase\x12\x1c.gitaly.FindMergeBaseRequest\x1a\x1d.gitaly.FindMergeBaseResponse\"\x06\xfa\x97(\x02\x08\x02\x12K\n\nCreateFork\x12\x19.gitaly.CreateForkRequest\x1a\x1a.gitaly.CreateForkResponse\"\x06\xfa\x97(\x02\x08\x01\x12r\n\x17\x43reateRepositoryFromURL\x12&.gitaly.CreateRepositoryFromURLRequest\x1a\'.gitaly.CreateRepositoryFromURLResponse\"\x06\xfa\x97(\x02\x08\x01\x12S\n\x0c\x43reateBundle\x12\x1b.gitaly.CreateBundleRequest\x1a\x1c.gitaly.CreateBundleResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12v\n\x17\x43reateBundleFromRefList\x12&.gitaly.CreateBundleFromRefListRequest\x1a\'.gitaly.CreateBundleFromRefListResponse\"\x06\xfa\x97(\x02\x08\x02(\x01\x30\x01\x12`\n\x11GenerateBundleURI\x12 .gitaly.GenerateBundleURIRequest\x1a!.gitaly.GenerateBundleURIResponse\"\x06\xfa\x97(\x02\x08\x02\x12P\n\x0b\x46\x65tchBundle\x12\x1a.gitaly.FetchBundleRequest\x1a\x1b.gitaly.FetchBundleResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x12}\n\x1a\x43reateRepositoryFromBundle\x12).gitaly.CreateRepositoryFromBundleRequest\x1a*.gitaly.CreateRepositoryFromBundleResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x12J\n\tGetConfig\x12\x18.gitaly.GetConfigRequest\x1a\x19.gitaly.GetConfigResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12N\n\x0b\x46indLicense\x12\x1a.gitaly.FindLicenseRequest\x1a\x1b.gitaly.FindLicenseResponse\"\x06\xfa\x97(\x02\x08\x02\x12\x65\n\x11GetInfoAttributes\x12 .gitaly.GetInfoAttributesRequest\x1a!.gitaly.GetInfoAttributesResponse\"\t\x88\x02\x01\xfa\x97(\x02\x08\x02\x30\x01\x12`\n\x11\x43\x61lculateChecksum\x12 .gitaly.CalculateChecksumRequest\x1a!.gitaly.CalculateChecksumResponse\"\x06\xfa\x97(\x02\x08\x02\x12P\n\x0bGetSnapshot\x12\x1a.gitaly.GetSnapshotRequest\x1a\x1b.gitaly.GetSnapshotResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\x81\x01\n\x1c\x43reateRepositoryFromSnapshot\x12+.gitaly.CreateRepositoryFromSnapshotRequest\x1a,.gitaly.CreateRepositoryFromSnapshotResponse\"\x06\xfa\x97(\x02\x08\x01\x12V\n\rGetRawChanges\x12\x1c.gitaly.GetRawChangesRequest\x1a\x1d.gitaly.GetRawChangesResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12k\n\x14SearchFilesByContent\x12#.gitaly.SearchFilesByContentRequest\x1a$.gitaly.SearchFilesByContentResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\x62\n\x11SearchFilesByName\x12 .gitaly.SearchFilesByNameRequest\x1a!.gitaly.SearchFilesByNameResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12h\n\x12RestoreCustomHooks\x12!.gitaly.RestoreCustomHooksRequest\x1a\".gitaly.RestoreCustomHooksResponse\"\t\x88\x02\x01\xfa\x97(\x02\x08\x01(\x01\x12Y\n\x0eSetCustomHooks\x12\x1d.gitaly.SetCustomHooksRequest\x1a\x1e.gitaly.SetCustomHooksResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x12\x65\n\x11\x42\x61\x63kupCustomHooks\x12 .gitaly.BackupCustomHooksRequest\x1a!.gitaly.BackupCustomHooksResponse\"\t\x88\x02\x01\xfa\x97(\x02\x08\x02\x30\x01\x12Y\n\x0eGetCustomHooks\x12\x1d.gitaly.GetCustomHooksRequest\x1a\x1e.gitaly.GetCustomHooksResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12o\n\x16GetObjectDirectorySize\x12%.gitaly.GetObjectDirectorySizeRequest\x1a&.gitaly.GetObjectDirectorySizeResponse\"\x06\xfa\x97(\x02\x08\x02\x12]\n\x10RemoveRepository\x12\x1f.gitaly.RemoveRepositoryRequest\x1a .gitaly.RemoveRepositoryResponse\"\x06\xfa\x97(\x02\x08\x01\x12\x66\n\x13ReplicateRepository\x12\".gitaly.ReplicateRepositoryRequest\x1a#.gitaly.ReplicateRepositoryResponse\"\x06\xfa\x97(\x02\x08\x01\x12\x63\n\x12OptimizeRepository\x12!.gitaly.OptimizeRepositoryRequest\x1a\".gitaly.OptimizeRepositoryResponse\"\x06\xfa\x97(\x02\x08\x03\x12r\n\x17PruneUnreachableObjects\x12&.gitaly.PruneUnreachableObjectsRequest\x1a\'.gitaly.PruneUnreachableObjectsResponse\"\x06\xfa\x97(\x02\x08\x03\x12]\n\x10\x42\x61\x63kupRepository\x12\x1f.gitaly.BackupRepositoryRequest\x1a .gitaly.BackupRepositoryResponse\"\x06\xfa\x97(\x02\x08\x02\x12`\n\x11RestoreRepository\x12 .gitaly.RestoreRepositoryRequest\x1a!.gitaly.RestoreRepositoryResponse\"\x06\xfa\x97(\x02\x08\x01\x12`\n\x11GetFileAttributes\x12 .gitaly.GetFileAttributesRequest\x1a!.gitaly.GetFileAttributesResponse\"\x06\xfa\x97(\x02\x08\x02\x42\x34Z2gitlab.com/gitlab-org/gitaly/v16/proto/go/gitalypbb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'repository_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -58,14 +58,16 @@
   _CREATEFORKREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
   _CREATEREPOSITORYFROMURLREQUEST.fields_by_name['repository']._options = None
   _CREATEREPOSITORYFROMURLREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
   _CREATEBUNDLEREQUEST.fields_by_name['repository']._options = None
   _CREATEBUNDLEREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
   _CREATEBUNDLEFROMREFLISTREQUEST.fields_by_name['repository']._options = None
   _CREATEBUNDLEFROMREFLISTREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
+  _GENERATEBUNDLEURIREQUEST.fields_by_name['repository']._options = None
+  _GENERATEBUNDLEURIREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
   _GETCONFIGREQUEST.fields_by_name['repository']._options = None
   _GETCONFIGREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
   _RESTORECUSTOMHOOKSREQUEST.fields_by_name['repository']._options = None
   _RESTORECUSTOMHOOKSREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
   _SETCUSTOMHOOKSREQUEST.fields_by_name['repository']._options = None
   _SETCUSTOMHOOKSREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
   _BACKUPCUSTOMHOOKSREQUEST.fields_by_name['repository']._options = None
@@ -96,20 +98,14 @@
   _REMOVEREPOSITORYREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
   _REPLICATEREPOSITORYREQUEST.fields_by_name['repository']._options = None
   _REPLICATEREPOSITORYREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
   _OPTIMIZEREPOSITORYREQUEST.fields_by_name['repository']._options = None
   _OPTIMIZEREPOSITORYREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
   _PRUNEUNREACHABLEOBJECTSREQUEST.fields_by_name['repository']._options = None
   _PRUNEUNREACHABLEOBJECTSREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
-  _SETFULLPATHREQUEST.fields_by_name['repository']._options = None
-  _SETFULLPATHREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
-  _FULLPATHREQUEST.fields_by_name['repository']._options = None
-  _FULLPATHREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
-  _REMOVEALLREQUEST.fields_by_name['storage_name']._options = None
-  _REMOVEALLREQUEST.fields_by_name['storage_name']._serialized_options = b'\210\306,\001'
   _BACKUPREPOSITORYREQUEST.fields_by_name['repository']._options = None
   _BACKUPREPOSITORYREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
   _RESTOREREPOSITORYREQUEST.fields_by_name['repository']._options = None
   _RESTOREREPOSITORYREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
   _GETFILEATTRIBUTESREQUEST.fields_by_name['repository']._options = None
   _GETFILEATTRIBUTESREQUEST.fields_by_name['repository']._serialized_options = b'\230\306,\001'
   _REPOSITORYSERVICE.methods_by_name['RepositoryExists']._options = None
@@ -144,14 +140,16 @@
   _REPOSITORYSERVICE.methods_by_name['CreateFork']._serialized_options = b'\372\227(\002\010\001'
   _REPOSITORYSERVICE.methods_by_name['CreateRepositoryFromURL']._options = None
   _REPOSITORYSERVICE.methods_by_name['CreateRepositoryFromURL']._serialized_options = b'\372\227(\002\010\001'
   _REPOSITORYSERVICE.methods_by_name['CreateBundle']._options = None
   _REPOSITORYSERVICE.methods_by_name['CreateBundle']._serialized_options = b'\372\227(\002\010\002'
   _REPOSITORYSERVICE.methods_by_name['CreateBundleFromRefList']._options = None
   _REPOSITORYSERVICE.methods_by_name['CreateBundleFromRefList']._serialized_options = b'\372\227(\002\010\002'
+  _REPOSITORYSERVICE.methods_by_name['GenerateBundleURI']._options = None
+  _REPOSITORYSERVICE.methods_by_name['GenerateBundleURI']._serialized_options = b'\372\227(\002\010\002'
   _REPOSITORYSERVICE.methods_by_name['FetchBundle']._options = None
   _REPOSITORYSERVICE.methods_by_name['FetchBundle']._serialized_options = b'\372\227(\002\010\001'
   _REPOSITORYSERVICE.methods_by_name['CreateRepositoryFromBundle']._options = None
   _REPOSITORYSERVICE.methods_by_name['CreateRepositoryFromBundle']._serialized_options = b'\372\227(\002\010\001'
   _REPOSITORYSERVICE.methods_by_name['GetConfig']._options = None
   _REPOSITORYSERVICE.methods_by_name['GetConfig']._serialized_options = b'\372\227(\002\010\002'
   _REPOSITORYSERVICE.methods_by_name['FindLicense']._options = None
@@ -184,20 +182,14 @@
   _REPOSITORYSERVICE.methods_by_name['RemoveRepository']._serialized_options = b'\372\227(\002\010\001'
   _REPOSITORYSERVICE.methods_by_name['ReplicateRepository']._options = None
   _REPOSITORYSERVICE.methods_by_name['ReplicateRepository']._serialized_options = b'\372\227(\002\010\001'
   _REPOSITORYSERVICE.methods_by_name['OptimizeRepository']._options = None
   _REPOSITORYSERVICE.methods_by_name['OptimizeRepository']._serialized_options = b'\372\227(\002\010\003'
   _REPOSITORYSERVICE.methods_by_name['PruneUnreachableObjects']._options = None
   _REPOSITORYSERVICE.methods_by_name['PruneUnreachableObjects']._serialized_options = b'\372\227(\002\010\003'
-  _REPOSITORYSERVICE.methods_by_name['SetFullPath']._options = None
-  _REPOSITORYSERVICE.methods_by_name['SetFullPath']._serialized_options = b'\210\002\001\372\227(\002\010\001'
-  _REPOSITORYSERVICE.methods_by_name['FullPath']._options = None
-  _REPOSITORYSERVICE.methods_by_name['FullPath']._serialized_options = b'\210\002\001\372\227(\002\010\002'
-  _REPOSITORYSERVICE.methods_by_name['RemoveAll']._options = None
-  _REPOSITORYSERVICE.methods_by_name['RemoveAll']._serialized_options = b'\210\002\001\372\227(\004\010\001\020\002'
   _REPOSITORYSERVICE.methods_by_name['BackupRepository']._options = None
   _REPOSITORYSERVICE.methods_by_name['BackupRepository']._serialized_options = b'\372\227(\002\010\002'
   _REPOSITORYSERVICE.methods_by_name['RestoreRepository']._options = None
   _REPOSITORYSERVICE.methods_by_name['RestoreRepository']._serialized_options = b'\372\227(\002\010\001'
   _REPOSITORYSERVICE.methods_by_name['GetFileAttributes']._options = None
   _REPOSITORYSERVICE.methods_by_name['GetFileAttributes']._serialized_options = b'\372\227(\002\010\002'
   _globals['_REPOSITORYEXISTSREQUEST']._serialized_start=54
@@ -278,124 +270,116 @@
   _globals['_CREATEBUNDLEREQUEST']._serialized_end=3127
   _globals['_CREATEBUNDLERESPONSE']._serialized_start=3129
   _globals['_CREATEBUNDLERESPONSE']._serialized_end=3165
   _globals['_CREATEBUNDLEFROMREFLISTREQUEST']._serialized_start=3167
   _globals['_CREATEBUNDLEFROMREFLISTREQUEST']._serialized_end=3263
   _globals['_CREATEBUNDLEFROMREFLISTRESPONSE']._serialized_start=3265
   _globals['_CREATEBUNDLEFROMREFLISTRESPONSE']._serialized_end=3312
-  _globals['_GETCONFIGREQUEST']._serialized_start=3314
-  _globals['_GETCONFIGREQUEST']._serialized_end=3378
-  _globals['_GETCONFIGRESPONSE']._serialized_start=3380
-  _globals['_GETCONFIGRESPONSE']._serialized_end=3413
-  _globals['_RESTORECUSTOMHOOKSREQUEST']._serialized_start=3415
-  _globals['_RESTORECUSTOMHOOKSREQUEST']._serialized_end=3502
-  _globals['_SETCUSTOMHOOKSREQUEST']._serialized_start=3504
-  _globals['_SETCUSTOMHOOKSREQUEST']._serialized_end=3587
-  _globals['_RESTORECUSTOMHOOKSRESPONSE']._serialized_start=3589
-  _globals['_RESTORECUSTOMHOOKSRESPONSE']._serialized_end=3617
-  _globals['_SETCUSTOMHOOKSRESPONSE']._serialized_start=3619
-  _globals['_SETCUSTOMHOOKSRESPONSE']._serialized_end=3643
-  _globals['_BACKUPCUSTOMHOOKSREQUEST']._serialized_start=3645
-  _globals['_BACKUPCUSTOMHOOKSREQUEST']._serialized_end=3717
-  _globals['_GETCUSTOMHOOKSREQUEST']._serialized_start=3719
-  _globals['_GETCUSTOMHOOKSREQUEST']._serialized_end=3788
-  _globals['_BACKUPCUSTOMHOOKSRESPONSE']._serialized_start=3790
-  _globals['_BACKUPCUSTOMHOOKSRESPONSE']._serialized_end=3831
-  _globals['_GETCUSTOMHOOKSRESPONSE']._serialized_start=3833
-  _globals['_GETCUSTOMHOOKSRESPONSE']._serialized_end=3871
-  _globals['_CREATEREPOSITORYFROMBUNDLEREQUEST']._serialized_start=3873
-  _globals['_CREATEREPOSITORYFROMBUNDLEREQUEST']._serialized_end=3968
-  _globals['_CREATEREPOSITORYFROMBUNDLERESPONSE']._serialized_start=3970
-  _globals['_CREATEREPOSITORYFROMBUNDLERESPONSE']._serialized_end=4006
-  _globals['_FINDLICENSEREQUEST']._serialized_start=4008
-  _globals['_FINDLICENSEREQUEST']._serialized_end=4074
-  _globals['_FINDLICENSERESPONSE']._serialized_start=4077
-  _globals['_FINDLICENSERESPONSE']._serialized_end=4217
-  _globals['_GETINFOATTRIBUTESREQUEST']._serialized_start=4219
-  _globals['_GETINFOATTRIBUTESREQUEST']._serialized_end=4291
-  _globals['_GETINFOATTRIBUTESRESPONSE']._serialized_start=4293
-  _globals['_GETINFOATTRIBUTESRESPONSE']._serialized_end=4340
-  _globals['_CALCULATECHECKSUMREQUEST']._serialized_start=4342
-  _globals['_CALCULATECHECKSUMREQUEST']._serialized_end=4414
-  _globals['_CALCULATECHECKSUMRESPONSE']._serialized_start=4416
-  _globals['_CALCULATECHECKSUMRESPONSE']._serialized_end=4461
-  _globals['_GETSNAPSHOTREQUEST']._serialized_start=4463
-  _globals['_GETSNAPSHOTREQUEST']._serialized_end=4529
-  _globals['_GETSNAPSHOTRESPONSE']._serialized_start=4531
-  _globals['_GETSNAPSHOTRESPONSE']._serialized_end=4566
-  _globals['_CREATEREPOSITORYFROMSNAPSHOTREQUEST']._serialized_start=4569
-  _globals['_CREATEREPOSITORYFROMSNAPSHOTREQUEST']._serialized_end=4732
-  _globals['_CREATEREPOSITORYFROMSNAPSHOTRESPONSE']._serialized_start=4734
-  _globals['_CREATEREPOSITORYFROMSNAPSHOTRESPONSE']._serialized_end=4772
-  _globals['_GETRAWCHANGESREQUEST']._serialized_start=4774
-  _globals['_GETRAWCHANGESREQUEST']._serialized_end=4886
-  _globals['_GETRAWCHANGESRESPONSE']._serialized_start=4889
-  _globals['_GETRAWCHANGESRESPONSE']._serialized_end=5333
-  _globals['_GETRAWCHANGESRESPONSE_RAWCHANGE']._serialized_start=4977
-  _globals['_GETRAWCHANGESRESPONSE_RAWCHANGE']._serialized_end=5333
-  _globals['_GETRAWCHANGESRESPONSE_RAWCHANGE_OPERATION']._serialized_start=5175
-  _globals['_GETRAWCHANGESRESPONSE_RAWCHANGE_OPERATION']._serialized_end=5280
-  _globals['_SEARCHFILESBYNAMEREQUEST']._serialized_start=5336
-  _globals['_SEARCHFILESBYNAMEREQUEST']._serialized_end=5483
-  _globals['_SEARCHFILESBYNAMERESPONSE']._serialized_start=5485
-  _globals['_SEARCHFILESBYNAMERESPONSE']._serialized_end=5527
-  _globals['_SEARCHFILESBYCONTENTREQUEST']._serialized_start=5529
-  _globals['_SEARCHFILESBYCONTENTREQUEST']._serialized_end=5656
-  _globals['_SEARCHFILESBYCONTENTRESPONSE']._serialized_start=5658
-  _globals['_SEARCHFILESBYCONTENTRESPONSE']._serialized_end=5745
-  _globals['_REMOTE']._serialized_start=5748
-  _globals['_REMOTE']._serialized_end=5883
-  _globals['_GETOBJECTDIRECTORYSIZEREQUEST']._serialized_start=5885
-  _globals['_GETOBJECTDIRECTORYSIZEREQUEST']._serialized_end=5962
-  _globals['_GETOBJECTDIRECTORYSIZERESPONSE']._serialized_start=5964
-  _globals['_GETOBJECTDIRECTORYSIZERESPONSE']._serialized_end=6010
-  _globals['_REMOVEREPOSITORYREQUEST']._serialized_start=6012
-  _globals['_REMOVEREPOSITORYREQUEST']._serialized_end=6083
-  _globals['_REMOVEREPOSITORYRESPONSE']._serialized_start=6085
-  _globals['_REMOVEREPOSITORYRESPONSE']._serialized_end=6111
-  _globals['_REPLICATEREPOSITORYREQUEST']._serialized_start=6114
-  _globals['_REPLICATEREPOSITORYREQUEST']._serialized_end=6283
-  _globals['_REPLICATEREPOSITORYRESPONSE']._serialized_start=6285
-  _globals['_REPLICATEREPOSITORYRESPONSE']._serialized_end=6314
-  _globals['_OPTIMIZEREPOSITORYREQUEST']._serialized_start=6317
-  _globals['_OPTIMIZEREPOSITORYREQUEST']._serialized_end=6536
-  _globals['_OPTIMIZEREPOSITORYREQUEST_STRATEGY']._serialized_start=6454
-  _globals['_OPTIMIZEREPOSITORYREQUEST_STRATEGY']._serialized_end=6536
-  _globals['_OPTIMIZEREPOSITORYRESPONSE']._serialized_start=6538
-  _globals['_OPTIMIZEREPOSITORYRESPONSE']._serialized_end=6566
-  _globals['_PRUNEUNREACHABLEOBJECTSREQUEST']._serialized_start=6568
-  _globals['_PRUNEUNREACHABLEOBJECTSREQUEST']._serialized_end=6646
-  _globals['_PRUNEUNREACHABLEOBJECTSRESPONSE']._serialized_start=6648
-  _globals['_PRUNEUNREACHABLEOBJECTSRESPONSE']._serialized_end=6681
-  _globals['_SETFULLPATHREQUEST']._serialized_start=6683
-  _globals['_SETFULLPATHREQUEST']._serialized_end=6763
-  _globals['_SETFULLPATHRESPONSE']._serialized_start=6765
-  _globals['_SETFULLPATHRESPONSE']._serialized_end=6786
-  _globals['_FULLPATHREQUEST']._serialized_start=6788
-  _globals['_FULLPATHREQUEST']._serialized_end=6851
-  _globals['_FULLPATHRESPONSE']._serialized_start=6853
-  _globals['_FULLPATHRESPONSE']._serialized_end=6885
-  _globals['_REMOVEALLREQUEST']._serialized_start=6887
-  _globals['_REMOVEALLREQUEST']._serialized_end=6933
-  _globals['_REMOVEALLRESPONSE']._serialized_start=6935
-  _globals['_REMOVEALLRESPONSE']._serialized_end=6954
-  _globals['_BACKUPREPOSITORYREQUEST']._serialized_start=6957
-  _globals['_BACKUPREPOSITORYREQUEST']._serialized_end=7115
-  _globals['_BACKUPREPOSITORYRESPONSE']._serialized_start=7117
-  _globals['_BACKUPREPOSITORYRESPONSE']._serialized_end=7159
-  _globals['_BACKUPREPOSITORYRESPONSE_SKIPPEDERROR']._serialized_start=7145
-  _globals['_BACKUPREPOSITORYRESPONSE_SKIPPEDERROR']._serialized_end=7159
-  _globals['_RESTOREREPOSITORYREQUEST']._serialized_start=7162
-  _globals['_RESTOREREPOSITORYREQUEST']._serialized_end=7323
-  _globals['_RESTOREREPOSITORYRESPONSE']._serialized_start=7325
-  _globals['_RESTOREREPOSITORYRESPONSE']._serialized_end=7368
-  _globals['_RESTOREREPOSITORYRESPONSE_SKIPPEDERROR']._serialized_start=7145
-  _globals['_RESTOREREPOSITORYRESPONSE_SKIPPEDERROR']._serialized_end=7159
-  _globals['_GETFILEATTRIBUTESREQUEST']._serialized_start=7370
-  _globals['_GETFILEATTRIBUTESREQUEST']._serialized_end=7495
-  _globals['_GETFILEATTRIBUTESRESPONSE']._serialized_start=7498
-  _globals['_GETFILEATTRIBUTESRESPONSE']._serialized_end=7664
-  _globals['_GETFILEATTRIBUTESRESPONSE_ATTRIBUTEINFO']._serialized_start=7601
-  _globals['_GETFILEATTRIBUTESRESPONSE_ATTRIBUTEINFO']._serialized_end=7664
-  _globals['_REPOSITORYSERVICE']._serialized_start=7667
-  _globals['_REPOSITORYSERVICE']._serialized_end=11813
+  _globals['_GENERATEBUNDLEURIREQUEST']._serialized_start=3314
+  _globals['_GENERATEBUNDLEURIREQUEST']._serialized_end=3386
+  _globals['_GENERATEBUNDLEURIRESPONSE']._serialized_start=3388
+  _globals['_GENERATEBUNDLEURIRESPONSE']._serialized_end=3415
+  _globals['_GETCONFIGREQUEST']._serialized_start=3417
+  _globals['_GETCONFIGREQUEST']._serialized_end=3481
+  _globals['_GETCONFIGRESPONSE']._serialized_start=3483
+  _globals['_GETCONFIGRESPONSE']._serialized_end=3516
+  _globals['_RESTORECUSTOMHOOKSREQUEST']._serialized_start=3518
+  _globals['_RESTORECUSTOMHOOKSREQUEST']._serialized_end=3605
+  _globals['_SETCUSTOMHOOKSREQUEST']._serialized_start=3607
+  _globals['_SETCUSTOMHOOKSREQUEST']._serialized_end=3690
+  _globals['_RESTORECUSTOMHOOKSRESPONSE']._serialized_start=3692
+  _globals['_RESTORECUSTOMHOOKSRESPONSE']._serialized_end=3720
+  _globals['_SETCUSTOMHOOKSRESPONSE']._serialized_start=3722
+  _globals['_SETCUSTOMHOOKSRESPONSE']._serialized_end=3746
+  _globals['_BACKUPCUSTOMHOOKSREQUEST']._serialized_start=3748
+  _globals['_BACKUPCUSTOMHOOKSREQUEST']._serialized_end=3820
+  _globals['_GETCUSTOMHOOKSREQUEST']._serialized_start=3822
+  _globals['_GETCUSTOMHOOKSREQUEST']._serialized_end=3891
+  _globals['_BACKUPCUSTOMHOOKSRESPONSE']._serialized_start=3893
+  _globals['_BACKUPCUSTOMHOOKSRESPONSE']._serialized_end=3934
+  _globals['_GETCUSTOMHOOKSRESPONSE']._serialized_start=3936
+  _globals['_GETCUSTOMHOOKSRESPONSE']._serialized_end=3974
+  _globals['_CREATEREPOSITORYFROMBUNDLEREQUEST']._serialized_start=3976
+  _globals['_CREATEREPOSITORYFROMBUNDLEREQUEST']._serialized_end=4071
+  _globals['_CREATEREPOSITORYFROMBUNDLERESPONSE']._serialized_start=4073
+  _globals['_CREATEREPOSITORYFROMBUNDLERESPONSE']._serialized_end=4109
+  _globals['_FINDLICENSEREQUEST']._serialized_start=4111
+  _globals['_FINDLICENSEREQUEST']._serialized_end=4177
+  _globals['_FINDLICENSERESPONSE']._serialized_start=4180
+  _globals['_FINDLICENSERESPONSE']._serialized_end=4320
+  _globals['_GETINFOATTRIBUTESREQUEST']._serialized_start=4322
+  _globals['_GETINFOATTRIBUTESREQUEST']._serialized_end=4394
+  _globals['_GETINFOATTRIBUTESRESPONSE']._serialized_start=4396
+  _globals['_GETINFOATTRIBUTESRESPONSE']._serialized_end=4443
+  _globals['_CALCULATECHECKSUMREQUEST']._serialized_start=4445
+  _globals['_CALCULATECHECKSUMREQUEST']._serialized_end=4517
+  _globals['_CALCULATECHECKSUMRESPONSE']._serialized_start=4519
+  _globals['_CALCULATECHECKSUMRESPONSE']._serialized_end=4564
+  _globals['_GETSNAPSHOTREQUEST']._serialized_start=4566
+  _globals['_GETSNAPSHOTREQUEST']._serialized_end=4632
+  _globals['_GETSNAPSHOTRESPONSE']._serialized_start=4634
+  _globals['_GETSNAPSHOTRESPONSE']._serialized_end=4669
+  _globals['_CREATEREPOSITORYFROMSNAPSHOTREQUEST']._serialized_start=4672
+  _globals['_CREATEREPOSITORYFROMSNAPSHOTREQUEST']._serialized_end=4835
+  _globals['_CREATEREPOSITORYFROMSNAPSHOTRESPONSE']._serialized_start=4837
+  _globals['_CREATEREPOSITORYFROMSNAPSHOTRESPONSE']._serialized_end=4875
+  _globals['_GETRAWCHANGESREQUEST']._serialized_start=4877
+  _globals['_GETRAWCHANGESREQUEST']._serialized_end=4989
+  _globals['_GETRAWCHANGESRESPONSE']._serialized_start=4992
+  _globals['_GETRAWCHANGESRESPONSE']._serialized_end=5436
+  _globals['_GETRAWCHANGESRESPONSE_RAWCHANGE']._serialized_start=5080
+  _globals['_GETRAWCHANGESRESPONSE_RAWCHANGE']._serialized_end=5436
+  _globals['_GETRAWCHANGESRESPONSE_RAWCHANGE_OPERATION']._serialized_start=5278
+  _globals['_GETRAWCHANGESRESPONSE_RAWCHANGE_OPERATION']._serialized_end=5383
+  _globals['_SEARCHFILESBYNAMEREQUEST']._serialized_start=5439
+  _globals['_SEARCHFILESBYNAMEREQUEST']._serialized_end=5586
+  _globals['_SEARCHFILESBYNAMERESPONSE']._serialized_start=5588
+  _globals['_SEARCHFILESBYNAMERESPONSE']._serialized_end=5630
+  _globals['_SEARCHFILESBYCONTENTREQUEST']._serialized_start=5632
+  _globals['_SEARCHFILESBYCONTENTREQUEST']._serialized_end=5759
+  _globals['_SEARCHFILESBYCONTENTRESPONSE']._serialized_start=5761
+  _globals['_SEARCHFILESBYCONTENTRESPONSE']._serialized_end=5848
+  _globals['_REMOTE']._serialized_start=5851
+  _globals['_REMOTE']._serialized_end=5986
+  _globals['_GETOBJECTDIRECTORYSIZEREQUEST']._serialized_start=5988
+  _globals['_GETOBJECTDIRECTORYSIZEREQUEST']._serialized_end=6065
+  _globals['_GETOBJECTDIRECTORYSIZERESPONSE']._serialized_start=6067
+  _globals['_GETOBJECTDIRECTORYSIZERESPONSE']._serialized_end=6113
+  _globals['_REMOVEREPOSITORYREQUEST']._serialized_start=6115
+  _globals['_REMOVEREPOSITORYREQUEST']._serialized_end=6186
+  _globals['_REMOVEREPOSITORYRESPONSE']._serialized_start=6188
+  _globals['_REMOVEREPOSITORYRESPONSE']._serialized_end=6214
+  _globals['_REPLICATEREPOSITORYREQUEST']._serialized_start=6216
+  _globals['_REPLICATEREPOSITORYREQUEST']._serialized_end=6326
+  _globals['_REPLICATEREPOSITORYRESPONSE']._serialized_start=6328
+  _globals['_REPLICATEREPOSITORYRESPONSE']._serialized_end=6357
+  _globals['_OPTIMIZEREPOSITORYREQUEST']._serialized_start=6360
+  _globals['_OPTIMIZEREPOSITORYREQUEST']._serialized_end=6579
+  _globals['_OPTIMIZEREPOSITORYREQUEST_STRATEGY']._serialized_start=6497
+  _globals['_OPTIMIZEREPOSITORYREQUEST_STRATEGY']._serialized_end=6579
+  _globals['_OPTIMIZEREPOSITORYRESPONSE']._serialized_start=6581
+  _globals['_OPTIMIZEREPOSITORYRESPONSE']._serialized_end=6609
+  _globals['_PRUNEUNREACHABLEOBJECTSREQUEST']._serialized_start=6611
+  _globals['_PRUNEUNREACHABLEOBJECTSREQUEST']._serialized_end=6689
+  _globals['_PRUNEUNREACHABLEOBJECTSRESPONSE']._serialized_start=6691
+  _globals['_PRUNEUNREACHABLEOBJECTSRESPONSE']._serialized_end=6724
+  _globals['_BACKUPREPOSITORYREQUEST']._serialized_start=6727
+  _globals['_BACKUPREPOSITORYREQUEST']._serialized_end=6885
+  _globals['_BACKUPREPOSITORYRESPONSE']._serialized_start=6887
+  _globals['_BACKUPREPOSITORYRESPONSE']._serialized_end=6929
+  _globals['_BACKUPREPOSITORYRESPONSE_SKIPPEDERROR']._serialized_start=6915
+  _globals['_BACKUPREPOSITORYRESPONSE_SKIPPEDERROR']._serialized_end=6929
+  _globals['_RESTOREREPOSITORYREQUEST']._serialized_start=6932
+  _globals['_RESTOREREPOSITORYREQUEST']._serialized_end=7093
+  _globals['_RESTOREREPOSITORYRESPONSE']._serialized_start=7095
+  _globals['_RESTOREREPOSITORYRESPONSE']._serialized_end=7138
+  _globals['_RESTOREREPOSITORYRESPONSE_SKIPPEDERROR']._serialized_start=6915
+  _globals['_RESTOREREPOSITORYRESPONSE_SKIPPEDERROR']._serialized_end=6929
+  _globals['_GETFILEATTRIBUTESREQUEST']._serialized_start=7140
+  _globals['_GETFILEATTRIBUTESREQUEST']._serialized_end=7265
+  _globals['_GETFILEATTRIBUTESRESPONSE']._serialized_start=7268
+  _globals['_GETFILEATTRIBUTESRESPONSE']._serialized_end=7434
+  _globals['_GETFILEATTRIBUTESRESPONSE_ATTRIBUTEINFO']._serialized_start=7371
+  _globals['_GETFILEATTRIBUTESRESPONSE_ATTRIBUTEINFO']._serialized_end=7434
+  _globals['_REPOSITORYSERVICE']._serialized_start=7437
+  _globals['_REPOSITORYSERVICE']._serialized_end=11445
 # @@protoc_insertion_point(module_scope)
```

### Comparing `hgitaly-1.5.0/hgitaly/stub/repository_pb2_grpc.py` & `hgitaly-1.6.0/hgitaly/stub/repository_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,19 @@
                 response_deserializer=repository__pb2.CreateBundleResponse.FromString,
                 )
         self.CreateBundleFromRefList = channel.stream_stream(
                 '/gitaly.RepositoryService/CreateBundleFromRefList',
                 request_serializer=repository__pb2.CreateBundleFromRefListRequest.SerializeToString,
                 response_deserializer=repository__pb2.CreateBundleFromRefListResponse.FromString,
                 )
+        self.GenerateBundleURI = channel.unary_unary(
+                '/gitaly.RepositoryService/GenerateBundleURI',
+                request_serializer=repository__pb2.GenerateBundleURIRequest.SerializeToString,
+                response_deserializer=repository__pb2.GenerateBundleURIResponse.FromString,
+                )
         self.FetchBundle = channel.stream_unary(
                 '/gitaly.RepositoryService/FetchBundle',
                 request_serializer=repository__pb2.FetchBundleRequest.SerializeToString,
                 response_deserializer=repository__pb2.FetchBundleResponse.FromString,
                 )
         self.CreateRepositoryFromBundle = channel.stream_unary(
                 '/gitaly.RepositoryService/CreateRepositoryFromBundle',
@@ -201,29 +206,14 @@
                 response_deserializer=repository__pb2.OptimizeRepositoryResponse.FromString,
                 )
         self.PruneUnreachableObjects = channel.unary_unary(
                 '/gitaly.RepositoryService/PruneUnreachableObjects',
                 request_serializer=repository__pb2.PruneUnreachableObjectsRequest.SerializeToString,
                 response_deserializer=repository__pb2.PruneUnreachableObjectsResponse.FromString,
                 )
-        self.SetFullPath = channel.unary_unary(
-                '/gitaly.RepositoryService/SetFullPath',
-                request_serializer=repository__pb2.SetFullPathRequest.SerializeToString,
-                response_deserializer=repository__pb2.SetFullPathResponse.FromString,
-                )
-        self.FullPath = channel.unary_unary(
-                '/gitaly.RepositoryService/FullPath',
-                request_serializer=repository__pb2.FullPathRequest.SerializeToString,
-                response_deserializer=repository__pb2.FullPathResponse.FromString,
-                )
-        self.RemoveAll = channel.unary_unary(
-                '/gitaly.RepositoryService/RemoveAll',
-                request_serializer=repository__pb2.RemoveAllRequest.SerializeToString,
-                response_deserializer=repository__pb2.RemoveAllResponse.FromString,
-                )
         self.BackupRepository = channel.unary_unary(
                 '/gitaly.RepositoryService/BackupRepository',
                 request_serializer=repository__pb2.BackupRepositoryRequest.SerializeToString,
                 response_deserializer=repository__pb2.BackupRepositoryResponse.FromString,
                 )
         self.RestoreRepository = channel.unary_unary(
                 '/gitaly.RepositoryService/RestoreRepository',
@@ -402,14 +392,21 @@
         """CreateBundleFromRefList creates a bundle from a stream of ref patterns.
         When the bundle would be empty the FailedPrecondition error code is returned.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GenerateBundleURI(self, request, context):
+        """GenerateBundleURI generates a bundle on the server for bundle-URI use.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def FetchBundle(self, request_iterator, context):
         """FetchBundle fetches references from a bundle into the local repository.
         refs will be mirrored to the target repository with the refspec
         "+refs/*:refs/*" and refs that do not exist in the bundle will be removed.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
@@ -585,40 +582,14 @@
         to make proper use of this RPC you thus need to call OptimizeRepository,
         wait 30 minutes, and then call PruneUnreachableObjects.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SetFullPath(self, request, context):
-        """SetFullPath writes the "gitlab.fullpath" configuration into the
-        repository's gitconfig. This is mainly to help debugging purposes in case
-        an admin inspects the repository's gitconfig such that he can easily see
-        what the repository name is.
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def FullPath(self, request, context):
-        """FullPath reads the "gitlab.fullpath" configuration from the repository's
-        gitconfig. Returns an error in case the full path has not been configured.
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def RemoveAll(self, request, context):
-        """RemoveAll deletes all repositories on a specified storage.
-        Deprecated in favour of individually removing repositories with RemoveRepository.
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def BackupRepository(self, request, context):
         """BackupRepository creates a full or incremental backup streamed directly to
         object-storage. The backup is created synchronously. The destination must
         be configured in config.backup.go_cloud_url
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
@@ -729,14 +700,19 @@
                     response_serializer=repository__pb2.CreateBundleResponse.SerializeToString,
             ),
             'CreateBundleFromRefList': grpc.stream_stream_rpc_method_handler(
                     servicer.CreateBundleFromRefList,
                     request_deserializer=repository__pb2.CreateBundleFromRefListRequest.FromString,
                     response_serializer=repository__pb2.CreateBundleFromRefListResponse.SerializeToString,
             ),
+            'GenerateBundleURI': grpc.unary_unary_rpc_method_handler(
+                    servicer.GenerateBundleURI,
+                    request_deserializer=repository__pb2.GenerateBundleURIRequest.FromString,
+                    response_serializer=repository__pb2.GenerateBundleURIResponse.SerializeToString,
+            ),
             'FetchBundle': grpc.stream_unary_rpc_method_handler(
                     servicer.FetchBundle,
                     request_deserializer=repository__pb2.FetchBundleRequest.FromString,
                     response_serializer=repository__pb2.FetchBundleResponse.SerializeToString,
             ),
             'CreateRepositoryFromBundle': grpc.stream_unary_rpc_method_handler(
                     servicer.CreateRepositoryFromBundle,
@@ -829,29 +805,14 @@
                     response_serializer=repository__pb2.OptimizeRepositoryResponse.SerializeToString,
             ),
             'PruneUnreachableObjects': grpc.unary_unary_rpc_method_handler(
                     servicer.PruneUnreachableObjects,
                     request_deserializer=repository__pb2.PruneUnreachableObjectsRequest.FromString,
                     response_serializer=repository__pb2.PruneUnreachableObjectsResponse.SerializeToString,
             ),
-            'SetFullPath': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetFullPath,
-                    request_deserializer=repository__pb2.SetFullPathRequest.FromString,
-                    response_serializer=repository__pb2.SetFullPathResponse.SerializeToString,
-            ),
-            'FullPath': grpc.unary_unary_rpc_method_handler(
-                    servicer.FullPath,
-                    request_deserializer=repository__pb2.FullPathRequest.FromString,
-                    response_serializer=repository__pb2.FullPathResponse.SerializeToString,
-            ),
-            'RemoveAll': grpc.unary_unary_rpc_method_handler(
-                    servicer.RemoveAll,
-                    request_deserializer=repository__pb2.RemoveAllRequest.FromString,
-                    response_serializer=repository__pb2.RemoveAllResponse.SerializeToString,
-            ),
             'BackupRepository': grpc.unary_unary_rpc_method_handler(
                     servicer.BackupRepository,
                     request_deserializer=repository__pb2.BackupRepositoryRequest.FromString,
                     response_serializer=repository__pb2.BackupRepositoryResponse.SerializeToString,
             ),
             'RestoreRepository': grpc.unary_unary_rpc_method_handler(
                     servicer.RestoreRepository,
@@ -1177,14 +1138,31 @@
         return grpc.experimental.stream_stream(request_iterator, target, '/gitaly.RepositoryService/CreateBundleFromRefList',
             repository__pb2.CreateBundleFromRefListRequest.SerializeToString,
             repository__pb2.CreateBundleFromRefListResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GenerateBundleURI(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/gitaly.RepositoryService/GenerateBundleURI',
+            repository__pb2.GenerateBundleURIRequest.SerializeToString,
+            repository__pb2.GenerateBundleURIResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def FetchBundle(request_iterator,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -1517,65 +1495,14 @@
         return grpc.experimental.unary_unary(request, target, '/gitaly.RepositoryService/PruneUnreachableObjects',
             repository__pb2.PruneUnreachableObjectsRequest.SerializeToString,
             repository__pb2.PruneUnreachableObjectsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SetFullPath(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/gitaly.RepositoryService/SetFullPath',
-            repository__pb2.SetFullPathRequest.SerializeToString,
-            repository__pb2.SetFullPathResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def FullPath(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/gitaly.RepositoryService/FullPath',
-            repository__pb2.FullPathRequest.SerializeToString,
-            repository__pb2.FullPathResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def RemoveAll(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/gitaly.RepositoryService/RemoveAll',
-            repository__pb2.RemoveAllRequest.SerializeToString,
-            repository__pb2.RemoveAllResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def BackupRepository(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `hgitaly-1.5.0/hgitaly/stub/server_pb2.py` & `hgitaly-1.6.0/hgitaly/stub/server_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/server_pb2_grpc.py` & `hgitaly-1.6.0/hgitaly/stub/server_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/stub/shared_pb2.py` & `hgitaly-1.6.0/hgitaly/stub/shared_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tag.py` & `hgitaly-1.6.0/hgitaly/tag.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/testing/bundle.py` & `hgitaly-1.6.0/hgitaly/testing/bundle.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/testing/context.py` & `hgitaly-1.6.0/hgitaly/testing/context.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/testing/grpc.py` & `hgitaly-1.6.0/hgitaly/testing/grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/testing/ssh.py` & `hgitaly-1.6.0/hgitaly/testing/ssh.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/testing/sshd.py` & `hgitaly-1.6.0/hgitaly/testing/sshd.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/testing/tests/test_sshd.py` & `hgitaly-1.6.0/hgitaly/testing/tests/test_sshd.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/common.py` & `hgitaly-1.6.0/hgitaly/tests/common.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_branch.py` & `hgitaly-1.6.0/hgitaly/tests/test_branch.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_diff.py` & `hgitaly-1.6.0/hgitaly/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_errors.py` & `hgitaly-1.6.0/hgitaly/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_feature.py` & `hgitaly-1.6.0/hgitaly/tests/test_feature.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_file_context.py` & `hgitaly-1.6.0/hgitaly/tests/test_file_context.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_gitlab_ref.py` & `hgitaly-1.6.0/hgitaly/tests/test_gitlab_ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_license_detector.py` & `hgitaly-1.6.0/hgitaly/tests/test_license_detector.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_linguist.py` & `hgitaly-1.6.0/hgitaly/tests/test_linguist.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_manifest.py` & `hgitaly-1.6.0/hgitaly/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_messages.py` & `hgitaly-1.6.0/hgitaly/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_oid.py` & `hgitaly-1.6.0/hgitaly/tests/test_oid.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_peer.py` & `hgitaly-1.6.0/hgitaly/tests/test_peer.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_repository.py` & `hgitaly-1.6.0/hgitaly/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_revision.py` & `hgitaly-1.6.0/hgitaly/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_revset.py` & `hgitaly-1.6.0/hgitaly/tests/test_revset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_servicer.py` & `hgitaly-1.6.0/hgitaly/tests/test_servicer.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_stream.py` & `hgitaly-1.6.0/hgitaly/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_tag.py` & `hgitaly-1.6.0/hgitaly/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/tests/test_workdir.py` & `hgitaly-1.6.0/hgitaly/tests/test_workdir.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/util.py` & `hgitaly-1.6.0/hgitaly/util.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly/workdir.py` & `hgitaly-1.6.0/hgitaly/workdir.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/hgitaly.egg-info/PKG-INFO` & `hgitaly-1.6.0/hgitaly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgitaly
-Version: 1.5.0
+Version: 1.6.0
 Summary: Server-side implementation of Gitaly protocol for Mercurial
 Home-page: https://foss.heptapod.net/heptapod/hgitaly
 Author: Georges Racinet
 Author-email: georges.racinet@octobus.net
 License: GPLv2+
 Keywords: hg mercurial heptapod gitlab
 Requires-Python: >=3.8
```

### Comparing `hgitaly-1.5.0/hgitaly.egg-info/SOURCES.txt` & `hgitaly-1.6.0/hgitaly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/setup.py` & `hgitaly-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/tests_with_gitaly/__init__.py` & `hgitaly-1.6.0/tests_with_gitaly/__init__.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/tests_with_gitaly/comparison.py` & `hgitaly-1.6.0/tests_with_gitaly/comparison.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 )
 from hgitaly import feature
 from hgitaly.errors import HGITALY_ISSUES_URL
 from hgitaly.gitlab_ref import (
     keep_around_ref_path,
     parse_keep_around_ref_path,
 )
+from hgitaly.servicer import SKIP_HOOKS_MD_KEY
 from hgitaly.stub.shared_pb2 import Repository
 
 try:
     from itertools import batched
 except ImportError:  # Python<3.12
     def batched(it, n):
         # not sure in which version `while batch :=` is possible
@@ -157,14 +158,15 @@
                               monkeypatch,
                               rhgitaly_channel=None,
                               ):
     common_relative_path = 'repo-' + hex(random.getrandbits(64))[2:]
     storage = 'default'
 
     gitaly_repo = Repository(relative_path=common_relative_path + '.git',
+                             gl_repository='project-1234',
                              storage_name=storage)
     hgitaly_repo = Repository(relative_path=common_relative_path + '.hg',
                               storage_name=storage)
 
     hg_config = dict(phases=dict(publish=False),
                      ui=dict(username='Hgitaly Tests <hgitaly@heptapod.test>'),
                      extensions={name: '' for name in ('evolve',
@@ -222,15 +224,17 @@
         self.init_stubs()
 
     def init_stubs(self):
         """To be provided by subclasses."""
         raise NotImplementedError  # pragma no cover
 
     def grpc_metadata(self):
-        return feature.as_grpc_metadata(self.feature_flags)
+        mds = feature.as_grpc_metadata(self.feature_flags)
+        mds.append((SKIP_HOOKS_MD_KEY, 'true'))
+        return mds
 
     def stream_requests(self, **kwargs):
         to_stream = kwargs.pop(self.streaming_request_field, [])
 
         req = kwargs  # only for first request
         for chunk in batched(iter(to_stream),
                              self.streaming_request_chunk_size):
@@ -441,14 +445,16 @@
 
         In that case, it is more convenient to take arguments as
         :meth:`assert_compare` does, hence providing conversion of arguments
         from Mercurial to Git.
         """
         self.apply_request_defaults(hg_kwargs)
         git_kwargs = self.request_kwargs_to_git(hg_kwargs)
+        if self.repository_arg:
+            git_kwargs.setdefault('repository', self.comparison.gitaly_repo)
         return self.rpc('git', **git_kwargs)
 
     def normalize_responses(self, hg_response, git_response):
         self.response_to_git(hg_response)
         norm = self.normalizer
         if norm is not None:
             norm(self, hg_response, vcs='hg')
```

### Comparing `hgitaly-1.5.0/tests_with_gitaly/conftest.py` & `hgitaly-1.6.0/tests_with_gitaly/conftest.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/tests_with_gitaly/gitaly.py` & `hgitaly-1.6.0/tests_with_gitaly/gitaly.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/tests_with_gitaly/hgitaly_rhgitaly_comparison.py` & `hgitaly-1.6.0/tests_with_gitaly/hgitaly_rhgitaly_comparison.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/tests_with_gitaly/rhgitaly.py` & `hgitaly-1.6.0/tests_with_gitaly/rhgitaly.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/tests_with_gitaly/test_blob_tree.py` & `hgitaly-1.6.0/tests_with_gitaly/test_blob_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,19 +211,24 @@
                                skip_flat_paths=skip_flat,
                                recursive=recursive)
 
     assert_compare_errors(path=b'.', revision=b'unknown')
     assert_compare_errors(path=b'')
 
     # case when path is actually a file
-    assert_compare(path=b'sub/bar')
+    assert_compare_errors(path=b'sub/bar')
+
+    # case when there is no result
+    for recursive in (False, True):
+        assert_compare_errors(path=b'no/such/dir', recursive=recursive)
 
     # sort parameter
     SortBy = GetTreeEntriesRequest.SortBy
     for recursive in (False, True):
+        # status code actually depends on `recursive` in Gitaly v17.0
         assert_compare(path=b'.', recursive=recursive,
                        sort=SortBy.TREES_FIRST)
 
     # tree first and nested trees
     nested = sub / 'nested'
     nested.mkdir()
     (nested / 'deeper').write_text('deep thoughts')
```

### Comparing `hgitaly-1.5.0/tests_with_gitaly/test_commit.py` & `hgitaly-1.6.0/tests_with_gitaly/test_commit.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/tests_with_gitaly/test_comparison.py` & `hgitaly-1.6.0/tests_with_gitaly/test_comparison.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/tests_with_gitaly/test_diff.py` & `hgitaly-1.6.0/tests_with_gitaly/test_diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/tests_with_gitaly/test_gitaly_server.py` & `hgitaly-1.6.0/tests_with_gitaly/test_gitaly_server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/tests_with_gitaly/test_operations.py` & `hgitaly-1.6.0/tests_with_gitaly/test_operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/tests_with_gitaly/test_ref.py` & `hgitaly-1.6.0/tests_with_gitaly/test_ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/tests_with_gitaly/test_repository_service.py` & `hgitaly-1.6.0/tests_with_gitaly/test_repository_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,23 +23,20 @@
 from hgitaly.stub.repository_pb2 import (
     CreateRepositoryRequest,
     CreateBundleRequest,
     CreateBundleFromRefListRequest,
     CreateRepositoryFromBundleRequest,
     FindLicenseRequest,
     FindMergeBaseRequest,
-    FullPathRequest,
     ObjectFormatRequest,
-    RemoveAllRequest,
     RemoveRepositoryRequest,
     RepositoryExistsRequest,
     RepositorySizeRequest,
     SearchFilesByContentRequest,
     SearchFilesByNameRequest,
-    SetFullPathRequest,
     WriteRefRequest,
 )
 from hgitaly.stub.shared_pb2 import (
         ObjectFormat,
 )
 from hgitaly.stub.commit_pb2_grpc import CommitServiceStub
 from hgitaly.stub.repository_pb2_grpc import RepositoryServiceStub
@@ -339,69 +336,14 @@
 
     # unknown storage
     assert_compare_errors(same_details=False,
                           repository=Repository(storage_name='unknown',
                                                 relative_path='/some/path'))
 
 
-def test_full_path(gitaly_comparison, server_repos_root):
-    fixture = gitaly_comparison
-    grpc_repo = fixture.gitaly_repo
-
-    rpc_helper = fixture.rpc_helper(
-        stub_cls=RepositoryServiceStub,
-        method_name='FullPath',
-        request_cls=FullPathRequest,
-    )
-    assert_compare_errors = rpc_helper.assert_compare_errors
-
-    # path not set on existing repo
-    assert_compare_errors(same_details=False)
-
-    # unknown storage and missing repo
-    assert_compare_errors(same_details=False,
-                          repository=Repository(storage_name='unknown',
-                                                relative_path='/some/path'))
-    assert_compare_errors(
-        same_details=False,
-        repository=Repository(storage_name=grpc_repo.storage_name,
-                              relative_path='no/such/path'))
-
-
-def test_set_full_path(gitaly_comparison, server_repos_root):
-    fixture = gitaly_comparison
-
-    rpc_helper = fixture.rpc_helper(
-        stub_cls=RepositoryServiceStub,
-        method_name='SetFullPath',
-        request_cls=SetFullPathRequest,
-    )
-    assert_compare = rpc_helper.assert_compare
-    assert_error_compare = rpc_helper.assert_compare_errors
-
-    # success case
-    assert_compare(path='group/project')
-
-    # error cases
-    assert_error_compare('')
-
-    assert_error_compare(path='some/full/path',
-                         repository=Repository(
-                             storage_name=fixture.gitaly_repo.storage_name,
-                             relative_path='no/such/repo'),
-                         same_details=False,
-                         )
-
-    assert_error_compare(path='some/full/path',
-                         same_details=False,
-                         repository=Repository(
-                             relative_path=fixture.gitaly_repo.relative_path,
-                             storage_name='unknown'))
-
-
 def assert_compare_hg_git_created_repos(target_hgrepo, target_gitrepo):
     # assert branches
     br_prefix = b'branch/'
     hgbranches = set(
         [br[0] for br in target_hgrepo.branchmap().iterbranches()])
     gitbranches = set(
         [br[len(br_prefix):] for br in target_gitrepo.branches().keys()])
@@ -775,28 +717,14 @@
     # missing repo, ref
     assert_compare_errors(ref=b'')
     assert_compare_errors(repository=None)
     fixture.gitaly_repo.relative_path = 'no/such/repo'
     assert_compare_errors(query='foo', same_details=False)
 
 
-def test_remove_all(gitaly_comparison, server_repos_root):
-    fixture = gitaly_comparison
-    rpc_helper = fixture.rpc_helper(
-        stub_cls=RepositoryServiceStub,
-        method_name='RemoveAll',
-        request_cls=RemoveAllRequest,
-        repository_arg=False,
-    )
-    assert_compare_errors = rpc_helper.assert_compare_errors
-
-    # unknown storage
-    assert_compare_errors(storage_name='unknown', same_details=False)
-
-
 def test_find_license(gitaly_comparison):
     fixture = gitaly_comparison
 
     rpc_helper = fixture.rpc_helper(
         stub_cls=RepositoryServiceStub,
         method_name='FindLicense',
         request_cls=FindLicenseRequest,
```

### Comparing `hgitaly-1.5.0/tests_with_gitaly/test_rhgitaly_server.py` & `hgitaly-1.6.0/tests_with_gitaly/test_rhgitaly_server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.5.0/tests_with_gitaly/test_server.py` & `hgitaly-1.6.0/tests_with_gitaly/test_server.py`

 * *Files identical despite different names*

